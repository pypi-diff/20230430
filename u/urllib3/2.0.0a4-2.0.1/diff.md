# Comparing `tmp/urllib3-2.0.0a4.tar.gz` & `tmp/urllib3-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Apr 25 18:20:53 2023, max compression
+gzip compressed data, last modified: Sun Apr 30 06:04:47 2023, max compression
```

## Comparing `urllib3-2.0.0a4.tar` & `urllib3-2.0.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0    59335 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/CHANGES.rst
--rw-r--r--   0        0        0      328 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dev-requirements.txt
--rw-r--r--   0        0        0     4602 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/Makefile
--rw-r--r--   0        0        0    21359 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/advanced-usage.rst
--rw-r--r--   0        0        0       59 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/changelog.rst
--rw-r--r--   0        0        0     3795 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/conf.py
--rw-r--r--   0        0        0     9500 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/contributing.rst
--rw-r--r--   0        0        0     3836 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/index.rst
--rw-r--r--   0        0        0     4513 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/make.bat
--rw-r--r--   0        0        0       72 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/requirements.txt
--rw-r--r--   0        0        0     3098 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/sponsors.rst
--rw-r--r--   0        0        0    16385 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/user-guide.rst
--rw-r--r--   0        0        0    12502 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/v2-migration-guide.rst
--rw-r--r--   0        0        0     1770 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/_static/banner.svg
--rw-r--r--   0        0        0     3999 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/_static/banner_github.svg
--rw-r--r--   0        0        0     1818 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/_static/dark-logo.svg
--rw-r--r--   0        0        0     7872 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/images/demo-button.png
--rw-r--r--   0        0        0      714 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/images/favicon.png
--rw-r--r--   0        0        0     6226 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/images/learn-more-button.png
--rw-r--r--   0        0        0     2165 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/images/logo.png
--rw-r--r--   0        0        0      516 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/images/logo.svg
--rw-r--r--   0        0        0      226 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/index.rst
--rw-r--r--   0        0        0      316 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.connection.rst
--rw-r--r--   0        0        0      408 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.connectionpool.rst
--rw-r--r--   0        0        0      185 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.exceptions.rst
--rw-r--r--   0        0        0      350 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.fields.rst
--rw-r--r--   0        0        0      338 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.poolmanager.rst
--rw-r--r--   0        0        0       71 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.request.rst
--rw-r--r--   0        0        0      788 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.response.rst
--rw-r--r--   0        0        0      555 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/urllib3.util.rst
--rw-r--r--   0        0        0      233 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/contrib/index.rst
--rw-r--r--   0        0        0      295 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/contrib/pyopenssl.rst
--rw-r--r--   0        0        0     1431 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/contrib/securetransport.rst
--rw-r--r--   0        0        0      124 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/docs/reference/contrib/socks.rst
--rw-r--r--   0        0        0        0 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/__init__.py
--rw-r--r--   0        0        0    13109 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/handlers.py
--rwxr-xr-x   0        0        0     1198 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/https_proxy.py
--rwxr-xr-x   0        0        0     5420 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/proxy.py
--rwxr-xr-x   0        0        0     9839 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/server.py
--rw-r--r--   0        0        0    11171 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/testcase.py
--rw-r--r--   0        0        0      511 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/certs/README.rst
--rw-r--r--   0        0        0     1679 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/certs/cacert.key
--rw-r--r--   0        0        0     1273 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/certs/cacert.pem
--rw-r--r--   0        0        0     1265 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/certs/server.crt
--rw-r--r--   0        0        0     1679 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/dummyserver/certs/server.key
--rw-r--r--   0        0        0     5028 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/__init__.py
--rw-r--r--   0        0        0     5651 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/_base_connection.py
--rw-r--r--   0        0        0    15561 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/_collections.py
--rw-r--r--   0        0        0     7756 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/_request_methods.py
--rw-r--r--   0        0        0      100 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/_version.py
--rw-r--r--   0        0        0    33299 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/connection.py
--rw-r--r--   0        0        0    42961 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9289 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/exceptions.py
--rw-r--r--   0        0        0    11026 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/fields.py
--rw-r--r--   0        0        0     2395 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/filepost.py
--rw-r--r--   0        0        0    22160 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/py.typed
--rw-r--r--   0        0        0    39725 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/response.py
--rw-r--r--   0        0        0        0 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0    19437 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34121 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7715 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    14452 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    16220 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0     1051 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4462 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/connection.py
--rw-r--r--   0        0        0     1148 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8111 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/request.py
--rw-r--r--   0        0        0     3374 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/response.py
--rw-r--r--   0        0        0    18375 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/retry.py
--rw-r--r--   0        0        0    18540 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5812 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     9045 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10529 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/timeout.py
--rw-r--r--   0        0        0    15213 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/src/urllib3/util/wait.py
--rw-r--r--   0        0        0    10763 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/__init__.py
--rw-r--r--   0        0        0    11211 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/conftest.py
--rw-r--r--   0        0        0     6222 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/port_helpers.py
--rw-r--r--   0        0        0    13035 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_collections.py
--rw-r--r--   0        0        0      692 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_compatibility.py
--rw-r--r--   0        0        0     9484 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_connection.py
--rw-r--r--   0        0        0    22772 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_connectionpool.py
--rw-r--r--   0        0        0     2164 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_exceptions.py
--rw-r--r--   0        0        0     4438 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_fields.py
--rw-r--r--   0        0        0     3751 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_filepost.py
--rw-r--r--   0        0        0      978 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_no_ssl.py
--rw-r--r--   0        0        0    17765 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_poolmanager.py
--rw-r--r--   0        0        0     3657 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_proxymanager.py
--rw-r--r--   0        0        0      761 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_queue_monkeypatch.py
--rw-r--r--   0        0        0    44750 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_response.py
--rw-r--r--   0        0        0    16568 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_retry.py
--rw-r--r--   0        0        0     7281 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_ssl.py
--rw-r--r--   0        0        0    20750 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_ssltransport.py
--rw-r--r--   0        0        0    43233 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_util.py
--rw-r--r--   0        0        0     5999 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/test_wait.py
--rw-r--r--   0        0        0     1211 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/tz_stub.py
--rw-r--r--   0        0        0        0 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/__init__.py
--rw-r--r--   0        0        0     1257 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/duplicate_san.pem
--rw-r--r--   0        0        0     3007 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/test_pyopenssl.py
--rw-r--r--   0        0        0     1988 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/test_pyopenssl_dependencies.py
--rw-r--r--   0        0        0     1690 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/test_securetransport.py
--rw-r--r--   0        0        0    25908 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/contrib/test_socks.py
--rw-r--r--   0        0        0        0 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/__init__.py
--rw-r--r--   0        0        0    10678 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_chunked_transfer.py
--rw-r--r--   0        0        0     3827 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_connection.py
--rw-r--r--   0        0        0    56860 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_connectionpool.py
--rw-r--r--   0        0        0    43583 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_https.py
--rw-r--r--   0        0        0     1104 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_no_ssl.py
--rw-r--r--   0        0        0    22082 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_poolmanager.py
--rw-r--r--   0        0        0    33489 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_proxy_poolmanager.py
--rw-r--r--   0        0        0    84327 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/test/with_dummyserver/test_socketlevel.py
--rw-r--r--   0        0        0       85 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/.gitignore
--rw-r--r--   0        0        0     1115 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/LICENSE.txt
--rw-r--r--   0        0        0     4393 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/README.md
--rw-r--r--   0        0        0     4025 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     6572 2023-04-25 18:20:53.000000 urllib3-2.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0    58021 2023-04-30 06:04:47.000000 urllib3-2.0.1/CHANGES.rst
+-rw-r--r--   0        0        0      328 2023-04-30 06:04:47.000000 urllib3-2.0.1/dev-requirements.txt
+-rw-r--r--   0        0        0     4602 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/Makefile
+-rw-r--r--   0        0        0    21359 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/advanced-usage.rst
+-rw-r--r--   0        0        0       59 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/changelog.rst
+-rw-r--r--   0        0        0     3795 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/conf.py
+-rw-r--r--   0        0        0     9500 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/contributing.rst
+-rw-r--r--   0        0        0     3836 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/index.rst
+-rw-r--r--   0        0        0     4513 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/make.bat
+-rw-r--r--   0        0        0       72 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0     1818 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/sponsors.rst
+-rw-r--r--   0        0        0    16385 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/user-guide.rst
+-rw-r--r--   0        0        0    12502 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/v2-migration-guide.rst
+-rw-r--r--   0        0        0     1770 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/_static/banner.svg
+-rw-r--r--   0        0        0     3999 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/_static/banner_github.svg
+-rw-r--r--   0        0        0     1818 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/_static/dark-logo.svg
+-rw-r--r--   0        0        0     7872 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/images/demo-button.png
+-rw-r--r--   0        0        0      714 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/images/favicon.png
+-rw-r--r--   0        0        0     6226 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/images/learn-more-button.png
+-rw-r--r--   0        0        0     2165 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/images/logo.png
+-rw-r--r--   0        0        0      516 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/images/logo.svg
+-rw-r--r--   0        0        0      226 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/index.rst
+-rw-r--r--   0        0        0      316 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.connection.rst
+-rw-r--r--   0        0        0      408 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.connectionpool.rst
+-rw-r--r--   0        0        0      185 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.exceptions.rst
+-rw-r--r--   0        0        0      350 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.fields.rst
+-rw-r--r--   0        0        0      338 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.poolmanager.rst
+-rw-r--r--   0        0        0       71 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.request.rst
+-rw-r--r--   0        0        0      788 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.response.rst
+-rw-r--r--   0        0        0      555 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.util.rst
+-rw-r--r--   0        0        0      233 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/contrib/index.rst
+-rw-r--r--   0        0        0      295 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/contrib/pyopenssl.rst
+-rw-r--r--   0        0        0     1431 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/contrib/securetransport.rst
+-rw-r--r--   0        0        0      124 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/contrib/socks.rst
+-rw-r--r--   0        0        0        0 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/__init__.py
+-rw-r--r--   0        0        0    13109 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/handlers.py
+-rwxr-xr-x   0        0        0     1198 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/https_proxy.py
+-rwxr-xr-x   0        0        0     5420 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/proxy.py
+-rwxr-xr-x   0        0        0     9839 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/server.py
+-rw-r--r--   0        0        0    11171 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/testcase.py
+-rw-r--r--   0        0        0      511 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/certs/README.rst
+-rw-r--r--   0        0        0     1679 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/certs/cacert.key
+-rw-r--r--   0        0        0     1273 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/certs/cacert.pem
+-rw-r--r--   0        0        0     1265 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/certs/server.crt
+-rw-r--r--   0        0        0     1679 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/certs/server.key
+-rw-r--r--   0        0        0     5028 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/__init__.py
+-rw-r--r--   0        0        0     5651 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/_base_connection.py
+-rw-r--r--   0        0        0    15561 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/_collections.py
+-rw-r--r--   0        0        0     7756 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/_request_methods.py
+-rw-r--r--   0        0        0       98 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/_version.py
+-rw-r--r--   0        0        0    33511 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/connection.py
+-rw-r--r--   0        0        0    42961 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9289 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/exceptions.py
+-rw-r--r--   0        0        0    11026 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/fields.py
+-rw-r--r--   0        0        0     2395 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/filepost.py
+-rw-r--r--   0        0        0    22160 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/py.typed
+-rw-r--r--   0        0        0    39769 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/response.py
+-rw-r--r--   0        0        0        0 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0    19437 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34121 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7715 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    14452 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    16220 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0     1051 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4462 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1148 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8111 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/request.py
+-rw-r--r--   0        0        0     3374 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/response.py
+-rw-r--r--   0        0        0    18375 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/retry.py
+-rw-r--r--   0        0        0    18540 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5812 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     9045 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10529 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    15213 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10763 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/__init__.py
+-rw-r--r--   0        0        0    11211 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/conftest.py
+-rw-r--r--   0        0        0     6222 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/port_helpers.py
+-rw-r--r--   0        0        0    13035 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_collections.py
+-rw-r--r--   0        0        0      692 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_compatibility.py
+-rw-r--r--   0        0        0    10737 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_connection.py
+-rw-r--r--   0        0        0    22772 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_connectionpool.py
+-rw-r--r--   0        0        0     2164 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_exceptions.py
+-rw-r--r--   0        0        0     4438 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_fields.py
+-rw-r--r--   0        0        0     3751 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_filepost.py
+-rw-r--r--   0        0        0      978 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_no_ssl.py
+-rw-r--r--   0        0        0    17765 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_poolmanager.py
+-rw-r--r--   0        0        0     3657 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_proxymanager.py
+-rw-r--r--   0        0        0      761 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_queue_monkeypatch.py
+-rw-r--r--   0        0        0    44819 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_response.py
+-rw-r--r--   0        0        0    16568 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_retry.py
+-rw-r--r--   0        0        0     7281 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_ssl.py
+-rw-r--r--   0        0        0    20750 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_ssltransport.py
+-rw-r--r--   0        0        0    43233 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_util.py
+-rw-r--r--   0        0        0     5999 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_wait.py
+-rw-r--r--   0        0        0     1211 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/tz_stub.py
+-rw-r--r--   0        0        0        0 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/__init__.py
+-rw-r--r--   0        0        0     1257 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/duplicate_san.pem
+-rw-r--r--   0        0        0     3007 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/test_pyopenssl.py
+-rw-r--r--   0        0        0     1988 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/test_pyopenssl_dependencies.py
+-rw-r--r--   0        0        0     1690 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/test_securetransport.py
+-rw-r--r--   0        0        0    25908 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/test_socks.py
+-rw-r--r--   0        0        0        0 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/__init__.py
+-rw-r--r--   0        0        0    10678 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_chunked_transfer.py
+-rw-r--r--   0        0        0     3827 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_connection.py
+-rw-r--r--   0        0        0    56860 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_connectionpool.py
+-rw-r--r--   0        0        0    43609 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_https.py
+-rw-r--r--   0        0        0     1104 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_no_ssl.py
+-rw-r--r--   0        0        0    22082 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_poolmanager.py
+-rw-r--r--   0        0        0    33489 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_proxy_poolmanager.py
+-rw-r--r--   0        0        0    84327 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_socketlevel.py
+-rw-r--r--   0        0        0       85 2023-04-30 06:04:47.000000 urllib3-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1115 2023-04-30 06:04:47.000000 urllib3-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     4393 2023-04-30 06:04:47.000000 urllib3-2.0.1/README.md
+-rw-r--r--   0        0        0     4069 2023-04-30 06:04:47.000000 urllib3-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6621 2023-04-30 06:04:47.000000 urllib3-2.0.1/PKG-INFO
```

### Comparing `urllib3-2.0.0a4/CHANGES.rst` & `urllib3-2.0.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-2.0.0a4 (2023-04-24)
-====================
+2.0.1 (2023-04-30)
+==================
 
