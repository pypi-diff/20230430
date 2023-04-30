# Comparing `tmp/kolombos-1.5.1.tar.gz` & `tmp/kolombos-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolombos-1.5.1.tar", last modified: Tue Feb  7 05:20:52 2023, max compression
+gzip compressed data, was "kolombos-1.5.2.tar", last modified: Sun Apr 30 14:54:27 2023, max compression
```

## Comparing `kolombos-1.5.1.tar` & `kolombos-1.5.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.599915 kolombos-1.5.1/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1076 2022-05-09 22:55:55.000000 kolombos-1.5.1/LICENSE
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    13770 2023-02-07 05:20:52.599915 kolombos-1.5.1/PKG-INFO
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    13198 2023-02-07 05:13:07.000000 kolombos-1.5.1/README.md
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.591915 kolombos-1.5.1/kolombos/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      391 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      366 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/__main__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      995 2023-02-07 05:02:28.000000 kolombos-1.5.1/kolombos/app.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    12687 2023-02-07 05:04:20.000000 kolombos-1.5.1/kolombos/arghelp.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.595915 kolombos-1.5.1/kolombos/byteio/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      644 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/byteio/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      317 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/byteio/common.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2090 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/const.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.595915 kolombos-1.5.1/kolombos/byteio/formatter/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      425 2022-06-26 06:50:16.000000 kolombos-1.5.1/kolombos/byteio/formatter/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2131 2022-09-12 06:34:27.000000 kolombos-1.5.1/kolombos/byteio/formatter/_abstract.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4448 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/formatter/binary.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      736 2022-05-10 09:36:33.000000 kolombos-1.5.1/kolombos/byteio/formatter/factory.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2161 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/formatter/text.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.595915 kolombos-1.5.1/kolombos/byteio/parser/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      336 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/byteio/parser/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1749 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/parser/buffer.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     8385 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/parser/parser.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1688 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/byteio/partial_override.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3928 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/reader.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.595915 kolombos-1.5.1/kolombos/byteio/segment/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      500 2022-05-10 09:36:33.000000 kolombos-1.5.1/kolombos/byteio/segment/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     8327 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/segment/buffer.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      540 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/byteio/segment/chainable.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      824 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/byteio/segment/printer.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2298 2022-05-10 09:36:33.000000 kolombos-1.5.1/kolombos/byteio/segment/segment.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1056 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/byteio/segment/sequence_ref.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.595915 kolombos-1.5.1/kolombos/byteio/template/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      665 2022-05-10 09:36:33.000000 kolombos-1.5.1/kolombos/byteio/template/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3257 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/template/registry.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4346 2023-02-07 05:04:20.000000 kolombos-1.5.1/kolombos/byteio/template/template.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2955 2022-07-01 12:01:40.000000 kolombos-1.5.1/kolombos/byteio/template/template_control.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2678 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/template/template_escape.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3579 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/template/template_escape_sgr.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1011 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/template/template_newline.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      779 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/byteio/template/template_printable.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1262 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/byteio/template/template_utf8.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      685 2023-02-07 05:04:20.000000 kolombos-1.5.1/kolombos/common.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    10579 2023-02-07 05:04:20.000000 kolombos-1.5.1/kolombos/console.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      640 2023-02-07 05:04:20.000000 kolombos-1.5.1/kolombos/demo.bin
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    24013 2023-02-07 05:13:33.000000 kolombos-1.5.1/kolombos/legend.ansi
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.595915 kolombos-1.5.1/kolombos/runner/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      481 2023-02-07 05:04:20.000000 kolombos-1.5.1/kolombos/runner/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      411 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/runner/_abstract.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2346 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/runner/byteio.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1050 2023-02-07 05:04:20.000000 kolombos-1.5.1/kolombos/runner/demo.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      790 2023-02-07 05:04:20.000000 kolombos-1.5.1/kolombos/runner/factory.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      664 2022-05-10 09:36:32.000000 kolombos-1.5.1/kolombos/runner/legend.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      635 2023-01-11 01:46:13.000000 kolombos-1.5.1/kolombos/runner/version.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4130 2023-02-07 05:04:20.000000 kolombos-1.5.1/kolombos/settings.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       22 2023-02-07 05:20:40.000000 kolombos-1.5.1/kolombos/version.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.591915 kolombos-1.5.1/kolombos.egg-info/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    13770 2023-02-07 05:20:52.000000 kolombos-1.5.1/kolombos.egg-info/PKG-INFO
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1922 2023-02-07 05:20:52.000000 kolombos-1.5.1/kolombos.egg-info/SOURCES.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)        1 2023-02-07 05:20:52.000000 kolombos-1.5.1/kolombos.egg-info/dependency_links.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       52 2023-02-07 05:20:52.000000 kolombos-1.5.1/kolombos.egg-info/entry_points.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       18 2023-02-07 05:20:52.000000 kolombos-1.5.1/kolombos.egg-info/top_level.txt
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      104 2022-05-09 22:55:55.000000 kolombos-1.5.1/pyproject.toml
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.595915 kolombos-1.5.1/pytermor/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      642 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      262 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/__main__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      290 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/_version.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    25301 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/ansi.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    27939 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/color.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1871 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/common.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    27766 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/render.py
-drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-02-07 05:20:52.599915 kolombos-1.5.1/pytermor/util/
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1160 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/util/__init__.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     5402 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/util/auto_float.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     7188 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/util/prefixed_unit.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1931 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/util/stdlib_ext.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3996 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/util/string_filter.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    10092 2023-01-11 01:46:13.000000 kolombos-1.5.1/pytermor/util/time_delta.py
--rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      798 2023-02-07 05:20:52.599915 kolombos-1.5.1/setup.cfg
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.135063 kolombos-1.5.2/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1076 2022-05-09 22:55:55.000000 kolombos-1.5.2/LICENSE
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    14085 2023-04-30 14:54:27.135063 kolombos-1.5.2/PKG-INFO
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    13513 2023-04-30 14:49:49.000000 kolombos-1.5.2/README.md
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.127063 kolombos-1.5.2/kolombos/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      391 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      366 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/__main__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      995 2023-02-07 05:02:28.000000 kolombos-1.5.2/kolombos/app.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    12687 2023-04-01 18:06:55.000000 kolombos-1.5.2/kolombos/arghelp.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.131063 kolombos-1.5.2/kolombos/byteio/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      644 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/byteio/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      317 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/byteio/common.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2090 2023-01-11 01:46:13.000000 kolombos-1.5.2/kolombos/byteio/const.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.131063 kolombos-1.5.2/kolombos/byteio/formatter/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      425 2022-06-26 06:50:16.000000 kolombos-1.5.2/kolombos/byteio/formatter/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2131 2022-09-12 06:34:27.000000 kolombos-1.5.2/kolombos/byteio/formatter/_abstract.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4448 2023-01-11 01:46:13.000000 kolombos-1.5.2/kolombos/byteio/formatter/binary.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      736 2022-05-10 09:36:33.000000 kolombos-1.5.2/kolombos/byteio/formatter/factory.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2161 2023-01-11 01:46:13.000000 kolombos-1.5.2/kolombos/byteio/formatter/text.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.131063 kolombos-1.5.2/kolombos/byteio/parser/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      336 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/byteio/parser/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1749 2023-01-11 01:46:13.000000 kolombos-1.5.2/kolombos/byteio/parser/buffer.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     8385 2023-04-01 18:06:55.000000 kolombos-1.5.2/kolombos/byteio/parser/parser.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1688 2023-04-01 18:06:55.000000 kolombos-1.5.2/kolombos/byteio/partial_override.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3928 2023-01-11 01:46:13.000000 kolombos-1.5.2/kolombos/byteio/reader.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.131063 kolombos-1.5.2/kolombos/byteio/segment/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      500 2022-05-10 09:36:33.000000 kolombos-1.5.2/kolombos/byteio/segment/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     8327 2023-01-11 01:46:13.000000 kolombos-1.5.2/kolombos/byteio/segment/buffer.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      540 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/byteio/segment/chainable.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      824 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/byteio/segment/printer.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2298 2022-05-10 09:36:33.000000 kolombos-1.5.2/kolombos/byteio/segment/segment.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1056 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/byteio/segment/sequence_ref.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.131063 kolombos-1.5.2/kolombos/byteio/template/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      665 2022-05-10 09:36:33.000000 kolombos-1.5.2/kolombos/byteio/template/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3257 2023-04-27 19:42:47.000000 kolombos-1.5.2/kolombos/byteio/template/registry.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4346 2023-04-01 18:06:55.000000 kolombos-1.5.2/kolombos/byteio/template/template.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2955 2022-07-01 12:01:40.000000 kolombos-1.5.2/kolombos/byteio/template/template_control.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2678 2023-01-11 01:46:13.000000 kolombos-1.5.2/kolombos/byteio/template/template_escape.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3579 2023-04-01 18:06:55.000000 kolombos-1.5.2/kolombos/byteio/template/template_escape_sgr.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1011 2023-04-01 18:06:55.000000 kolombos-1.5.2/kolombos/byteio/template/template_newline.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      779 2023-04-01 18:06:55.000000 kolombos-1.5.2/kolombos/byteio/template/template_printable.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1262 2023-04-01 18:06:55.000000 kolombos-1.5.2/kolombos/byteio/template/template_utf8.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      685 2023-02-07 05:22:33.000000 kolombos-1.5.2/kolombos/common.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    10579 2023-02-07 05:22:33.000000 kolombos-1.5.2/kolombos/console.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      640 2023-04-01 18:06:55.000000 kolombos-1.5.2/kolombos/demo.bin
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    24013 2023-04-30 14:54:22.000000 kolombos-1.5.2/kolombos/legend.ansi
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.131063 kolombos-1.5.2/kolombos/runner/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      481 2023-02-07 05:22:33.000000 kolombos-1.5.2/kolombos/runner/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      411 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/runner/_abstract.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     2346 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/runner/byteio.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1050 2023-02-07 05:22:33.000000 kolombos-1.5.2/kolombos/runner/demo.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      790 2023-02-07 05:22:33.000000 kolombos-1.5.2/kolombos/runner/factory.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      664 2022-05-10 09:36:32.000000 kolombos-1.5.2/kolombos/runner/legend.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      635 2023-01-11 01:46:13.000000 kolombos-1.5.2/kolombos/runner/version.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     4130 2023-04-01 18:06:55.000000 kolombos-1.5.2/kolombos/settings.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       22 2023-04-30 14:52:29.000000 kolombos-1.5.2/kolombos/version.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.127063 kolombos-1.5.2/kolombos.egg-info/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    14085 2023-04-30 14:54:27.000000 kolombos-1.5.2/kolombos.egg-info/PKG-INFO
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1922 2023-04-30 14:54:27.000000 kolombos-1.5.2/kolombos.egg-info/SOURCES.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)        1 2023-04-30 14:54:27.000000 kolombos-1.5.2/kolombos.egg-info/dependency_links.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       52 2023-04-30 14:54:27.000000 kolombos-1.5.2/kolombos.egg-info/entry_points.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)       18 2023-04-30 14:54:27.000000 kolombos-1.5.2/kolombos.egg-info/top_level.txt
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      104 2022-05-09 22:55:55.000000 kolombos-1.5.2/pyproject.toml
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.131063 kolombos-1.5.2/pytermor/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      642 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      262 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/__main__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      290 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/_version.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    25301 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/ansi.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    27939 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/color.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1871 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/common.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    27766 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/render.py
+drwxrwxr-x   0 a.shavykin  (1001) a.shavykin  (1001)        0 2023-04-30 14:54:27.135063 kolombos-1.5.2/pytermor/util/
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1160 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/util/__init__.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     5402 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/util/auto_float.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     7188 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/util/prefixed_unit.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     1931 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/util/stdlib_ext.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)     3996 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/util/string_filter.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)    10092 2023-01-11 01:46:13.000000 kolombos-1.5.2/pytermor/util/time_delta.py
+-rw-rw-r--   0 a.shavykin  (1001) a.shavykin  (1001)      798 2023-04-30 14:54:27.135063 kolombos-1.5.2/setup.cfg
```

### Comparing `kolombos-1.5.1/LICENSE` & `kolombos-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/PKG-INFO` & `kolombos-1.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: kolombos
-Version: 1.5.1
+Version: 1.5.2
 Summary: CLI control characters and escape sequences viewer/visualizer
 Home-page: https://github.com/es7s/kolombos
 Author: Aleksandr Shavykin
 Author-email: 0.delameter@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Terminals
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<div align="center">
+   <img src="https://user-images.githubusercontent.com/50381946/235359002-8a1f72bc-12b4-42de-bc70-3774c30ecec8.png" width="96" height="96"><br>
+   <img src="https://user-images.githubusercontent.com/50381946/219900506-491a3fc0-2e84-4782-ae3d-da4ae9825664.png" width="400" height="64">
+</div>
+
+<div align="center">
+  <img src="https://img.shields.io/badge/python-3.7-3776AB?logo=python&logoColor=white&labelColor=333333">
+  <a href="https://pypi.org/project/kolombos/"><img alt="PyPI" src="https://img.shields.io/pypi/v/kolombos"></a>
+  <a href="https://pepy.tech/project/kolombos/">
+    <img alt="Downloads" src="https://pepy.tech/badge/kolombos">
+  </a>
+</div>
+<h1> </h1>
 
