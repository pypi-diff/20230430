# Comparing `tmp/sdmx1-2.8.0.tar.gz` & `tmp/sdmx1-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmx1-2.8.0.tar", last modified: Fri Mar 31 14:47:08 2023, max compression
+gzip compressed data, was "sdmx1-2.9.0.tar", last modified: Sun Apr 30 16:08:34 2023, max compression
```

## Comparing `sdmx1-2.8.0.tar` & `sdmx1-2.9.0.tar`

### file list

```diff
@@ -1,130 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.849648 sdmx1-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-31 14:46:49.000000 sdmx1-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-31 14:46:49.000000 sdmx1-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-03-31 14:47:08.849648 sdmx1-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-03-31 14:46:49.000000 sdmx1-2.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-31 14:46:49.000000 sdmx1-2.8.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.837648 sdmx1-2.8.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.841648 sdmx1-2.8.0/doc/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/api/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/api/reader.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/api/writer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/dev.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.841648 sdmx1-2.8.0/doc/howto/
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/howto/create.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13171 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/implementation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16374 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/sources.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/walkthrough.rst
--rw-r--r--   0 runner    (1001) docker     (123)    30832 2023-03-31 14:46:49.000000 sdmx1-2.8.0/doc/whatsnew.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-31 14:46:49.000000 sdmx1-2.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.841648 sdmx1-2.8.0/sdmx/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.841648 sdmx1-2.8.0/sdmx/format/
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/format/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/format/json.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/format/protobuf_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/format/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.841648 sdmx1-2.8.0/sdmx/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22849 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/model/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/model/internationalstring.py
--rw-r--r--   0 runner    (1001) docker     (123)    48720 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/model/v21.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/model/v30.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.841648 sdmx1-2.8.0/sdmx/reader/
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/reader/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/reader/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/reader/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    51337 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/reader/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.845648 sdmx1-2.8.0/sdmx/source/
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/abs.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/bbk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/estat.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/ilo.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/insee.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/istat.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/lsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/sgr.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/wb.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/source/wb_wdi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/sources.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.845648 sdmx1-2.8.0/sdmx/testing/
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/testing/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.845648 sdmx1-2.8.0/sdmx/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.845648 sdmx1-2.8.0/sdmx/tests/format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/format/test_format_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.849648 sdmx1-2.8.0/sdmx/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/model/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/model/test_internationalstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.849648 sdmx1-2.8.0/sdmx/tests/reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/reader/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/reader/test_reader_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/reader/test_reader_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/reader/test_reader_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_dataset_bare.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_dataset_ss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_dsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_insee.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.849648 sdmx1-2.8.0/sdmx/tests/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/writer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/writer/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/writer/test_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/tests/writer/test_writer_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.849648 sdmx1-2.8.0/sdmx/writer/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/writer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18301 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/writer/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/writer/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    18322 2023-03-31 14:46:49.000000 sdmx1-2.8.0/sdmx/writer/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.849648 sdmx1-2.8.0/sdmx1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-03-31 14:47:08.000000 sdmx1-2.8.0/sdmx1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-03-31 14:47:08.000000 sdmx1-2.8.0/sdmx1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 14:47:08.000000 sdmx1-2.8.0/sdmx1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-31 14:47:08.000000 sdmx1-2.8.0/sdmx1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 14:47:08.000000 sdmx1-2.8.0/sdmx1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 14:47:08.849648 sdmx1-2.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.284207 sdmx1-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-30 16:08:08.000000 sdmx1-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-30 16:08:08.000000 sdmx1-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-30 16:08:34.284207 sdmx1-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-30 16:08:08.000000 sdmx1-2.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-30 16:08:08.000000 sdmx1-2.9.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.256207 sdmx1-2.9.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.256207 sdmx1-2.9.0/doc/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/api/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/api/reader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/api/writer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/dev.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.256207 sdmx1-2.9.0/doc/howto/
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/howto/create.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/implementation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16327 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/sources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20838 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/walkthrough.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    32458 2023-04-30 16:08:08.000000 sdmx1-2.9.0/doc/whatsnew.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-30 16:08:08.000000 sdmx1-2.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.260207 sdmx1-2.9.0/sdmx/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.260207 sdmx1-2.9.0/sdmx/format/
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/format/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/format/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/format/protobuf_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/format/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.264207 sdmx1-2.9.0/sdmx/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23654 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/model/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/model/internationalstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49540 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/model/v21.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/model/v30.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.264207 sdmx1-2.9.0/sdmx/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/reader/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/reader/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/reader/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51825 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/reader/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.264207 sdmx1-2.9.0/sdmx/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/abs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/bbk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/estat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/ilo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/insee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/istat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/lsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/sgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/wb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/source/wb_wdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/sources.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.264207 sdmx1-2.9.0/sdmx/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/testing/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.272207 sdmx1-2.9.0/sdmx/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.276207 sdmx1-2.9.0/sdmx/tests/format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/format/test_format_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.276207 sdmx1-2.9.0/sdmx/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/model/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/model/test_internationalstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/model/test_v21.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.276207 sdmx1-2.9.0/sdmx/tests/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/reader/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/reader/test_reader_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/reader/test_reader_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/reader/test_reader_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_dataset_bare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_dataset_ss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_dsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_insee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19519 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16541 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.280207 sdmx1-2.9.0/sdmx/tests/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/writer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/writer/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/writer/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/writer/test_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/tests/writer/test_writer_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.280207 sdmx1-2.9.0/sdmx/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/writer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/writer/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18315 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/writer/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/writer/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-04-30 16:08:08.000000 sdmx1-2.9.0/sdmx/writer/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 16:08:34.284207 sdmx1-2.9.0/sdmx1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-30 16:08:34.000000 sdmx1-2.9.0/sdmx1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-30 16:08:34.000000 sdmx1-2.9.0/sdmx1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 16:08:34.000000 sdmx1-2.9.0/sdmx1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-30 16:08:34.000000 sdmx1-2.9.0/sdmx1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-30 16:08:34.000000 sdmx1-2.9.0/sdmx1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 16:08:34.284207 sdmx1-2.9.0/setup.cfg
```

### Comparing `sdmx1-2.8.0/LICENSE` & `sdmx1-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/PKG-INFO` & `sdmx1-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: sdmx1
-Version: 2.8.0
+Version: 2.9.0
 Summary: Statistical Data and Metadata eXchange (SDMX)
 Author: SDMX Python developers
 Maintainer-email: Paul Natsuo Kishimoto <mail@paul.kishimoto.name>
 Project-URL: homepage, https://github.com/khaeru/sdmx
 Project-URL: repository, https://github.com/khaeru/sdmx
 Project-URL: documentation, https://sdmx1.readthedocs.io/en/latest
 Keywords: statistics,SDMX,pandas,data,economics,science
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.7.2
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: cache
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 sdmx: Statistical data and metadata exchange
```

### Comparing `sdmx1-2.8.0/README.rst` & `sdmx1-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/Makefile` & `sdmx1-2.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/api/model.rst` & `sdmx1-2.9.0/doc/api/model.rst`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/api/writer.rst` & `sdmx1-2.9.0/doc/api/writer.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 .. currentmodule:: sdmx.writer
 
 Convert ``sdmx`` objects to other formats
 *****************************************
 
+.. _writer-csv:
+
+``writer.csv``: Write to SDMX-CSV
+=================================
+
+.. versionadded:: 2.9.0
+
+See :func:`.to_csv`.
+
+.. automodule:: sdmx.writer.csv
+   :members:
+   :exclude-members: to_csv
+   :show-inheritance:
+
 .. _writer-pandas:
 
 ``writer.pandas``: Convert to ``pandas`` objects
 ================================================
 
 .. currentmodule:: sdmx.writer.pandas
 
@@ -58,28 +72,26 @@
 .. automodule:: sdmx.writer.pandas
    :members: DEFAULT_RTYPE, write_dataset, write_datamessage, write_itemscheme, write_structuremessage
 
 .. todo::
    Support selection of language for conversion of
    :class:`InternationalString <sdmx.model.InternationalString>`.
 
-
 ``writer.xml``: Write to SDMX-ML
 ================================
 
 .. versionadded:: 1.1
 
 See :func:`.to_xml`.
 
 .. automodule:: sdmx.writer.xml
    :members:
    :exclude-members: to_xml
    :show-inheritance:
 
-
 Writer API
 ==========
 
 .. currentmodule:: sdmx.writer
 
 .. automodule:: sdmx.writer
    :members:
```

