# Comparing `tmp/FlipperNested-2.1.1.tar.gz` & `tmp/FlipperNested-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-2.1.1.tar", last modified: Sun Apr 30 14:31:20 2023, max compression
+gzip compressed data, was "FlipperNested-2.1.2.tar", last modified: Sun Apr 30 14:45:46 2023, max compression
```

## Comparing `FlipperNested-2.1.1.tar` & `FlipperNested-2.1.2.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:20.095095 FlipperNested-2.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:20.075095 FlipperNested-2.1.1/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:20.075095 FlipperNested-2.1.1/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:20.075095 FlipperNested-2.1.1/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-30 14:31:20.000000 FlipperNested-2.1.1/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-30 14:31:20.000000 FlipperNested-2.1.1/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:31:20.000000 FlipperNested-2.1.1/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-30 14:31:20.000000 FlipperNested-2.1.1/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 14:31:20.000000 FlipperNested-2.1.1/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-30 14:31:20.000000 FlipperNested-2.1.1/FlipperNested.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:20.079095 FlipperNested-2.1.1/HardNestedSolver/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2504 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/bucketsort.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/bucketsort.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    87569 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/cmdhfmfhard.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1361 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/cmdhfmfhard.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    18805 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/crapto1.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2951 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/crapto1.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     6561 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/crypto1.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:20.087095 FlipperNested-2.1.1/HardNestedSolver/hardnested/
--rwxr-xr-x   0 runner    (1001) docker     (123)   494104 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_benchmark_data.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    33334 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bf_core.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     4073 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bf_core.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    31568 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bitarray_core.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3347 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bitarray_core.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    20997 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bruteforce.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2249 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bruteforce.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    24142 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_tables.c
--rwxr-xr-x   0 runner    (1001) docker     (123)  5060431 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/hardnested/tables.c
--rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/hardnested/tables.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/library.c
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/library.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     3340 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/parity.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:20.091095 FlipperNested-2.1.1/HardNestedSolver/pm3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3252 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/ansi.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5556 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/common.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     6876 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/commonutil.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3164 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/commonutil.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    35936 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/comms.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2762 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/comms.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5824 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/crc.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3532 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/crc.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    10060 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/crc16.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/crc16.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1686 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/crc32.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/crc32.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     6604 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/crc64.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1012 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/crc64.h
--rwxr-xr-x   0 runner    (1001) docker     (123)   110555 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/emojis.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/emojis_alt.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    39500 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/fileutils.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     9687 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/fileutils.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    30683 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/pm3_cmd.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:20.091095 FlipperNested-2.1.1/HardNestedSolver/pm3/uart/
--rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/uart/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     3010 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/uart/uart.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    17390 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/uart/uart_posix.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    12654 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/uart/uart_win32.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    24666 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/ui.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     3296 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/ui.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    35946 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/util.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     7580 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/util.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/util_darwin.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     2874 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/util_darwin.m
--rwxr-xr-x   0 runner    (1001) docker     (123)     4044 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/util_posix.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/pm3/util_posix.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/HardNestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:20.095095 FlipperNested-2.1.1/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/progress.c
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/progress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-30 14:31:20.095095 FlipperNested-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:31:20.095095 FlipperNested-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:31:20.095095 FlipperNested-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-30 14:31:11.000000 FlipperNested-2.1.1/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.607293 FlipperNested-2.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.587293 FlipperNested-2.1.2/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.591293 FlipperNested-2.1.2/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.587293 FlipperNested-2.1.2/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-30 14:45:46.000000 FlipperNested-2.1.2/FlipperNested.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.591293 FlipperNested-2.1.2/HardNestedSolver/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2504 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/bucketsort.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/bucketsort.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    87569 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/cmdhfmfhard.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1361 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/cmdhfmfhard.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18805 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/crapto1.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2951 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/crapto1.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6561 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/crypto1.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.599293 FlipperNested-2.1.2/HardNestedSolver/hardnested/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   494104 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_benchmark_data.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33334 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bf_core.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4073 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bf_core.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31568 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bitarray_core.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3347 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bitarray_core.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20997 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bruteforce.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2249 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bruteforce.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24142 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_tables.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)  5060431 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/tables.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/hardnested/tables.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/library.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/library.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3340 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/parity.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.603293 FlipperNested-2.1.2/HardNestedSolver/pm3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3252 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/ansi.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5556 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/common.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6876 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/commonutil.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3164 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/commonutil.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35936 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/comms.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2762 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/comms.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5824 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3532 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10060 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc16.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc16.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1686 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc32.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc32.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6604 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc64.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1012 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/crc64.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)   110555 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/emojis.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/emojis_alt.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39500 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/fileutils.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9687 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/fileutils.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30683 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/pm3_cmd.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.603293 FlipperNested-2.1.2/HardNestedSolver/pm3/uart/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/uart/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3010 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/uart/uart.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17390 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/uart/uart_posix.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12654 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/uart/uart_win32.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24666 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/ui.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3296 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/ui.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35946 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7580 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util_darwin.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2874 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util_darwin.m
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4044 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util_posix.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/pm3/util_posix.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/HardNestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.607293 FlipperNested-2.1.2/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-30 14:45:46.607293 FlipperNested-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:45:46.607293 FlipperNested-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:45:46.607293 FlipperNested-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-30 14:45:36.000000 FlipperNested-2.1.2/tests/test_parse.py
```

### Comparing `FlipperNested-2.1.1/FlipperNested/bridge.py` & `FlipperNested-2.1.2/FlipperNested/bridge.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/FlipperNested/cli.py` & `FlipperNested-2.1.2/FlipperNested/cli.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/FlipperNested/main.py` & `FlipperNested-2.1.2/FlipperNested/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,28 +75,34 @@
                     sec, key_type = values[-2:]
                     if sec not in self.nonces[key_type].keys():
                         self.nonces[key_type][sec] = []
                     file = tempfile.NamedTemporaryFile(delete=False)
                     nonces_filename = values[1].rsplit("/", 1)[1]
                     if self.connection:
                         value = self.connection.file_read(values[1])