-<h1 align="center">
-  <img src="https://user-images.githubusercontent.com/50381946/167742137-3c250ada-0b2c-4124-9604-e02abec50b7e.png">
-  <br>
-  <code>kolombos</code>
-  <br>
-</h1>
-  
-  <p align="center">
-    <a href="https://pypi.org/project/kolombos/"><img alt="PyPI" src="https://img.shields.io/pypi/v/kolombos"></a>
-    <a href="https://pepy.tech/project/kolombos/">
-      <img alt="Downloads" src="https://pepy.tech/badge/kolombos">
-    </a>
-  </p>
 
 CLI application for visualising usually invisible characters and bytes:
 
 - whitespace characters;
 - ASCII control characters;
 - ANSI escape sequences;
 - UTF-8 encoded characters;
@@ -217,14 +217,24 @@
 Even more information can be seen after running `kolombos --legend`.
 
 
 ## Changelog
 
 
 
+### v1.5.2
+
+- UPDATE: icon redraw
+
+
+### v1.5.1
+
+- FIX: packaging assets
+
+
 ### v1.5
 - NEW: `--demo` mode
 
 
 ### v1.4.1
 - Temporarily injected `pytermor` v2.1
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: kolombos Version: 1.5.1 Summary: CLI control
+Metadata-Version: 2.1 Name: kolombos Version: 1.5.2 Summary: CLI control
 characters and escape sequences viewer/visualizer Home-page: https://
 github.com/es7s/kolombos Author: Aleksandr Shavykin Author-email:
 0.delameter@gmail.com Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Terminals Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