### Comparing `sdmx1-2.8.0/doc/api.rst` & `sdmx1-2.9.0/doc/api.rst`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 - :mod:`sdmx.model`: :doc:`api/model`.
 - :mod:`sdmx.reader`: :doc:`api/reader`.
 - :mod:`sdmx.writer`: :doc:`api/writer`.
 - :mod:`sdmx.source` on the page :doc:`sources`.
 
 See also the :doc:`implementation`.
 
-.. contents::
-   :local:
-   :backlinks: none
-
 Top-level methods and classes
 -----------------------------
 
 .. automodule:: sdmx
    :members:
 
    .. autosummary::
@@ -32,14 +28,15 @@
       Client
       Resource
       add_source
       list_sources
       log
       read_sdmx
       read_url
+      to_csv
       to_pandas
       to_xml
 
 ``format``: SDMX file formats
 -----------------------------
 
 .. automodule:: sdmx.format
```

### Comparing `sdmx1-2.8.0/doc/conf.py` & `sdmx1-2.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/dev.rst` & `sdmx1-2.9.0/doc/dev.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 
 This page describes the development of :mod:`sdmx`.
 Contributions are welcome!
 
 - For current development priorities, see the list of `GitHub milestones <https://github.com/khaeru/sdmx/milestones>`_ and issues/PRs targeted to each.
 - For wishlist features, see issues on GitHub tagged `‘enh’ <https://github.com/khaeru/sdmx/labels/enh>`_ or `‘wishlist’ <https://github.com/khaeru/sdmx/labels/wishlist>`_.
 
-.. contents::
-   :local:
-   :backlinks: none
-
 Code style
 ==========
 
 - Apply the following to new or modified code::
 
     isort -rc . && black . && mypy . && flake8
```

### Comparing `sdmx1-2.8.0/doc/example.rst` & `sdmx1-2.9.0/doc/example.rst`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/glossary.rst` & `sdmx1-2.9.0/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/howto/create.rst` & `sdmx1-2.9.0/doc/howto/create.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 
 :mod:`sdmx` was developed to retrieve SDMX-formatted data from web services and convert it to :mod:`pandas` objects.
 
 The opposite—creating SDMX messages from Python or pandas objects—is also possible.
 (Helper code to simplify this process is still a :doc:`planned future development </dev>`.)
 This page gives a minimal demonstration.
 
-.. contents::
-   :local:
-   :backlinks: none
-
-
 Create some example data
 ========================
 
 This data has:
 
 - 8 *observations*.
 - 2 *dimensions* with the identifiers (IDs) "TIME_DETAIL" and "REF_AREA".
```

### Comparing `sdmx1-2.8.0/doc/howto.rst` & `sdmx1-2.9.0/doc/howto.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 How to…
 =======
 
-.. contents::
-   :local:
-   :backlinks: none
-
 On other pages:
 
 .. toctree::
    :maxdepth: 1
 
    howto/create
 
@@ -111,15 +107,15 @@
 Select data frame layouts returned by :func:`.to_pandas`
 --------------------------------------------------------
 
 :func:`.to_pandas` provides multiple ways to customize the type and layout of pandas objects returned for :class:`.DataMessage` input.
 One is the `datetime` argument; see :ref:`datetime`.
 The other is the `rtype` argument.
 
-To select the same behaviour as pandSDMX 0.9, give `rtype` = 'compat', or set :data:`.DEFAULT_RTYPE` to 'compat':
+To select the same behaviour as pandaSDMX 0.9, give `rtype` = 'compat', or set :data:`.DEFAULT_RTYPE` to 'compat':
 
 .. ipython:: python
 
    sdmx.writer.DEFAULT_RYPE = 'compat'
 
 With 'compat', the returned layout varies with the concept of “dimension at the observation level,” as follows:
```

### Comparing `sdmx1-2.8.0/doc/implementation.rst` & `sdmx1-2.9.0/doc/implementation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,14 @@
 
 :mod:`sdmx.model` implements the SDMX :term:`information model`.
 This page gives brief explanations of **how** :mod:`sdmx` **implements the standards**, focusing on additional features, conveniences, or interpretations/naming choices that are not strictly determined by the standards.
 
 Although this page is organized to correspond to the standards, it **does not recapitulate them** (:ref:`as stated <not-the-standard>`)—nor does it set out to teach all their details.
 For those purposes, see :doc:`resources`; or the :doc:`walkthrough`, which includes some incidental explanations.
 
-.. contents::
-   :backlinks: none
-   :local:
-
 .. _sdmx-version-policy:
 
 SDMX versions 2.0, 2.1, and 3.0
 ===============================
 
 Multiple versions of the SDMX standards have been published:
