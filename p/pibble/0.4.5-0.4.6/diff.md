# Comparing `tmp/pibble-0.4.5.tar.gz` & `tmp/pibble-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibble-0.4.5.tar", last modified: Sun Apr 30 01:25:08 2023, max compression
+gzip compressed data, was "pibble-0.4.6.tar", last modified: Sun Apr 30 02:20:26 2023, max compression
```

## Comparing `pibble-0.4.5.tar` & `pibble-0.4.6.tar`

### file list

```diff
@@ -1,208 +1,208 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.785169 pibble-0.4.5/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6410 2023-04-30 01:25:08.785169 pibble-0.4.5/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5960 2023-04-30 01:25:08.000000 pibble-0.4.5/README.md
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8383 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/api/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3287 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/api/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/api/client/apachethrift/
--rw-------   0 benjamin  (1000) benjamin  (1000)     6189 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/apachethrift/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1326 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/api/client/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    14182 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/file/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9703 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/file/hdfs.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12462 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/file/local.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    19644 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4126 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/api/client/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4698 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16829 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2330 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/api/client/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11322 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4770 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10558 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6564 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/webservice/soap.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7325 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/webservice/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/client/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/configuration.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6084 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/exceptions.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/api/helpers/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/helpers/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15593 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/helpers/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    20508 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/helpers/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24123 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/helpers/googlerpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13134 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/helpers/store.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13916 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/helpers/wrappers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/api/meta/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/meta/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9353 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/meta/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2958 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/meta/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/api/middleware/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble/api/middleware/apachethrift/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/apachethrift/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/apachethrift/screening.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/middleware/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3112 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/database/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/middleware/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      438 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/file/temp.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/middleware/googlerpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/googlerpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/googlerpc/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/googlerpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/googlerpc/metadata.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3027 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/middleware/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/webservice/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/middleware/webservice/authentication/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/webservice/authentication/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/webservice/authentication/basic.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/webservice/authentication/bearer.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13466 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/webservice/authentication/digest.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/webservice/authentication/header.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    17694 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/webservice/authentication/oauth.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3248 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/webservice/limit.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/middleware/webservice/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/protocol/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/protocol/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19471 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/protocol/apachethrift.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2443 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1983 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/server/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15450 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5445 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/server/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2377 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7264 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/awslambda.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    40698 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15361 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/handler.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3182 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/server/webservice/mixin/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/mixin/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      718 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/mixin/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      987 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/server/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4212 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6486 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11970 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16833 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/soap.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/api/server/webservice/template/
--rw-------   0 benjamin  (1000) benjamin  (1000)     9566 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/template/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9195 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/template/extensions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9368 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/api/server/webservice/template/loader.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7772 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/database/dedupe.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10216 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/database/engine.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/database/exceptions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    26389 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/database/orm.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2667 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/database/util.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.777169 pibble-0.4.5/pibble/ext/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/cms/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/cms/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/cms/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/cms/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/cms/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/cms/database/interface.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/cms/database/menu.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/cms/database/view.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/cms/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/cms/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6382 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/cms/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2998 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/cms/server/extension.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      350 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/cms/server/mixin.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/dam/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/dam/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/dam/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/dam/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/dam/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/dam/database/files.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/dam/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/dam/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/dam/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/rest/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/rest/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/rest/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/rest/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/rest/database/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/rest/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/rest/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15691 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/rest/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7707 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/rest/server/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/session/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/session/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/session/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/session/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/session/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/session/database/session.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/session/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/session/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5026 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/session/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/user/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/user/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/client/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      963 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/user/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/database/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/database/notification.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/database/permission.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/database/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.781169 pibble-0.4.5/pibble/ext/user/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    23592 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/ext/user/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.785169 pibble-0.4.5/pibble/hooks/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/hooks/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5971 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/hooks/aws.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.785169 pibble-0.4.5/pibble/media/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/media/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10231 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/media/thumbnail.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.785169 pibble-0.4.5/pibble/resources/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/resources/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10649 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/resources/retriever.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2651 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/setup.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.785169 pibble-0.4.5/pibble/util/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/util/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8375 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/util/encryption.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16134 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/util/files.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    32731 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/util/helpers.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/util/imaging.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/util/log.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1610 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/util/numeric.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    26217 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/util/strings.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.785169 pibble-0.4.5/pibble/web/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/web/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble/web/scraper.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 01:25:08.773169 pibble-0.4.5/pibble.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6410 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5413 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1818 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-04-30 01:25:08.000000 pibble-0.4.5/pibble.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-04-30 01:25:08.785169 pibble-0.4.5/setup.cfg
--rw-------   0 benjamin  (1000) benjamin  (1000)     2651 2023-04-30 01:25:08.000000 pibble-0.4.5/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.946003 pibble-0.4.6/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6410 2023-04-30 02:20:26.946003 pibble-0.4.6/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5960 2023-04-30 02:20:26.000000 pibble-0.4.6/README.md
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.934004 pibble-0.4.6/pibble/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8891 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/__main__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.934004 pibble-0.4.6/pibble/api/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3287 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.934004 pibble-0.4.6/pibble/api/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.934004 pibble-0.4.6/pibble/api/client/apachethrift/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6189 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/apachethrift/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1326 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.934004 pibble-0.4.6/pibble/api/client/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    14182 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/file/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9703 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/file/hdfs.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12462 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/file/local.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    19644 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4126 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.934004 pibble-0.4.6/pibble/api/client/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4698 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16829 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2330 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/webservice/jsonapi.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.934004 pibble-0.4.6/pibble/api/client/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11322 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4770 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10558 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6564 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/webservice/soap.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7325 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/webservice/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/client/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/configuration.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6084 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/exceptions.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.934004 pibble-0.4.6/pibble/api/helpers/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/helpers/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15593 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/helpers/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    20508 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/helpers/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24123 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/helpers/googlerpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13134 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/helpers/store.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13916 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/helpers/wrappers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.934004 pibble-0.4.6/pibble/api/meta/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/meta/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9353 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/meta/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2958 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/meta/helpers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/middleware/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/middleware/apachethrift/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/apachethrift/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/apachethrift/screening.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/middleware/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3112 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/database/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/middleware/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      438 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/file/temp.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/middleware/googlerpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/googlerpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/googlerpc/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/googlerpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/googlerpc/metadata.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3027 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/middleware/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/webservice/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/middleware/webservice/authentication/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/webservice/authentication/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/webservice/authentication/basic.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/webservice/authentication/bearer.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13466 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/webservice/authentication/digest.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/webservice/authentication/header.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    17694 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/webservice/authentication/oauth.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3248 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/webservice/limit.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/middleware/webservice/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/protocol/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/protocol/__init__.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19471 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/protocol/apachethrift.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2443 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1983 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/server/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15450 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5445 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/server/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2377 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7264 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/awslambda.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    40698 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15361 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/handler.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3182 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/jsonapi.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/server/webservice/mixin/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/mixin/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      718 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/mixin/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      987 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/server/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4212 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6486 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11970 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16833 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/soap.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.938004 pibble-0.4.6/pibble/api/server/webservice/template/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9667 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/template/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9195 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/template/extensions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9364 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/api/server/webservice/template/loader.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7772 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/database/dedupe.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10216 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/database/engine.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/database/exceptions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    26389 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/database/orm.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2667 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/database/util.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/cms/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/cms/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/cms/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/cms/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/cms/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/cms/database/interface.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/cms/database/menu.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/cms/database/view.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/cms/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/cms/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6382 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/cms/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2998 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/cms/server/extension.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      350 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/cms/server/mixin.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/dam/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/dam/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/dam/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/dam/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/dam/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/dam/database/files.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/dam/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/dam/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/dam/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/rest/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/rest/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/rest/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/rest/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/rest/database/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/rest/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/rest/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15691 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/rest/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7707 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/rest/server/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/session/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/session/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/session/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/session/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/session/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/session/database/session.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/session/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/session/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5026 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/session/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/user/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/user/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/client/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      963 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/user/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/database/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/database/notification.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/database/permission.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/database/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/ext/user/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    23592 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/ext/user/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/hooks/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/hooks/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5971 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/hooks/aws.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/media/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/media/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10231 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/media/thumbnail.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.942003 pibble-0.4.6/pibble/resources/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/resources/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10649 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/resources/retriever.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2651 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.946003 pibble-0.4.6/pibble/util/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/util/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8375 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/util/encryption.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16134 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/util/files.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    32731 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/util/helpers.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/util/imaging.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/util/log.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1610 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/util/numeric.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    26217 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/util/strings.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.946003 pibble-0.4.6/pibble/web/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/web/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble/web/scraper.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-04-30 02:20:26.934004 pibble-0.4.6/pibble.egg-info/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6410 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble.egg-info/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5413 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble.egg-info/entry_points.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1818 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble.egg-info/requires.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-04-30 02:20:26.000000 pibble-0.4.6/pibble.egg-info/top_level.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-04-30 02:20:26.946003 pibble-0.4.6/setup.cfg
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2651 2023-04-30 02:20:26.000000 pibble-0.4.6/setup.py
```

### Comparing `pibble-0.4.5/PKG-INFO` & `pibble-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.4.5
+Version: 0.4.6
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.4.5/README.md` & `pibble-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/__main__.py` & `pibble-0.4.6/pibble/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,33 +39,48 @@
 
 
 @main.command(short_help="Start a server based on configuration.")
 @click.argument("configuration")
 @click.option(
     "--debug", is_flag=True, help="Turn on debug unified logging.", default=False
 )