-****** [https://user-images.githubusercontent.com/50381946/167742137-3c250ada-
-                       0b2c-4124-9604-e02abec50b7e.png]
-                                   kolombos
-                                     ******
-                              [PyPI] [Downloads]
+ [https://user-images.githubusercontent.com/50381946/235359002-8a1f72bc-12b4-
+                          42de-bc70-3774c30ecec8.png]
+ [https://user-images.githubusercontent.com/50381946/219900506-491a3fc0-2e84-
+                          4782-ae3d-da4ae9825664.png]
+                   [https://img.shields.io/badge/python-3.7-
+   3776AB?logo=python&logoColor=white&labelColor=333333] [PyPI] [Downloads]
 CLI application for visualising usually invisible characters and bytes: -
 whitespace characters; - ASCII control characters; - ANSI escape sequences; -
 UTF-8 encoded characters; - binary data. ## Installation ### Via `pipx` pipx
 install kolombos ### Without `pipx` #### System-wide install (`sudo`) python -
 m pip install kolombos #### User install (no `sudo`) python -m pip install --
 user kolombos export PATH="${PATH}:${HOME}/.local/bin/" ## Usage Application
 can be useful for a variety of tasks, e.g. browsing unknown data formats,
@@ -156,18 +157,19 @@
 boxes by default, but still can be decoded with `-d`|`--decode` option (note
 the same requirement as for escape sequence markers — hex value length must
 always correspond to text representation length):
                                     [ss12]
 ## Legend
                                    [ss13v3]
 Even more information can be seen after running `kolombos --legend`. ##