-- Removed the ``setup.py`` shim, ``python setup.py install`` will print ``[Errno 2] No such file or directory`` instead of a warning to use pip (`#2975 <https://github.com/urllib3/urllib3/issues/2975>`__)
-- Added optional ``backoff_jitter`` parameter to ``Retry``. (`#2952 <https://github.com/urllib3/urllib3/issues/2952>`__)
-- Fixed URL encoding by removing '!' from the 'unreserved' character set specified in RFC 3986. (`#2899 <https://github.com/urllib3/urllib3/issues/2899>`__)
-- Fixed a sign error in a check for whether a character is in the ASCII range. (`#2901 <https://github.com/urllib3/urllib3/issues/2901>`__)
-- Fixed ``urllib3.contrib.pyopenssl.WrappedSocket`` and ``urllib3.contrib.securetransport.WrappedSocket`` close methods (`#2970 <https://github.com/urllib3/urllib3/issues/2970>`__)
+Fixes
+-----
 
-2.0.0a3 (2023-01-11)
-====================
+- Fixed a socket leak when fingerprint or hostname verifications fail. (`#2991 <https://github.com/urllib3/urllib3/issues/2991>`__)
+- Fixed an error when ``HTTPResponse.read(0)`` was the first ``read`` call or when the internal response body buffer was otherwise empty. (`#2998 <https://github.com/urllib3/urllib3/issues/2998>`__)
 
-* Fix logging error when using ``add_stderr_logger``. (`#2839 <https://github.com/urllib3/urllib3/issues/2839>`__)
 