-                    elif os.path.isfile(os.path.dirname(self.filename) + "/" + nonces_filename):
-                        # file in same folder as input file
+                    elif os.path.dirname(self.filename) and os.path.isfile(
+                            os.path.dirname(self.filename) + "/" + nonces_filename):
+                        # file in same directory as input file
                         value = open(os.path.dirname(self.filename) + "/" + nonces_filename, "rb").read()
-                    elif os.path.isfile(os.path.dirname(self.filename) + "/" + self.filename.rsplit(".", 1)[1] + "/" +
-                                        nonces_filename):
-                        # copied from .nested folder with UID
-                        value = open(os.path.dirname(self.filename) + "/" + self.filename.rsplit(".", 1)[1] + "/" +
-                                     nonces_filename, "rb").read()
+                    elif os.path.dirname(self.filename) and os.path.isfile(
+                            os.path.dirname(self.filename) + "/" + self.filename.rsplit(".", 1)[
+                                0] + "/" + nonces_filename):
+                        # copied from .nested directory with UID
+                        value = open(os.path.dirname(self.filename) + "/" + self.filename.rsplit(".", 1)[
+                            0] + "/" + nonces_filename, "rb").read()
+                    elif os.path.isfile(self.filename.rsplit(".", 1)[
+                                0] + "/" + nonces_filename):
+                        # copied from .nested directory with UID, from current directory
+                        value = open(self.filename.rsplit(".", 1)[
+                            0] + "/" + nonces_filename, "rb").read()
                     elif os.path.isfile(nonces_filename):
                         # file in current directory (--save)
                         value = open(nonces_filename, "rb").read()
                     else:
-                        print(
-                            "[!] Missing {} file and Flipper Zero isn't connected".format(nonces_filename))
+                        print("[!] Missing {} file and Flipper Zero isn't connected".format(nonces_filename))
                         print("[?] If you are trying to recover from Hard Nested offline, you should copy this file")
                         return False
                     open(file.name, "wb+").write(b"\n".join(value.split(b"\n")[4:]))
                     if self.save:
                         open(nonces_filename, "wb+").write(value)
                     values[1] = file.name
                     self.nonces[key_type][sec].append(values)