-def server(configuration: str, debug: bool = False) -> None:
+@click.option(
+    "--interactive",
+    is_flag=True,
+    help="After instantiation, enter an interactive console instead of serving.",
+    default=False,
+)
+def server(configuration: str, debug: bool = False, interactive: bool = False) -> None:
     """
     Starts a server, synchronously, using a configuration file.
 
     The configuration file format is specified by its extension (.yml/.yaml being YAML, .json being JSON). No other formats are accepted.
     """
     factory = MetaFactory.from_file(configuration)
 
     if debug:
         context = DebugUnifiedLoggingContext()
     else:
         context = ConfigurationLoggingContext(factory.api_configuration)  # type: ignore
 
     with context:
         service = factory("server")
-        try:
-            service.serve()
-        finally:
-            service.destroy()
+        if interactive:
+            print(
+                termcolor.colored(
+                    "Entering console. Use global object 'server' as instantiated server.",
+                    "cyan",
+                )
+            )
+            code.interact(local={"server": service.instance})
+        else:
+            try:
+                service.serve()
+            finally:
+                service.destroy()
 
 
 @main.command(short_help="Start multiple servers based on configurations.")
 @click.argument("configuration", nargs=-1)
 @click.option(
     "--debug", is_flag=True, help="Turn on debug unified logging.", default=False
 )
