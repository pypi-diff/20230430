# Comparing `tmp/ipytablewidgets-0.3.0.tar.gz` & `tmp/ipytablewidgets-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipytablewidgets-0.3.0.tar", last modified: Thu Feb 23 09:08:42 2023, max compression
+gzip compressed data, was "ipytablewidgets-0.3.1.tar", last modified: Sun Apr 30 13:28:27 2023, max compression
```

## Comparing `ipytablewidgets-0.3.0.tar` & `ipytablewidgets-0.3.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.213383 ipytablewidgets-0.3.0/
--rw-rw-r--   0 poli      (1000) poli      (1000)     1541 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/LICENSE
--rw-rw-r--   0 poli      (1000) poli      (1000)      378 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/MANIFEST.in
--rw-rw-r--   0 poli      (1000) poli      (1000)     4123 2023-02-23 09:08:42.213383 ipytablewidgets-0.3.0/PKG-INFO
--rw-rw-r--   0 poli      (1000) poli      (1000)     3645 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/README.md
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.209383 ipytablewidgets-0.3.0/ipytablewidgets/
--rw-rw-r--   0 poli      (1000) poli      (1000)     1266 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/__init__.py
--rw-rw-r--   0 poli      (1000) poli      (1000)      220 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/_frontend.py
--rw-rw-r--   0 poli      (1000) poli      (1000)      359 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/_version.py
--rw-rw-r--   0 poli      (1000) poli      (1000)      955 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/compressors.py
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.209383 ipytablewidgets-0.3.0/ipytablewidgets/labextension/
--rw-rw-r--   0 poli      (1000) poli      (1000)     2502 2023-02-23 09:08:41.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/package.json
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.209383 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/
--rw-rw-r--   0 poli      (1000) poli      (1000)    53467 2023-02-23 09:08:41.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/149.511825bb9d94bbe4bf05.js
--rw-rw-r--   0 poli      (1000) poli      (1000)     4766 2023-02-23 09:08:41.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/261.30f6acbfe21f61ea9fcb.js
--rw-rw-r--   0 poli      (1000) poli      (1000)     4836 2023-02-23 09:08:41.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/405.6e1d012d86b0ed03bddf.js
--rw-rw-r--   0 poli      (1000) poli      (1000)    46806 2023-02-23 09:08:41.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/424.e42e48076aba64887fd2.js
--rw-rw-r--   0 poli      (1000) poli      (1000)     4493 2023-02-23 09:08:41.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/568.d147460c8c05ef5ec171.js
--rw-rw-r--   0 poli      (1000) poli      (1000)     6826 2023-02-23 09:08:41.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/861.78ea6fdd74d109f94c90.js
--rw-rw-r--   0 poli      (1000) poli      (1000)      120 2023-02-23 09:08:41.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/861.78ea6fdd74d109f94c90.js.LICENSE.txt
--rw-rw-r--   0 poli      (1000) poli      (1000)     7404 2023-02-23 09:08:41.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/remoteEntry.1cfba1745e46fef97d30.js
--rw-rw-r--   0 poli      (1000) poli      (1000)      118 2023-02-23 09:08:39.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/style.js
--rw-rw-r--   0 poli      (1000) poli      (1000)    13841 2023-02-23 09:08:41.000000 ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/third-party-licenses.json
--rw-rw-r--   0 poli      (1000) poli      (1000)      995 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/numpy_adapter.py
--rw-rw-r--   0 poli      (1000) poli      (1000)     6005 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/pandas_adapter.py
--rw-rw-r--   0 poli      (1000) poli      (1000)      892 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/progressivis_adapter.py
--rw-rw-r--   0 poli      (1000) poli      (1000)     3177 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/serializers.py
--rw-rw-r--   0 poli      (1000) poli      (1000)     1078 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/source_adapter.py
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.209383 ipytablewidgets-0.3.0/ipytablewidgets/static/
--rw-rw-r--   0 poli      (1000) poli      (1000)      307 2023-02-23 09:08:34.000000 ipytablewidgets-0.3.0/ipytablewidgets/static/extension.js
--rw-rw-r--   0 poli      (1000) poli      (1000)   116771 2023-02-23 09:08:36.000000 ipytablewidgets-0.3.0/ipytablewidgets/static/index.js
--rw-rw-r--   0 poli      (1000) poli      (1000)      120 2023-02-23 09:08:36.000000 ipytablewidgets-0.3.0/ipytablewidgets/static/index.js.LICENSE.txt
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.209383 ipytablewidgets-0.3.0/ipytablewidgets/tests/
--rw-rw-r--   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/tests/__init__.py
--rw-rw-r--   0 poli      (1000) poli      (1000)     2257 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/tests/test_compression.py
--rw-rw-r--   0 poli      (1000) poli      (1000)      596 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/tests/test_frontend_version.py
--rw-rw-r--   0 poli      (1000) poli      (1000)     1841 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/tests/test_serialization.py
--rw-rw-r--   0 poli      (1000) poli      (1000)     5676 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/tests/test_table.py
--rw-rw-r--   0 poli      (1000) poli      (1000)     1049 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/tests/test_traitlets.py
--rw-rw-r--   0 poli      (1000) poli      (1000)     1321 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/traitlets.py
--rw-rw-r--   0 poli      (1000) poli      (1000)     1785 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/ipytablewidgets/widgets.py
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.209383 ipytablewidgets-0.3.0/ipytablewidgets.egg-info/
--rw-rw-r--   0 poli      (1000) poli      (1000)     4123 2023-02-23 09:08:42.000000 ipytablewidgets-0.3.0/ipytablewidgets.egg-info/PKG-INFO
--rw-rw-r--   0 poli      (1000) poli      (1000)     2298 2023-02-23 09:08:42.000000 ipytablewidgets-0.3.0/ipytablewidgets.egg-info/SOURCES.txt
--rw-rw-r--   0 poli      (1000) poli      (1000)        1 2023-02-23 09:08:42.000000 ipytablewidgets-0.3.0/ipytablewidgets.egg-info/dependency_links.txt
--rw-rw-r--   0 poli      (1000) poli      (1000)        1 2023-02-23 09:08:27.000000 ipytablewidgets-0.3.0/ipytablewidgets.egg-info/not-zip-safe
--rw-rw-r--   0 poli      (1000) poli      (1000)      102 2023-02-23 09:08:42.000000 ipytablewidgets-0.3.0/ipytablewidgets.egg-info/requires.txt
--rw-rw-r--   0 poli      (1000) poli      (1000)       16 2023-02-23 09:08:42.000000 ipytablewidgets-0.3.0/ipytablewidgets.egg-info/top_level.txt
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.213383 ipytablewidgets-0.3.0/js/
--rw-rw-r--   0 poli      (1000) poli      (1000)      447 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/README.md
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.213383 ipytablewidgets-0.3.0/js/dist/
--rw-rw-r--   0 poli      (1000) poli      (1000)   116771 2023-02-23 09:08:37.000000 ipytablewidgets-0.3.0/js/dist/index.js
--rw-rw-r--   0 poli      (1000) poli      (1000)      120 2023-02-23 09:08:37.000000 ipytablewidgets-0.3.0/js/dist/index.js.LICENSE.txt
--rw-rw-r--   0 poli      (1000) poli      (1000)      191 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/install.json
--rw-rw-r--   0 poli      (1000) poli      (1000)       74 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/jupyter-tablewidgets.json
--rw-rw-r--   0 poli      (1000) poli      (1000)     1407 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/karma.conf.js
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.213383 ipytablewidgets-0.3.0/js/lib/
--rw-rw-r--   0 poli      (1000) poli      (1000)       67 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/compression.d.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)      515 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/compression.js
--rw-rw-r--   0 poli      (1000) poli      (1000)       56 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/extension.d.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)      465 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/extension.js
--rw-rw-r--   0 poli      (1000) poli      (1000)      236 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/index.d.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)     1373 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/index.js
--rw-rw-r--   0 poli      (1000) poli      (1000)       11 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/labplugin.d.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)      510 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/labplugin.js
--rw-rw-r--   0 poli      (1000) poli      (1000)     1241 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/serializers.d.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)     3896 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/serializers.js
--rw-rw-r--   0 poli      (1000) poli      (1000)      631 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/widgets.d.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)     3269 2023-02-23 09:08:33.000000 ipytablewidgets-0.3.0/js/lib/widgets.js
--rw-rw-r--   0 poli      (1000) poli      (1000)     2386 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/package.json
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.213383 ipytablewidgets-0.3.0/js/src/
--rw-rw-r--   0 poli      (1000) poli      (1000)      475 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/src/compression.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)      278 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/src/extension.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)      365 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/src/index.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)      371 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/src/labplugin.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)     4519 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/src/serializers.ts
-drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-02-23 09:08:42.213383 ipytablewidgets-0.3.0/js/src/tests/
--rw-rw-r--   0 poli      (1000) poli      (1000)     5645 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/src/tests/allSpec.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)      353 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/src/tests/tsconfig.json
--rw-rw-r--   0 poli      (1000) poli      (1000)       56 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/src/types.d.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)     2104 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/src/widgets.ts
--rw-rw-r--   0 poli      (1000) poli      (1000)      460 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/tsconfig.json
--rw-rw-r--   0 poli      (1000) poli      (1000)     1055 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/webpack.config.js
--rw-rw-r--   0 poli      (1000) poli      (1000)   253238 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/js/yarn.lock
--rw-rw-r--   0 poli      (1000) poli      (1000)      154 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/pyproject.toml
--rw-rw-r--   0 poli      (1000) poli      (1000)     1273 2023-02-23 09:08:42.217383 ipytablewidgets-0.3.0/setup.cfg
--rw-rw-r--   0 poli      (1000) poli      (1000)     1555 2023-02-23 09:08:12.000000 ipytablewidgets-0.3.0/setup.py
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.268473 ipytablewidgets-0.3.1/
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1541 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/LICENSE
+-rw-rw-r--   0 poli      (1000) poli      (1000)      378 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/MANIFEST.in
+-rw-rw-r--   0 poli      (1000) poli      (1000)     4123 2023-04-30 13:28:27.268473 ipytablewidgets-0.3.1/PKG-INFO
+-rw-rw-r--   0 poli      (1000) poli      (1000)     3645 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/README.md
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.260473 ipytablewidgets-0.3.1/ipytablewidgets/
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1266 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/__init__.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)      220 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/_frontend.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)      359 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/_version.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)      955 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/compressors.py
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.260473 ipytablewidgets-0.3.1/ipytablewidgets/labextension/
+-rw-rw-r--   0 poli      (1000) poli      (1000)     2502 2023-04-30 13:28:26.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/package.json
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.260473 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/
+-rw-rw-r--   0 poli      (1000) poli      (1000)    53467 2023-04-30 13:28:26.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/149.511825bb9d94bbe4bf05.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)     4766 2023-04-30 13:28:26.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/261.bc115825a135ccbef0e9.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)     4836 2023-04-30 13:28:26.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/405.6e1d012d86b0ed03bddf.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)    46806 2023-04-30 13:28:26.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/424.e42e48076aba64887fd2.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)     4493 2023-04-30 13:28:26.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/568.46074a0ad0e0cb2bad6c.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)     6826 2023-04-30 13:28:26.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/861.78ea6fdd74d109f94c90.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)      120 2023-04-30 13:28:26.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/861.78ea6fdd74d109f94c90.js.LICENSE.txt
+-rw-rw-r--   0 poli      (1000) poli      (1000)     7404 2023-04-30 13:28:26.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/remoteEntry.f37ccf70604f30c0f9de.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)      118 2023-04-30 13:28:23.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/style.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)    13841 2023-04-30 13:28:26.000000 ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/third-party-licenses.json
+-rw-rw-r--   0 poli      (1000) poli      (1000)      995 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/numpy_adapter.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)     6005 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/pandas_adapter.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)      892 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/progressivis_adapter.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)     3177 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/serializers.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1078 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/source_adapter.py
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.260473 ipytablewidgets-0.3.1/ipytablewidgets/static/
+-rw-rw-r--   0 poli      (1000) poli      (1000)      307 2023-04-30 13:28:18.000000 ipytablewidgets-0.3.1/ipytablewidgets/static/extension.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)   116771 2023-04-30 13:28:21.000000 ipytablewidgets-0.3.1/ipytablewidgets/static/index.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)      120 2023-04-30 13:28:21.000000 ipytablewidgets-0.3.1/ipytablewidgets/static/index.js.LICENSE.txt
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.264473 ipytablewidgets-0.3.1/ipytablewidgets/tests/
+-rw-rw-r--   0 poli      (1000) poli      (1000)        0 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/tests/__init__.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)     2257 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/tests/test_compression.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)      596 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/tests/test_frontend_version.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1841 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/tests/test_serialization.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)     5676 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/tests/test_table.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1049 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/tests/test_traitlets.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1321 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/traitlets.py
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1785 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/ipytablewidgets/widgets.py
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.260473 ipytablewidgets-0.3.1/ipytablewidgets.egg-info/
+-rw-rw-r--   0 poli      (1000) poli      (1000)     4123 2023-04-30 13:28:27.000000 ipytablewidgets-0.3.1/ipytablewidgets.egg-info/PKG-INFO
+-rw-rw-r--   0 poli      (1000) poli      (1000)     2298 2023-04-30 13:28:27.000000 ipytablewidgets-0.3.1/ipytablewidgets.egg-info/SOURCES.txt
+-rw-rw-r--   0 poli      (1000) poli      (1000)        1 2023-04-30 13:28:27.000000 ipytablewidgets-0.3.1/ipytablewidgets.egg-info/dependency_links.txt
+-rw-rw-r--   0 poli      (1000) poli      (1000)        1 2023-04-30 13:28:11.000000 ipytablewidgets-0.3.1/ipytablewidgets.egg-info/not-zip-safe
+-rw-rw-r--   0 poli      (1000) poli      (1000)      102 2023-04-30 13:28:27.000000 ipytablewidgets-0.3.1/ipytablewidgets.egg-info/requires.txt
+-rw-rw-r--   0 poli      (1000) poli      (1000)       16 2023-04-30 13:28:27.000000 ipytablewidgets-0.3.1/ipytablewidgets.egg-info/top_level.txt
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.264473 ipytablewidgets-0.3.1/js/
+-rw-rw-r--   0 poli      (1000) poli      (1000)      447 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/README.md
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.264473 ipytablewidgets-0.3.1/js/dist/
+-rw-rw-r--   0 poli      (1000) poli      (1000)   116771 2023-04-30 13:28:21.000000 ipytablewidgets-0.3.1/js/dist/index.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)      120 2023-04-30 13:28:21.000000 ipytablewidgets-0.3.1/js/dist/index.js.LICENSE.txt
+-rw-rw-r--   0 poli      (1000) poli      (1000)      191 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/install.json
+-rw-rw-r--   0 poli      (1000) poli      (1000)       74 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/jupyter-tablewidgets.json
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1407 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/karma.conf.js
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.264473 ipytablewidgets-0.3.1/js/lib/
+-rw-rw-r--   0 poli      (1000) poli      (1000)       67 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/compression.d.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)      515 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/compression.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)       56 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/extension.d.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)      465 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/extension.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)      236 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/index.d.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1373 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/index.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)       11 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/labplugin.d.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)      510 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/labplugin.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1241 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/serializers.d.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)     3896 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/serializers.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)      631 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/widgets.d.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)     3269 2023-04-30 13:28:17.000000 ipytablewidgets-0.3.1/js/lib/widgets.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)     2386 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/package.json
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.268473 ipytablewidgets-0.3.1/js/src/
+-rw-rw-r--   0 poli      (1000) poli      (1000)      475 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/src/compression.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)      278 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/src/extension.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)      365 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/src/index.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)      371 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/src/labplugin.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)     4519 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/src/serializers.ts
+drwxrwxr-x   0 poli      (1000) poli      (1000)        0 2023-04-30 13:28:27.268473 ipytablewidgets-0.3.1/js/src/tests/
+-rw-rw-r--   0 poli      (1000) poli      (1000)     5645 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/src/tests/allSpec.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)      353 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/src/tests/tsconfig.json
+-rw-rw-r--   0 poli      (1000) poli      (1000)       56 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/src/types.d.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)     2104 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/src/widgets.ts
+-rw-rw-r--   0 poli      (1000) poli      (1000)      460 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/tsconfig.json
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1055 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/webpack.config.js
+-rw-rw-r--   0 poli      (1000) poli      (1000)   253238 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/js/yarn.lock
+-rw-rw-r--   0 poli      (1000) poli      (1000)      154 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/pyproject.toml
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1273 2023-04-30 13:28:27.268473 ipytablewidgets-0.3.1/setup.cfg
+-rw-rw-r--   0 poli      (1000) poli      (1000)     1555 2023-04-30 13:27:53.000000 ipytablewidgets-0.3.1/setup.py
```

### Comparing `ipytablewidgets-0.3.0/LICENSE` & `ipytablewidgets-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/PKG-INFO` & `ipytablewidgets-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipytablewidgets
-Version: 0.3.0
+Version: 0.3.1
 Summary: A set of widgets to help facilitate reuse of large tables across widgets
 Home-page: https://github.com/progressivis/ipytablewidgets
 Author: Jean-Daniel Fekete, Christian Poli
 Author-email: ipytablewidgets@inria.fr
 License: BSD-3-Clause
 Keywords: ipython,jupyter,widgets
 Platform: Linux
