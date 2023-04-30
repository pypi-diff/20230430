# Comparing `tmp/g8fyi-beancount-1.0.8.tar.gz` & `tmp/g8fyi-beancount-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g8fyi-beancount-1.0.8.tar", last modified: Wed Mar 29 14:31:54 2023, max compression
+gzip compressed data, was "g8fyi-beancount-1.0.9.tar", last modified: Sun Apr 30 17:11:16 2023, max compression
```

## Comparing `g8fyi-beancount-1.0.8.tar` & `g8fyi-beancount-1.0.9.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.609380 g8fyi-beancount-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)    18343 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/COPYING
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      963 2023-03-29 14:31:54.608379 g8fyi-beancount-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2871 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.472370 g8fyi-beancount-1.0.8/beancount/
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/VERSION
--rw-rw-rw-   0 root         (0) root         (0)     1292 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.487371 g8fyi-beancount-1.0.8/beancount/core/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7273 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/account.py
--rw-rw-rw-   0 root         (0) root         (0)     7258 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/account_test.py
--rw-rw-rw-   0 root         (0) root         (0)     6876 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/account_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5214 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/account_types_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7678 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/amount.py
--rw-rw-rw-   0 root         (0) root         (0)     5904 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/amount_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7364 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/compare.py
--rw-rw-rw-   0 root         (0) root         (0)     6172 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/compare_test.py
--rw-rw-rw-   0 root         (0) root         (0)     9103 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/convert.py
--rw-rw-rw-   0 root         (0) root         (0)    12411 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/convert_test.py
--rw-rw-rw-   0 root         (0) root         (0)    28179 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/data.py
--rw-rw-rw-   0 root         (0) root         (0)    14641 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/data_test.py
--rw-rw-rw-   0 root         (0) root         (0)    15077 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/display_context.py
--rw-rw-rw-   0 root         (0) root         (0)     8179 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/display_context_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2101 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/distribution_test.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/flags_test.py
--rw-rw-rw-   0 root         (0) root         (0)    11128 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/getters.py
--rw-rw-rw-   0 root         (0) root         (0)     8910 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/getters_test.py
--rw-rw-rw-   0 root         (0) root         (0)    13680 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/interpolate.py
--rw-rw-rw-   0 root         (0) root         (0)    22402 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/interpolate_test.py
--rw-rw-rw-   0 root         (0) root         (0)    17862 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/inventory_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2801 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/number.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/number_test.py
--rw-rw-rw-   0 root         (0) root         (0)    13305 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/position.py
--rw-rw-rw-   0 root         (0) root         (0)    13610 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/position_test.py
--rw-rw-rw-   0 root         (0) root         (0)    14486 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/prices.py
--rw-rw-rw-   0 root         (0) root         (0)    11757 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/prices_test.py
--rw-rw-rw-   0 root         (0) root         (0)    26763 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/realization.py
--rw-rw-rw-   0 root         (0) root         (0)    29660 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/core/realization_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.495371 g8fyi-beancount-1.0.8/beancount/ingest/
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2737 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/cache_test.py
--rw-rw-rw-   0 root         (0) root         (0)     9630 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    14690 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/extract_test.py
--rw-rw-rw-   0 root         (0) root         (0)    12169 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/file.py
--rw-rw-rw-   0 root         (0) root         (0)    17337 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/file_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3614 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/identify.py
--rw-rw-rw-   0 root         (0) root         (0)     5494 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/identify_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importer.py
--rw-rw-rw-   0 root         (0) root         (0)      741 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importer_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.499372 g8fyi-beancount-1.0.8/beancount/ingest/importers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2798 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/config_test.py
--rw-rw-rw-   0 root         (0) root         (0)    15322 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    14590 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/csv_test.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/fileonly.py
--rw-rw-rw-   0 root         (0) root         (0)     1408 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/fileonly_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.501372 g8fyi-beancount-1.0.8/beancount/ingest/importers/mixins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/mixins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/mixins/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/mixins/filing.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/mixins/identifier.py
--rw-rw-rw-   0 root         (0) root         (0)    10681 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/ofx.py
--rw-rw-rw-   0 root         (0) root         (0)    18051 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/importers/ofx_test.py
--rw-rw-rw-   0 root         (0) root         (0)     9245 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     5957 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/regression_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)     7351 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/regression_test.py
--rw-rw-rw-   0 root         (0) root         (0)    17376 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/scripts_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4677 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/scripts_utils_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5550 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/similar.py
--rw-rw-rw-   0 root         (0) root         (0)     5795 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ingest/similar_test.py
--rw-rw-rw-   0 root         (0) root         (0)    28931 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/loader.py
--rw-rw-rw-   0 root         (0) root         (0)    25352 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/loader_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.509372 g8fyi-beancount-1.0.8/beancount/ops/
--rw-rw-rw-   0 root         (0) root         (0)      220 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7644 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/balance.py
--rw-rw-rw-   0 root         (0) root         (0)    13449 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/balance_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2611 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/basicops.py
--rw-rw-rw-   0 root         (0) root         (0)     5009 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/basicops_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4623 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/compress.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/compress_test.py
--rw-rw-rw-   0 root         (0) root         (0)     6194 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/documents.py
--rw-rw-rw-   0 root         (0) root         (0)     9169 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/documents_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4041 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/find_prices.py
--rw-rw-rw-   0 root         (0) root         (0)     4345 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/find_prices_test.py
--rw-rw-rw-   0 root         (0) root         (0)    20860 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/holdings.py
--rw-rw-rw-   0 root         (0) root         (0)    25309 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/holdings_test.py
--rw-rw-rw-   0 root         (0) root         (0)     8451 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/lifetimes.py
--rw-rw-rw-   0 root         (0) root         (0)    16849 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/lifetimes_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7655 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/pad.py
--rw-rw-rw-   0 root         (0) root         (0)    21566 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/pad_test.py
--rw-rw-rw-   0 root         (0) root         (0)    28484 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/summarize.py
--rw-rw-rw-   0 root         (0) root         (0)    51297 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/summarize_test.py
--rw-rw-rw-   0 root         (0) root         (0)    15183 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/validation.py
--rw-rw-rw-   0 root         (0) root         (0)    15717 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/ops/validation_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.525374 g8fyi-beancount-1.0.8/beancount/parser/
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8598 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/booking.py
--rw-rw-rw-   0 root         (0) root         (0)    41024 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/booking_full.py
--rw-rw-rw-   0 root         (0) root         (0)   114109 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/booking_full_test.py
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/booking_method.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/booking_method_test.py
--rw-rw-rw-   0 root         (0) root         (0)     6612 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/booking_test.py
--rw-rw-rw-   0 root         (0) root         (0)     9952 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/cmptest.py
--rw-rw-rw-   0 root         (0) root         (0)     8232 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/cmptest_test.py
--rw-rw-rw-   0 root         (0) root         (0)     6989 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/context.py
--rw-rw-rw-   0 root         (0) root         (0)     4660 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/context_test.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/decimal.c
--rw-rw-rw-   0 root         (0) root         (0)      933 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/decimal.h
--rw-rw-rw-   0 root         (0) root         (0)   102362 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/grammar.c
--rw-rw-rw-   0 root         (0) root         (0)     7232 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/grammar.h
--rw-rw-rw-   0 root         (0) root         (0)    40241 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/grammar.py
--rw-rw-rw-   0 root         (0) root         (0)    92323 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/grammar_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/hashsrc.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/hashsrc_test.py
--rw-rw-rw-   0 root         (0) root         (0)   102749 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/lexer.c
--rw-rw-rw-   0 root         (0) root         (0)    14169 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/lexer.h
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/lexer.py
--rw-rw-rw-   0 root         (0) root         (0)    22123 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/lexer_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3565 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/macros.h
--rw-rw-rw-   0 root         (0) root         (0)    22979 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/options.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/options_test.py
--rw-rw-rw-   0 root         (0) root         (0)    12956 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/parser.c
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/parser.h
--rwxrwxrwx   0 root         (0) root         (0)    12089 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/parser.py
--rw-rw-rw-   0 root         (0) root         (0)    14718 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/parser_test.py
--rw-rw-rw-   0 root         (0) root         (0)    19852 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/printer.py
--rw-rw-rw-   0 root         (0) root         (0)    19605 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/printer_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/tokens.c
--rw-rw-rw-   0 root         (0) root         (0)     3759 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/tokens.h
--rw-rw-rw-   0 root         (0) root         (0)     2879 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/tokens_test.c
--rw-rw-rw-   0 root         (0) root         (0)     1911 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/parser/version_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.549375 g8fyi-beancount-1.0.8/beancount/plugins/
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14406 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/amortize.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/auto.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/auto_accounts.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/auto_accounts_test.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/auto_test.py
--rw-rw-rw-   0 root         (0) root         (0)    18479 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/book_conversions.py
--rw-rw-rw-   0 root         (0) root         (0)    10940 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/book_conversions_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/check_average_cost.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/check_average_cost_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2908 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/check_closing.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/check_closing_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/check_commodity.py
--rw-rw-rw-   0 root         (0) root         (0)     3162 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/check_commodity_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3464 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/check_drained.py
--rw-rw-rw-   0 root         (0) root         (0)     5238 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/check_drained_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/coherent_cost.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/coherent_cost_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2590 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/commodity_attr.py
--rw-rw-rw-   0 root         (0) root         (0)     1454 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/commodity_attr_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5545 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/currency_accounts.py
--rw-rw-rw-   0 root         (0) root         (0)     8037 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/currency_accounts_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3347 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/divert_expenses.py
--rw-rw-rw-   0 root         (0) root         (0)     3598 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/divert_expenses_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/exclude_tag.py
--rw-rw-rw-   0 root         (0) root         (0)     1123 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/exclude_tag_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/fill_account.py
--rw-rw-rw-   0 root         (0) root         (0)     2566 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/fill_account_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4367 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/fix_payees.py
--rw-rw-rw-   0 root         (0) root         (0)     2473 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/fix_payees_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5010 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/forecast.py
--rw-rw-rw-   0 root         (0) root         (0)     2047 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/forecast_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5348 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/implicit_prices.py
--rw-rw-rw-   0 root         (0) root         (0)    11750 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/implicit_prices_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7952 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/ira_contribs.py
--rw-rw-rw-   0 root         (0) root         (0)     5095 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/ira_contribs_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/leafonly.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/leafonly_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2349 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/mark_unverified.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/mark_unverified_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2907 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/merge_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     3994 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/merge_meta_test.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/noduplicates.py
--rw-rw-rw-   0 root         (0) root         (0)     4392 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/noduplicates_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/nounused.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/nounused_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4359 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/onecommodity.py
--rw-rw-rw-   0 root         (0) root         (0)     3041 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/onecommodity_test.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/pedantic.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/pedantic_test.py
--rw-rw-rw-   0 root         (0) root         (0)     6038 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/sellgains.py
--rw-rw-rw-   0 root         (0) root         (0)     2969 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/sellgains_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4207 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/settle.py
--rw-rw-rw-   0 root         (0) root         (0)     3990 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/settle_inv.py
--rwxrwxrwx   0 root         (0) root         (0)    12320 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/split_expenses.py
--rw-rw-rw-   0 root         (0) root         (0)     5468 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/split_expenses_test.py
--rwxrwxrwx   0 root         (0) root         (0)     3648 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/tag_pending.py
--rw-rw-rw-   0 root         (0) root         (0)     1546 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/tag_pending_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2324 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/unique_prices.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/unique_prices_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7895 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/unrealized.py
--rw-rw-rw-   0 root         (0) root         (0)    11592 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/plugins/unrealized_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.551375 g8fyi-beancount-1.0.8/beancount/prices/
--rw-rw-rw-   0 root         (0) root         (0)     5458 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25251 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/price.py
--rw-rw-rw-   0 root         (0) root         (0)    21302 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/price_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.556376 g8fyi-beancount-1.0.8/beancount/prices/sources/
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/coinbase.py
--rw-rw-rw-   0 root         (0) root         (0)     2014 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/coinbase_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/iex.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/iex_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4186 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/oanda.py
--rw-rw-rw-   0 root         (0) root         (0)     7218 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/oanda_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4895 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/quandl.py
--rw-rw-rw-   0 root         (0) root         (0)     7426 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/quandl_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4374 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/tsp.py
--rw-rw-rw-   0 root         (0) root         (0)     6496 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/tsp_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5073 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/yahoo.py
--rw-rw-rw-   0 root         (0) root         (0)     8321 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/prices/sources/yahoo_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.558376 g8fyi-beancount-1.0.8/beancount/projects/
--rw-rw-rw-   0 root         (0) root         (0)      451 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/projects/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    12812 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/projects/export.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/projects/export_test.py
--rwxrwxrwx   0 root         (0) root         (0)    10368 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/projects/will.py
--rw-rw-rw-   0 root         (0) root         (0)     5046 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/projects/will_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.565376 g8fyi-beancount-1.0.8/beancount/query/
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8368 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/numberify.py
--rw-rw-rw-   0 root         (0) root         (0)     5606 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/numberify_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2112 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query.py
--rw-rw-rw-   0 root         (0) root         (0)    37915 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_compile.py
--rw-rw-rw-   0 root         (0) root         (0)    30550 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_compile_test.py
--rw-rw-rw-   0 root         (0) root         (0)    55470 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_env.py
--rw-rw-rw-   0 root         (0) root         (0)    11466 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_env_test.py
--rw-rw-rw-   0 root         (0) root         (0)    15542 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_execute.py
--rw-rw-rw-   0 root         (0) root         (0)    31217 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_execute_test.py
--rw-rw-rw-   0 root         (0) root         (0)    21152 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    24926 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_parser_test.py
--rw-rw-rw-   0 root         (0) root         (0)    21907 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_render.py
--rw-rw-rw-   0 root         (0) root         (0)     9163 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_render_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/query_test.py
--rw-rw-rw-   0 root         (0) root         (0)    29781 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     7042 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/query/shell_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.578377 g8fyi-beancount-1.0.8/beancount/reports/
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5474 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/balance_reports.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/balance_reports_test.py
--rw-rw-rw-   0 root         (0) root         (0)    10237 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6317 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/base_test.py
--rw-rw-rw-   0 root         (0) root         (0)    13089 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/convert_reports.py
--rw-rw-rw-   0 root         (0) root         (0)    11473 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/convert_reports_test.py
--rw-rw-rw-   0 root         (0) root         (0)    20546 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/export_reports.py
--rw-rw-rw-   0 root         (0) root         (0)    12298 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/export_reports_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/gviz.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/gviz_test.py
--rw-rw-rw-   0 root         (0) root         (0)    12774 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/holdings_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     3463 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/holdings_reports_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3999 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/html_formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     1740 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/html_formatter_test.py
--rw-rw-rw-   0 root         (0) root         (0)    11407 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/journal_html.py
--rw-rw-rw-   0 root         (0) root         (0)     4375 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/journal_html_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5757 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/journal_reports.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/journal_reports_test.py
--rw-rw-rw-   0 root         (0) root         (0)    13932 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/journal_text.py
--rw-rw-rw-   0 root         (0) root         (0)     6284 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/journal_text_test.py
--rw-rw-rw-   0 root         (0) root         (0)    10690 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/misc_reports.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/misc_reports_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7507 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/price_reports.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/price_reports_test.py
--rwxrwxrwx   0 root         (0) root         (0)     9944 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/report.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/report_test.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/template.html
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/tree_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2927 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/tree_table_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4406 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/tutorial.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/reports/tutorial_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.585378 g8fyi-beancount-1.0.8/beancount/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11513 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/bake.py
--rw-rw-rw-   0 root         (0) root         (0)     9861 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/bake_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2155 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/check.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/check_examples_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/check_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5572 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/deps.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/deps_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2417 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/directories.py
--rw-rw-rw-   0 root         (0) root         (0)     2000 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/directories_test.py
--rwxrwxrwx   0 root         (0) root         (0)    16108 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/doctor.py
--rw-rw-rw-   0 root         (0) root         (0)     9936 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/doctor_test.py
--rwxrwxrwx   0 root         (0) root         (0)    69206 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/example.py
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/example_test.py
--rwxrwxrwx   0 root         (0) root         (0)     7699 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/format.py
--rw-rw-rw-   0 root         (0) root         (0)     8080 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/format_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5073 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/setup_test.py
--rw-rw-rw-   0 root         (0) root         (0)    10682 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/sql.py
--rw-rw-rw-   0 root         (0) root         (0)     2007 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/scripts/sql_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.587378 g8fyi-beancount-1.0.8/beancount/tools/
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/tools/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17930 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/tools/sheets_upload.py
--rw-rw-rw-   0 root         (0) root         (0)     2775 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/tools/sheets_upload_test.py
--rwxrwxrwx   0 root         (0) root         (0)    14623 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/tools/treeify.py
--rw-rw-rw-   0 root         (0) root         (0)    23893 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/tools/treeify_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.602379 g8fyi-beancount-1.0.8/beancount/utils/
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1517 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/bisect_key.py
--rw-rw-rw-   0 root         (0) root         (0)     1468 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/bisect_key_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5709 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/csv_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7340 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/csv_utils_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/date_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/date_utils_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/defdict.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/defdict_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1994 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/encryption.py
--rw-rw-rw-   0 root         (0) root         (0)     6679 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/encryption_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2176 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/file_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3225 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/file_type_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3682 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/file_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3089 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/file_utils_test.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/import_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/import_utils_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/invariants.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/invariants_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1896 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/memo.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/memo_test.py
--rw-rw-rw-   0 root         (0) root         (0)    18462 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/misc_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    10000 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/misc_utils_test.py
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/net_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/net_utils_test.py
--rw-rw-rw-   0 root         (0) root         (0)     7053 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/pager.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/pager_test.py
--rw-rw-rw-   0 root         (0) root         (0)    20069 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/regexp_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/regexp_utils_test.py
--rw-rw-rw-   0 root         (0) root         (0)     6098 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/scrape.py
--rw-rw-rw-   0 root         (0) root         (0)     4782 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/scrape_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3151 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/snoop.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/snoop_test.py
--rw-rw-rw-   0 root         (0) root         (0)     9907 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/table.py
--rw-rw-rw-   0 root         (0) root         (0)     4860 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/table_test.py
--rw-rw-rw-   0 root         (0) root         (0)    14761 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5585 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/test_utils_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1783 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/text_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/utils/text_utils_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.605379 g8fyi-beancount-1.0.8/beancount/web/
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2526 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/bottle_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/bottle_utils_test.py
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.606379 g8fyi-beancount-1.0.8/beancount/web/third_party/
--rw-rw-rw-   0 root         (0) root         (0)    16877 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/third_party/sorttable.js
--rw-rw-rw-   0 root         (0) root         (0)    10802 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6674 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/views_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5034 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/web.css
--rw-rw-rw-   0 root         (0) root         (0)     1140 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/web.html
--rw-rw-rw-   0 root         (0) root         (0)    46156 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/web.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/beancount/web/web_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:31:54.608379 g8fyi-beancount-1.0.8/g8fyi_beancount.egg-info/
--rw-r--r--   0 root         (0) root         (0)      963 2023-03-29 14:31:54.000000 g8fyi-beancount-1.0.8/g8fyi_beancount.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11068 2023-03-29 14:31:54.000000 g8fyi-beancount-1.0.8/g8fyi_beancount.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 14:31:54.000000 g8fyi-beancount-1.0.8/g8fyi_beancount.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      697 2023-03-29 14:31:54.000000 g8fyi-beancount-1.0.8/g8fyi_beancount.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      145 2023-03-29 14:31:54.000000 g8fyi-beancount-1.0.8/g8fyi_beancount.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-29 14:31:54.000000 g8fyi-beancount-1.0.8/g8fyi_beancount.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-29 14:31:54.609380 g8fyi-beancount-1.0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     8346 2023-03-29 14:31:40.000000 g8fyi-beancount-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.709806 g8fyi-beancount-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    18343 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-30 17:11:16.709806 g8fyi-beancount-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2871 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.600798 g8fyi-beancount-1.0.9/beancount/
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.611798 g8fyi-beancount-1.0.9/beancount/core/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7273 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/account_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6876 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/account_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5214 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/account_types_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7678 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/amount.py
+-rw-rw-rw-   0 root         (0) root         (0)     5904 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/amount_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7364 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/compare.py
+-rw-rw-rw-   0 root         (0) root         (0)     6172 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/compare_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     9103 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)    12411 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/convert_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    28179 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/data.py
+-rw-rw-rw-   0 root         (0) root         (0)    14641 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/data_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    15077 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/display_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     8179 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/display_context_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2101 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/distribution_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/flags_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    11128 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/getters.py
+-rw-rw-rw-   0 root         (0) root         (0)     8910 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/getters_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    13680 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/interpolate.py
+-rw-rw-rw-   0 root         (0) root         (0)    22402 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/interpolate_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    17862 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)    18983 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/inventory_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/number.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/number_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    13305 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/position.py
+-rw-rw-rw-   0 root         (0) root         (0)    13610 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/position_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    14486 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/prices.py
+-rw-rw-rw-   0 root         (0) root         (0)    11757 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/prices_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    26763 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/realization.py
+-rw-rw-rw-   0 root         (0) root         (0)    29660 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/core/realization_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.618799 g8fyi-beancount-1.0.9/beancount/ingest/
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2737 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/cache_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     9630 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    14690 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/extract_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    12169 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/file.py
+-rw-rw-rw-   0 root         (0) root         (0)    17337 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/file_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3614 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/identify.py
+-rw-rw-rw-   0 root         (0) root         (0)     5494 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/identify_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)      741 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importer_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.621799 g8fyi-beancount-1.0.9/beancount/ingest/importers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2798 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/config_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    15322 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    14590 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/csv_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/fileonly.py
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/fileonly_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.623799 g8fyi-beancount-1.0.9/beancount/ingest/importers/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/mixins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/mixins/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/mixins/filing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/mixins/identifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    10681 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/ofx.py
+-rw-rw-rw-   0 root         (0) root         (0)    18051 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/importers/ofx_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     9245 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)     5957 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/regression_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)     7351 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/regression_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    17376 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/scripts_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4677 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/scripts_utils_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5550 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/similar.py
+-rw-rw-rw-   0 root         (0) root         (0)     5795 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ingest/similar_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    28931 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)    25352 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/loader_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.630800 g8fyi-beancount-1.0.9/beancount/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7644 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/balance.py
+-rw-rw-rw-   0 root         (0) root         (0)    13449 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/balance_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2611 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/basicops.py
+-rw-rw-rw-   0 root         (0) root         (0)     5009 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/basicops_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4623 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/compress.py
+-rw-rw-rw-   0 root         (0) root         (0)     3870 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/compress_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6194 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/documents.py
+-rw-rw-rw-   0 root         (0) root         (0)     9169 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/documents_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4041 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/find_prices.py
+-rw-rw-rw-   0 root         (0) root         (0)     4345 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/find_prices_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    20860 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/holdings.py
+-rw-rw-rw-   0 root         (0) root         (0)    25309 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/holdings_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/lifetimes.py
+-rw-rw-rw-   0 root         (0) root         (0)    16849 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/lifetimes_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7655 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/pad.py
+-rw-rw-rw-   0 root         (0) root         (0)    21566 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/pad_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    28484 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/summarize.py
+-rw-rw-rw-   0 root         (0) root         (0)    51297 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/summarize_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    15183 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/validation.py
+-rw-rw-rw-   0 root         (0) root         (0)    15717 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/ops/validation_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.642801 g8fyi-beancount-1.0.9/beancount/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8598 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/booking.py
+-rw-rw-rw-   0 root         (0) root         (0)    41024 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/booking_full.py
+-rw-rw-rw-   0 root         (0) root         (0)   114109 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/booking_full_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/booking_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/booking_method_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6612 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/booking_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     9952 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/cmptest.py
+-rw-rw-rw-   0 root         (0) root         (0)     8232 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/cmptest_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6989 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4660 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/context_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/decimal.c
+-rw-rw-rw-   0 root         (0) root         (0)      933 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/decimal.h
+-rw-rw-rw-   0 root         (0) root         (0)   102362 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/grammar.c
+-rw-rw-rw-   0 root         (0) root         (0)     7232 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/grammar.h
+-rw-rw-rw-   0 root         (0) root         (0)    40241 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/grammar.py
+-rw-rw-rw-   0 root         (0) root         (0)    92323 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/grammar_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/hashsrc.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/hashsrc_test.py
+-rw-rw-rw-   0 root         (0) root         (0)   102749 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/lexer.c
+-rw-rw-rw-   0 root         (0) root         (0)    14169 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/lexer.h
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/lexer.py
+-rw-rw-rw-   0 root         (0) root         (0)    22123 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/lexer_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3565 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/macros.h
+-rw-rw-rw-   0 root         (0) root         (0)    22979 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/options_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    12956 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/parser.c
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/parser.h
+-rwxrwxrwx   0 root         (0) root         (0)    12089 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14718 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/parser_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    19852 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/printer.py
+-rw-rw-rw-   0 root         (0) root         (0)    19605 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/printer_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/tokens.c
+-rw-rw-rw-   0 root         (0) root         (0)     3759 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/tokens.h
+-rw-rw-rw-   0 root         (0) root         (0)     2879 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/tokens_test.c
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/parser/version_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.661802 g8fyi-beancount-1.0.9/beancount/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14406 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/amortize.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/auto.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/auto_accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/auto_accounts_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/auto_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    18479 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/book_conversions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10940 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/book_conversions_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/check_average_cost.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/check_average_cost_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2908 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/check_closing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/check_closing_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/check_commodity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3162 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/check_commodity_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3464 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/check_drained.py
+-rw-rw-rw-   0 root         (0) root         (0)     5238 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/check_drained_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/coherent_cost.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/coherent_cost_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/commodity_attr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/commodity_attr_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5545 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/currency_accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8037 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/currency_accounts_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3347 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/divert_expenses.py
+-rw-rw-rw-   0 root         (0) root         (0)     3598 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/divert_expenses_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/exclude_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/exclude_tag_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/fill_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     2566 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/fill_account_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4367 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/fix_payees.py
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/fix_payees_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5010 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/forecast.py
+-rw-rw-rw-   0 root         (0) root         (0)     2047 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/forecast_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5348 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/implicit_prices.py
+-rw-rw-rw-   0 root         (0) root         (0)    11750 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/implicit_prices_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7952 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/ira_contribs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5095 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/ira_contribs_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/leafonly.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/leafonly_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2349 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/mark_unverified.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/mark_unverified_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2907 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/merge_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     3994 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/merge_meta_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/noduplicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4392 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/noduplicates_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/nounused.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/nounused_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4359 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/onecommodity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3041 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/onecommodity_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/pedantic.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/pedantic_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6038 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/sellgains.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/sellgains_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/settle.py
+-rw-rw-rw-   0 root         (0) root         (0)     3990 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/settle_inv.py
+-rwxrwxrwx   0 root         (0) root         (0)    12320 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/split_expenses.py
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/split_expenses_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     3648 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/tag_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)     1546 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/tag_pending_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2324 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/unique_prices.py
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/unique_prices_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7895 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/unrealized.py
+-rw-rw-rw-   0 root         (0) root         (0)    11592 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/plugins/unrealized_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.663802 g8fyi-beancount-1.0.9/beancount/prices/
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25251 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/price.py
+-rw-rw-rw-   0 root         (0) root         (0)    21302 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/price_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.667803 g8fyi-beancount-1.0.9/beancount/prices/sources/
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/coinbase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2014 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/coinbase_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/iex.py
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/iex_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4186 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/oanda.py
+-rw-rw-rw-   0 root         (0) root         (0)     7218 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/oanda_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4895 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/quandl.py
+-rw-rw-rw-   0 root         (0) root         (0)     7426 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/quandl_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4374 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/tsp.py
+-rw-rw-rw-   0 root         (0) root         (0)     6496 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/tsp_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5073 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/yahoo.py
+-rw-rw-rw-   0 root         (0) root         (0)     8321 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/prices/sources/yahoo_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.668803 g8fyi-beancount-1.0.9/beancount/projects/
+-rw-rw-rw-   0 root         (0) root         (0)      451 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/projects/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    12812 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/projects/export.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/projects/export_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    10368 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/projects/will.py
+-rw-rw-rw-   0 root         (0) root         (0)     5046 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/projects/will_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.674803 g8fyi-beancount-1.0.9/beancount/query/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8368 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/numberify.py
+-rw-rw-rw-   0 root         (0) root         (0)     5606 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/numberify_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2112 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query.py
+-rw-rw-rw-   0 root         (0) root         (0)    37915 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_compile.py
+-rw-rw-rw-   0 root         (0) root         (0)    30550 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_compile_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    55470 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_env.py
+-rw-rw-rw-   0 root         (0) root         (0)    11466 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_env_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    15542 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)    31217 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_execute_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    21152 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    24926 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_parser_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    21907 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_render.py
+-rw-rw-rw-   0 root         (0) root         (0)     9163 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_render_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/query_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    29781 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     7042 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/query/shell_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.684804 g8fyi-beancount-1.0.9/beancount/reports/
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5474 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/balance_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/balance_reports_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    10237 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6317 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/base_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    13089 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/convert_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/convert_reports_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    20546 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/export_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/export_reports_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/gviz.py
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/gviz_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    12774 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/holdings_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     3463 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/holdings_reports_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3999 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/html_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1740 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/html_formatter_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    11407 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/journal_html.py
+-rw-rw-rw-   0 root         (0) root         (0)     4375 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/journal_html_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5757 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/journal_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/journal_reports_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    13932 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/journal_text.py
+-rw-rw-rw-   0 root         (0) root         (0)     6284 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/journal_text_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    10690 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/misc_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/misc_reports_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7507 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/price_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/price_reports_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     9944 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/report_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/template.html
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/tree_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2927 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/tree_table_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4406 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/tutorial.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/reports/tutorial_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.690805 g8fyi-beancount-1.0.9/beancount/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11513 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/bake.py
+-rw-rw-rw-   0 root         (0) root         (0)     9861 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/bake_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2155 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/check.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/check_examples_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/check_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5572 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/deps.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/deps_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2417 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/directories.py
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/directories_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    16108 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/doctor.py
+-rw-rw-rw-   0 root         (0) root         (0)     9936 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/doctor_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    69206 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/example.py
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/example_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     7699 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/format.py
+-rw-rw-rw-   0 root         (0) root         (0)     8080 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/format_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5073 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/setup_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    10682 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     2007 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/scripts/sql_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.691805 g8fyi-beancount-1.0.9/beancount/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/tools/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    17930 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/tools/sheets_upload.py
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/tools/sheets_upload_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    14623 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/tools/treeify.py
+-rw-rw-rw-   0 root         (0) root         (0)    23893 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/tools/treeify_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.703806 g8fyi-beancount-1.0.9/beancount/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1517 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/bisect_key.py
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/bisect_key_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5709 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/csv_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     7340 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/csv_utils_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/date_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/date_utils_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/defdict.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/defdict_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1994 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/encryption.py
+-rw-rw-rw-   0 root         (0) root         (0)     6679 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/encryption_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/file_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3225 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/file_type_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3682 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/file_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/file_utils_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/import_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/import_utils_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/invariants.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/invariants_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1896 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/memo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/memo_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    18462 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/misc_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    10000 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/misc_utils_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/net_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/net_utils_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     7053 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/pager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/pager_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    20069 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/regexp_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/regexp_utils_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6098 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/scrape.py
+-rw-rw-rw-   0 root         (0) root         (0)     4782 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/scrape_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/snoop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/snoop_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     9907 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     4860 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/table_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    14761 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5585 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/test_utils_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1783 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/text_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/utils/text_utils_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.706806 g8fyi-beancount-1.0.9/beancount/web/
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/bottle_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/bottle_utils_test.py
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.707806 g8fyi-beancount-1.0.9/beancount/web/third_party/
+-rw-rw-rw-   0 root         (0) root         (0)    16877 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/third_party/sorttable.js
+-rw-rw-rw-   0 root         (0) root         (0)    10802 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6674 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/views_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5034 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/web.css
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/web.html
+-rw-rw-rw-   0 root         (0) root         (0)    46156 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/web.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/beancount/web/web_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 17:11:16.708806 g8fyi-beancount-1.0.9/g8fyi_beancount.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-30 17:11:16.000000 g8fyi-beancount-1.0.9/g8fyi_beancount.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11068 2023-04-30 17:11:16.000000 g8fyi-beancount-1.0.9/g8fyi_beancount.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 17:11:16.000000 g8fyi-beancount-1.0.9/g8fyi_beancount.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      697 2023-04-30 17:11:16.000000 g8fyi-beancount-1.0.9/g8fyi_beancount.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-30 17:11:16.000000 g8fyi-beancount-1.0.9/g8fyi_beancount.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-30 17:11:16.000000 g8fyi-beancount-1.0.9/g8fyi_beancount.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-30 17:11:16.709806 g8fyi-beancount-1.0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     8384 2023-04-30 17:11:04.000000 g8fyi-beancount-1.0.9/setup.py
```

### Comparing `g8fyi-beancount-1.0.8/COPYING` & `g8fyi-beancount-1.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/PKG-INFO` & `g8fyi-beancount-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g8fyi-beancount
-Version: 1.0.8
+Version: 1.0.9
 Summary: Command-line Double-Entry Accounting
 Home-page: http://furius.ca/beancount
 Download-URL: https://github.com/beancount/beancount
 Author: Martin Blais
 Author-email: blais@furius.ca
 License: GNU GPLv2 only
 Requires-Python: >=3.6