@@ -254,15 +269,17 @@
     height: int = 128,
 ) -> None:
     """
     Builds a thumbnail from an input path.
     """
     with LevelUnifiedLoggingContext(logging.DEBUG if debug else logging.WARNING):
         from pibble.media.thumbnail import ThumbnailBuilder
+
         ThumbnailBuilder(input).build(output, width, height, trim=trim)
 
+
 try:
     main()
 except Exception as ex:
     print(termcolor.colored(str(ex), "red"))
     sys.exit(5)
 sys.exit(0)
```

### Comparing `pibble-0.4.5/pibble/api/base.py` & `pibble-0.4.6/pibble/api/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/apachethrift/__init__.py` & `pibble-0.4.6/pibble/api/client/apachethrift/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/apachethrift/wrapper.py` & `pibble-0.4.6/pibble/api/client/apachethrift/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/base.py` & `pibble-0.4.6/pibble/api/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/file/base.py` & `pibble-0.4.6/pibble/api/client/file/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/file/ftp.py` & `pibble-0.4.6/pibble/api/client/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/file/hdfs.py` & `pibble-0.4.6/pibble/api/client/file/hdfs.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/file/local.py` & `pibble-0.4.6/pibble/api/client/file/local.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/file/sftp.py` & `pibble-0.4.6/pibble/api/client/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/googlerpc.py` & `pibble-0.4.6/pibble/api/client/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/webservice/apachethrift.py` & `pibble-0.4.6/pibble/api/client/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/webservice/base.py` & `pibble-0.4.6/pibble/api/client/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/webservice/jsonapi.py` & `pibble-0.4.6/pibble/api/client/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/webservice/rpc/base.py` & `pibble-0.4.6/pibble/api/client/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/webservice/rpc/jsonrpc.py` & `pibble-0.4.6/pibble/api/client/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/webservice/rpc/xmlrpc.py` & `pibble-0.4.6/pibble/api/client/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/webservice/soap.py` & `pibble-0.4.6/pibble/api/client/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/webservice/wrapper.py` & `pibble-0.4.6/pibble/api/client/webservice/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/client/wrapper.py` & `pibble-0.4.6/pibble/api/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/configuration.py` & `pibble-0.4.6/pibble/api/configuration.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/exceptions.py` & `pibble-0.4.6/pibble/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/helpers/apachethrift.py` & `pibble-0.4.6/pibble/api/helpers/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/helpers/authentication.py` & `pibble-0.4.6/pibble/api/helpers/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/helpers/googlerpc.py` & `pibble-0.4.6/pibble/api/helpers/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/helpers/store.py` & `pibble-0.4.6/pibble/api/helpers/store.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/helpers/wrappers.py` & `pibble-0.4.6/pibble/api/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/meta/base.py` & `pibble-0.4.6/pibble/api/meta/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/meta/helpers.py` & `pibble-0.4.6/pibble/api/meta/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/apachethrift/base.py` & `pibble-0.4.6/pibble/api/middleware/apachethrift/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/apachethrift/screening.py` & `pibble-0.4.6/pibble/api/middleware/apachethrift/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/database/orm.py` & `pibble-0.4.6/pibble/api/middleware/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/googlerpc/authentication.py` & `pibble-0.4.6/pibble/api/middleware/googlerpc/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/googlerpc/base.py` & `pibble-0.4.6/pibble/api/middleware/googlerpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/googlerpc/metadata.py` & `pibble-0.4.6/pibble/api/middleware/googlerpc/metadata.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/screening.py` & `pibble-0.4.6/pibble/api/middleware/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/webservice/authentication/basic.py` & `pibble-0.4.6/pibble/api/middleware/webservice/authentication/basic.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/webservice/authentication/bearer.py` & `pibble-0.4.6/pibble/api/middleware/webservice/authentication/bearer.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/webservice/authentication/digest.py` & `pibble-0.4.6/pibble/api/middleware/webservice/authentication/digest.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/webservice/authentication/header.py` & `pibble-0.4.6/pibble/api/middleware/webservice/authentication/header.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/webservice/authentication/oauth.py` & `pibble-0.4.6/pibble/api/middleware/webservice/authentication/oauth.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/webservice/base.py` & `pibble-0.4.6/pibble/api/middleware/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/webservice/limit.py` & `pibble-0.4.6/pibble/api/middleware/webservice/limit.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/middleware/webservice/screening.py` & `pibble-0.4.6/pibble/api/middleware/webservice/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/protocol/apachethrift.py` & `pibble-0.4.6/pibble/api/protocol/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/apachethrift.py` & `pibble-0.4.6/pibble/api/server/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/base.py` & `pibble-0.4.6/pibble/api/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/file/ftp.py` & `pibble-0.4.6/pibble/api/server/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/file/sftp.py` & `pibble-0.4.6/pibble/api/server/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/googlerpc.py` & `pibble-0.4.6/pibble/api/server/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/apachethrift.py` & `pibble-0.4.6/pibble/api/server/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/awslambda.py` & `pibble-0.4.6/pibble/api/server/webservice/awslambda.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/base.py` & `pibble-0.4.6/pibble/api/server/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/handler.py` & `pibble-0.4.6/pibble/api/server/webservice/handler.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/jsonapi.py` & `pibble-0.4.6/pibble/api/server/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/mixin/base.py` & `pibble-0.4.6/pibble/api/server/webservice/mixin/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/orm.py` & `pibble-0.4.6/pibble/api/server/webservice/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/rpc/base.py` & `pibble-0.4.6/pibble/api/server/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/rpc/jsonrpc.py` & `pibble-0.4.6/pibble/api/server/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/rpc/xmlrpc.py` & `pibble-0.4.6/pibble/api/server/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/soap.py` & `pibble-0.4.6/pibble/api/server/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/template/__init__.py` & `pibble-0.4.6/pibble/api/server/webservice/template/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,17 @@
 
     def on_configure(self) -> None:
         """
         Create the template loader.
 
         This does not require any actual configuration, but see :class:pibble.api.server.webservice.html.server.TemplateServerTemplateLoader for optional keys.
         """