```

### Comparing `ipytablewidgets-0.3.0/README.md` & `ipytablewidgets-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/__init__.py` & `ipytablewidgets-0.3.1/ipytablewidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/compressors.py` & `ipytablewidgets-0.3.1/ipytablewidgets/compressors.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/labextension/package.json` & `ipytablewidgets-0.3.1/js/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9553571428571429%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.3.1'"}*

```diff
@@ -37,18 +37,14 @@
     },
     "files": [
         "lib/",
         "dist/"
     ],
     "homepage": "https://github.com/progressivis/ipytablewidgets/#readme",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.1cfba1745e46fef97d30.js"
-        },
         "extension": "lib/labplugin",
         "outputDir": "../ipytablewidgets/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -71,9 +67,9 @@
         "test": "npm run test:firefox",
         "test:chrome": "karma start --browsers=Chrome karma.conf.js",
         "test:ci": "karma start --browsers=ChromeCI karma.conf.js",
         "test:debug": "karma start --browsers=Chrome --singleRun=false --debug=true karma.conf.js",
         "test:firefox": "karma start --browsers=Firefox karma.conf.js",
         "watch": "webpack --mode development --watch"
     },
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/149.511825bb9d94bbe4bf05.js` & `ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/149.511825bb9d94bbe4bf05.js`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/261.30f6acbfe21f61ea9fcb.js` & `ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/261.bc115825a135ccbef0e9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -249,12 +249,12 @@
                     }))
                 }
             }
             t.EchoTableWidgetView = c
         },
         147: e => {
             e.exports = {
-                version: "0.3.0"
+                version: "0.3.1"
             }
         }
     }
 ]);