```

### Comparing `sdmx1-2.8.0/doc/index.rst` & `sdmx1-2.9.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/install.rst` & `sdmx1-2.9.0/doc/install.rst`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/license.rst` & `sdmx1-2.9.0/doc/license.rst`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/make.bat` & `sdmx1-2.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/resources.rst` & `sdmx1-2.9.0/doc/resources.rst`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/doc/sources.rst` & `sdmx1-2.9.0/doc/sources.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,14 @@
 
 :mod:`sdmx` identifies each data source using a string such as ``'ABS'``, and has built-in support for a number of data sources.
 Use :meth:`list_sources` to list these.
 Read the following sections, or the file :file:`sources.json` in the package source code, for more details.
 
 :mod:`sdmx` also supports adding other data sources; see :meth:`add_source` and :class:`~.source.Source`.
 
-.. contents::
-   :local:
-   :backlinks: none
-
-
 Data source limitations
 -----------------------
 
 Each SDMX web service provides a subset of the full SDMX feature set, so the same request made to two different sources may yield different results, or an error message.
 In order to anticipate and handle these differences:
 
 1. :meth:`add_source` accepts "data_content_type" and "supported" keys. For
```

### Comparing `sdmx1-2.8.0/doc/walkthrough.rst` & `sdmx1-2.9.0/doc/walkthrough.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 Walkthrough
 ***********
 
 This page walks through an example :mod:`sdmx` workflow, providing explanations of some SDMX concepts along the way.
 See also :doc:`resources`, :doc:`HOWTOs <howto>` for miscellaneous tasks, and follow links to the :doc:`glossary` where some terms are explained.
 
-.. contents::
-   :local:
-   :backlinks: none
-
-
 SDMX workflow
 =============
 
 Working with statistical data often includes some or all of the following steps.
 :mod:`sdmx` builds on SDMX features to make the steps straightforward:
 
 1. Choose a data provider.
```

### Comparing `sdmx1-2.8.0/doc/whatsnew.rst` & `sdmx1-2.9.0/doc/whatsnew.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,39 @@
 :tocdepth: 2
 
 What's new?
 ***********
 
-.. contents::
-   :local:
-   :backlinks: none
-   :depth: 1
-
 .. Next release
 .. ============
 
+v2.9.0 (2023-04-30)
+===================
+
+- Add :func:`.to_csv` (:mod:`.writer.csv`) to generate SDMX-CSV 1.0 (corresponding to SDMX 2.1) representation of :class:`DataSets <.DataSet>` (:issue:`36`, :pull:`125`).
+- Information Model classes (:pull:`125`):
+
+  - Add :meth:`.AnnotableArtefact.eval_annotation`, which can be used to retrieve Python data structures stored using :func:`repr` as :attr:`.Annotation.text` on an object.
+  - Implement :meth:`.KeyValue.__lt__`, for use with Python :func:`.sorted`.
+  - Implement :meth:`.DataSet.__str__`.
+    The previous default string representation included the representation of *every* observation in the data set, which could be excessively verbose.
+    Use ``repr(ds)`` explicitly if this is desired.
+  - :meth:`.ComponentList.append` (thus also child classes including :class:`.DimensionDescriptor`) now sets :attr:`.DimensionComponent.order` on the appended components (dimensions), if not already set.
+  - Add :meth:`.ComponentList.extend`.
+
+- :mod:`sdmx.writer.xml` (:pull:`125`):
+
+  - Write :attr:`.DataSet.attrib`, i.e. :class:`AttributeValue` attached directly to a data set, rather than to its contents.
+  - Write :class:`.Contact`, e.g. within an :class:`.AgencyScheme`.
+
+- Bugfix: correctly handle ``&detail=referencepartial`` REST query parameter and :class:`.StructureMessage` containing ≥2 :class:`.MaintainableArtefact` with the same maintainer and ID, but different versions (:issue:`116`, :pull:`124`).
+  See the documentation for :mod:`.reader.xml`.
+- :mod:`sdmx` is fully compatible with pandas 2.0.0, released 2023-04-03 (:pull:`124`).
+  The minimum version of Python is increased from 3.7 (EOL 2023-06-27) to 3.8.
+
 v2.8.0 (2023-03-31)
 ===================
 
 Migration notes
 ---------------
 
 In order to prepare for future support of SDMX 3.0, code such as the following will emit a :class:`DeprecationWarning`:
```

### Comparing `sdmx1-2.8.0/pyproject.toml` & `sdmx1-2.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,23 +23,22 @@
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Financial and Insurance Industry",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering",
   "Topic :: Scientific/Engineering :: Information Analysis",
 ]