-        self.templates = TemplateLoader(self.configuration, server=self)
+        if not hasattr(self, "templates"):
+            logger.debug("Creating template loader.")
+            self.templates = TemplateLoader(self.configuration, server=self)
 
     def prepare_context_all(self, request: Request, response: Response) -> None:
         """
         Runs all "prepareContext" functions.
         """
 
         handler = getattr(request, "handler", None)
```

### Comparing `pibble-0.4.5/pibble/api/server/webservice/template/extensions.py` & `pibble-0.4.6/pibble/api/server/webservice/template/extensions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/api/server/webservice/template/loader.py` & `pibble-0.4.6/pibble/api/server/webservice/template/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,36 +153,36 @@
                 "{0}Extension".format(extension.__name__), (extension,), lambdas
             )
 
             if issubclass(extension, TestExtensionBase):
                 if extension in self.tests:
                     logger.debug("Tried to extend template loader with duplicate test {0}".format(extension))
                     return
-                logger.debug("Template loading adding test {0}".format(extension))
+                logger.debug("Template loader adding test {0}".format(extension))
                 self.tests.append(extension)
                 extension.assign(self.environment)
             elif issubclass(extension, FilterExtensionBase):
                 if extension in self.filters:
                     logger.debug("Tried to extend template loader with duplicate filter {0}".format(extension))
                     return