-Changelog ### v1.5 - NEW: `--demo` mode ### v1.4.1 - Temporarily injected
-`pytermor` v2.1 ### v1.4 - REFACTOR: base colors - REFACTOR: extended legend -
-DOCS: update README and screenshots ### v1.3 - Swap -D and -d (debug/decode) -
-Make '--marker 0' default (was 1) - Update legend - Upgrade `pytermor` to 2.1
-### v1.2.1 - Minor update. ### v1.2 - Separators additional styling. -
-Separators auto-hide from `-m0`. - `--no-sep[arators]` launch option. - `run`
-dev script for quick launch of repo versions. - Updated output format of SGR
-color prefixes. - SGR labels are now getting colored instead of marker details
-(if `-m0` is set). - Updated legend. ### v1.1 - Additional separators around
-escape seqs (in text mode) for better readability. ### v1.0.2 - Added logos. -
-Fixed pipy README images. ### v1.0.1 - First public version.
+Changelog ### v1.5.2 - UPDATE: icon redraw ### v1.5.1 - FIX: packaging assets
+### v1.5 - NEW: `--demo` mode ### v1.4.1 - Temporarily injected `pytermor` v2.1
+### v1.4 - REFACTOR: base colors - REFACTOR: extended legend - DOCS: update
+README and screenshots ### v1.3 - Swap -D and -d (debug/decode) - Make '--
+marker 0' default (was 1) - Update legend - Upgrade `pytermor` to 2.1 ###
+v1.2.1 - Minor update. ### v1.2 - Separators additional styling. - Separators
+auto-hide from `-m0`. - `--no-sep[arators]` launch option. - `run` dev script
+for quick launch of repo versions. - Updated output format of SGR color
+prefixes. - SGR labels are now getting colored instead of marker details (if `-
+m0` is set). - Updated legend. ### v1.1 - Additional separators around escape
+seqs (in text mode) for better readability. ### v1.0.2 - Added logos. - Fixed
+pipy README images. ### v1.0.1 - First public version.
```

### Comparing `kolombos-1.5.1/README.md` & `kolombos-1.5.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+<div align="center">
+   <img src="https://user-images.githubusercontent.com/50381946/235359002-8a1f72bc-12b4-42de-bc70-3774c30ecec8.png" width="96" height="96"><br>
+   <img src="https://user-images.githubusercontent.com/50381946/219900506-491a3fc0-2e84-4782-ae3d-da4ae9825664.png" width="400" height="64">
+</div>
+
+<div align="center">
+  <img src="https://img.shields.io/badge/python-3.7-3776AB?logo=python&logoColor=white&labelColor=333333">
+  <a href="https://pypi.org/project/kolombos/"><img alt="PyPI" src="https://img.shields.io/pypi/v/kolombos"></a>
+  <a href="https://pepy.tech/project/kolombos/">
+    <img alt="Downloads" src="https://pepy.tech/badge/kolombos">
+  </a>
+</div>
+<h1> </h1>
 