```

### Comparing `FlipperNested-2.1.1/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-2.1.2/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/FlipperNested/proto/storage_pb2.py` & `FlipperNested-2.1.2/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-2.1.2/FlipperNested.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 2.1.1
+Version: 2.1.2
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-2.1.1/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-2.1.2/FlipperNested.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/bucketsort.c` & `FlipperNested-2.1.2/HardNestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/bucketsort.h` & `FlipperNested-2.1.2/HardNestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/cmdhfmfhard.c` & `FlipperNested-2.1.2/HardNestedSolver/cmdhfmfhard.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/cmdhfmfhard.h` & `FlipperNested-2.1.2/HardNestedSolver/cmdhfmfhard.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/crapto1.c` & `FlipperNested-2.1.2/HardNestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/crapto1.h` & `FlipperNested-2.1.2/HardNestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/crypto1.c` & `FlipperNested-2.1.2/HardNestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_benchmark_data.h` & `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_benchmark_data.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bf_core.c` & `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bf_core.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bf_core.h` & `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bf_core.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bitarray_core.c` & `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bitarray_core.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bitarray_core.h` & `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bitarray_core.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bruteforce.c` & `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bruteforce.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_bruteforce.h` & `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_bruteforce.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/hardnested/hardnested_tables.c` & `FlipperNested-2.1.2/HardNestedSolver/hardnested/hardnested_tables.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/hardnested/tables.c` & `FlipperNested-2.1.2/HardNestedSolver/hardnested/tables.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/hardnested/tables.h` & `FlipperNested-2.1.2/HardNestedSolver/hardnested/tables.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/parity.h` & `FlipperNested-2.1.2/HardNestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/ansi.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/ansi.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/common.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/common.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/commonutil.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/commonutil.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/commonutil.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/commonutil.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/comms.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/comms.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/comms.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/comms.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/crc.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/crc.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/crc.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/crc.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/crc16.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/crc16.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/crc16.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/crc16.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/crc32.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/crc32.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/crc32.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/crc32.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/crc64.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/crc64.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/crc64.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/crc64.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/emojis.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/emojis.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/emojis_alt.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/emojis_alt.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/fileutils.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/fileutils.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/fileutils.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/fileutils.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/pm3_cmd.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/pm3_cmd.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/uart/README.md` & `FlipperNested-2.1.2/HardNestedSolver/pm3/uart/README.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/uart/uart.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/uart/uart.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/uart/uart_posix.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/uart/uart_posix.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/uart/uart_win32.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/uart/uart_win32.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/ui.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/ui.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/ui.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/ui.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/util.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/util.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/util.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/util.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/util_darwin.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/util_darwin.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/util_darwin.m` & `FlipperNested-2.1.2/HardNestedSolver/pm3/util_darwin.m`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/util_posix.c` & `FlipperNested-2.1.2/HardNestedSolver/pm3/util_posix.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/pm3/util_posix.h` & `FlipperNested-2.1.2/HardNestedSolver/pm3/util_posix.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/HardNestedSolver/python.c` & `FlipperNested-2.1.2/HardNestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/LICENSE.md` & `FlipperNested-2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/NestedSolver/bucketsort.c` & `FlipperNested-2.1.2/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/NestedSolver/bucketsort.h` & `FlipperNested-2.1.2/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/NestedSolver/crapto1.c` & `FlipperNested-2.1.2/NestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/NestedSolver/crapto1.h` & `FlipperNested-2.1.2/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/NestedSolver/crypto1.c` & `FlipperNested-2.1.2/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/NestedSolver/library.c` & `FlipperNested-2.1.2/NestedSolver/library.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/NestedSolver/library.h` & `FlipperNested-2.1.2/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/NestedSolver/parity.h` & `FlipperNested-2.1.2/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/NestedSolver/progress.c` & `FlipperNested-2.1.2/NestedSolver/progress.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/NestedSolver/python.c` & `FlipperNested-2.1.2/NestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/PKG-INFO` & `FlipperNested-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 2.1.1
+Version: 2.1.2
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-2.1.1/README.md` & `FlipperNested-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-2.1.1/setup.py` & `FlipperNested-2.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                               libraries=libraries)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FlipperNested",
-    version="2.1.1",
+    version="2.1.2",
     author="AloneLiberty",
     description="Recover keys from collected nonces",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AloneLiberty/FlipperNestedRecovery",
     entry_points={'console_scripts': ['FlipperNested = FlipperNested.cli:main']},
     install_requires=['protobuf>4', 'pyserial'],
```

### Comparing `FlipperNested-2.1.1/tests/test_calculate.py` & `FlipperNested-2.1.2/tests/test_calculate.py`

 * *Files identical despite different names*