-                logger.debug("Template loading adding filter {0}".format(extension))
+                logger.debug("Template loader adding filter {0}".format(extension))
                 self.filters.append(extension)
                 extension.assign(self.environment)
             elif issubclass(extension, FunctionExtensionBase):
                 if extension in self.functions:
                     logger.debug("Tried to extend template loader with duplicate function {0}".format(extension))
                     return
-                logger.debug("Template loading adding function {0}".format(extension))
+                logger.debug("Template loader adding function {0}".format(extension))
                 self.functions.append(extension)
                 extension.assign(self.environment)
             elif issubclass(extension, Extension):
                 if extension in self.extensions:
                     logger.debug("Tried to extend template loader with duplicate extension {0}".format(extension))
                     return
-                logger.debug("Template loading adding extension {0}".format(extension))
+                logger.debug("Template loader adding extension {0}".format(extension))
                 self.extensions.append(extension)
                 self.environment.add_extension(extension)
             else:
                 raise ConfigurationError(
                     "Extension does not extend either a base or assignable Jinja2 extension."
                 )
```

### Comparing `pibble-0.4.5/pibble/database/dedupe.py` & `pibble-0.4.6/pibble/database/dedupe.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/database/engine.py` & `pibble-0.4.6/pibble/database/engine.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/database/orm.py` & `pibble-0.4.6/pibble/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/database/util.py` & `pibble-0.4.6/pibble/database/util.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/cms/database/__init__.py` & `pibble-0.4.6/pibble/ext/cms/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/cms/database/interface.py` & `pibble-0.4.6/pibble/ext/cms/database/interface.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/cms/database/menu.py` & `pibble-0.4.6/pibble/ext/cms/database/menu.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/cms/database/view.py` & `pibble-0.4.6/pibble/ext/cms/database/view.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/cms/server/base.py` & `pibble-0.4.6/pibble/ext/cms/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/cms/server/extension.py` & `pibble-0.4.6/pibble/ext/cms/server/extension.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/dam/database/files.py` & `pibble-0.4.6/pibble/ext/dam/database/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/rest/server/base.py` & `pibble-0.4.6/pibble/ext/rest/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/rest/server/user.py` & `pibble-0.4.6/pibble/ext/rest/server/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/session/database/session.py` & `pibble-0.4.6/pibble/ext/session/database/session.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/session/server/base.py` & `pibble-0.4.6/pibble/ext/session/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/user/client/base.py` & `pibble-0.4.6/pibble/ext/user/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/user/database/__init__.py` & `pibble-0.4.6/pibble/ext/user/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/user/database/authentication.py` & `pibble-0.4.6/pibble/ext/user/database/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/user/database/notification.py` & `pibble-0.4.6/pibble/ext/user/database/notification.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/user/database/permission.py` & `pibble-0.4.6/pibble/ext/user/database/permission.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/user/database/user.py` & `pibble-0.4.6/pibble/ext/user/database/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/ext/user/server/base.py` & `pibble-0.4.6/pibble/ext/user/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/hooks/aws.py` & `pibble-0.4.6/pibble/hooks/aws.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/media/thumbnail.py` & `pibble-0.4.6/pibble/media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/resources/retriever.py` & `pibble-0.4.6/pibble/resources/retriever.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/setup.py` & `pibble-0.4.6/pibble/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "4"
-version_patch = "5"
+version_patch = "6"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

### Comparing `pibble-0.4.5/pibble/util/encryption.py` & `pibble-0.4.6/pibble/util/encryption.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/util/files.py` & `pibble-0.4.6/pibble/util/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/util/helpers.py` & `pibble-0.4.6/pibble/util/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/util/imaging.py` & `pibble-0.4.6/pibble/util/imaging.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/util/log.py` & `pibble-0.4.6/pibble/util/log.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/util/numeric.py` & `pibble-0.4.6/pibble/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/util/strings.py` & `pibble-0.4.6/pibble/util/strings.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble/web/scraper.py` & `pibble-0.4.6/pibble/web/scraper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble.egg-info/PKG-INFO` & `pibble-0.4.6/pibble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.4.5
+Version: 0.4.6
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.4.5/pibble.egg-info/SOURCES.txt` & `pibble-0.4.6/pibble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/pibble.egg-info/requires.txt` & `pibble-0.4.6/pibble.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.4.5/setup.py` & `pibble-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "4"
-version_patch = "5"
+version_patch = "6"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