```

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/405.6e1d012d86b0ed03bddf.js` & `ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/405.6e1d012d86b0ed03bddf.js`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/424.e42e48076aba64887fd2.js` & `ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/424.e42e48076aba64887fd2.js`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/568.d147460c8c05ef5ec171.js` & `ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/568.46074a0ad0e0cb2bad6c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -230,12 +230,12 @@
                     }))
                 }
             }
             t.EchoTableWidgetView = c
         },
         147: e => {
             e.exports = {
-                version: "0.3.0"
+                version: "0.3.1"
             }
         }
     }
 ]);
```

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/861.78ea6fdd74d109f94c90.js` & `ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/861.78ea6fdd74d109f94c90.js`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/remoteEntry.1cfba1745e46fef97d30.js` & `ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/remoteEntry.f37ccf70604f30c0f9de.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, f, d, s, c, p, h, b, v, g, m = {
-            309: (e, r, t) => {
+    var e, r, t, n, a, o, i, u, l, d, s, f, p, c, h, v, b, g, m = {
+            858: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(426), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(426), t.e(261)]).then((() => () => t(261)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
@@ -37,58 +37,58 @@
     w.m = m, w.c = y, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
         149: "511825bb9d94bbe4bf05",
-        261: "30f6acbfe21f61ea9fcb",
+        261: "bc115825a135ccbef0e9",
         405: "6e1d012d86b0ed03bddf",
         424: "e42e48076aba64887fd2",
         426: "281905b24712b5be0d7d",
-        568: "d147460c8c05ef5ec171",
+        568: "46074a0ad0e0cb2bad6c",
         861: "78ea6fdd74d109f94c90"
     } [e] + ".js?v=" + {
         149: "511825bb9d94bbe4bf05",
-        261: "30f6acbfe21f61ea9fcb",
+        261: "bc115825a135ccbef0e9",
         405: "6e1d012d86b0ed03bddf",
         424: "e42e48076aba64887fd2",
         426: "281905b24712b5be0d7d",
-        568: "d147460c8c05ef5ec171",
+        568: "46074a0ad0e0cb2bad6c",
         861: "78ea6fdd74d109f94c90"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), w.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "jupyter-tablewidgets:", w.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var d = l[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
-                        i = d;
+                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
+                    var s = l[d];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, w.nc && i.setAttribute("nonce", w.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var s = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+            var f = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, w.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -110,15 +110,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("jupyter-tablewidgets", "0.3.0", (() => Promise.all([w.e(426), w.e(568)]).then((() => () => w(568))))), u("lz4js", "0.2.0", (() => w.e(405).then((() => () => w(405))))), u("ndarray-unpack", "1.0.0", (() => w.e(149).then((() => () => w(149))))), u("ndarray", "1.0.19", (() => w.e(861).then((() => () => w(861))))), u("pako", "2.1.0", (() => w.e(424).then((() => () => w(424)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyter-tablewidgets", "0.3.1", (() => Promise.all([w.e(426), w.e(568)]).then((() => () => w(568))))), u("lz4js", "0.2.0", (() => w.e(405).then((() => () => w(405))))), u("ndarray-unpack", "1.0.0", (() => w.e(149).then((() => () => w(149))))), u("ndarray", "1.0.19", (() => w.e(861).then((() => () => w(861))))), u("pako", "2.1.0", (() => w.e(424).then((() => () => w(424)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -167,90 +167,90 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !a : "" == s != a);
-                if ("u" == d) {
-                    if (!l || "u" != s) return !1
+                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > n && !a : "" == f != a);
+                if ("u" == s) {
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (s == d)
+                    if (f == s)
                         if (u <= n) {
-                            if (f != e[u]) return !1
+                            if (d != e[u]) return !1
                         } else {
-                            if (a ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (l = !1)
+                            if (a ? d > e[u] : d < e[u]) return !1;
+                            d != e[u] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != f && "n" != f) {
                     if (a || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < s != a) return !1;
+                    if (u <= n || s < f != a) return !1;
                     l = !1
-                } else "s" != s && "n" != s && (l = !1, u--)
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
         var a = u(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), s(e[t][a])
-    }, d = (e, r, t) => {
+        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), f(e[t][a])
+    }, s = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, s = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, a) {
+    }, f = e => (e.loaded = 1, e.get()), c = (p = e => function(r, t, n, a) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, n, a)) : e(r, w.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
-        var o = r && w.o(r, t) && d(r, t, n);
-        return o ? s(o) : a()
-    })), b = {}, v = {
+    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), h = p(((e, r, t, n, a) => {
+        var o = r && w.o(r, t) && s(r, t, n);
+        return o ? f(o) : a()
+    })), v = {}, b = {
         41: () => h("default", "ndarray-unpack", [1, 1, 0, 0], (() => w.e(149).then((() => () => w(149))))),
         178: () => h("default", "lz4js", [2, 0, 2, 0], (() => w.e(405).then((() => () => w(405))))),
-        395: () => p("default", "@jupyter-widgets/base", [, [1, 6],
+        395: () => c("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ]),
         496: () => h("default", "pako", [1, 2, 0, 3], (() => w.e(424).then((() => () => w(424))))),
         825: () => h("default", "ndarray", [1, 1, 0, 19], (() => w.e(861).then((() => () => w(861)))))
     }, g = {
         426: [41, 178, 395, 496, 825]
     }, w.f.consumes = (e, r) => {
         w.o(g, e) && g[e].forEach((e => {
-            if (w.o(b, e)) return r.push(b[e]);
+            if (w.o(v, e)) return r.push(v[e]);
             var t = r => {
-                    b[e] = 0, w.m[e] = t => {
+                    v[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete b[e], w.m[e] = t => {
+                    delete v[e], w.m[e] = t => {
                         throw delete w.c[e], r
                     }
                 };
             try {
-                var a = v[e]();
-                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
+                var a = b[e]();
+                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             887: 0
@@ -281,10 +281,10 @@
                     u && u(w)
                 }
                 for (r && r(t); l < o.length; l++) a = o[l], w.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkjupyter_tablewidgets = self.webpackChunkjupyter_tablewidgets || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var j = w(309);
+    var j = w(858);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["jupyter-tablewidgets"] = j
 })();
```

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/labextension/static/third-party-licenses.json` & `ipytablewidgets-0.3.1/ipytablewidgets/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/numpy_adapter.py` & `ipytablewidgets-0.3.1/ipytablewidgets/numpy_adapter.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/pandas_adapter.py` & `ipytablewidgets-0.3.1/ipytablewidgets/pandas_adapter.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/progressivis_adapter.py` & `ipytablewidgets-0.3.1/ipytablewidgets/progressivis_adapter.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/serializers.py` & `ipytablewidgets-0.3.1/ipytablewidgets/serializers.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/source_adapter.py` & `ipytablewidgets-0.3.1/ipytablewidgets/source_adapter.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/static/index.js` & `ipytablewidgets-0.3.1/ipytablewidgets/static/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3732,15 +3732,15 @@
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
                 e.exports = {
-                    version: "0.3.0"
+                    version: "0.3.1"
                 }
             }
         },
         r = {};
 
     function n(e) {
         var a = r[e];
```

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/tests/test_compression.py` & `ipytablewidgets-0.3.1/ipytablewidgets/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/tests/test_frontend_version.py` & `ipytablewidgets-0.3.1/ipytablewidgets/tests/test_frontend_version.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/tests/test_serialization.py` & `ipytablewidgets-0.3.1/ipytablewidgets/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/tests/test_table.py` & `ipytablewidgets-0.3.1/ipytablewidgets/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/tests/test_traitlets.py` & `ipytablewidgets-0.3.1/ipytablewidgets/tests/test_traitlets.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/traitlets.py` & `ipytablewidgets-0.3.1/ipytablewidgets/traitlets.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets/widgets.py` & `ipytablewidgets-0.3.1/ipytablewidgets/widgets.py`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets.egg-info/PKG-INFO` & `ipytablewidgets-0.3.1/ipytablewidgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipytablewidgets
-Version: 0.3.0
+Version: 0.3.1
 Summary: A set of widgets to help facilitate reuse of large tables across widgets
 Home-page: https://github.com/progressivis/ipytablewidgets
 Author: Jean-Daniel Fekete, Christian Poli
 Author-email: ipytablewidgets@inria.fr
 License: BSD-3-Clause
 Keywords: ipython,jupyter,widgets
 Platform: Linux
```

### Comparing `ipytablewidgets-0.3.0/ipytablewidgets.egg-info/SOURCES.txt` & `ipytablewidgets-0.3.1/ipytablewidgets.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 ipytablewidgets.egg-info/SOURCES.txt
 ipytablewidgets.egg-info/dependency_links.txt
 ipytablewidgets.egg-info/not-zip-safe
 ipytablewidgets.egg-info/requires.txt
 ipytablewidgets.egg-info/top_level.txt
 ipytablewidgets/labextension/package.json
 ipytablewidgets/labextension/static/149.511825bb9d94bbe4bf05.js
-ipytablewidgets/labextension/static/261.30f6acbfe21f61ea9fcb.js
+ipytablewidgets/labextension/static/261.bc115825a135ccbef0e9.js
 ipytablewidgets/labextension/static/405.6e1d012d86b0ed03bddf.js
 ipytablewidgets/labextension/static/424.e42e48076aba64887fd2.js
-ipytablewidgets/labextension/static/568.d147460c8c05ef5ec171.js
+ipytablewidgets/labextension/static/568.46074a0ad0e0cb2bad6c.js
 ipytablewidgets/labextension/static/861.78ea6fdd74d109f94c90.js
 ipytablewidgets/labextension/static/861.78ea6fdd74d109f94c90.js.LICENSE.txt
-ipytablewidgets/labextension/static/remoteEntry.1cfba1745e46fef97d30.js
+ipytablewidgets/labextension/static/remoteEntry.f37ccf70604f30c0f9de.js
 ipytablewidgets/labextension/static/style.js
 ipytablewidgets/labextension/static/third-party-licenses.json
 ipytablewidgets/static/extension.js
 ipytablewidgets/static/index.js
 ipytablewidgets/static/index.js.LICENSE.txt
 ipytablewidgets/tests/__init__.py
 ipytablewidgets/tests/test_compression.py
```

### Comparing `ipytablewidgets-0.3.0/js/dist/index.js` & `ipytablewidgets-0.3.1/js/dist/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3732,15 +3732,15 @@
             146: t => {
                 "use strict";
                 t.exports = e
             },
             147: e => {
                 "use strict";
                 e.exports = {
-                    version: "0.3.0"
+                    version: "0.3.1"
                 }
             }
         },
         r = {};
 
     function n(e) {
         var a = r[e];
```

### Comparing `ipytablewidgets-0.3.0/js/karma.conf.js` & `ipytablewidgets-0.3.1/js/karma.conf.js`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/lib/compression.js` & `ipytablewidgets-0.3.1/js/lib/compression.js`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/lib/index.js` & `ipytablewidgets-0.3.1/js/lib/index.js`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/lib/serializers.d.ts` & `ipytablewidgets-0.3.1/js/lib/serializers.d.ts`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/lib/serializers.js` & `ipytablewidgets-0.3.1/js/lib/serializers.js`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/lib/widgets.d.ts` & `ipytablewidgets-0.3.1/js/lib/widgets.d.ts`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/lib/widgets.js` & `ipytablewidgets-0.3.1/js/lib/widgets.js`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/package.json` & `ipytablewidgets-0.3.1/ipytablewidgets/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9553571428571429%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.f37ccf70604f30c0f9de.js'), "*

 * *                 "('extension', './extension')])}",*

 * * "'version'": "'0.3.1'"}*

```diff
@@ -37,14 +37,18 @@
     },
     "files": [
         "lib/",
         "dist/"
     ],
     "homepage": "https://github.com/progressivis/ipytablewidgets/#readme",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.f37ccf70604f30c0f9de.js"