```

### Comparing `g8fyi-beancount-1.0.8/README.rst` & `g8fyi-beancount-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/__init__.py` & `g8fyi-beancount-1.0.9/beancount/__init__.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/account.py` & `g8fyi-beancount-1.0.9/beancount/core/account.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/account_test.py` & `g8fyi-beancount-1.0.9/beancount/core/account_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/account_types.py` & `g8fyi-beancount-1.0.9/beancount/core/account_types.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/account_types_test.py` & `g8fyi-beancount-1.0.9/beancount/core/account_types_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/amount.py` & `g8fyi-beancount-1.0.9/beancount/core/amount.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/amount_test.py` & `g8fyi-beancount-1.0.9/beancount/core/amount_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/compare.py` & `g8fyi-beancount-1.0.9/beancount/core/compare.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/compare_test.py` & `g8fyi-beancount-1.0.9/beancount/core/compare_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/convert.py` & `g8fyi-beancount-1.0.9/beancount/core/convert.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/convert_test.py` & `g8fyi-beancount-1.0.9/beancount/core/convert_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/data.py` & `g8fyi-beancount-1.0.9/beancount/core/data.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/data_test.py` & `g8fyi-beancount-1.0.9/beancount/core/data_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/display_context.py` & `g8fyi-beancount-1.0.9/beancount/core/display_context.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/display_context_test.py` & `g8fyi-beancount-1.0.9/beancount/core/display_context_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/distribution.py` & `g8fyi-beancount-1.0.9/beancount/core/distribution.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/distribution_test.py` & `g8fyi-beancount-1.0.9/beancount/core/distribution_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/flags.py` & `g8fyi-beancount-1.0.9/beancount/core/flags.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/flags_test.py` & `g8fyi-beancount-1.0.9/beancount/core/flags_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/getters.py` & `g8fyi-beancount-1.0.9/beancount/core/getters.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/getters_test.py` & `g8fyi-beancount-1.0.9/beancount/core/getters_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/interpolate.py` & `g8fyi-beancount-1.0.9/beancount/core/interpolate.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/interpolate_test.py` & `g8fyi-beancount-1.0.9/beancount/core/interpolate_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/inventory.py` & `g8fyi-beancount-1.0.9/beancount/core/inventory.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/inventory_test.py` & `g8fyi-beancount-1.0.9/beancount/core/inventory_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/number.py` & `g8fyi-beancount-1.0.9/beancount/core/number.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/number_test.py` & `g8fyi-beancount-1.0.9/beancount/core/number_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/position.py` & `g8fyi-beancount-1.0.9/beancount/core/position.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/position_test.py` & `g8fyi-beancount-1.0.9/beancount/core/position_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/prices.py` & `g8fyi-beancount-1.0.9/beancount/core/prices.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/prices_test.py` & `g8fyi-beancount-1.0.9/beancount/core/prices_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/realization.py` & `g8fyi-beancount-1.0.9/beancount/core/realization.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/core/realization_test.py` & `g8fyi-beancount-1.0.9/beancount/core/realization_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/__init__.py` & `g8fyi-beancount-1.0.9/beancount/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/cache.py` & `g8fyi-beancount-1.0.9/beancount/ingest/cache.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/cache_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/cache_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/extract.py` & `g8fyi-beancount-1.0.9/beancount/ingest/extract.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/extract_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/extract_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/file.py` & `g8fyi-beancount-1.0.9/beancount/ingest/file.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/file_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/file_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/identify.py` & `g8fyi-beancount-1.0.9/beancount/ingest/identify.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/identify_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/identify_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importer.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importer.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importer_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importer_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importers/config.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importers/config.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importers/config_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importers/config_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importers/csv.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importers/csv.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importers/csv_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importers/csv_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importers/fileonly_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importers/fileonly_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importers/mixins/config.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importers/mixins/config.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importers/mixins/filing.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importers/mixins/filing.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importers/mixins/identifier.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importers/mixins/identifier.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importers/ofx.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importers/ofx.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/importers/ofx_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/importers/ofx_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/regression.py` & `g8fyi-beancount-1.0.9/beancount/ingest/regression.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/regression_pytest.py` & `g8fyi-beancount-1.0.9/beancount/ingest/regression_pytest.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/regression_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/regression_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/scripts_utils.py` & `g8fyi-beancount-1.0.9/beancount/ingest/scripts_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/scripts_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/scripts_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/similar.py` & `g8fyi-beancount-1.0.9/beancount/ingest/similar.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ingest/similar_test.py` & `g8fyi-beancount-1.0.9/beancount/ingest/similar_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/loader.py` & `g8fyi-beancount-1.0.9/beancount/loader.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/loader_test.py` & `g8fyi-beancount-1.0.9/beancount/loader_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/balance.py` & `g8fyi-beancount-1.0.9/beancount/ops/balance.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/balance_test.py` & `g8fyi-beancount-1.0.9/beancount/ops/balance_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/basicops.py` & `g8fyi-beancount-1.0.9/beancount/ops/basicops.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/basicops_test.py` & `g8fyi-beancount-1.0.9/beancount/ops/basicops_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/compress.py` & `g8fyi-beancount-1.0.9/beancount/ops/compress.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/compress_test.py` & `g8fyi-beancount-1.0.9/beancount/ops/compress_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/documents.py` & `g8fyi-beancount-1.0.9/beancount/ops/documents.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/documents_test.py` & `g8fyi-beancount-1.0.9/beancount/ops/documents_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/find_prices.py` & `g8fyi-beancount-1.0.9/beancount/ops/find_prices.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/find_prices_test.py` & `g8fyi-beancount-1.0.9/beancount/ops/find_prices_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/holdings.py` & `g8fyi-beancount-1.0.9/beancount/ops/holdings.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/holdings_test.py` & `g8fyi-beancount-1.0.9/beancount/ops/holdings_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/lifetimes.py` & `g8fyi-beancount-1.0.9/beancount/ops/lifetimes.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/lifetimes_test.py` & `g8fyi-beancount-1.0.9/beancount/ops/lifetimes_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/pad.py` & `g8fyi-beancount-1.0.9/beancount/ops/pad.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/pad_test.py` & `g8fyi-beancount-1.0.9/beancount/ops/pad_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/summarize.py` & `g8fyi-beancount-1.0.9/beancount/ops/summarize.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/summarize_test.py` & `g8fyi-beancount-1.0.9/beancount/ops/summarize_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/validation.py` & `g8fyi-beancount-1.0.9/beancount/ops/validation.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/ops/validation_test.py` & `g8fyi-beancount-1.0.9/beancount/ops/validation_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/booking.py` & `g8fyi-beancount-1.0.9/beancount/parser/booking.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/booking_full.py` & `g8fyi-beancount-1.0.9/beancount/parser/booking_full.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/booking_full_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/booking_full_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/booking_method.py` & `g8fyi-beancount-1.0.9/beancount/parser/booking_method.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/booking_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/booking_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/cmptest.py` & `g8fyi-beancount-1.0.9/beancount/parser/cmptest.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/cmptest_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/cmptest_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/context.py` & `g8fyi-beancount-1.0.9/beancount/parser/context.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/context_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/context_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/decimal.h` & `g8fyi-beancount-1.0.9/beancount/parser/decimal.h`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/grammar.c` & `g8fyi-beancount-1.0.9/beancount/parser/grammar.c`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/grammar.h` & `g8fyi-beancount-1.0.9/beancount/parser/grammar.h`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/grammar.py` & `g8fyi-beancount-1.0.9/beancount/parser/grammar.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/grammar_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/grammar_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/hashsrc.py` & `g8fyi-beancount-1.0.9/beancount/parser/hashsrc.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/hashsrc_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/hashsrc_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/lexer.c` & `g8fyi-beancount-1.0.9/beancount/parser/lexer.c`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/lexer.h` & `g8fyi-beancount-1.0.9/beancount/parser/lexer.h`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/lexer.py` & `g8fyi-beancount-1.0.9/beancount/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/lexer_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/lexer_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/macros.h` & `g8fyi-beancount-1.0.9/beancount/parser/macros.h`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/options.py` & `g8fyi-beancount-1.0.9/beancount/parser/options.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/options_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/options_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/parser.c` & `g8fyi-beancount-1.0.9/beancount/parser/parser.c`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/parser.py` & `g8fyi-beancount-1.0.9/beancount/parser/parser.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/parser_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/parser_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/printer.py` & `g8fyi-beancount-1.0.9/beancount/parser/printer.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/printer_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/printer_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/tokens.c` & `g8fyi-beancount-1.0.9/beancount/parser/tokens.c`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/tokens.h` & `g8fyi-beancount-1.0.9/beancount/parser/tokens.h`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/tokens_test.c` & `g8fyi-beancount-1.0.9/beancount/parser/tokens_test.c`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/version.py` & `g8fyi-beancount-1.0.9/beancount/parser/version.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/parser/version_test.py` & `g8fyi-beancount-1.0.9/beancount/parser/version_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/amortize.py` & `g8fyi-beancount-1.0.9/beancount/plugins/amortize.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/auto.py` & `g8fyi-beancount-1.0.9/beancount/plugins/auto.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/auto_accounts.py` & `g8fyi-beancount-1.0.9/beancount/plugins/auto_accounts.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/auto_accounts_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/auto_accounts_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/book_conversions.py` & `g8fyi-beancount-1.0.9/beancount/plugins/book_conversions.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/book_conversions_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/book_conversions_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/check_average_cost.py` & `g8fyi-beancount-1.0.9/beancount/plugins/check_average_cost.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/check_average_cost_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/check_average_cost_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/check_closing.py` & `g8fyi-beancount-1.0.9/beancount/plugins/check_closing.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/check_closing_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/check_closing_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/check_commodity.py` & `g8fyi-beancount-1.0.9/beancount/plugins/check_commodity.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/check_commodity_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/check_commodity_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/check_drained.py` & `g8fyi-beancount-1.0.9/beancount/plugins/check_drained.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/check_drained_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/check_drained_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/coherent_cost.py` & `g8fyi-beancount-1.0.9/beancount/plugins/coherent_cost.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/coherent_cost_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/coherent_cost_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/commodity_attr.py` & `g8fyi-beancount-1.0.9/beancount/plugins/commodity_attr.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/commodity_attr_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/commodity_attr_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/currency_accounts.py` & `g8fyi-beancount-1.0.9/beancount/plugins/currency_accounts.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/currency_accounts_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/currency_accounts_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/divert_expenses.py` & `g8fyi-beancount-1.0.9/beancount/plugins/divert_expenses.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/divert_expenses_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/divert_expenses_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/exclude_tag.py` & `g8fyi-beancount-1.0.9/beancount/plugins/exclude_tag.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/exclude_tag_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/exclude_tag_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/fill_account.py` & `g8fyi-beancount-1.0.9/beancount/plugins/fill_account.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/fill_account_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/fill_account_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/fix_payees.py` & `g8fyi-beancount-1.0.9/beancount/plugins/fix_payees.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/fix_payees_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/fix_payees_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/forecast.py` & `g8fyi-beancount-1.0.9/beancount/plugins/forecast.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/forecast_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/forecast_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/implicit_prices.py` & `g8fyi-beancount-1.0.9/beancount/plugins/implicit_prices.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/implicit_prices_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/implicit_prices_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/ira_contribs.py` & `g8fyi-beancount-1.0.9/beancount/plugins/ira_contribs.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/ira_contribs_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/ira_contribs_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/leafonly.py` & `g8fyi-beancount-1.0.9/beancount/plugins/leafonly.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/leafonly_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/leafonly_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/mark_unverified.py` & `g8fyi-beancount-1.0.9/beancount/plugins/mark_unverified.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/mark_unverified_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/mark_unverified_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/merge_meta.py` & `g8fyi-beancount-1.0.9/beancount/plugins/merge_meta.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/merge_meta_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/merge_meta_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/noduplicates.py` & `g8fyi-beancount-1.0.9/beancount/plugins/noduplicates.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/noduplicates_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/noduplicates_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/nounused.py` & `g8fyi-beancount-1.0.9/beancount/plugins/nounused.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/nounused_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/nounused_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/onecommodity.py` & `g8fyi-beancount-1.0.9/beancount/plugins/onecommodity.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/onecommodity_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/onecommodity_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/pedantic.py` & `g8fyi-beancount-1.0.9/beancount/plugins/pedantic.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/pedantic_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/pedantic_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/sellgains.py` & `g8fyi-beancount-1.0.9/beancount/plugins/sellgains.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/sellgains_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/sellgains_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/settle.py` & `g8fyi-beancount-1.0.9/beancount/plugins/settle.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/settle_inv.py` & `g8fyi-beancount-1.0.9/beancount/plugins/settle_inv.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/split_expenses.py` & `g8fyi-beancount-1.0.9/beancount/plugins/split_expenses.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/split_expenses_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/split_expenses_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/tag_pending.py` & `g8fyi-beancount-1.0.9/beancount/plugins/tag_pending.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/tag_pending_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/tag_pending_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/unique_prices.py` & `g8fyi-beancount-1.0.9/beancount/plugins/unique_prices.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/unique_prices_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/unique_prices_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/unrealized.py` & `g8fyi-beancount-1.0.9/beancount/plugins/unrealized.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/plugins/unrealized_test.py` & `g8fyi-beancount-1.0.9/beancount/plugins/unrealized_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/__init__.py` & `g8fyi-beancount-1.0.9/beancount/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/price.py` & `g8fyi-beancount-1.0.9/beancount/prices/price.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/price_test.py` & `g8fyi-beancount-1.0.9/beancount/prices/price_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/source.py` & `g8fyi-beancount-1.0.9/beancount/prices/source.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/coinbase.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/coinbase.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/coinbase_test.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/coinbase_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/iex.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/iex.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/iex_test.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/iex_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/oanda.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/oanda.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/oanda_test.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/oanda_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/quandl.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/quandl.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/quandl_test.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/quandl_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/tsp.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/tsp.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/tsp_test.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/tsp_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/yahoo.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/yahoo.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/prices/sources/yahoo_test.py` & `g8fyi-beancount-1.0.9/beancount/prices/sources/yahoo_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/projects/export.py` & `g8fyi-beancount-1.0.9/beancount/projects/export.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/projects/export_test.py` & `g8fyi-beancount-1.0.9/beancount/projects/export_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/projects/will.py` & `g8fyi-beancount-1.0.9/beancount/projects/will.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/projects/will_test.py` & `g8fyi-beancount-1.0.9/beancount/projects/will_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/numberify.py` & `g8fyi-beancount-1.0.9/beancount/query/numberify.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/numberify_test.py` & `g8fyi-beancount-1.0.9/beancount/query/numberify_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query.py` & `g8fyi-beancount-1.0.9/beancount/query/query.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_compile.py` & `g8fyi-beancount-1.0.9/beancount/query/query_compile.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_compile_test.py` & `g8fyi-beancount-1.0.9/beancount/query/query_compile_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_env.py` & `g8fyi-beancount-1.0.9/beancount/query/query_env.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_env_test.py` & `g8fyi-beancount-1.0.9/beancount/query/query_env_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_execute.py` & `g8fyi-beancount-1.0.9/beancount/query/query_execute.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_execute_test.py` & `g8fyi-beancount-1.0.9/beancount/query/query_execute_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_parser.py` & `g8fyi-beancount-1.0.9/beancount/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_parser_test.py` & `g8fyi-beancount-1.0.9/beancount/query/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_render.py` & `g8fyi-beancount-1.0.9/beancount/query/query_render.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_render_test.py` & `g8fyi-beancount-1.0.9/beancount/query/query_render_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/query_test.py` & `g8fyi-beancount-1.0.9/beancount/query/query_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/shell.py` & `g8fyi-beancount-1.0.9/beancount/query/shell.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/query/shell_test.py` & `g8fyi-beancount-1.0.9/beancount/query/shell_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/balance_reports.py` & `g8fyi-beancount-1.0.9/beancount/reports/balance_reports.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/balance_reports_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/balance_reports_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/base.py` & `g8fyi-beancount-1.0.9/beancount/reports/base.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/base_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/base_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/convert_reports.py` & `g8fyi-beancount-1.0.9/beancount/reports/convert_reports.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/convert_reports_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/convert_reports_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/export_reports.py` & `g8fyi-beancount-1.0.9/beancount/reports/export_reports.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/export_reports_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/export_reports_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/gviz.py` & `g8fyi-beancount-1.0.9/beancount/reports/gviz.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/gviz_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/gviz_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/holdings_reports.py` & `g8fyi-beancount-1.0.9/beancount/reports/holdings_reports.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/holdings_reports_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/holdings_reports_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/html_formatter.py` & `g8fyi-beancount-1.0.9/beancount/reports/html_formatter.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/html_formatter_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/html_formatter_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/journal_html.py` & `g8fyi-beancount-1.0.9/beancount/reports/journal_html.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/journal_html_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/journal_html_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/journal_reports.py` & `g8fyi-beancount-1.0.9/beancount/reports/journal_reports.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/journal_reports_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/journal_reports_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/journal_text.py` & `g8fyi-beancount-1.0.9/beancount/reports/journal_text.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/journal_text_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/journal_text_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/misc_reports.py` & `g8fyi-beancount-1.0.9/beancount/reports/misc_reports.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/misc_reports_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/misc_reports_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/price_reports.py` & `g8fyi-beancount-1.0.9/beancount/reports/price_reports.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/price_reports_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/price_reports_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/report.py` & `g8fyi-beancount-1.0.9/beancount/reports/report.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/report_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/report_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/tree_table.py` & `g8fyi-beancount-1.0.9/beancount/reports/tree_table.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/tree_table_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/tree_table_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/tutorial.py` & `g8fyi-beancount-1.0.9/beancount/reports/tutorial.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/reports/tutorial_test.py` & `g8fyi-beancount-1.0.9/beancount/reports/tutorial_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/bake.py` & `g8fyi-beancount-1.0.9/beancount/scripts/bake.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/bake_test.py` & `g8fyi-beancount-1.0.9/beancount/scripts/bake_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/check.py` & `g8fyi-beancount-1.0.9/beancount/scripts/check.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/check_examples_test.py` & `g8fyi-beancount-1.0.9/beancount/scripts/check_examples_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/check_test.py` & `g8fyi-beancount-1.0.9/beancount/scripts/check_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/deps.py` & `g8fyi-beancount-1.0.9/beancount/scripts/deps.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/deps_test.py` & `g8fyi-beancount-1.0.9/beancount/scripts/deps_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/directories.py` & `g8fyi-beancount-1.0.9/beancount/scripts/directories.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/directories_test.py` & `g8fyi-beancount-1.0.9/beancount/scripts/directories_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/doctor.py` & `g8fyi-beancount-1.0.9/beancount/scripts/doctor.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/doctor_test.py` & `g8fyi-beancount-1.0.9/beancount/scripts/doctor_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/example.py` & `g8fyi-beancount-1.0.9/beancount/scripts/example.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/example_test.py` & `g8fyi-beancount-1.0.9/beancount/scripts/example_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/format.py` & `g8fyi-beancount-1.0.9/beancount/scripts/format.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/format_test.py` & `g8fyi-beancount-1.0.9/beancount/scripts/format_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/setup_test.py` & `g8fyi-beancount-1.0.9/beancount/scripts/setup_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/sql.py` & `g8fyi-beancount-1.0.9/beancount/scripts/sql.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/scripts/sql_test.py` & `g8fyi-beancount-1.0.9/beancount/scripts/sql_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/tools/__init__.py` & `g8fyi-beancount-1.0.9/beancount/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/tools/sheets_upload.py` & `g8fyi-beancount-1.0.9/beancount/tools/sheets_upload.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/tools/sheets_upload_test.py` & `g8fyi-beancount-1.0.9/beancount/tools/sheets_upload_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/tools/treeify.py` & `g8fyi-beancount-1.0.9/beancount/tools/treeify.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/tools/treeify_test.py` & `g8fyi-beancount-1.0.9/beancount/tools/treeify_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/bisect_key.py` & `g8fyi-beancount-1.0.9/beancount/utils/bisect_key.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/bisect_key_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/bisect_key_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/csv_utils.py` & `g8fyi-beancount-1.0.9/beancount/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/csv_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/csv_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/date_utils.py` & `g8fyi-beancount-1.0.9/beancount/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/date_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/date_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/defdict.py` & `g8fyi-beancount-1.0.9/beancount/utils/defdict.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/defdict_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/defdict_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/encryption.py` & `g8fyi-beancount-1.0.9/beancount/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/encryption_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/encryption_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/file_type.py` & `g8fyi-beancount-1.0.9/beancount/utils/file_type.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/file_type_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/file_type_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/file_utils.py` & `g8fyi-beancount-1.0.9/beancount/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/file_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/file_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/import_utils.py` & `g8fyi-beancount-1.0.9/beancount/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/import_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/import_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/invariants.py` & `g8fyi-beancount-1.0.9/beancount/utils/invariants.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/invariants_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/invariants_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/memo.py` & `g8fyi-beancount-1.0.9/beancount/utils/memo.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/memo_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/memo_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/misc_utils.py` & `g8fyi-beancount-1.0.9/beancount/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/misc_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/misc_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/net_utils.py` & `g8fyi-beancount-1.0.9/beancount/utils/net_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/net_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/net_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/pager.py` & `g8fyi-beancount-1.0.9/beancount/utils/pager.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/pager_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/pager_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/regexp_utils.py` & `g8fyi-beancount-1.0.9/beancount/utils/regexp_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/regexp_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/regexp_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/scrape.py` & `g8fyi-beancount-1.0.9/beancount/utils/scrape.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/scrape_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/scrape_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/snoop.py` & `g8fyi-beancount-1.0.9/beancount/utils/snoop.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/snoop_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/snoop_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/table.py` & `g8fyi-beancount-1.0.9/beancount/utils/table.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/table_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/table_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/test_utils.py` & `g8fyi-beancount-1.0.9/beancount/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/test_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/text_utils.py` & `g8fyi-beancount-1.0.9/beancount/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/utils/text_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/utils/text_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/web/bottle_utils.py` & `g8fyi-beancount-1.0.9/beancount/web/bottle_utils.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/web/bottle_utils_test.py` & `g8fyi-beancount-1.0.9/beancount/web/bottle_utils_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/web/third_party/sorttable.js` & `g8fyi-beancount-1.0.9/beancount/web/third_party/sorttable.js`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/web/views.py` & `g8fyi-beancount-1.0.9/beancount/web/views.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/web/views_test.py` & `g8fyi-beancount-1.0.9/beancount/web/views_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/web/web.css` & `g8fyi-beancount-1.0.9/beancount/web/web.css`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/web/web.html` & `g8fyi-beancount-1.0.9/beancount/web/web.html`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/web/web.py` & `g8fyi-beancount-1.0.9/beancount/web/web.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/beancount/web/web_test.py` & `g8fyi-beancount-1.0.9/beancount/web/web_test.py`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/g8fyi_beancount.egg-info/PKG-INFO` & `g8fyi-beancount-1.0.9/g8fyi_beancount.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g8fyi-beancount
-Version: 1.0.8
+Version: 1.0.9
 Summary: Command-line Double-Entry Accounting
 Home-page: http://furius.ca/beancount
 Download-URL: https://github.com/beancount/beancount
 Author: Martin Blais
 Author-email: blais@furius.ca
 License: GNU GPLv2 only
 Requires-Python: >=3.6
```

### Comparing `g8fyi-beancount-1.0.8/g8fyi_beancount.egg-info/SOURCES.txt` & `g8fyi-beancount-1.0.9/g8fyi_beancount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/g8fyi_beancount.egg-info/entry_points.txt` & `g8fyi-beancount-1.0.9/g8fyi_beancount.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `g8fyi-beancount-1.0.8/setup.py` & `g8fyi-beancount-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,17 @@
     # Spreadsheet for live intra-day monitoring.
     'google-api-python-client',
 
     # This library is needed to identify the type of a file for
     # import. It uses ctypes to wrap the libmagic library which is
     # not generally available on Windows nor is easily installed,
     # thus the conditional dependency.
-    'python-magic>=0.4.12; sys_platform != "win32"'
+    'python-magic>=0.4.12; sys_platform != "win32"',
+    
+    'beancount-periodic==0.1.2'
 ]
 
 # Create a setup.
 # Please read: http://furius.ca/beancount/doc/install about version numbers.
 setup(name="g8fyi-beancount",
       version=version,
       description="Command-line Double-Entry Accounting",
```