-2.0.0a2 (2022-11-23)
-====================
+2.0.0 (2023-04-26)
+==================
 
 Read the `v2.0 migration guide <https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html>`__ for help upgrading to the latest version of urllib3.
 
-* Changed ``HTTPResponse.read()`` to raise an error when calling with ``decode_content=False`` after using ``decode_content=True`` to prevent data loss (`#2800 <https://github.com/urllib3/urllib3/issues/2800>`__).
-* Changed ``HTTPResponse.getheaders()`` and ``.getheader()`` to previous behavior in 1.26.x.
-  Instead we are deprecating these methods in favor of ``HTTPResponse.headers.items()`` and ``HTTPResponse.headers.get()``. Both deprecated
-  methods will be removed in v2.1.0 (`#2814 <https://github.com/urllib3/urllib3/issues/2814>`__)
-* Fixed an issue where parsing a URL with leading zeroes in the port would be rejected
-  even when the port number after removing the zeroes was valid. (`#2806 <https://github.com/urllib3/urllib3/pull/2806>`__)
-* Fixed deprecation warning when using cryptography v39.0.0. This fix requires using pyOpenSSL>=17.1.0 and cryptography>=1.9. (`#2829 <https://github.com/urllib3/urllib3/pull/2829>`__)
+Removed
+-------
 