+        },
         "extension": "lib/labplugin",
         "outputDir": "../ipytablewidgets/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -67,9 +71,9 @@
         "test": "npm run test:firefox",
         "test:chrome": "karma start --browsers=Chrome karma.conf.js",
         "test:ci": "karma start --browsers=ChromeCI karma.conf.js",
         "test:debug": "karma start --browsers=Chrome --singleRun=false --debug=true karma.conf.js",
         "test:firefox": "karma start --browsers=Firefox karma.conf.js",
         "watch": "webpack --mode development --watch"
     },
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `ipytablewidgets-0.3.0/js/src/serializers.ts` & `ipytablewidgets-0.3.1/js/src/serializers.ts`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/src/tests/allSpec.ts` & `ipytablewidgets-0.3.1/js/src/tests/allSpec.ts`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/src/widgets.ts` & `ipytablewidgets-0.3.1/js/src/widgets.ts`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/webpack.config.js` & `ipytablewidgets-0.3.1/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/js/yarn.lock` & `ipytablewidgets-0.3.1/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `ipytablewidgets-0.3.0/setup.cfg` & `ipytablewidgets-0.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	ipytablewidgets
 	ipytablewidgets.tests
 install_requires = 
 	ipywidgets>=7.5.0,<9
 	traitlets>=4.3.0
 	traittypes>=0.0.6
 	numpy>=1.10.4,<2.0.0
-	pandas>=1.0.0,<2.0.0
+	pandas>=1.0.0,<3.0.0
 	lz4
 classifiers = 
 	Framework :: Jupyter
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Topic :: Multimedia :: Graphics
 	License :: OSI Approved :: BSD
```

### Comparing `ipytablewidgets-0.3.0/setup.py` & `ipytablewidgets-0.3.1/setup.py`

 * *Files identical despite different names*