-requires-python = ">=3.7.2"
+requires-python = ">=3.8"
 dependencies = [
   "lxml >= 3.6",
   "pandas >= 1.0",
   "pydantic >= 1.9.2",
   "python-dateutil",
   "requests >= 2.7",
   "typing_extensions",
```

### Comparing `sdmx1-2.8.0/sdmx/client.py` & `sdmx1-2.9.0/sdmx/client.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/experimental.py` & `sdmx1-2.9.0/sdmx/experimental.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/format/__init__.py` & `sdmx1-2.9.0/sdmx/format/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/format/xml.py` & `sdmx1-2.9.0/sdmx/format/xml.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/message.py` & `sdmx1-2.9.0/sdmx/message.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/model/__init__.py` & `sdmx1-2.9.0/sdmx/model/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     AnnotableArtefact,
     Categorisation,
     Category,
     CategoryScheme,
     Concept,
     ConceptScheme,
     ConstraintRoleType,
+    Contact,
     IdentifiableArtefact,
     Item,
     ItemScheme,
     MaintainableArtefact,
     Organisation,
     OrganisationScheme,
     Representation,
@@ -30,14 +31,15 @@
     "AnnotableArtefact",
     "Categorisation",
     "Category",
     "CategoryScheme",
     "Concept",
     "ConceptScheme",
     "ConstraintRoleType",
+    "Contact",
     "IdentifiableArtefact",
     "InternationalString",
     "Item",
     "ItemScheme",
     "MaintainableArtefact",
     "Organisation",
     "OrganisationScheme",
```

### Comparing `sdmx1-2.8.0/sdmx/model/common.py` & `sdmx1-2.9.0/sdmx/model/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 # Utility classes not specified in the SDMX standard
 
 
 class _MissingID(str):
     def __str__(self):
         return "(missing id)"
 
+    def __hash__(self):
+        return hash(None)
+
     def __eq__(self, other):
         return isinstance(other, self.__class__)
 
 
 MissingID = _MissingID()
 
 
@@ -92,22 +95,41 @@
         """
         for i, anno in enumerate(self.annotations):
             if all(getattr(anno, key, None) == value for key, value in attrib.items()):
                 return self.annotations.pop(i)
 
         raise KeyError(attrib)
 
+    def eval_annotation(self, id: str, globals=None):
+        """Retrieve the annotation with the given `id` and :func:`eval` its contents.
+
+        This can be used for unpacking Python values (e.g. :class:`dict`) stored as an
+        annotation on an AnnotableArtefact (e.g. :class:`~sdmx.model.Code`).
+
+        Returns :obj:`None` if no attribute exists with the given `id`.
+        """
+        try:
+            value = str(self.get_annotation(id=id).text)
+        except KeyError:  # No such attribute
+            return None
+
+        try:
+            return eval(value, globals or {})
+        except Exception as e:  # Something that can't be eval()'d, e.g. a plain string
+            log.debug(f"Could not eval({value!r}): {e}")
+            return value
+
 
 class IdentifiableArtefact(AnnotableArtefact):
     #: Unique identifier of the object.
     id: str = MissingID
     #: Universal resource identifier that may or may not be resolvable.
     uri: Optional[str] = None
-    #: Universal resource name. For use in SDMX registries; all registered
-    #: objects have a URN.
+    #: Universal resource name. For use in SDMX registries; all registered objects have
+    #: a URN.
     urn: Optional[str] = None
 
     urn_group: Dict = dict()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -268,16 +290,15 @@
 
 class MaintainableArtefact(VersionableArtefact):
     #: True if the object is final; otherwise it is in a draft state.
     is_final: Optional[bool] = None
     #: :obj:`True` if the content of the object is held externally; i.e., not
     #: the current :class:`Message`.
     is_external_reference: Optional[bool] = None
-    #: URL of an SDMX-compliant web service from which the object can be
-    #: retrieved.
+    #: URL of an SDMX-compliant web service from which the object can be retrieved.
     service_url: Optional[str] = None
     #: URL of an SDMX-ML document containing the object.
     structure_url: Optional[str] = None
     #: Association to the Agency responsible for maintaining the object.
     maintainer: Optional["Agency"] = None
 
     def __init__(self, **kwargs):
```

### Comparing `sdmx1-2.8.0/sdmx/model/internationalstring.py` & `sdmx1-2.9.0/sdmx/model/internationalstring.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/model/v21.py` & `sdmx1-2.9.0/sdmx/model/v21.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
-from warnings import warn
 
 from sdmx.rest import Resource
 from sdmx.util import (
     BaseModel,
     DictLike,
     compare,
     dictlike_field,
@@ -126,26 +125,34 @@
 
 CT = TypeVar("CT", bound=Component)
 
 
 class ComponentList(IdentifiableArtefact, Generic[CT]):
     #:
     components: List[CT] = []
-    #:
+    #: Counter used to automatically populate :attr:`.DimensionComponent.order` values.
     auto_order = 1
 
     # The default type of the Components in the ComponentList. See comment on
     # ItemScheme._Item
     _Component: Type = Component
 
     # Convenience access to the components
-    def append(self, value: CT):
+    def append(self, value: CT) -> None:
         """Append *value* to :attr:`components`."""
+        if hasattr(value, "order") and value.order is None:
+            value.order = max(self.auto_order, len(self.components) + 1)
+            self.auto_order = value.order + 1
         self.components.append(value)
 
+    def extend(self, values: Iterable[CT]) -> None:
+        """Extend :attr:`components` with *values*."""
+        for value in values:
+            self.append(value)
+
     def get(self, id) -> CT:
         """Return the component with the given *id*."""
         # Search for an existing Component
         for c in self.components:
             if c.id == id:
                 return c
         raise KeyError(id)
@@ -481,27 +488,25 @@
     content: Set[ConstrainableArtefact] = set()
     # metadata_content_region: MetadataTargetRegion = None
 
     def __contains__(self, value):
         if self.data_content_region:
             return all(value in cr for cr in self.data_content_region)
         else:
-            raise NotImplementedError(
-                "ContentConstraint does not contain a CubeRegion."
-            )
+            raise NotImplementedError("ContentConstraint does not contain a CubeRegion")
 
     def to_query_string(self, structure):
         cr_count = len(self.data_content_region)
         try:
             if cr_count > 1:
-                warn(f"to_query_string() using first of {cr_count} " "CubeRegions.")
+                log.warning(f"to_query_string() using first of {cr_count} CubeRegions")
 
             return self.data_content_region[0].to_query_string(structure)
         except IndexError:
-            raise RuntimeError("ContentConstraint does not contain a CubeRegion.")
+            raise RuntimeError("ContentConstraint does not contain a CubeRegion")
 
     def iter_keys(
         self,
         obj: Union["DataStructureDefinition", "DataflowDefinition"],
         dims: List[str] = [],
     ) -> Generator["Key", None, None]:
         """Iterate over keys.
@@ -539,15 +544,15 @@
     pass
 
 
 class _NoSpecifiedRelationship(AttributeRelationship):
     pass
 
 
-#: A singleton.
+#: A singleton. Indicates that the attribute is attached to the entire data set.
 NoSpecifiedRelationship = _NoSpecifiedRelationship()
 
 
 class _PrimaryMeasureRelationship(AttributeRelationship):
     pass
 
 
@@ -996,22 +1001,31 @@
 
     def __eq__(self, other):
         """Compare the value to a simple Python built-in type or other key-like.
 
         `other` may be :class:`.KeyValue` or :class:`.ComponentValue`; if so, and both
         `self` and `other` have :attr:`.value_for`, these must refer to the same object.
         """
+        other_value = self._compare_value(other)
+        result = self.value == other_value
         if isinstance(other, (KeyValue, ComponentValue)):
-            return (self.value == other.value) and (
+            result &= (
                 self.value_for in (None, other.value_for) or other.value_for is None
             )
-        elif isinstance(other, MemberValue):
-            return self.value == other.value
+        return result
+
+    @staticmethod
+    def _compare_value(other):
+        if isinstance(other, (KeyValue, ComponentValue, MemberValue)):
+            return other.value
         else:
-            return self.value == other
+            return other
+
+    def __lt__(self, other):
+        return self.value < self._compare_value(other)
 
     def __str__(self):
         return "{0.id}={0.value}".format(self)
 
     def __repr__(self):
         return "<{0.__class__.__name__}: {0.id}={0.value}>".format(self)
 
@@ -1281,16 +1295,16 @@
         return view
 
 
 @validate_dictlike
 class Observation(BaseModel):
     """SDMX 2.1 Observation.
 
-    This class also implements the spec classes ObservationValue,
-    UncodedObservationValue, and CodedObservation.
+    This class also implements the IM classes ObservationValue, UncodedObservationValue,
+    and CodedObservation.
     """
 
     #:
     attached_attribute: DictLike[str, AttributeValue] = dictlike_field()
     #:
     series_key: Optional[SeriesKey] = None
     #: Key for dimension(s) varying at the observation level.
@@ -1422,14 +1436,20 @@
     @validator("action")
     def _validate_action(cls, value):
         if value in ActionType:
             return value
         else:
             return ActionType[value]
 
+    def __str__(self):
+        return (
+            f"<DataSet structured_by={self.structured_by!r} with {len(self)} "
+            "observations>"
+        )
+
     def compare(self, other, strict=True):
         """Return :obj:`True` if `self` is the same as `other`.
 
         Two DataSets are the same if:
 
         - their :attr:`action`, :attr:`valid_from` compare equal.
         - all dataset-level attached attributes compare equal.
```

### Comparing `sdmx1-2.8.0/sdmx/reader/__init__.py` & `sdmx1-2.9.0/sdmx/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/reader/base.py` & `sdmx1-2.9.0/sdmx/reader/base.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/reader/json.py` & `sdmx1-2.9.0/sdmx/reader/json.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/reader/xml.py` & `sdmx1-2.9.0/sdmx/reader/xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""SDMXML v2.1 reader."""
+"""SDMX-ML v2.1 reader."""
 # Contents of this file are organized in the order:
 #
 # - Utility methods and global variables.
 # - Reference and Reader classes.
 # - Parser functions for sdmx.message classes, in the same order as message.py
 # - Parser functions for sdmx.model classes, in the same order as model.py
 
@@ -363,35 +363,42 @@
         for s, values in (self.pop_single("_stash") or {}).items():
             self.stack[s].update(values)
 
     def get_single(
         self,
         cls_or_name: Union[Type, str],
         id: Optional[str] = None,
+        version: Optional[str] = None,
         subclass: bool = False,
     ) -> Optional[Any]:
         """Return a reference to an object while leaving it in its stack.
 
         Always returns 1 object. Returns :obj:`None` if no matching object exists, or if
         2 or more objects meet the conditions.
 
-        If `id` is given, only return an IdentifiableArtefact with the matching ID.
+        If `id` (and `version`) is/are given, only return an IdentifiableArtefact with
+        the matching ID (and version).
 
         If `cls_or_name` is a class and `subclass` is :obj:`True`; check all objects in
         the stack `cls_or_name` *or any stack for a subclass of this class*.
         """
         if subclass:
             keys: Iterable[Union[Type, str]] = filter(
                 matching_class(cls_or_name), self.stack.keys()
             )
             results: Mapping = ChainMap(*[self.stack[k] for k in keys])
         else:
             results = self.stack.get(cls_or_name, dict())
 
-        if id:
+        if id and version:
+            for v in results.values():
+                if v.id == id and v.version == version:
+                    return v
+            return None
+        elif id:
             return results.get(id)
         elif len(results) != 1:
             # 0 or ≥2 results
             return None
         else:
             return next(iter(results.values()))
 
@@ -434,15 +441,17 @@
     def resolve(self, ref):
         """Resolve the Reference instance `ref`, returning the referred object."""
         if not isinstance(ref, Reference):
             # None, already resolved, or not a Reference
             return ref
 
         # Try to get the target directly
-        target = self.get_single(ref.target_cls, ref.target_id, subclass=True)
+        target = self.get_single(
+            ref.target_cls, ref.target_id, ref.version, subclass=True
+        )
 
         if target:
             return target
 
         # MaintainableArtefact with is_external_reference=True; either a new object, or
         # reference to an existing object
         target_or_parent = self.maintainable(
@@ -755,26 +764,35 @@
         ("constraint", model.ContentConstraint),
         ("dataflow", model.DataflowDefinition),
         ("metadataflow", model.MetadataflowDefinition),
         ("organisation_scheme", model.OrganisationScheme),
         ("provisionagreement", model.ProvisionAgreement),
         ("structure", model.DataStructureDefinition),
     ):
-        for obj in reader.pop_all(name, subclass=True):
-            target = getattr(msg, attr)
-            if obj.id not in target:
-                # Store using ID alone
-                target[obj.id] = obj
-            else:
-                # ID already exists; this occurs when two MaintainableArtefacts have the
-                # same ID, but different maintainers. Re-store using IDs that will be
-                # unique
-                existing = target.pop(obj.id)
-                target[f"{existing.maintainer.id}:{existing.id}"] = existing
-                target[f"{obj.maintainer.id}:{obj.id}"] = obj
+        target = getattr(msg, attr)
+
+        # Store using maintainer, ID, and version
+        tmp = {
+            (getattr(obj.maintainer, "id", None), obj.id, obj.version): obj
+            for obj in reader.pop_all(name, subclass=True)
+        }
+
+        # Construct string IDs
+        if len(set(k[0:2] for k in tmp.keys())) < len(tmp):
+            # Some non-unique (maintainer ID, object ID) pairs; include version
+            id_expr = "{0}:{1}({2})"
+        elif len(set(k[1] for k in tmp.keys())) < len(tmp):
+            # Some non-unique object IDs; include maintainer ID
+            id_expr = "{0}:{1}"
+        else:
+            # Only object ID
+            id_expr = "{1}"
+
+        for k, obj in tmp.items():
+            target[id_expr.format(*k)] = obj
 
 
 # Parsers for sdmx.model classes
 # §3.2: Base structures
 
 
 @end(
@@ -902,15 +920,15 @@
 @end(
     "str:AgencyScheme str:Codelist str:ConceptScheme str:CategoryScheme "
     "str:DataConsumerScheme str:DataProviderScheme",
 )
 def _itemscheme(reader, elem):
     cls = class_for_tag(elem.tag)
 
-    is_ = reader.maintainable(cls, elem)
+    is_ = reader.maintainable(cls, elem, is_partial=elem.attrib.get("isPartial"))
 
     # Iterate over all Item objects *and* their children
     iter_all = chain(*[iter(item) for item in reader.pop_all(cls._Item)])
 
     # Set of objects already added to `items`
     seen = dict()
```

### Comparing `sdmx1-2.8.0/sdmx/rest.py` & `sdmx1-2.9.0/sdmx/rest.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/session.py` & `sdmx1-2.9.0/sdmx/session.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/source/__init__.py` & `sdmx1-2.9.0/sdmx/source/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import importlib.resources
 import json
 from enum import Enum
 from importlib import import_module
-from io import IOBase, TextIOWrapper
+from io import IOBase
 from typing import Any, Dict, Optional, Tuple, Union
 
-from pkg_resources import resource_stream
 from requests import Response
 
 from sdmx.model.v21 import DataStructureDefinition
 from sdmx.rest import Resource
 from sdmx.util import BaseModel, validator
 
 sources: Dict[str, "Source"] = {}
@@ -217,14 +217,21 @@
     These can be used to create :class:`Client` instances.
     """
     return sorted(sources.keys())
 
 
 def load_package_sources():
     """Discover all sources listed in :file:`sources.json`."""
-    with resource_stream("sdmx", "sources.json") as f:
-        # TextIOWrapper is for Python 3.5 compatibility
-        for info in json.load(TextIOWrapper(f)):
+    try:
+        ref = importlib.resources.files("sdmx").joinpath("sources.json")
+    except AttributeError:  # Python <3.9
+        from copy import copy
+
+        with importlib.resources.path("sdmx", "sources.json") as path:
+            ref = copy(path)
+
+    with ref.open("rb") as f:
+        for info in json.load(f):
             add_source(info)
 
 
 load_package_sources()
```

### Comparing `sdmx1-2.8.0/sdmx/source/abs.py` & `sdmx1-2.9.0/sdmx/source/abs.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/source/bbk.py` & `sdmx1-2.9.0/sdmx/source/bbk.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/source/estat.py` & `sdmx1-2.9.0/sdmx/source/estat.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/source/ilo.py` & `sdmx1-2.9.0/sdmx/source/ilo.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/source/insee.py` & `sdmx1-2.9.0/sdmx/source/insee.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/source/istat.py` & `sdmx1-2.9.0/sdmx/source/istat.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/source/sgr.py` & `sdmx1-2.9.0/sdmx/source/sgr.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/source/wb_wdi.py` & `sdmx1-2.9.0/sdmx/source/wb_wdi.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/sources.json` & `sdmx1-2.9.0/sdmx/sources.json`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/testing/__init__.py` & `sdmx1-2.9.0/sdmx/testing/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,15 @@
 
         # Miscellaneous XML structure files
         specimens.extend(
             (base_path.joinpath(*parts), "xml", "structure")
             for parts in [
                 ("ECB", "orgscheme.xml"),
                 ("ESTAT", "apro_mk_cola-structure.xml"),
+                ("ESTAT", "GOV_10Q_GGNFA.xml"),
                 ("IMF", "1PI-structure.xml"),
                 # Manually reduced subset of the response for this DSD. Test for
                 # <str:CubeRegion> containing both <com:KeyValue> and <com:Attribute>
                 ("IMF", "ECOFIN_DSD-structure.xml"),
                 ("INSEE", "CNA-2010-CONSO-SI-A17-structure.xml"),
                 ("INSEE", "dataflow.xml"),
                 ("INSEE", "IPI-2010-A21-structure.xml"),
```

### Comparing `sdmx1-2.8.0/sdmx/testing/report.py` & `sdmx1-2.9.0/sdmx/testing/report.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/__init__.py` & `sdmx1-2.9.0/sdmx/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/model/test_internationalstring.py` & `sdmx1-2.9.0/sdmx/tests/model/test_internationalstring.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/reader/test_base.py` & `sdmx1-2.9.0/sdmx/tests/reader/test_base.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/reader/test_reader_csv.py` & `sdmx1-2.9.0/sdmx/tests/reader/test_reader_csv.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/reader/test_reader_xml.py` & `sdmx1-2.9.0/sdmx/tests/reader/test_reader_xml.py`

 * *Files 16% similar despite different names*

```diff
@@ -97,14 +97,42 @@
     assert re.match(
         r"Use provided <DataStructureDefinition IT1:FOO\(1\.0\): .* for "
         'structureRef="IT1_DCIS_POPRES1_1_0" not defined in message',
         caplog.messages[-1],
     )
 
 
+def test_gh_116(specimen):
+    """Test of https://github.com/khaeru/sdmx/issues/116.
+
+    See also
+    --------
+    .test_sources.TestESTAT.test_gh_116
+    """
+    with specimen("ESTAT/GOV_10Q_GGNFA.xml") as f:
+        msg = sdmx.read_sdmx(f)
+
+    # Both versions of the GEO codelist are accessible in the message
+    cl1 = msg.codelist["ESTAT:GEO(13.0)"]
+    cl2 = msg.codelist["ESTAT:GEO(13.1)"]
+
+    # cl1 is complete and items are available
+    assert not cl1.is_partial and 0 < len(cl1)
+    # cl2 is partial, and fewer codes are included than in cl1
+    assert cl2.is_partial and 0 < len(cl2) < len(cl1)
+
+    cl3 = msg.codelist["ESTAT:UNIT(15.1)"]
+    cl4 = msg.codelist["ESTAT:UNIT(15.2)"]
+
+    # cl3 is complete and items are available
+    assert not cl3.is_partial and 0 < len(cl3)
+    # cl4 is partial, and fewer codes are included than in cl1
+    assert cl4.is_partial and 0 < len(cl4) < len(cl3)
+
+
 # Each entry is a tuple with 2 elements:
 # 1. an instance of lxml.etree.Element to be parsed.
 # 2. Either:
 #   - A sdmx.model object, in which case the parsed element must match the object.
 #   - A string, in which case parsing the element is expected to fail, raising an
 #     exception matching the string.
 ELEMENTS = [
```

### Comparing `sdmx1-2.8.0/sdmx/tests/test_client.py` & `sdmx1-2.9.0/sdmx/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_compat.py` & `sdmx1-2.9.0/sdmx/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_dataset.py` & `sdmx1-2.9.0/sdmx/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_dataset_bare.py` & `sdmx1-2.9.0/sdmx/tests/test_dataset_bare.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_dataset_ss.py` & `sdmx1-2.9.0/sdmx/tests/test_dataset_ss.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_docs.py` & `sdmx1-2.9.0/sdmx/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_dsd.py` & `sdmx1-2.9.0/sdmx/tests/test_dsd.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_experimental.py` & `sdmx1-2.9.0/sdmx/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_format.py` & `sdmx1-2.9.0/sdmx/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_insee.py` & `sdmx1-2.9.0/sdmx/tests/test_insee.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_message.py` & `sdmx1-2.9.0/sdmx/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_model.py` & `sdmx1-2.9.0/sdmx/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_performance.py` & `sdmx1-2.9.0/sdmx/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_reader.py` & `sdmx1-2.9.0/sdmx/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_rest.py` & `sdmx1-2.9.0/sdmx/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_session.py` & `sdmx1-2.9.0/sdmx/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_source.py` & `sdmx1-2.9.0/sdmx/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_sources.py` & `sdmx1-2.9.0/sdmx/tests/test_sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,14 +203,43 @@
                 dsd=dsd,
                 # commented: for debugging
                 # tofile="temp.xml",
             )
         )
         client.data(**args)
 
+    @pytest.mark.network
+    def test_gh_116(self, caplog, cache_path, client):
+        """Test of https://github.com/khaeru/sdmx/issues/116.
+
+        See also
+        --------
+        .test_reader_xml.test_gh_116
+        """
+        msg = client.get(
+            "dataflow", "GOV_10Q_GGNFA", params=dict(detail="referencepartial")
+        )
+
+        # Both versions of the GEO codelist are accessible in the message
+        cl1 = msg.codelist["ESTAT:GEO(13.0)"]
+        cl2 = msg.codelist["ESTAT:GEO(13.1)"]
+
+        # cl1 is complete and items are available
+        assert not cl1.is_partial and 0 < len(cl1)
+        # cl2 is partial, and fewer codes are included than in cl1
+        assert cl2.is_partial and 0 < len(cl2) < len(cl1)
+
+        cl3 = msg.codelist["ESTAT:UNIT(15.1)"]
+        cl4 = msg.codelist["ESTAT:UNIT(15.2)"]
+
+        # cl3 is complete and items are available
+        assert not cl3.is_partial and 0 < len(cl3)
+        # cl4 is partial, and fewer codes are included than in cl1
+        assert cl4.is_partial and 0 < len(cl4) < len(cl3)
+
 
 class TestILO(DataSourceTest):
     source_id = "ILO"
     xfail = {
         "agencyscheme": HTTPError,  # 400
         # TODO provide endpoint_args for the following 3 to select 1 or a few objects
         "codelist": HTTPError,  # 413 Client Error: Payload Too Large
```

### Comparing `sdmx1-2.8.0/sdmx/tests/test_urn.py` & `sdmx1-2.9.0/sdmx/tests/test_urn.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/test_util.py` & `sdmx1-2.9.0/sdmx/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/writer/conftest.py` & `sdmx1-2.9.0/sdmx/tests/writer/conftest.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/writer/test_pandas.py` & `sdmx1-2.9.0/sdmx/tests/writer/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/tests/writer/test_writer_xml.py` & `sdmx1-2.9.0/sdmx/tests/writer/test_writer_xml.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from sdmx import message
 from sdmx.model import v21 as m
 from sdmx.model.v21 import DataSet, DataStructureDefinition, Dimension, Key, Observation
 from sdmx.writer.xml import writer as XMLWriter
 
 log = logging.getLogger(__name__)
 
+# Fixtures
+
 
 @pytest.fixture
 def dsd():
     dsd = DataStructureDefinition()
 
     for order, id in enumerate(["FOO", "BAR", "BAZ"]):
         dsd.dimensions.append(Dimension(id=id, order=order))
@@ -36,15 +38,35 @@
                 included=True,
                 key_value={dim: m.ComponentValue(value_for=dim, value="foo0")},
             )
         ],
     )
 
 
-def test_codelist(tmp_path, codelist):
+# Test specific methods associated with specific classes
+
+
+def test_contact() -> None:
+    c = m.Contact(
+        name="John Smith", org_unit="Human Resources", telephone="+1234567890"
+    )
+
+    result = sdmx.to_xml(c, pretty_print=True)
+
+    assert result.decode().endswith(
+        """
+  <com:Name xml:lang="en">John Smith</com:Name>
+  <str:Department xml:lang="en">Human Resources</str:Department>
+  <str:Telephone>+1234567890</str:Telephone>
+</str:Contact>
+"""
+    )
+
+
+def test_codelist(codelist):
     result = sdmx.to_xml(codelist, pretty_print=True)
     print(result.decode())
 
 
 def test_DataKeySet(dks):
     """:class:`.DataKeySet` can be written to XML."""
     sdmx.to_xml(dks)
@@ -117,14 +139,17 @@
 
 
 def test_Footer(footer):
     """:class:`.Footer` can be written."""
     sdmx.to_xml(footer)
 
 
+# sdmx.message classes
+
+
 def test_structuremessage(tmp_path, structuremessage):
     result = sdmx.to_xml(structuremessage, pretty_print=True)
 
     # Message can be round-tripped to/from file
     path = tmp_path / "output.xml"
     path.write_bytes(result)
     msg = sdmx.read_sdmx(path)
```

### Comparing `sdmx1-2.8.0/sdmx/urn.py` & `sdmx1-2.9.0/sdmx/urn.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/util.py` & `sdmx1-2.9.0/sdmx/util.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/writer/base.py` & `sdmx1-2.9.0/sdmx/writer/base.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/writer/pandas.py` & `sdmx1-2.9.0/sdmx/writer/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     Observation,
     SeriesKey,
     TimeDimension,
 )
 from sdmx.util import DictLike
 from sdmx.writer.base import BaseWriter
 
-#: Default return type for :func:`write_dataset` and similar methods. Either
-#: 'compat' or 'rows'. See the ref:`HOWTO <howto-rtype>`.
+#: Default return type for :func:`write_dataset` and similar methods. Either 'compat' or
+#: 'rows'. See the ref:`HOWTO <howto-rtype>`.
 DEFAULT_RTYPE = "rows"
 
 
 writer = BaseWriter("pandas")
 
 
 def to_pandas(obj, *args, **kwargs):
@@ -64,16 +64,16 @@
         if (
             len(set(map(lambda s: s.index.name, result.values()))) == 1
             and len(result) > 1
         ):
             # Can safely concatenate these to a pd.MultiIndex'd Series.
             return pd.concat(result)
         else:
-            # The individual pd.Series are indexed by different dimensions; do
-            # not concatenate.
+            # The individual pd.Series are indexed by different dimensions; do not
+            # concatenate
             return DictLike(result)
     elif result_type == {str}:
         return pd.Series(result)
     elif result_type == {DictLike}:
         return result
     elif result_type == set():
         # No results
@@ -128,16 +128,16 @@
 def write_structuremessage(obj: message.StructureMessage, include=None, **kwargs):
     """Convert :class:`.StructureMessage`.
 
     Parameters
     ----------
     obj : .StructureMessage
     include : iterable of str or str, optional
-        One or more of the attributes of the StructureMessage (
-        'category_scheme', 'codelist', etc.) to transform.
+        One or more of the attributes of the StructureMessage ('category_scheme',
+        'codelist', etc.) to transform.
     kwargs :
         Passed to :meth:`write` for each attribute.
 
     Returns
     -------
     .DictLike
         Keys are StructureMessage attributes; values are pandas objects.
@@ -267,16 +267,16 @@
           ``value`` as the first column, and additional columns for each attribute;
         - if `datetime` is given, various layouts as described above; or
         - if `_rtype` (passed from :func:`write_datamessage`) is 'compat', various
           layouts as described in the :ref:`HOWTO <howto-rtype>`.
     :class:`pandas.Series` with :class:`pandas.MultiIndex`
         Otherwise.
     """
-    # If called directly on a DataSet (rather than a parent DataMessage),
-    # cannot determine the "dimension at observation level"
+    # If called directly on a DataSet (rather than a parent DataMessage), cannot
+    # determine the "dimension at observation level"
     rtype = kwargs.setdefault("_rtype", "rows")
 
     # Validate attributes argument
     attributes = attributes or ""
     try:
         attributes = attributes.lower()
     except AttributeError:
@@ -340,19 +340,19 @@
     if isinstance(obs_dim, list) and len(obs_dim) == 1:
         # Unwrap a length-1 list
         obs_dim = obs_dim[0]
 
     if obs_dim in (AllDimensions, None):
         pass  # Do nothing
     elif isinstance(obs_dim, TimeDimension):
-        # Don't modify *df*; only change arguments so that
-        # _maybe_convert_datetime performs the desired changes
+        # Don't modify *df*; only change arguments so that _maybe_convert_datetime
+        # performs the desired changes
         if datetime is False or datetime is True:
-            # Either datetime is not given, or True without specifying a
-            # dimension; overwrite
+            # Either datetime is not given, or True without specifying a dimension;
+            # overwrite
             datetime = obs_dim
         elif isinstance(datetime, dict):
             # Dict argument; ensure the 'dim' key is the same as obs_dim
             if datetime.setdefault("dim", obs_dim) != obs_dim:
                 msg = (
                     f"datetime={datetime} conflicts with rtype='compat' and"
                     f" {obs_dim} at observation level"
@@ -432,15 +432,15 @@
                 break
         if not param["dim"]:
             raise ValueError(f"no TimeDimension in {dims}")
 
     # Unstack all but the time dimension and convert
     other_dims = list(filter(lambda d: d != param["dim"], df.index.names))
     df = df.unstack(other_dims)
-    df.index = pd.to_datetime(df.index)
+    df.index = pd.to_datetime(df.index, format="mixed")
 
     if param["freq"]:
         # Determine frequency string, Dimension, or Attribute
         freq = param["freq"]
         if isinstance(freq, str) and freq not in prefix_mapping:
             # ID of a Dimension or Attribute
             for component in chain(_get_dims(), _get_attrs()):
```

### Comparing `sdmx1-2.8.0/sdmx/writer/protobuf.py` & `sdmx1-2.9.0/sdmx/writer/protobuf.py`

 * *Files identical despite different names*

### Comparing `sdmx1-2.8.0/sdmx/writer/xml.py` & `sdmx1-2.9.0/sdmx/writer/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """SDMXML v2.1 writer."""
 # Contents of this file are organized in the order:
 #
 # - Utility methods and global variables.
 # - writer functions for sdmx.message classes, in the same order as message.py
 # - writer functions for sdmx.model classes, in the same order as model.py
 
-from typing import Iterable, cast
+from typing import Iterable, List, cast
 
 from lxml import etree
 from lxml.builder import ElementMaker
 
 import sdmx.urn
 from sdmx import message
 from sdmx.format.xml import NS, qname, tag_for_class
@@ -226,15 +226,15 @@
     return elem
 
 
 # Writers for sdmx.model classes
 # §3.2: Base structures
 
 
-def i11lstring(obj, name):
+def i11lstring(obj, name) -> List[etree._Element]:
     """InternationalString.
 
     Returns a list of elements with name `name`.
     """
     elems = []
 
     for locale, label in obj.localizations.items():
@@ -315,14 +315,17 @@
 
     if isinstance(obj.parent, obj.__class__):
         # Reference to parent Item
         e_parent = Element("str:Parent")
         e_parent.append(Element(":Ref", id=obj.parent.id, style="Ref"))
         elem.append(e_parent)
 
+    if isinstance(obj, model.Organisation):
+        elem.extend(writer.recurse(c) for c in obj.contact)
+
     return elem
 
 
 @writer
 def _is(obj: model.ItemScheme):
     elem = maintainable(obj)
 
@@ -360,14 +363,31 @@
 
     if obj.core_representation:
         elem.append(writer.recurse(obj.core_representation, "CoreRepresentation"))
 
     return elem
 
 
+# §4.6: Organisations
+
+
+@writer
+def _contact(obj: model.Contact):
+    elem = Element("str:Contact")
+    elem.extend(
+        i11lstring(obj.name, "com:Name")
+        + i11lstring(obj.org_unit, "str:Department")
+        + i11lstring(obj.responsibility, "str:Role")
+        + ([Element("str:Telephone", obj.telephone)] if obj.telephone else [])
+        + [Element("str:URI", text=value) for value in obj.uri]
+        + [Element("str:Email", text=value) for value in obj.email]
+    )
+    return elem
+
+
 # §3.3: Basic Inheritance
 
 
 @writer
 def _component(obj: model.Component):
     elem = identifiable(obj)
     if obj.concept_identity:
@@ -617,14 +637,18 @@
     attrib = dict()
     if obj.action:
         attrib["action"] = str(obj.action)
     if obj.structured_by:
         attrib["structureRef"] = obj.structured_by.id
     elem = Element("mes:DataSet", **attrib)
 
+    # AttributeValues attached to the data set
+    if len(obj.attrib):
+        elem.append(_av("gen:Attributes", obj.attrib.values()))
+
     obs_to_write = set(map(id, obj.obs))
 
     struct_spec = isinstance(
         obj, (model.StructureSpecificDataSet, model.StructureSpecificTimeSeriesDataSet)
     )
 
     for sk, observations in obj.series.items():
```

### Comparing `sdmx1-2.8.0/sdmx1.egg-info/PKG-INFO` & `sdmx1-2.9.0/sdmx1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: sdmx1
-Version: 2.8.0
+Version: 2.9.0
 Summary: Statistical Data and Metadata eXchange (SDMX)
 Author: SDMX Python developers
 Maintainer-email: Paul Natsuo Kishimoto <mail@paul.kishimoto.name>
 Project-URL: homepage, https://github.com/khaeru/sdmx
 Project-URL: repository, https://github.com/khaeru/sdmx
 Project-URL: documentation, https://sdmx1.readthedocs.io/en/latest
 Keywords: statistics,SDMX,pandas,data,economics,science
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.7.2
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: cache
 Provides-Extra: docs
 Provides-Extra: tests
 License-File: LICENSE
 
 sdmx: Statistical data and metadata exchange
```

### Comparing `sdmx1-2.8.0/sdmx1.egg-info/SOURCES.txt` & `sdmx1-2.9.0/sdmx1.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,26 +85,29 @@
 sdmx/tests/test_urn.py
 sdmx/tests/test_util.py
 sdmx/tests/format/__init__.py
 sdmx/tests/format/test_format_xml.py
 sdmx/tests/model/__init__.py
 sdmx/tests/model/test_common.py
 sdmx/tests/model/test_internationalstring.py
+sdmx/tests/model/test_v21.py
 sdmx/tests/reader/__init__.py
 sdmx/tests/reader/test_base.py
 sdmx/tests/reader/test_reader_csv.py
 sdmx/tests/reader/test_reader_json.py
 sdmx/tests/reader/test_reader_xml.py
 sdmx/tests/writer/__init__.py
 sdmx/tests/writer/conftest.py
+sdmx/tests/writer/test_csv.py
 sdmx/tests/writer/test_pandas.py
 sdmx/tests/writer/test_protobuf.py
 sdmx/tests/writer/test_writer_xml.py
 sdmx/writer/__init__.py
 sdmx/writer/base.py
+sdmx/writer/csv.py
 sdmx/writer/pandas.py
 sdmx/writer/protobuf.py
 sdmx/writer/xml.py
 sdmx1.egg-info/PKG-INFO
 sdmx1.egg-info/SOURCES.txt
 sdmx1.egg-info/dependency_links.txt
 sdmx1.egg-info/requires.txt
```