-2.0.0a1 (2022-11-15)
-====================
+* Removed support for Python 2.7, 3.5, and 3.6 (`#883 <https://github.com/urllib3/urllib3/issues/883>`__, `#2336 <https://github.com/urllib3/urllib3/issues/2336>`__).
+* Removed fallback on certificate ``commonName`` in ``match_hostname()`` function.
+  This behavior was deprecated in May 2000 in RFC 2818. Instead only ``subjectAltName``
+  is used to verify the hostname by default. To enable verifying the hostname against
+  ``commonName`` use ``SSLContext.hostname_checks_common_name = True`` (`#2113 <https://github.com/urllib3/urllib3/issues/2113>`__).
+* Removed support for Python with an ``ssl`` module compiled with LibreSSL, CiscoSSL,
+  wolfSSL, and all other OpenSSL alternatives. Python is moving to require OpenSSL with PEP 644 (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
+* Removed support for OpenSSL versions earlier than 1.1.1 or that don't have SNI support.
+  When an incompatible OpenSSL version is detected an ``ImportError`` is raised (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
+* Removed the list of default ciphers for OpenSSL 1.1.1+ and SecureTransport as their own defaults are already secure (`#2082 <https://github.com/urllib3/urllib3/issues/2082>`__).
+* Removed ``urllib3.contrib.appengine.AppEngineManager`` and support for Google App Engine Standard Environment (`#2044 <https://github.com/urllib3/urllib3/issues/2044>`__).
+* Removed deprecated ``Retry`` options ``method_whitelist``, ``DEFAULT_REDIRECT_HEADERS_BLACKLIST`` (`#2086 <https://github.com/urllib3/urllib3/issues/2086>`__).
+* Removed ``urllib3.HTTPResponse.from_httplib`` (`#2648 <https://github.com/urllib3/urllib3/issues/2648>`__).
+* Removed default value of ``None`` for the ``request_context`` parameter of ``urllib3.PoolManager.connection_from_pool_key``. This change should have no effect on users as the default value of ``None`` was an invalid option and was never used (`#1897 <https://github.com/urllib3/urllib3/issues/1897>`__).
+* Removed the ``urllib3.request`` module. ``urllib3.request.RequestMethods`` has been made a private API.
+  This change was made to ensure that ``from urllib3 import request`` imported the top-level ``request()``
+  function instead of the ``urllib3.request`` module (`#2269 <https://github.com/urllib3/urllib3/issues/2269>`__).
+* Removed support for SSLv3.0 from the ``urllib3.contrib.pyopenssl`` even when support is available from the compiled OpenSSL library (`#2233 <https://github.com/urllib3/urllib3/issues/2233>`__).
+* Removed the deprecated ``urllib3.contrib.ntlmpool`` module (`#2339 <https://github.com/urllib3/urllib3/issues/2339>`__).
+* Removed ``DEFAULT_CIPHERS``, ``HAS_SNI``, ``USE_DEFAULT_SSLCONTEXT_CIPHERS``, from the private module ``urllib3.util.ssl_`` (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
+* Removed ``urllib3.exceptions.SNIMissingWarning`` (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
+* Removed the ``_prepare_conn`` method from ``HTTPConnectionPool``. Previously this was only used to call ``HTTPSConnection.set_cert()`` by ``HTTPSConnectionPool`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
+* Removed ``tls_in_tls_required`` property from ``HTTPSConnection``. This is now determined from the ``scheme`` parameter in ``HTTPConnection.set_tunnel()`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
 
-Read the `v2.0 migration guide <https://urllib3.readthedocs.io/en/latest/v2-migration-guide.html>`__ for help upgrading to the latest version of urllib3.
+Deprecated
+----------
+
+* Deprecated ``HTTPResponse.getheaders()`` and ``HTTPResponse.getheader()`` which will be removed in urllib3 v2.1.0. Instead use ``HTTPResponse.headers`` and ``HTTPResponse.headers.get(name, default)``. (`#1543 <https://github.com/urllib3/urllib3/issues/1543>`__, `#2814 <https://github.com/urllib3/urllib3/issues/2814>`__).
+* Deprecated ``urllib3.contrib.pyopenssl`` module which will be removed in urllib3 v2.1.0 (`#2691 <https://github.com/urllib3/urllib3/issues/2691>`__).
+* Deprecated ``urllib3.contrib.securetransport`` module which will be removed in urllib3 v2.1.0 (`#2692 <https://github.com/urllib3/urllib3/issues/2692>`__).
+* Deprecated ``ssl_version`` option in favor of ``ssl_minimum_version``. ``ssl_version`` will be removed in urllib3 v2.1.0 (`#2110 <https://github.com/urllib3/urllib3/issues/2110>`__).
+* Deprecated the ``strict`` parameter as it's not longer needed in Python 3.x. It will be removed in urllib3 v2.1.0 (`#2267 <https://github.com/urllib3/urllib3/issues/2267>`__)
+* Deprecated the ``NewConnectionError.pool`` attribute which will be removed in urllib3 v2.1.0 (`#2271 <https://github.com/urllib3/urllib3/issues/2271>`__).
+* Deprecated ``format_header_param_html5`` and ``format_header_param`` in favor of ``format_multipart_header_param`` (`#2257 <https://github.com/urllib3/urllib3/issues/2257>`__).
+* Deprecated ``RequestField.header_formatter`` parameter which will be removed in urllib3 v2.1.0 (`#2257 <https://github.com/urllib3/urllib3/issues/2257>`__).
+* Deprecated ``HTTPSConnection.set_cert()`` method. Instead pass parameters to the ``HTTPSConnection`` constructor (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
+* Deprecated ``HTTPConnection.request_chunked()`` method which will be removed in urllib3 v2.1.0. Instead pass ``chunked=True`` to ``HTTPConnection.request()`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
+
+Added
+-----
 
+* Added top-level ``urllib3.request`` function which uses a preconfigured module-global ``PoolManager`` instance (`#2150 <https://github.com/urllib3/urllib3/issues/2150>`__).
+* Added the ``json`` parameter to ``urllib3.request()``, ``PoolManager.request()``, and ``ConnectionPool.request()`` methods to send JSON bodies in requests. Using this parameter will set the header ``Content-Type: application/json`` if ``Content-Type`` isn't already defined.
+  Added support for parsing JSON response bodies with ``HTTPResponse.json()`` method (`#2243 <https://github.com/urllib3/urllib3/issues/2243>`__).
 * Added type hints to the ``urllib3`` module (`#1897 <https://github.com/urllib3/urllib3/issues/1897>`__).
 * Added ``ssl_minimum_version`` and ``ssl_maximum_version`` options which set
   ``SSLContext.minimum_version`` and ``SSLContext.maximum_version`` (`#2110 <https://github.com/urllib3/urllib3/issues/2110>`__).
 * Added support for Zstandard (RFC 8878) when ``zstandard`` 1.18.0 or later is installed.
   Added the ``zstd`` extra which installs the ``zstandard`` package (`#1992 <https://github.com/urllib3/urllib3/issues/1992>`__).
 * Added ``urllib3.response.BaseHTTPResponse`` class. All future response classes will be subclasses of ``BaseHTTPResponse`` (`#2083 <https://github.com/urllib3/urllib3/issues/2083>`__).
-* Added top-level ``urllib3.request`` function which uses a preconfigured module-global ``PoolManager`` instance (`#2150 <https://github.com/urllib3/urllib3/issues/2150>`__).
 * Added ``FullPoolError`` which is raised when ``PoolManager(block=True)`` and a connection is returned to a full pool (`#2197 <https://github.com/urllib3/urllib3/issues/2197>`__).
 * Added ``HTTPHeaderDict`` to the top-level ``urllib3`` namespace (`#2216 <https://github.com/urllib3/urllib3/issues/2216>`__).
-* Added the ``json`` parameter to ``urllib3.request()``, ``PoolManager.request()``, and ``ConnectionPool.request()`` methods to send JSON bodies in requests. Using this parameter will set the header ``Content-Type: application/json`` if ``Content-Type`` isn't already defined.
-  Added support for parsing JSON response bodies with ``HTTPResponse.json()`` method (`#2243 <https://github.com/urllib3/urllib3/issues/2243>`__).
 * Added support for configuring header merging behavior with HTTPHeaderDict
   When using a ``HTTPHeaderDict`` to provide headers for a request, by default duplicate
   header values will be repeated. But if ``combine=True`` is passed into a call to
   ``HTTPHeaderDict.add``, then the added header value will be merged in with an existing
   value into a comma-separated list (``X-My-Header: foo, bar``) (`#2242 <https://github.com/urllib3/urllib3/issues/2242>`__).
 * Added ``NameResolutionError`` exception when a DNS error occurs (`#2305 <https://github.com/urllib3/urllib3/issues/2305>`__).
 * Added ``proxy_assert_hostname`` and ``proxy_assert_fingerprint`` kwargs to ``ProxyManager`` (`#2409 <https://github.com/urllib3/urllib3/issues/2409>`__).
 * Added a configurable ``backoff_max`` parameter to the ``Retry`` class.
   If a custom ``backoff_max`` is provided to the ``Retry`` class, it
   will replace the ``Retry.DEFAULT_BACKOFF_MAX`` (`#2494 <https://github.com/urllib3/urllib3/issues/2494>`__).
 * Added the ``authority`` property to the Url class as per RFC 3986 3.2. This property should be used in place of ``netloc`` for users who want to include the userinfo (auth) component of the URI (`#2520 <https://github.com/urllib3/urllib3/issues/2520>`__).
 * Added the ``scheme`` parameter to ``HTTPConnection.set_tunnel`` to configure the scheme of the origin being tunnelled to (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
 * Added the ``is_closed``, ``is_connected`` and ``has_connected_to_proxy`` properties to ``HTTPConnection`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
+* Added optional ``backoff_jitter`` parameter to ``Retry``. (`#2952 <https://github.com/urllib3/urllib3/issues/2952>`__)
 
-* Removed support for Python 2.7, 3.5, and 3.6 (`#883 <https://github.com/urllib3/urllib3/issues/883>`__, `#2336 <https://github.com/urllib3/urllib3/issues/2336>`__).
-* Removed fallback on certificate ``commonName`` in ``match_hostname()`` function.
-  This behavior was deprecated in May 2000 in RFC 2818. Instead only ``subjectAltName``
-  is used to verify the hostname by default. To enable verifying the hostname against
-  ``commonName`` use ``SSLContext.hostname_checks_common_name = True`` (`#2113 <https://github.com/urllib3/urllib3/issues/2113>`__).
-* Removed support for Python with an ``ssl`` module compiled with LibreSSL, CiscoSSL,
-  wolfSSL, and all other OpenSSL alternatives. Python is moving to require OpenSSL with PEP 644 (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
-* Removed support for OpenSSL versions earlier than 1.1.1 or that don't have SNI support.
-  When an incompatible OpenSSL version is detected an ``ImportError`` is raised (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
-* Removed the list of default ciphers for OpenSSL 1.1.1+ and SecureTransport as their own defaults are already secure (`#2082 <https://github.com/urllib3/urllib3/issues/2082>`__).
-* Removed ``urllib3.contrib.appengine.AppEngineManager`` and support for Google App Engine Standard Environment (`#2044 <https://github.com/urllib3/urllib3/issues/2044>`__).
-* Removed deprecated ``Retry`` options ``method_whitelist``, ``DEFAULT_REDIRECT_HEADERS_BLACKLIST`` (`#2086 <https://github.com/urllib3/urllib3/issues/2086>`__).
-* Removed ``urllib3.HTTPResponse.from_httplib`` (`#2648 <https://github.com/urllib3/urllib3/issues/2648>`__).
-* Removed default value of ``None`` for the ``request_context`` parameter of ``urllib3.PoolManager.connection_from_pool_key``. This change should have no effect on users as the default value of ``None`` was an invalid option and was never used (`#1897 <https://github.com/urllib3/urllib3/issues/1897>`__).
-* Removed the ``urllib3.request`` module. ``urllib3.request.RequestMethods`` has been made a private API.
-  This change was made to ensure that ``from urllib3 import request`` imported the top-level ``request()``
-  function instead of the ``urllib3.request`` module (`#2269 <https://github.com/urllib3/urllib3/issues/2269>`__).
-* Removed support for SSLv3.0 from the ``urllib3.contrib.pyopenssl`` even when support is available from the compiled OpenSSL library (`#2233 <https://github.com/urllib3/urllib3/issues/2233>`__).
-* Removed the deprecated ``urllib3.contrib.ntlmpool`` module (`#2339 <https://github.com/urllib3/urllib3/issues/2339>`__).
-* Removed ``DEFAULT_CIPHERS``, ``HAS_SNI``, ``USE_DEFAULT_SSLCONTEXT_CIPHERS``, from the private module ``urllib3.util.ssl_`` (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
-* Removed ``urllib3.exceptions.SNIMissingWarning`` (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
-* Removed the ``_prepare_conn`` method from ``HTTPConnectionPool``. Previously this was only used to call ``HTTPSConnection.set_cert()`` by ``HTTPSConnectionPool`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
-* Removed ``tls_in_tls_required`` property from ``HTTPSConnection``. This is now determined from the ``scheme`` parameter in ``HTTPConnection.set_tunnel()`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
+Changed
+-------
 
 * Changed ``urllib3.response.HTTPResponse.read`` to respect the semantics of ``io.BufferedIOBase`` regardless of compression. Specifically, this method:
 
   * Only returns an empty bytes object to indicate EOF (that is, the response has been fully consumed).
   * Never returns more bytes than requested.
   * Can issue any number of system calls: zero, one or multiple.
 
   If you want each ``urllib3.response.HTTPResponse.read`` call to issue a single system call, you need to disable decompression by setting ``decode_content=False`` (`#2128 <https://github.com/urllib3/urllib3/issues/2128>`__).
+* Changed ``urllib3.HTTPConnection.getresponse`` to return an instance of ``urllib3.HTTPResponse`` instead of ``http.client.HTTPResponse`` (`#2648 <https://github.com/urllib3/urllib3/issues/2648>`__).
 * Changed ``ssl_version`` to instead set the corresponding ``SSLContext.minimum_version``
   and ``SSLContext.maximum_version`` values.  Regardless of ``ssl_version`` passed
   ``SSLContext`` objects are now constructed using ``ssl.PROTOCOL_TLS_CLIENT`` (`#2110 <https://github.com/urllib3/urllib3/issues/2110>`__).
 * Changed default ``SSLContext.minimum_version`` to be ``TLSVersion.TLSv1_2`` in line with Python 3.10 (`#2373 <https://github.com/urllib3/urllib3/issues/2373>`__).
 * Changed ``ProxyError`` to wrap any connection error (timeout, TLS, DNS) that occurs when connecting to the proxy (`#2482 <https://github.com/urllib3/urllib3/pull/2482>`__).
 * Changed ``urllib3.util.create_urllib3_context`` to not override the system cipher suites with
   a default value. The new default will be cipher suites configured by the operating system (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
 * Changed ``multipart/form-data`` header parameter formatting matches the WHATWG HTML Standard as of 2021-06-10. Control characters in filenames are no longer percent encoded (`#2257 <https://github.com/urllib3/urllib3/issues/2257>`__).
-* Changed ``urllib3.HTTPConnection.getresponse`` to return an instance of ``urllib3.HTTPResponse`` instead of ``http.client.HTTPResponse`` (`#2648 <https://github.com/urllib3/urllib3/issues/2648>`__).
 * Changed the error raised when connecting via HTTPS when the ``ssl`` module isn't available from ``SSLError`` to ``ImportError`` (`#2589 <https://github.com/urllib3/urllib3/issues/2589>`__).
 * Changed ``HTTPConnection.request()`` to always use lowercase chunk boundaries when sending requests with ``Transfer-Encoding: chunked`` (`#2515 <https://github.com/urllib3/urllib3/issues/2515>`__).
-* Changed `enforce_content_length` default to True, preventing silent data loss when reading streamed responses (`#2514 <https://github.com/urllib3/urllib3/issues/2514>`__).
+* Changed ``enforce_content_length`` default to True, preventing silent data loss when reading streamed responses (`#2514 <https://github.com/urllib3/urllib3/issues/2514>`__).
 * Changed internal implementation of ``HTTPHeaderDict`` to use ``dict`` instead of ``collections.OrderedDict`` for better performance (`#2080 <https://github.com/urllib3/urllib3/issues/2080>`__).
 * Changed the ``urllib3.contrib.pyopenssl`` module to wrap ``OpenSSL.SSL.Error`` with ``ssl.SSLError`` in ``PyOpenSSLContext.load_cert_chain`` (`#2628 <https://github.com/urllib3/urllib3/issues/2628>`__).
 * Changed usage of the deprecated ``socket.error`` to ``OSError`` (`#2120 <https://github.com/urllib3/urllib3/issues/2120>`__).
 * Changed all parameters in the ``HTTPConnection`` and ``HTTPSConnection`` constructors to be keyword-only except ``host`` and ``port`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
-* Changed ``urllib3.util.is_connection_dropped()`` to use ``HTTPConnection.is_connected`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
 * Changed ``HTTPConnection.getresponse()`` to set the socket timeout from ``HTTPConnection.timeout`` value before reading
   data from the socket. This previously was done manually by the ``HTTPConnectionPool`` calling ``HTTPConnection.sock.settimeout(...)`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
 * Changed the ``_proxy_host`` property to ``_tunnel_host`` in ``HTTPConnectionPool`` to more closely match how the property is used (value in ``HTTPConnection.set_tunnel()``) (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
 * Changed name of ``Retry.BACK0FF_MAX`` to be ``Retry.DEFAULT_BACKOFF_MAX``.
 * Changed TLS handshakes to use ``SSLContext.check_hostname`` when possible (`#2452 <https://github.com/urllib3/urllib3/pull/2452>`__).
 * Changed ``server_hostname`` to behave like other parameters only used by ``HTTPSConnectionPool`` (`#2537 <https://github.com/urllib3/urllib3/pull/2537>`__).
 * Changed the default ``blocksize`` to 16KB to match OpenSSL's default read amounts (`#2348 <https://github.com/urllib3/urllib3/pull/2348>`__).
+* Changed ``HTTPResponse.read()`` to raise an error when calling with ``decode_content=False`` after using ``decode_content=True`` to prevent data loss (`#2800 <https://github.com/urllib3/urllib3/issues/2800>`__).
 
-* Deprecated ``HTTPResponse.getheaders()`` and ``HTTPResponse.getheader()`` which will be removed in urllib3 v2.1.0. Instead use ``HTTPResponse.headers`` and ``HTTPResponse.headers.get(name, default)``. (`#1543 <https://github.com/urllib3/urllib3/issues/1543>`__, `#2814 <https://github.com/urllib3/urllib3/issues/2814>`__).
-* Deprecated ``urllib3.contrib.pyopenssl`` module which will be removed in urllib3 v2.1.0 (`#2691 <https://github.com/urllib3/urllib3/issues/2691>`__).
-* Deprecated ``urllib3.contrib.securetransport`` module which will be removed in urllib3 v2.1.0 (`#2692 <https://github.com/urllib3/urllib3/issues/2692>`__).
-* Deprecated ``ssl_version`` option in favor of ``ssl_minimum_version``. ``ssl_version`` will be removed in urllib3 v2.1.0 (`#2110 <https://github.com/urllib3/urllib3/issues/2110>`__).
-* Deprecated the ``strict`` parameter as it's not longer needed in Python 3.x. It will be removed in urllib3 v2.1.0 (`#2267 <https://github.com/urllib3/urllib3/issues/2267>`__)
-* Deprecated the ``NewConnectionError.pool`` attribute which will be removed in urllib3 v2.1.0 (`#2271 <https://github.com/urllib3/urllib3/issues/2271>`__).
-* Deprecated ``format_header_param_html5`` and ``format_header_param`` in favor of ``format_multipart_header_param`` (`#2257 <https://github.com/urllib3/urllib3/issues/2257>`__).
-* Deprecated ``RequestField.header_formatter`` parameter which will be removed in urllib3 v2.1.0 (`#2257 <https://github.com/urllib3/urllib3/issues/2257>`__).
-* Deprecated ``HTTPSConnection.set_cert()`` method. Instead pass parameters to the ``HTTPSConnection`` constructor (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
-* Deprecated ``HTTPConnection.request_chunked()`` method which will be removed in urllib3 v2.1.0. Instead pass ``chunked=True`` to ``HTTPConnection.request()`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
+Fixed
+-----
 
-* Fixed thread-safety issue where accessing a `PoolManager` with many distinct origins would cause connection pools to be closed while requests are in progress (`#1252 <https://github.com/urllib3/urllib3/issues/1252>`__).
+* Fixed thread-safety issue where accessing a ``PoolManager`` with many distinct origins would cause connection pools to be closed while requests are in progress (`#1252 <https://github.com/urllib3/urllib3/issues/1252>`__).
 * Fixed an issue where an ``HTTPConnection`` instance would erroneously reuse the socket read timeout value from reading the previous response instead of a newly configured connect timeout.
   Instead now if ``HTTPConnection.timeout`` is updated before sending the next request the new timeout value will be used (`#2645 <https://github.com/urllib3/urllib3/issues/2645>`__).
 * Fixed ``socket.error.errno`` when raised from pyOpenSSL's ``OpenSSL.SSL.SysCallError`` (`#2118 <https://github.com/urllib3/urllib3/issues/2118>`__).
 * Fixed the default value of ``HTTPSConnection.socket_options`` to match ``HTTPConnection`` (`#2213 <https://github.com/urllib3/urllib3/issues/2213>`__).
 * Fixed a bug where ``headers`` would be modified by the ``remove_headers_on_redirect`` feature (`#2272 <https://github.com/urllib3/urllib3/issues/2272>`__).
 * Fixed a reference cycle bug in ``urllib3.util.connection.create_connection()`` (`#2277 <https://github.com/urllib3/urllib3/issues/2277>`__).
 * Fixed a socket leak if ``HTTPConnection.connect()`` fails (`#2571 <https://github.com/urllib3/urllib3/pull/2571>`__).
+* Fixed ``urllib3.contrib.pyopenssl.WrappedSocket`` and ``urllib3.contrib.securetransport.WrappedSocket`` close methods (`#2970 <https://github.com/urllib3/urllib3/issues/2970>`__)
 
 1.26.15 (2023-03-10)
---------------------
+====================
 
 * Fix socket timeout value when ``HTTPConnection`` is reused (`#2645 <https://github.com/urllib3/urllib3/issues/2645>`__)
 * Remove "!" character from the unreserved characters in IPv6 Zone ID parsing
   (`#2899 <https://github.com/urllib3/urllib3/issues/2899>`__)
 * Fix IDNA handling of '\x80' byte (`#2901 <https://github.com/urllib3/urllib3/issues/2901>`__)
 
 1.26.14 (2023-01-11)
---------------------
+====================
 
 * Fixed parsing of port 0 (zero) returning None, instead of 0. (`#2850 <https://github.com/urllib3/urllib3/issues/2850>`__)
 * Removed deprecated getheaders() calls in contrib module. Fixed the type hint of ``PoolKey.key_retries`` by adding ``bool`` to the union. (`#2865 <https://github.com/urllib3/urllib3/issues/2865>`__)
 
 1.26.13 (2022-11-23)
---------------------
+====================
 
 * Deprecated the ``HTTPResponse.getheaders()`` and ``HTTPResponse.getheader()`` methods.
 * Fixed an issue where parsing a URL with leading zeroes in the port would be rejected
   even when the port number after removing the zeroes was valid.
 * Fixed a deprecation warning when using cryptography v39.0.0.
 * Removed the ``<4`` in the ``Requires-Python`` packaging metadata field.
```

### Comparing `urllib3-2.0.0a4/docs/Makefile` & `urllib3-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/advanced-usage.rst` & `urllib3-2.0.1/docs/advanced-usage.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/conf.py` & `urllib3-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/contributing.rst` & `urllib3-2.0.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/index.rst` & `urllib3-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/make.bat` & `urllib3-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/user-guide.rst` & `urllib3-2.0.1/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/v2-migration-guide.rst` & `urllib3-2.0.1/docs/v2-migration-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/_static/banner.svg` & `urllib3-2.0.1/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/_static/banner_github.svg` & `urllib3-2.0.1/docs/_static/banner_github.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/_static/dark-logo.svg` & `urllib3-2.0.1/docs/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/images/demo-button.png` & `urllib3-2.0.1/docs/images/demo-button.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/images/favicon.png` & `urllib3-2.0.1/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/images/learn-more-button.png` & `urllib3-2.0.1/docs/images/learn-more-button.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/images/logo.png` & `urllib3-2.0.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/images/logo.svg` & `urllib3-2.0.1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/reference/urllib3.response.rst` & `urllib3-2.0.1/docs/reference/urllib3.response.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/reference/urllib3.util.rst` & `urllib3-2.0.1/docs/reference/urllib3.util.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/docs/reference/contrib/securetransport.rst` & `urllib3-2.0.1/docs/reference/contrib/securetransport.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/dummyserver/handlers.py` & `urllib3-2.0.1/dummyserver/handlers.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/dummyserver/https_proxy.py` & `urllib3-2.0.1/dummyserver/https_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/dummyserver/proxy.py` & `urllib3-2.0.1/dummyserver/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/dummyserver/server.py` & `urllib3-2.0.1/dummyserver/server.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/dummyserver/testcase.py` & `urllib3-2.0.1/dummyserver/testcase.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/dummyserver/certs/cacert.key` & `urllib3-2.0.1/dummyserver/certs/cacert.key`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/dummyserver/certs/cacert.pem` & `urllib3-2.0.1/dummyserver/certs/cacert.pem`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/dummyserver/certs/server.crt` & `urllib3-2.0.1/dummyserver/certs/server.crt`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/dummyserver/certs/server.key` & `urllib3-2.0.1/dummyserver/certs/server.key`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/__init__.py` & `urllib3-2.0.1/src/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/_base_connection.py` & `urllib3-2.0.1/src/urllib3/_base_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/_collections.py` & `urllib3-2.0.1/src/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/_request_methods.py` & `urllib3-2.0.1/src/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/connection.py` & `urllib3-2.0.1/src/urllib3/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,44 +780,50 @@
         ca_cert_dir=ca_cert_dir,
         ca_cert_data=ca_cert_data,
         server_hostname=server_hostname,
         ssl_context=context,
         tls_in_tls=tls_in_tls,
     )
 
-    if assert_fingerprint:
-        _assert_fingerprint(ssl_sock.getpeercert(binary_form=True), assert_fingerprint)
-    elif (
-        context.verify_mode != ssl.CERT_NONE
-        and not context.check_hostname
-        and assert_hostname is not False
-    ):
-        cert: _TYPE_PEER_CERT_RET_DICT = ssl_sock.getpeercert()  # type: ignore[assignment]
-
-        # Need to signal to our match_hostname whether to use 'commonName' or not.
-        # If we're using our own constructed SSLContext we explicitly set 'False'
-        # because PyPy hard-codes 'True' from SSLContext.hostname_checks_common_name.
-        if default_ssl_context:
-            hostname_checks_common_name = False
-        else:
-            hostname_checks_common_name = (
-                getattr(context, "hostname_checks_common_name", False) or False
+    try:
+        if assert_fingerprint:
+            _assert_fingerprint(
+                ssl_sock.getpeercert(binary_form=True), assert_fingerprint
+            )
+        elif (
+            context.verify_mode != ssl.CERT_NONE
+            and not context.check_hostname
+            and assert_hostname is not False
+        ):
+            cert: _TYPE_PEER_CERT_RET_DICT = ssl_sock.getpeercert()  # type: ignore[assignment]
+
+            # Need to signal to our match_hostname whether to use 'commonName' or not.
+            # If we're using our own constructed SSLContext we explicitly set 'False'
+            # because PyPy hard-codes 'True' from SSLContext.hostname_checks_common_name.
+            if default_ssl_context:
+                hostname_checks_common_name = False
+            else:
+                hostname_checks_common_name = (
+                    getattr(context, "hostname_checks_common_name", False) or False
+                )
+
+            _match_hostname(
+                cert,
+                assert_hostname or server_hostname,  # type: ignore[arg-type]
+                hostname_checks_common_name,
             )
 
-        _match_hostname(
-            cert,
-            assert_hostname or server_hostname,  # type: ignore[arg-type]
-            hostname_checks_common_name,
+        return _WrappedAndVerifiedSocket(
+            socket=ssl_sock,
+            is_verified=context.verify_mode == ssl.CERT_REQUIRED
+            or bool(assert_fingerprint),
         )
-
-    return _WrappedAndVerifiedSocket(
-        socket=ssl_sock,
-        is_verified=context.verify_mode == ssl.CERT_REQUIRED
-        or bool(assert_fingerprint),
-    )
+    except BaseException:
+        ssl_sock.close()
+        raise
 
 
 def _match_hostname(
     cert: _TYPE_PEER_CERT_RET_DICT | None,
     asserted_hostname: str,
     hostname_checks_common_name: bool = False,
 ) -> None:
```

### Comparing `urllib3-2.0.0a4/src/urllib3/connectionpool.py` & `urllib3-2.0.1/src/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/exceptions.py` & `urllib3-2.0.1/src/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/fields.py` & `urllib3-2.0.1/src/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/filepost.py` & `urllib3-2.0.1/src/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/poolmanager.py` & `urllib3-2.0.1/src/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/response.py` & `urllib3-2.0.1/src/urllib3/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,17 @@
         return self._size
 
     def put(self, data: bytes) -> None:
         self.buffer.append(data)
         self._size += len(data)
 
     def get(self, n: int) -> bytes:
-        if not self.buffer:
+        if n == 0:
+            return b""
+        elif not self.buffer:
             raise RuntimeError("buffer is empty")
         elif n < 0:
             raise ValueError("n should be > 0")
 
         fetched = 0
         ret = io.BytesIO()
         while fetched < n:
```

### Comparing `urllib3-2.0.0a4/src/urllib3/contrib/pyopenssl.py` & `urllib3-2.0.1/src/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/contrib/securetransport.py` & `urllib3-2.0.1/src/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/contrib/socks.py` & `urllib3-2.0.1/src/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/contrib/_securetransport/bindings.py` & `urllib3-2.0.1/src/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/contrib/_securetransport/low_level.py` & `urllib3-2.0.1/src/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/__init__.py` & `urllib3-2.0.1/src/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/connection.py` & `urllib3-2.0.1/src/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/proxy.py` & `urllib3-2.0.1/src/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/request.py` & `urllib3-2.0.1/src/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/response.py` & `urllib3-2.0.1/src/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/retry.py` & `urllib3-2.0.1/src/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/ssl_.py` & `urllib3-2.0.1/src/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/ssl_match_hostname.py` & `urllib3-2.0.1/src/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/ssltransport.py` & `urllib3-2.0.1/src/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/timeout.py` & `urllib3-2.0.1/src/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/url.py` & `urllib3-2.0.1/src/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/util.py` & `urllib3-2.0.1/src/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/src/urllib3/util/wait.py` & `urllib3-2.0.1/src/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/__init__.py` & `urllib3-2.0.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/conftest.py` & `urllib3-2.0.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/port_helpers.py` & `urllib3-2.0.1/test/port_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_collections.py` & `urllib3-2.0.1/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_compatibility.py` & `urllib3-2.0.1/test/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_connection.py` & `urllib3-2.0.1/test/test_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     CertificateError,
     HTTPConnection,
     HTTPSConnection,
     _match_hostname,
     _url_from_connection,
     _wrap_proxy_error,
 )
-from urllib3.exceptions import HTTPError, ProxyError
+from urllib3.exceptions import HTTPError, ProxyError, SSLError
+from urllib3.util import ssl_
 from urllib3.util.ssl_match_hostname import (
     CertificateError as ImplementationCertificateError,
 )
 from urllib3.util.ssl_match_hostname import _dnsname_match, match_hostname
 
 if typing.TYPE_CHECKING:
     from urllib3.util.ssl_ import _TYPE_PEER_CERT_RET_DICT
@@ -231,7 +232,36 @@
 
     def test_getresponse_requires_reponseoptions(self) -> None:
         conn = HTTPConnection("google.com", port=80)
 
         # Should error if a request has not been sent
         with pytest.raises(ResponseNotReady):
             conn.getresponse()
+
+    def test_assert_fingerprint_closes_socket(self) -> None:
+        context = mock.create_autospec(ssl_.SSLContext)
+        context.wrap_socket.return_value.getpeercert.return_value = b"fake cert"
+        conn = HTTPSConnection(
+            "google.com",
+            port=443,
+            assert_fingerprint="AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA",
+            ssl_context=context,
+        )
+        with mock.patch.object(conn, "_new_conn"):
+            with pytest.raises(SSLError):
+                conn.connect()
+
+        context.wrap_socket.return_value.close.assert_called_once_with()
+
+    def test_assert_hostname_closes_socket(self) -> None:
+        context = mock.create_autospec(ssl_.SSLContext)
+        context.wrap_socket.return_value.getpeercert.return_value = {
+            "subjectAltName": (("DNS", "google.com"),)
+        }
+        conn = HTTPSConnection(
+            "google.com", port=443, assert_hostname="example.com", ssl_context=context
+        )
+        with mock.patch.object(conn, "_new_conn"):
+            with pytest.raises(ImplementationCertificateError):
+                conn.connect()
+
+        context.wrap_socket.return_value.close.assert_called_once_with()
```

### Comparing `urllib3-2.0.0a4/test/test_connectionpool.py` & `urllib3-2.0.1/test/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_exceptions.py` & `urllib3-2.0.1/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_fields.py` & `urllib3-2.0.1/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_filepost.py` & `urllib3-2.0.1/test/test_filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_no_ssl.py` & `urllib3-2.0.1/test/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_poolmanager.py` & `urllib3-2.0.1/test/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_proxymanager.py` & `urllib3-2.0.1/test/test_proxymanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_queue_monkeypatch.py` & `urllib3-2.0.1/test/test_queue_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_response.py` & `urllib3-2.0.1/test/test_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 class TestBytesQueueBuffer:
     def test_single_chunk(self) -> None:
         buffer = BytesQueueBuffer()
         assert len(buffer) == 0
         with pytest.raises(RuntimeError, match="buffer is empty"):
             assert buffer.get(10)
 
+        assert buffer.get(0) == b""
+
         buffer.put(b"foo")
         with pytest.raises(ValueError, match="n should be > 0"):
             buffer.get(-1)
 
         assert buffer.get(1) == b"f"
         assert buffer.get(2) == b"oo"
         with pytest.raises(RuntimeError, match="buffer is empty"):
@@ -177,14 +179,15 @@
         with pytest.raises(DecodeError):
             HTTPResponse(fp, headers={"content-encoding": "deflate"})
 
     def test_reference_read(self) -> None:
         fp = BytesIO(b"foo")
         r = HTTPResponse(fp, preload_content=False)
 
+        assert r.read(0) == b""
         assert r.read(1) == b"f"
         assert r.read(2) == b"oo"
         assert r.read() == b""
         assert r.read() == b""
 
     def test_decode_deflate(self) -> None:
         data = zlib.compress(b"foo")
```

### Comparing `urllib3-2.0.0a4/test/test_retry.py` & `urllib3-2.0.1/test/test_retry.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_ssl.py` & `urllib3-2.0.1/test/test_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_ssltransport.py` & `urllib3-2.0.1/test/test_ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_util.py` & `urllib3-2.0.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/test_wait.py` & `urllib3-2.0.1/test/test_wait.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/tz_stub.py` & `urllib3-2.0.1/test/tz_stub.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/contrib/duplicate_san.pem` & `urllib3-2.0.1/test/contrib/duplicate_san.pem`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/contrib/test_pyopenssl.py` & `urllib3-2.0.1/test/contrib/test_pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/contrib/test_pyopenssl_dependencies.py` & `urllib3-2.0.1/test/contrib/test_pyopenssl_dependencies.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/contrib/test_securetransport.py` & `urllib3-2.0.1/test/contrib/test_securetransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/contrib/test_socks.py` & `urllib3-2.0.1/test/contrib/test_socks.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/with_dummyserver/test_chunked_transfer.py` & `urllib3-2.0.1/test/with_dummyserver/test_chunked_transfer.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/with_dummyserver/test_connection.py` & `urllib3-2.0.1/test/with_dummyserver/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/with_dummyserver/test_connectionpool.py` & `urllib3-2.0.1/test/with_dummyserver/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/with_dummyserver/test_https.py` & `urllib3-2.0.1/test/with_dummyserver/test_https.py`

 * *Files 2% similar despite different names*

```diff
@@ -456,47 +456,44 @@
 
     def test_assert_fingerprint_md5(self) -> None:
         with HTTPSConnectionPool(
             "localhost",
             self.port,
             cert_reqs="CERT_REQUIRED",
             ca_certs=DEFAULT_CA,
+            assert_fingerprint=("55:39:BF:70:05:12:43:FA:1F:D1:BF:4E:E8:1B:07:1D"),
             ssl_minimum_version=self.tls_version(),
         ) as https_pool:
-            https_pool.assert_fingerprint = (
-                "55:39:BF:70:05:12:43:FA:1F:D1:BF:4E:E8:1B:07:1D"
-            )
-
             https_pool.request("GET", "/")
 
     def test_assert_fingerprint_sha1(self) -> None:
         with HTTPSConnectionPool(
             "localhost",
             self.port,
             cert_reqs="CERT_REQUIRED",
             ca_certs=DEFAULT_CA,
+            assert_fingerprint=(
+                "72:8B:55:4C:9A:FC:1E:88:A1:1C:AD:1B:B2:E7:CC:3E:DB:C8:F9:8A"
+            ),
             ssl_minimum_version=self.tls_version(),
         ) as https_pool:
-            https_pool.assert_fingerprint = (
-                "72:8B:55:4C:9A:FC:1E:88:A1:1C:AD:1B:B2:E7:CC:3E:DB:C8:F9:8A"
-            )
             https_pool.request("GET", "/")
 
     def test_assert_fingerprint_sha256(self) -> None:
         with HTTPSConnectionPool(
             "localhost",
             self.port,
             cert_reqs="CERT_REQUIRED",
             ca_certs=DEFAULT_CA,
-            ssl_minimum_version=self.tls_version(),
-        ) as https_pool:
-            https_pool.assert_fingerprint = (
+            assert_fingerprint=(
                 "E3:59:8E:69:FF:C5:9F:C7:88:87:44:58:22:7F:90:8D:D9:BC:12:C4:90:79:D5:"
                 "DC:A8:5D:4F:60:40:1E:A6:D2"
-            )
+            ),
+            ssl_minimum_version=self.tls_version(),
+        ) as https_pool:
             https_pool.request("GET", "/")
 
     def test_assert_invalid_fingerprint(self) -> None:
         def _test_request(pool: HTTPSConnectionPool) -> SSLError:
             with pytest.raises(MaxRetryError) as cm:
                 pool.request("GET", "/", retries=0)
             assert isinstance(cm.value.reason, SSLError)
@@ -506,15 +503,15 @@
             self.host,
             self.port,
             cert_reqs="CERT_REQUIRED",
             ca_certs=DEFAULT_CA,
             ssl_minimum_version=self.tls_version(),
         ) as https_pool:
             https_pool.assert_fingerprint = (
-                "AA:AA:AA:AA:AA:AAAA:AA:AAAA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA"
+                "AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA"
             )
             e = _test_request(https_pool)
             expected = "aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa"
             got = "728b554c9afc1e88a11cad1bb2e7cc3edbc8f98a"
             assert (
                 str(e)
                 == f'Fingerprints did not match. Expected "{expected}", got "{got}"'
@@ -528,52 +525,54 @@
             # Invalid length
             https_pool.assert_fingerprint = "AA"
             e = _test_request(https_pool)
             assert "Fingerprint of invalid length:" in str(e)
 
     def test_verify_none_and_bad_fingerprint(self) -> None:
         with HTTPSConnectionPool(
-            "127.0.0.1", self.port, cert_reqs="CERT_NONE", ca_certs=self.bad_ca_path
+            "127.0.0.1",
+            self.port,
+            cert_reqs="CERT_NONE",
+            assert_hostname=False,
+            assert_fingerprint=(
+                "AA:8B:55:4C:9A:FC:1E:88:A1:1C:AD:1B:B2:E7:CC:3E:DB:C8:F9:8A"
+            ),
         ) as https_pool:
-            https_pool.assert_fingerprint = (
-                "AA:AA:AA:AA:AA:AAAA:AA:AAAA:AA:AA:AA:AA:AA:AA:AA:AA:AA:AA"
-            )
             with pytest.raises(MaxRetryError) as cm:
                 https_pool.request("GET", "/", retries=0)
             assert isinstance(cm.value.reason, SSLError)
 
     def test_verify_none_and_good_fingerprint(self) -> None:
         with HTTPSConnectionPool(
             "127.0.0.1",
             self.port,
             cert_reqs="CERT_NONE",
-            ca_certs=self.bad_ca_path,
-            ssl_minimum_version=self.tls_version(),
-        ) as https_pool:
-            https_pool.assert_fingerprint = (
+            assert_hostname=False,
+            assert_fingerprint=(
                 "72:8B:55:4C:9A:FC:1E:88:A1:1C:AD:1B:B2:E7:CC:3E:DB:C8:F9:8A"
-            )
+            ),
+        ) as https_pool:
             https_pool.request("GET", "/")
 
     @notSecureTransport()
     def test_good_fingerprint_and_hostname_mismatch(self) -> None:
         # This test doesn't run with SecureTransport because we don't turn off
         # hostname validation without turning off all validation, which this
         # test doesn't do (deliberately). We should revisit this if we make
         # new decisions.
         with HTTPSConnectionPool(
             "127.0.0.1",
             self.port,
             cert_reqs="CERT_REQUIRED",
             ca_certs=DEFAULT_CA,
+            assert_fingerprint=(
+                "72:8B:55:4C:9A:FC:1E:88:A1:1C:AD:1B:B2:E7:CC:3E:DB:C8:F9:8A"
+            ),
             ssl_minimum_version=self.tls_version(),
         ) as https_pool:
-            https_pool.assert_fingerprint = (
-                "72:8B:55:4C:9A:FC:1E:88:A1:1C:AD:1B:B2:E7:CC:3E:DB:C8:F9:8A"
-            )
             https_pool.request("GET", "/")
 
     @requires_network()
     def test_https_timeout(self) -> None:
         timeout = Timeout(total=None, connect=SHORT_TIMEOUT)
         with HTTPSConnectionPool(
             TARPIT_HOST,
@@ -589,20 +588,23 @@
         timeout = Timeout(read=0.01)
         with HTTPSConnectionPool(
             self.host,
             self.port,
             timeout=timeout,
             retries=False,
             cert_reqs="CERT_REQUIRED",
+            ca_certs=DEFAULT_CA,
+            assert_fingerprint=(
+                "72:8B:55:4C:9A:FC:1E:88:A1:1C:AD:1B:B2:E7:CC:3E:DB:C8:F9:8A"
+            ),
             ssl_minimum_version=self.tls_version(),
         ) as https_pool:
-            https_pool.ca_certs = DEFAULT_CA
-            https_pool.assert_fingerprint = (
-                "72:8B:55:4C:9A:FC:1E:88:A1:1C:AD:1B:B2:E7:CC:3E:DB:C8:F9:8A"
-            )
+            # TODO This was removed in https://github.com/urllib3/urllib3/pull/703/files
+            # We need to put something back or remove this block.
+            pass
 
         timeout = Timeout(total=None)
         with HTTPSConnectionPool(
             self.host,
             self.port,
             timeout=timeout,
             cert_reqs="CERT_NONE",
```

### Comparing `urllib3-2.0.0a4/test/with_dummyserver/test_no_ssl.py` & `urllib3-2.0.1/test/with_dummyserver/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/with_dummyserver/test_poolmanager.py` & `urllib3-2.0.1/test/with_dummyserver/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/with_dummyserver/test_proxy_poolmanager.py` & `urllib3-2.0.1/test/with_dummyserver/test_proxy_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/test/with_dummyserver/test_socketlevel.py` & `urllib3-2.0.1/test/with_dummyserver/test_socketlevel.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/LICENSE.txt` & `urllib3-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/README.md` & `urllib3-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.0a4/pyproject.toml` & `urllib3-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">=3.7"
```

### Comparing `urllib3-2.0.0a4/PKG-INFO` & `urllib3-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3
-Version: 2.0.0a4
+Version: 2.0.1
 Summary: HTTP library with thread-safe connection pooling, file post, and more.
 Project-URL: Changelog, https://github.com/urllib3/urllib3/blob/main/CHANGES.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/urllib3/urllib3
 Project-URL: Issue tracker, https://github.com/urllib3/urllib3/issues
 Author-email: Andrey Petrov <andrey.petrov@shazow.net>
 Maintainer-email: Seth Michael Larson <sethmichaellarson@gmail.com>, Quentin Pradet <quentin@pradet.me>
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Provides-Extra: brotli
 Requires-Dist: brotli>=1.0.9; platform_python_implementation == 'CPython' and extra == 'brotli'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: urllib3 Version: 2.0.0a4 Summary: HTTP library with
+Metadata-Version: 2.1 Name: urllib3 Version: 2.0.1 Summary: HTTP library with
 thread-safe connection pooling, file post, and more. Project-URL: Changelog,
 https://github.com/urllib3/urllib3/blob/main/CHANGES.rst Project-URL:
 Documentation, https://urllib3.readthedocs.io Project-URL: Code, https://
 github.com/urllib3/urllib3 Project-URL: Issue tracker, https://github.com/
 urllib3/urllib3/issues Author-email: Andrey Petrov
 petrov@shazow.net> Maintainer-email: Seth Michael Larson
 gmail.com>, Quentin Pradet
@@ -12,19 +12,20 @@
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Programming Language :: Python
-:: Implementation :: PyPy Classifier: Topic :: Internet :: WWW/HTTP Classifier:
-Topic :: Software Development :: Libraries Requires-Python: >=3.7 Provides-
-Extra: brotli Requires-Dist: brotli>=1.0.9; platform_python_implementation ==
-'CPython' and extra == 'brotli' Requires-Dist: brotlicffi>=0.8.0;
+Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Software
+Development :: Libraries Requires-Python: >=3.7 Provides-Extra: brotli
+Requires-Dist: brotli>=1.0.9; platform_python_implementation == 'CPython' and
+extra == 'brotli' Requires-Dist: brotlicffi>=0.8.0;
 platform_python_implementation != 'CPython' and extra == 'brotli' Provides-
 Extra: secure Requires-Dist: certifi; extra == 'secure' Requires-Dist:
 cryptography>=1.9; extra == 'secure' Requires-Dist: idna>=2.0.0; extra ==
 'secure' Requires-Dist: pyopenssl>=17.1.0; extra == 'secure' Requires-Dist:
 urllib3-secure-extra; extra == 'secure' Provides-Extra: socks Requires-Dist:
 pysocks!=1.5.7,<2.0,>=1.5.6; extra == 'socks' Provides-Extra: zstd Requires-
 Dist: zstandard>=0.18.0; extra == 'zstd' Description-Content-Type: text/
```