-<h1 align="center">
-  <img src="https://user-images.githubusercontent.com/50381946/167742137-3c250ada-0b2c-4124-9604-e02abec50b7e.png">
-  <br>
-  <code>kolombos</code>
-  <br>
-</h1>
-  
-  <p align="center">
-    <a href="https://pypi.org/project/kolombos/"><img alt="PyPI" src="https://img.shields.io/pypi/v/kolombos"></a>
-    <a href="https://pepy.tech/project/kolombos/">
-      <img alt="Downloads" src="https://pepy.tech/badge/kolombos">
-    </a>
-  </p>
 
 CLI application for visualising usually invisible characters and bytes:
 
 - whitespace characters;
 - ASCII control characters;
 - ANSI escape sequences;
 - UTF-8 encoded characters;
@@ -200,14 +200,24 @@
 Even more information can be seen after running `kolombos --legend`.
 
 
 ## Changelog
 
 
 
+### v1.5.2
+
+- UPDATE: icon redraw
+
+
+### v1.5.1
+
+- FIX: packaging assets
+
+
 ### v1.5
 - NEW: `--demo` mode
 
 
 ### v1.4.1
 - Temporarily injected `pytermor` v2.1
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-****** [https://user-images.githubusercontent.com/50381946/167742137-3c250ada-
-                       0b2c-4124-9604-e02abec50b7e.png]
-                                   kolombos
-                                     ******
-                              [PyPI] [Downloads]
+ [https://user-images.githubusercontent.com/50381946/235359002-8a1f72bc-12b4-
+                          42de-bc70-3774c30ecec8.png]
+ [https://user-images.githubusercontent.com/50381946/219900506-491a3fc0-2e84-
+                          4782-ae3d-da4ae9825664.png]
+                   [https://img.shields.io/badge/python-3.7-
+   3776AB?logo=python&logoColor=white&labelColor=333333] [PyPI] [Downloads]
 CLI application for visualising usually invisible characters and bytes: -
 whitespace characters; - ASCII control characters; - ANSI escape sequences; -
 UTF-8 encoded characters; - binary data. ## Installation ### Via `pipx` pipx
 install kolombos ### Without `pipx` #### System-wide install (`sudo`) python -
 m pip install kolombos #### User install (no `sudo`) python -m pip install --
 user kolombos export PATH="${PATH}:${HOME}/.local/bin/" ## Usage Application
 can be useful for a variety of tasks, e.g. browsing unknown data formats,
@@ -148,18 +149,19 @@
 boxes by default, but still can be decoded with `-d`|`--decode` option (note
 the same requirement as for escape sequence markers — hex value length must
 always correspond to text representation length):
                                     [ss12]
 ## Legend
                                    [ss13v3]
 Even more information can be seen after running `kolombos --legend`. ##
