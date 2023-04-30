# Comparing `tmp/openweather_report-0.1.4.tar.gz` & `tmp/openweather_report-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openweather_report-0.1.4.tar", max compression
+gzip compressed data, was "openweather_report-0.1.5.tar", last modified: Sun Apr 30 19:57:41 2023, max compression
```

## Comparing `openweather_report-0.1.4.tar` & `openweather_report-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0     1074 2022-07-19 23:47:50.572866 openweather_report-0.1.4/LICENSE
--rw-r--r--   0        0        0      116 2022-07-21 22:22:12.015829 openweather_report-0.1.4/README.rst
--rw-r--r--   0        0        0        0 2022-07-19 23:56:16.439825 openweather_report-0.1.4/openweather_report/__init__.py
--rw-r--r--   0        0        0      616 2022-07-21 22:22:24.052687 openweather_report-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      886 2022-07-21 22:22:27.693178 openweather_report-0.1.4/setup.py
--rw-r--r--   0        0        0      774 2022-07-21 22:22:27.693585 openweather_report-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-04-02 00:48:07.133842 openweather_report-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1084 2023-04-23 23:04:51.068456 openweather_report-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2169 2023-04-30 19:52:52.554394 openweather_report-0.1.5/README.md
+-rw-r--r--   0        0        0      142 2023-04-30 19:54:54.172767 openweather_report-0.1.5/openweather_report/__init__.py
+-rw-r--r--   0        0        0       92 2023-04-23 23:38:28.389965 openweather_report-0.1.5/openweather_report/__main__.py
+-rw-r--r--   0        0        0     2754 2023-04-30 19:53:25.599066 openweather_report-0.1.5/openweather_report/cli.py
+-rw-r--r--   0        0        0     1474 2023-04-30 18:19:19.230151 openweather_report-0.1.5/openweather_report/openweather.py
+-rw-r--r--   0        0        0      531 2023-04-30 01:37:10.704123 openweather_report-0.1.5/openweather_report/openweather.sql
+-rw-r--r--   0        0        0     1617 2023-04-30 18:38:04.204670 openweather_report-0.1.5/openweather_report/postgres.py
+-rw-r--r--   0        0        0     1578 2023-04-30 18:40:37.149476 openweather_report-0.1.5/openweather_report/sqlite.py
+-rw-r--r--   0        0        0     2628 2023-04-30 19:10:36.966398 openweather_report-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 openweather_report-0.1.5/PKG-INFO
```

### Comparing `openweather_report-0.1.4/LICENSE` & `openweather_report-0.1.5/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
+The MIT License (MIT)
 
-Copyright (c) 2022 Christopher Tyler
+Copyright (c) 2023 Christopher Tyler
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