-Changelog ### v1.5 - NEW: `--demo` mode ### v1.4.1 - Temporarily injected
-`pytermor` v2.1 ### v1.4 - REFACTOR: base colors - REFACTOR: extended legend -
-DOCS: update README and screenshots ### v1.3 - Swap -D and -d (debug/decode) -
-Make '--marker 0' default (was 1) - Update legend - Upgrade `pytermor` to 2.1
-### v1.2.1 - Minor update. ### v1.2 - Separators additional styling. -
-Separators auto-hide from `-m0`. - `--no-sep[arators]` launch option. - `run`
-dev script for quick launch of repo versions. - Updated output format of SGR
-color prefixes. - SGR labels are now getting colored instead of marker details
-(if `-m0` is set). - Updated legend. ### v1.1 - Additional separators around
-escape seqs (in text mode) for better readability. ### v1.0.2 - Added logos. -
-Fixed pipy README images. ### v1.0.1 - First public version.
+Changelog ### v1.5.2 - UPDATE: icon redraw ### v1.5.1 - FIX: packaging assets
+### v1.5 - NEW: `--demo` mode ### v1.4.1 - Temporarily injected `pytermor` v2.1
+### v1.4 - REFACTOR: base colors - REFACTOR: extended legend - DOCS: update
+README and screenshots ### v1.3 - Swap -D and -d (debug/decode) - Make '--
+marker 0' default (was 1) - Update legend - Upgrade `pytermor` to 2.1 ###
+v1.2.1 - Minor update. ### v1.2 - Separators additional styling. - Separators
+auto-hide from `-m0`. - `--no-sep[arators]` launch option. - `run` dev script
+for quick launch of repo versions. - Updated output format of SGR color
+prefixes. - SGR labels are now getting colored instead of marker details (if `-
+m0` is set). - Updated legend. ### v1.1 - Additional separators around escape
+seqs (in text mode) for better readability. ### v1.0.2 - Added logos. - Fixed
+pipy README images. ### v1.0.1 - First public version.
```

### Comparing `kolombos-1.5.1/kolombos/app.py` & `kolombos-1.5.2/kolombos/app.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/arghelp.py` & `kolombos-1.5.2/kolombos/arghelp.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/__init__.py` & `kolombos-1.5.2/kolombos/byteio/__init__.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/const.py` & `kolombos-1.5.2/kolombos/byteio/const.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/formatter/_abstract.py` & `kolombos-1.5.2/kolombos/byteio/formatter/_abstract.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/formatter/binary.py` & `kolombos-1.5.2/kolombos/byteio/formatter/binary.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/formatter/factory.py` & `kolombos-1.5.2/kolombos/byteio/formatter/factory.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/formatter/text.py` & `kolombos-1.5.2/kolombos/byteio/formatter/text.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/parser/buffer.py` & `kolombos-1.5.2/kolombos/byteio/parser/buffer.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/parser/parser.py` & `kolombos-1.5.2/kolombos/byteio/parser/parser.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/partial_override.py` & `kolombos-1.5.2/kolombos/byteio/partial_override.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/reader.py` & `kolombos-1.5.2/kolombos/byteio/reader.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/segment/buffer.py` & `kolombos-1.5.2/kolombos/byteio/segment/buffer.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/segment/chainable.py` & `kolombos-1.5.2/kolombos/byteio/segment/chainable.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/segment/printer.py` & `kolombos-1.5.2/kolombos/byteio/segment/printer.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/segment/segment.py` & `kolombos-1.5.2/kolombos/byteio/segment/segment.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/segment/sequence_ref.py` & `kolombos-1.5.2/kolombos/byteio/segment/sequence_ref.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/template/__init__.py` & `kolombos-1.5.2/kolombos/byteio/template/__init__.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/template/registry.py` & `kolombos-1.5.2/kolombos/byteio/template/registry.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/template/template.py` & `kolombos-1.5.2/kolombos/byteio/template/template.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/template/template_control.py` & `kolombos-1.5.2/kolombos/byteio/template/template_control.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/template/template_escape.py` & `kolombos-1.5.2/kolombos/byteio/template/template_escape.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/template/template_escape_sgr.py` & `kolombos-1.5.2/kolombos/byteio/template/template_escape_sgr.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/template/template_newline.py` & `kolombos-1.5.2/kolombos/byteio/template/template_newline.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/template/template_printable.py` & `kolombos-1.5.2/kolombos/byteio/template/template_printable.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/byteio/template/template_utf8.py` & `kolombos-1.5.2/kolombos/byteio/template/template_utf8.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/common.py` & `kolombos-1.5.2/kolombos/common.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/console.py` & `kolombos-1.5.2/kolombos/console.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/demo.bin` & `kolombos-1.5.2/kolombos/demo.bin`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/legend.ansi` & `kolombos-1.5.2/kolombos/legend.ansi`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [1;92m    __         [34m__                __[m
 [1;92m   / /[92m__[94m____  / /___  ____ ___  / /_  ____ [93m _____[m
 [1;32m  / //_/[36m __ \/ / __ \[35m/ __ '__ \/ __ \/ __ \[33m/ ___/[m
 [1;94m / ,< [36m/ /_/ / / /_/ [35m/ / / / / / /_/ / /_/ [33m(__  )[m
 [1;34m/_/|_|[34m\____/_/\____/_/ /_/ /_/\.___/\____[33m/____/[m
-                                            [93mv1.5.0[m
+                                            [93mv1.5.2[m
 
 [97;1mCHARACTER CLASSES[m
   [90m<[m[1mS[m[90m>[m   ASCII whitespace chars   09-0d, 20      [90;1m-s -S[m
   [90m<[m[1mC[m[90m>[m   ASCII control chars      01-08, 0e-1f   [90;1m-c -C[m
   [90m<[m[1mP[m[90m>[m   ASCII printable chars    21-7e          [90;1m-p -P[m
   [90m<[m[1mI[m[90m>[m   binary data              80-ff          [90;1m-i -I[m
   [90m<[m[1mU[m[90m>[m   UTF-8 sequences          various        [90;1m-u -U[m
@@ -61,8 +61,8 @@
    [1;38;2;255;255;255;48;2;0;0;0m Ꙅ [22;39;49m       [33mꙄ[39m           [33m 1b[39m[33;48;5;16;4m 73[39;49;24m    [90m<[m[1mE[m[90m>[m  Fs sequence
  [38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m[38;2;51;51;51m─[39m
 
 [90mFor the best view your terminal should be [1m88[22m chars wide (or wider)[m
 
 [90mIs a part of [1;37mes7s[90m pack[m
 [90m(c) 2022 A. Shavykin <[33m0[90m.delameter@gmail.com>[m
-# Generated at  7-Feb-23 08:13
+# Generated at 30-Apr-23 17:54
```

### Comparing `kolombos-1.5.1/kolombos/runner/byteio.py` & `kolombos-1.5.2/kolombos/runner/byteio.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/runner/demo.py` & `kolombos-1.5.2/kolombos/runner/demo.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/runner/factory.py` & `kolombos-1.5.2/kolombos/runner/factory.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/runner/legend.py` & `kolombos-1.5.2/kolombos/runner/legend.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/runner/version.py` & `kolombos-1.5.2/kolombos/runner/version.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos/settings.py` & `kolombos-1.5.2/kolombos/settings.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/kolombos.egg-info/PKG-INFO` & `kolombos-1.5.2/kolombos.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: kolombos
-Version: 1.5.1
+Version: 1.5.2
 Summary: CLI control characters and escape sequences viewer/visualizer
 Home-page: https://github.com/es7s/kolombos
 Author: Aleksandr Shavykin
 Author-email: 0.delameter@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Terminals
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<div align="center">
+   <img src="https://user-images.githubusercontent.com/50381946/235359002-8a1f72bc-12b4-42de-bc70-3774c30ecec8.png" width="96" height="96"><br>
+   <img src="https://user-images.githubusercontent.com/50381946/219900506-491a3fc0-2e84-4782-ae3d-da4ae9825664.png" width="400" height="64">
+</div>
+
+<div align="center">
+  <img src="https://img.shields.io/badge/python-3.7-3776AB?logo=python&logoColor=white&labelColor=333333">
+  <a href="https://pypi.org/project/kolombos/"><img alt="PyPI" src="https://img.shields.io/pypi/v/kolombos"></a>
+  <a href="https://pepy.tech/project/kolombos/">
+    <img alt="Downloads" src="https://pepy.tech/badge/kolombos">
+  </a>
+</div>
+<h1> </h1>
 
-<h1 align="center">
-  <img src="https://user-images.githubusercontent.com/50381946/167742137-3c250ada-0b2c-4124-9604-e02abec50b7e.png">
-  <br>
-  <code>kolombos</code>
-  <br>
-</h1>
-  
-  <p align="center">
-    <a href="https://pypi.org/project/kolombos/"><img alt="PyPI" src="https://img.shields.io/pypi/v/kolombos"></a>
-    <a href="https://pepy.tech/project/kolombos/">
-      <img alt="Downloads" src="https://pepy.tech/badge/kolombos">
-    </a>
-  </p>
 
 CLI application for visualising usually invisible characters and bytes:
 
 - whitespace characters;
 - ASCII control characters;
 - ANSI escape sequences;
 - UTF-8 encoded characters;
@@ -217,14 +217,24 @@
 Even more information can be seen after running `kolombos --legend`.
 
 
 ## Changelog
 
 
 
+### v1.5.2
+
+- UPDATE: icon redraw
+
+
+### v1.5.1
+
+- FIX: packaging assets
+
+
 ### v1.5
 - NEW: `--demo` mode
 
 
 ### v1.4.1
 - Temporarily injected `pytermor` v2.1
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: kolombos Version: 1.5.1 Summary: CLI control
+Metadata-Version: 2.1 Name: kolombos Version: 1.5.2 Summary: CLI control
 characters and escape sequences viewer/visualizer Home-page: https://
 github.com/es7s/kolombos Author: Aleksandr Shavykin Author-email:
 0.delameter@gmail.com Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Terminals Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
-****** [https://user-images.githubusercontent.com/50381946/167742137-3c250ada-
-                       0b2c-4124-9604-e02abec50b7e.png]
-                                   kolombos
-                                     ******
-                              [PyPI] [Downloads]
+ [https://user-images.githubusercontent.com/50381946/235359002-8a1f72bc-12b4-
+                          42de-bc70-3774c30ecec8.png]
+ [https://user-images.githubusercontent.com/50381946/219900506-491a3fc0-2e84-
+                          4782-ae3d-da4ae9825664.png]
+                   [https://img.shields.io/badge/python-3.7-
+   3776AB?logo=python&logoColor=white&labelColor=333333] [PyPI] [Downloads]
 CLI application for visualising usually invisible characters and bytes: -
 whitespace characters; - ASCII control characters; - ANSI escape sequences; -
 UTF-8 encoded characters; - binary data. ## Installation ### Via `pipx` pipx
 install kolombos ### Without `pipx` #### System-wide install (`sudo`) python -
 m pip install kolombos #### User install (no `sudo`) python -m pip install --
 user kolombos export PATH="${PATH}:${HOME}/.local/bin/" ## Usage Application
 can be useful for a variety of tasks, e.g. browsing unknown data formats,
@@ -156,18 +157,19 @@
 boxes by default, but still can be decoded with `-d`|`--decode` option (note
 the same requirement as for escape sequence markers — hex value length must
 always correspond to text representation length):
                                     [ss12]
 ## Legend
                                    [ss13v3]
 Even more information can be seen after running `kolombos --legend`. ##
-Changelog ### v1.5 - NEW: `--demo` mode ### v1.4.1 - Temporarily injected
-`pytermor` v2.1 ### v1.4 - REFACTOR: base colors - REFACTOR: extended legend -
-DOCS: update README and screenshots ### v1.3 - Swap -D and -d (debug/decode) -
-Make '--marker 0' default (was 1) - Update legend - Upgrade `pytermor` to 2.1
-### v1.2.1 - Minor update. ### v1.2 - Separators additional styling. -
-Separators auto-hide from `-m0`. - `--no-sep[arators]` launch option. - `run`
-dev script for quick launch of repo versions. - Updated output format of SGR
-color prefixes. - SGR labels are now getting colored instead of marker details
-(if `-m0` is set). - Updated legend. ### v1.1 - Additional separators around
-escape seqs (in text mode) for better readability. ### v1.0.2 - Added logos. -
-Fixed pipy README images. ### v1.0.1 - First public version.
+Changelog ### v1.5.2 - UPDATE: icon redraw ### v1.5.1 - FIX: packaging assets
+### v1.5 - NEW: `--demo` mode ### v1.4.1 - Temporarily injected `pytermor` v2.1
+### v1.4 - REFACTOR: base colors - REFACTOR: extended legend - DOCS: update
+README and screenshots ### v1.3 - Swap -D and -d (debug/decode) - Make '--
+marker 0' default (was 1) - Update legend - Upgrade `pytermor` to 2.1 ###
+v1.2.1 - Minor update. ### v1.2 - Separators additional styling. - Separators
+auto-hide from `-m0`. - `--no-sep[arators]` launch option. - `run` dev script
+for quick launch of repo versions. - Updated output format of SGR color
+prefixes. - SGR labels are now getting colored instead of marker details (if `-
+m0` is set). - Updated legend. ### v1.1 - Additional separators around escape
+seqs (in text mode) for better readability. ### v1.0.2 - Added logos. - Fixed
+pipy README images. ### v1.0.1 - First public version.
```

### Comparing `kolombos-1.5.1/kolombos.egg-info/SOURCES.txt` & `kolombos-1.5.2/kolombos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/__init__.py` & `kolombos-1.5.2/pytermor/__init__.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/ansi.py` & `kolombos-1.5.2/pytermor/ansi.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/color.py` & `kolombos-1.5.2/pytermor/color.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/common.py` & `kolombos-1.5.2/pytermor/common.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/render.py` & `kolombos-1.5.2/pytermor/render.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/util/__init__.py` & `kolombos-1.5.2/pytermor/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/util/auto_float.py` & `kolombos-1.5.2/pytermor/util/auto_float.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/util/prefixed_unit.py` & `kolombos-1.5.2/pytermor/util/prefixed_unit.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/util/stdlib_ext.py` & `kolombos-1.5.2/pytermor/util/stdlib_ext.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/util/string_filter.py` & `kolombos-1.5.2/pytermor/util/string_filter.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/pytermor/util/time_delta.py` & `kolombos-1.5.2/pytermor/util/time_delta.py`

 * *Files identical despite different names*

### Comparing `kolombos-1.5.1/setup.cfg` & `kolombos-1.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kolombos
-version = 1.5.1
+version = 1.5.2
 author = Aleksandr Shavykin
 author_email = 0.delameter@gmail.com
 description = CLI control characters and escape sequences viewer/visualizer
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/es7s/kolombos
 project_urls =
```

