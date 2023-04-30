# Comparing `tmp/mimesis-8.0.0.tar.gz` & `tmp/mimesis-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimesis-8.0.0.tar", max compression
+gzip compressed data, was "mimesis-9.0.0.tar", max compression
```

## Comparing `mimesis-8.0.0.tar` & `mimesis-9.0.0.tar`

### file list

```diff
@@ -1,286 +1,287 @@
--rw-r--r--   0        0        0     1123 2023-04-16 14:18:20.002791 mimesis-8.0.0/LICENSE
--rw-r--r--   0        0        0     6945 2023-04-16 14:18:20.002791 mimesis-8.0.0/README.rst
--rw-r--r--   0        0        0     2312 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/__init__.py
--rw-r--r--   0        0        0      552 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/__init__.py
--rw-r--r--   0        0        0      428 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/base.py
--rw-r--r--   0        0        0     3671 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/da.py
--rw-r--r--   0        0        0     1776 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/en.py
--rw-r--r--   0        0        0     1543 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/it.py
--rw-r--r--   0        0        0     1535 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/nl.py
--rw-r--r--   0        0        0     3281 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/pl.py
--rw-r--r--   0        0        0     3354 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/pt_br.py
--rw-r--r--   0        0        0     7494 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/ru.py
--rw-r--r--   0        0        0     1083 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/uk.py
--rw-r--r--   0        0        0      127 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/compat.py
--rw-r--r--   0        0        0      403 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/data/__init__.py
--rw-r--r--   0        0        0   182787 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/data/bin/sample.aac
--rw-r--r--   0        0        0   385692 2023-04-16 14:18:20.014791 mimesis-8.0.0/mimesis/data/bin/sample.docx
--rw-r--r--   0        0        0   115256 2023-04-16 14:18:20.014791 mimesis-8.0.0/mimesis/data/bin/sample.gif
--rw-r--r--   0        0        0      269 2023-04-16 14:18:20.014791 mimesis-8.0.0/mimesis/data/bin/sample.gz
--rw-r--r--   0        0        0    88187 2023-04-16 14:18:20.014791 mimesis-8.0.0/mimesis/data/bin/sample.jpg
--rw-r--r--   0        0        0   281424 2023-04-16 14:18:20.014791 mimesis-8.0.0/mimesis/data/bin/sample.mov
--rw-r--r--   0        0        0    67911 2023-04-16 14:18:20.018791 mimesis-8.0.0/mimesis/data/bin/sample.mp3
--rw-r--r--   0        0        0   304520 2023-04-16 14:18:20.018791 mimesis-8.0.0/mimesis/data/bin/sample.mp4
--rw-r--r--   0        0        0   414593 2023-04-16 14:18:20.022791 mimesis-8.0.0/mimesis/data/bin/sample.pdf
--rw-r--r--   0        0        0   221697 2023-04-16 14:18:20.022791 mimesis-8.0.0/mimesis/data/bin/sample.png
--rw-r--r--   0        0        0   223362 2023-04-16 14:18:20.022791 mimesis-8.0.0/mimesis/data/bin/sample.pptx
--rw-r--r--   0        0        0     4857 2023-04-16 14:18:20.022791 mimesis-8.0.0/mimesis/data/bin/sample.xlsx
--rw-r--r--   0        0        0      673 2023-04-16 14:18:20.022791 mimesis-8.0.0/mimesis/data/bin/sample.zip
--rw-r--r--   0        0        0    79583 2023-04-16 14:18:41.762841 mimesis-8.0.0/mimesis/data/cs/address.json
--rw-r--r--   0        0        0      515 2023-04-16 14:18:41.762841 mimesis-8.0.0/mimesis/data/cs/datetime.json
--rw-r--r--   0        0        0     1340 2023-04-16 14:18:41.762841 mimesis-8.0.0/mimesis/data/cs/finance.json
--rw-r--r--   0        0        0     1845 2023-04-16 14:18:41.762841 mimesis-8.0.0/mimesis/data/cs/food.json
--rw-r--r--   0        0        0    33117 2023-04-16 14:18:41.766841 mimesis-8.0.0/mimesis/data/cs/person.json
--rw-r--r--   0        0        0    49335 2023-04-16 14:18:41.766841 mimesis-8.0.0/mimesis/data/cs/text.json
--rw-r--r--   0        0        0    82900 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/address.json
--rw-r--r--   0        0        0      494 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/datetime.json
--rw-r--r--   0        0        0     4656 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/finance.json
--rw-r--r--   0        0        0     3873 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/food.json
--rw-r--r--   0        0        0    23273 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/person.json
--rw-r--r--   0        0        0    17323 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/text.json
--rw-r--r--   0        0        0   251577 2023-04-16 14:18:41.778841 mimesis-8.0.0/mimesis/data/de/address.json
--rw-r--r--   0        0        0      512 2023-04-16 14:18:41.778841 mimesis-8.0.0/mimesis/data/de/datetime.json
--rw-r--r--   0        0        0     3497 2023-04-16 14:18:41.782841 mimesis-8.0.0/mimesis/data/de/finance.json
--rw-r--r--   0        0        0     6237 2023-04-16 14:18:41.782841 mimesis-8.0.0/mimesis/data/de/food.json
--rw-r--r--   0        0        0    18346 2023-04-16 14:18:41.782841 mimesis-8.0.0/mimesis/data/de/person.json
--rw-r--r--   0        0        0   773143 2023-04-16 14:18:41.798841 mimesis-8.0.0/mimesis/data/de/text.json
--rw-r--r--   0        0        0    73006 2023-04-16 14:18:41.798841 mimesis-8.0.0/mimesis/data/de-at/address.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.798841 mimesis-8.0.0/mimesis/data/de-at/datetime.json
--rw-r--r--   0        0        0     4538 2023-04-16 14:18:41.798841 mimesis-8.0.0/mimesis/data/de-at/finance.json
--rw-r--r--   0        0        0     2335 2023-04-16 14:18:41.798841 mimesis-8.0.0/mimesis/data/de-at/food.json
--rw-r--r--   0        0        0    28622 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-at/person.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-at/text.json
--rw-r--r--   0        0        0    42841 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-ch/address.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-ch/datetime.json
--rw-r--r--   0        0        0     9750 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-ch/finance.json
--rw-r--r--   0        0        0      152 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-ch/food.json
--rw-r--r--   0        0        0    71143 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/de-ch/person.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/de-ch/text.json
--rw-r--r--   0        0        0    99824 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/address.json
--rw-r--r--   0        0        0      817 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/datetime.json
--rw-r--r--   0        0        0     2249 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/finance.json
--rw-r--r--   0        0        0     4461 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/food.json
--rw-r--r--   0        0        0    14494 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/person.json
--rw-r--r--   0        0        0    10297 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/text.json
--rw-r--r--   0        0        0    50488 2023-04-16 14:18:41.810841 mimesis-8.0.0/mimesis/data/en/address.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.810841 mimesis-8.0.0/mimesis/data/en/builtin.json
--rw-r--r--   0        0        0      501 2023-04-16 14:18:41.810841 mimesis-8.0.0/mimesis/data/en/datetime.json
--rw-r--r--   0        0        0    24968 2023-04-16 14:18:41.810841 mimesis-8.0.0/mimesis/data/en/finance.json
--rw-r--r--   0        0        0    14076 2023-04-16 14:18:41.810841 mimesis-8.0.0/mimesis/data/en/food.json
--rw-r--r--   0        0        0    64738 2023-04-16 14:18:41.814841 mimesis-8.0.0/mimesis/data/en/person.json
--rw-r--r--   0        0        0   343508 2023-04-16 14:18:41.822841 mimesis-8.0.0/mimesis/data/en/text.json
--rw-r--r--   0        0        0    68774 2023-04-16 14:18:41.822841 mimesis-8.0.0/mimesis/data/en-au/address.json
--rw-r--r--   0        0        0       49 2023-04-16 14:18:41.822841 mimesis-8.0.0/mimesis/data/en-au/datetime.json
--rw-r--r--   0        0        0   117507 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-au/finance.json
--rw-r--r--   0        0        0      504 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-au/food.json
--rw-r--r--   0        0        0    41658 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-au/person.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-au/text.json
--rw-r--r--   0        0        0    24229 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/address.json
--rw-r--r--   0        0        0       49 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/datetime.json
--rw-r--r--   0        0        0     3053 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/finance.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/food.json
--rw-r--r--   0        0        0    13729 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/person.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/text.json
--rw-r--r--   0        0        0    84033 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/address.json
--rw-r--r--   0        0        0       49 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/datetime.json
--rw-r--r--   0        0        0     9072 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/finance.json
--rw-r--r--   0        0        0     1316 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/food.json
--rw-r--r--   0        0        0    45054 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/person.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/text.json
--rw-r--r--   0        0        0    23805 2023-04-16 14:18:41.834841 mimesis-8.0.0/mimesis/data/es/address.json
--rw-r--r--   0        0        0      561 2023-04-16 14:18:41.834841 mimesis-8.0.0/mimesis/data/es/datetime.json
--rw-r--r--   0        0        0     2416 2023-04-16 14:18:41.834841 mimesis-8.0.0/mimesis/data/es/finance.json
--rw-r--r--   0        0        0     4757 2023-04-16 14:18:41.834841 mimesis-8.0.0/mimesis/data/es/food.json
--rw-r--r--   0        0        0    14143 2023-04-16 14:18:41.834841 mimesis-8.0.0/mimesis/data/es/person.json
--rw-r--r--   0        0        0   128149 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es/text.json
--rw-r--r--   0        0        0    11619 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/address.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/datetime.json
--rw-r--r--   0        0        0     2610 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/finance.json
--rw-r--r--   0        0        0     1081 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/food.json
--rw-r--r--   0        0        0    16998 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/person.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/text.json
--rw-r--r--   0        0        0    21806 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/et/address.json
--rw-r--r--   0        0        0      533 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/et/datetime.json
--rw-r--r--   0        0        0     6635 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/et/finance.json
--rw-r--r--   0        0        0     3683 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/et/food.json
--rw-r--r--   0        0        0    33842 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/et/person.json
--rw-r--r--   0        0        0    11545 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/et/text.json
--rw-r--r--   0        0        0    13562 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/fa/address.json
--rw-r--r--   0        0        0      665 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/fa/datetime.json
--rw-r--r--   0        0        0     2589 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/fa/finance.json
--rw-r--r--   0        0        0     6628 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/fa/food.json
--rw-r--r--   0        0        0    56905 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fa/person.json
--rw-r--r--   0        0        0    11302 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fa/text.json
--rw-r--r--   0        0        0     5488 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fi/address.json
--rw-r--r--   0        0        0      542 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fi/datetime.json
--rw-r--r--   0        0        0     7886 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fi/finance.json
--rw-r--r--   0        0        0     3674 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fi/food.json
--rw-r--r--   0        0        0    26719 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fi/person.json
--rw-r--r--   0        0        0    57968 2023-04-16 14:18:41.850841 mimesis-8.0.0/mimesis/data/fi/text.json
--rw-r--r--   0        0        0    39318 2023-04-16 14:18:41.850841 mimesis-8.0.0/mimesis/data/fr/address.json
--rw-r--r--   0        0        0      529 2023-04-16 14:18:41.850841 mimesis-8.0.0/mimesis/data/fr/datetime.json
--rw-r--r--   0        0        0     4390 2023-04-16 14:18:41.850841 mimesis-8.0.0/mimesis/data/fr/finance.json
--rw-r--r--   0        0        0     7024 2023-04-16 14:18:41.850841 mimesis-8.0.0/mimesis/data/fr/food.json
--rw-r--r--   0        0        0    46272 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/fr/person.json
--rw-r--r--   0        0        0    37433 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/fr/text.json
--rw-r--r--   0        0        0    13842 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/hu/address.json
--rw-r--r--   0        0        0      515 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/hu/datetime.json
--rw-r--r--   0        0        0      762 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/hu/finance.json
--rw-r--r--   0        0        0     4302 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/hu/food.json
--rw-r--r--   0        0        0    26944 2023-04-16 14:18:41.858841 mimesis-8.0.0/mimesis/data/hu/person.json
--rw-r--r--   0        0        0    22876 2023-04-16 14:18:41.858841 mimesis-8.0.0/mimesis/data/hu/text.json
--rw-r--r--   0        0        0      398 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/__init__.py
--rw-r--r--   0        0        0    20986 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/address.py
--rw-r--r--   0        0        0     2735 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/code.py
--rw-r--r--   0        0        0     2223 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/common.py
--rw-r--r--   0        0        0    27537 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/cryptographic.py
--rw-r--r--   0        0        0    11625 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/datetime.py
--rw-r--r--   0        0        0     7778 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/development.py
--rw-r--r--   0        0        0    67892 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/file.py
--rw-r--r--   0        0        0   264126 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/finance.py
--rw-r--r--   0        0        0     5221 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/hardware.py
--rw-r--r--   0        0        0    37473 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/internet.py
--rw-r--r--   0        0        0      320 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/path.py
--rw-r--r--   0        0        0      171 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/payment.py
--rw-r--r--   0        0        0   140341 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/person.py
--rw-r--r--   0        0        0      606 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/scientific.py
--rw-r--r--   0        0        0      364 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/text.py
--rw-r--r--   0        0        0    31498 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/transport.py
--rw-r--r--   0        0        0   121675 2023-04-16 14:18:41.862841 mimesis-8.0.0/mimesis/data/is/address.json
--rw-r--r--   0        0        0      546 2023-04-16 14:18:41.862841 mimesis-8.0.0/mimesis/data/is/datetime.json
--rw-r--r--   0        0        0     1539 2023-04-16 14:18:41.862841 mimesis-8.0.0/mimesis/data/is/finance.json
--rw-r--r--   0        0        0     1651 2023-04-16 14:18:41.862841 mimesis-8.0.0/mimesis/data/is/food.json
--rw-r--r--   0        0        0    68768 2023-04-16 14:18:41.866841 mimesis-8.0.0/mimesis/data/is/person.json
--rw-r--r--   0        0        0    51794 2023-04-16 14:18:41.866841 mimesis-8.0.0/mimesis/data/is/text.json
--rw-r--r--   0        0        0   123349 2023-04-16 14:18:41.870841 mimesis-8.0.0/mimesis/data/it/address.json
--rw-r--r--   0        0        0      142 2023-04-16 14:18:41.870841 mimesis-8.0.0/mimesis/data/it/builtin.json
--rw-r--r--   0        0        0      535 2023-04-16 14:18:41.870841 mimesis-8.0.0/mimesis/data/it/datetime.json
--rw-r--r--   0        0        0     5058 2023-04-16 14:18:41.870841 mimesis-8.0.0/mimesis/data/it/finance.json
--rw-r--r--   0        0        0     5352 2023-04-16 14:18:41.870841 mimesis-8.0.0/mimesis/data/it/food.json
--rw-r--r--   0        0        0    64650 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/it/person.json
--rw-r--r--   0        0        0    77862 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/it/text.json
--rw-r--r--   0        0        0    10631 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/ja/address.json
--rw-r--r--   0        0        0      494 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/ja/datetime.json
--rw-r--r--   0        0        0    23842 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/ja/finance.json
--rw-r--r--   0        0        0    13902 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/ja/food.json
--rw-r--r--   0        0        0    69460 2023-04-16 14:18:41.878841 mimesis-8.0.0/mimesis/data/ja/person.json
--rw-r--r--   0        0        0    56672 2023-04-16 14:18:41.878841 mimesis-8.0.0/mimesis/data/ja/text.json
--rw-r--r--   0        0        0    33301 2023-04-16 14:18:41.878841 mimesis-8.0.0/mimesis/data/kk/address.json
--rw-r--r--   0        0        0      768 2023-04-16 14:18:41.878841 mimesis-8.0.0/mimesis/data/kk/datetime.json
--rw-r--r--   0        0        0     6707 2023-04-16 14:18:41.878841 mimesis-8.0.0/mimesis/data/kk/finance.json
--rw-r--r--   0        0        0       95 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/kk/food.json
--rw-r--r--   0        0        0    28448 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/kk/person.json
--rw-r--r--   0        0        0    14350 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/kk/text.json
--rw-r--r--   0        0        0    30313 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/ko/address.json
--rw-r--r--   0        0        0      492 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/ko/datetime.json
--rw-r--r--   0        0        0    17722 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/ko/finance.json
--rw-r--r--   0        0        0    12695 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/ko/food.json
--rw-r--r--   0        0        0    39279 2023-04-16 14:18:41.886841 mimesis-8.0.0/mimesis/data/ko/person.json
--rw-r--r--   0        0        0    68560 2023-04-16 14:18:41.886841 mimesis-8.0.0/mimesis/data/ko/text.json
--rw-r--r--   0        0        0    60825 2023-04-16 14:18:41.890841 mimesis-8.0.0/mimesis/data/nl/address.json
--rw-r--r--   0        0        0      507 2023-04-16 14:18:41.890841 mimesis-8.0.0/mimesis/data/nl/datetime.json
--rw-r--r--   0        0        0     2771 2023-04-16 14:18:41.890841 mimesis-8.0.0/mimesis/data/nl/finance.json
--rw-r--r--   0        0        0     7412 2023-04-16 14:18:41.890841 mimesis-8.0.0/mimesis/data/nl/food.json
--rw-r--r--   0        0        0   109294 2023-04-16 14:18:41.894841 mimesis-8.0.0/mimesis/data/nl/person.json
--rw-r--r--   0        0        0   202851 2023-04-16 14:18:41.898841 mimesis-8.0.0/mimesis/data/nl/text.json
--rw-r--r--   0        0        0    53656 2023-04-16 14:18:41.898841 mimesis-8.0.0/mimesis/data/nl-be/address.json
--rw-r--r--   0        0        0       31 2023-04-16 14:18:41.898841 mimesis-8.0.0/mimesis/data/nl-be/datetime.json
--rw-r--r--   0        0        0     2303 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/nl-be/finance.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/nl-be/food.json
--rw-r--r--   0        0        0     1371 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/nl-be/person.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/nl-be/text.json
--rw-r--r--   0        0        0    40052 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/no/address.json
--rw-r--r--   0        0        0      500 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/no/datetime.json
--rw-r--r--   0        0        0     9731 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/no/finance.json
--rw-r--r--   0        0        0     4479 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/no/food.json
--rw-r--r--   0        0        0    43488 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/no/person.json
--rw-r--r--   0        0        0    31334 2023-04-16 14:18:41.906841 mimesis-8.0.0/mimesis/data/no/text.json
--rw-r--r--   0        0        0    80118 2023-04-16 14:18:41.906841 mimesis-8.0.0/mimesis/data/pl/address.json
--rw-r--r--   0        0        0      567 2023-04-16 14:18:41.906841 mimesis-8.0.0/mimesis/data/pl/datetime.json
--rw-r--r--   0        0        0    10830 2023-04-16 14:18:41.906841 mimesis-8.0.0/mimesis/data/pl/finance.json
--rw-r--r--   0        0        0     4693 2023-04-16 14:18:41.910841 mimesis-8.0.0/mimesis/data/pl/food.json
--rw-r--r--   0        0        0    27705 2023-04-16 14:18:41.910841 mimesis-8.0.0/mimesis/data/pl/person.json
--rw-r--r--   0        0        0    65088 2023-04-16 14:18:41.910841 mimesis-8.0.0/mimesis/data/pl/text.json
--rw-r--r--   0        0        0    19169 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/address.json
--rw-r--r--   0        0        0      563 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/datetime.json
--rw-r--r--   0        0        0     2572 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/finance.json
--rw-r--r--   0        0        0     4310 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/food.json
--rw-r--r--   0        0        0    38175 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/person.json
--rw-r--r--   0        0        0    25766 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/text.json
--rw-r--r--   0        0        0    94350 2023-04-16 14:18:41.918841 mimesis-8.0.0/mimesis/data/pt-br/address.json
--rw-r--r--   0        0        0      564 2023-04-16 14:18:41.918841 mimesis-8.0.0/mimesis/data/pt-br/datetime.json
--rw-r--r--   0        0        0    24208 2023-04-16 14:18:41.918841 mimesis-8.0.0/mimesis/data/pt-br/finance.json
--rw-r--r--   0        0        0     3162 2023-04-16 14:18:41.918841 mimesis-8.0.0/mimesis/data/pt-br/food.json
--rw-r--r--   0        0        0    63714 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/pt-br/person.json
--rw-r--r--   0        0        0        2 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/pt-br/text.json
--rw-r--r--   0        0        0   101129 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/ru/address.json
--rw-r--r--   0        0        0    10949 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/ru/builtin.json
--rw-r--r--   0        0        0      790 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/ru/datetime.json
--rw-r--r--   0        0        0    22783 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/ru/finance.json
--rw-r--r--   0        0        0    20262 2023-04-16 14:18:41.926841 mimesis-8.0.0/mimesis/data/ru/food.json
--rw-r--r--   0        0        0    86369 2023-04-16 14:18:41.926841 mimesis-8.0.0/mimesis/data/ru/person.json
--rw-r--r--   0        0        0    89215 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/ru/text.json
--rw-r--r--   0        0        0    38882 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/address.json
--rw-r--r--   0        0        0      485 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/datetime.json
--rw-r--r--   0        0        0      816 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/finance.json
--rw-r--r--   0        0        0      284 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/food.json
--rw-r--r--   0        0        0     5828 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/person.json
--rw-r--r--   0        0        0      752 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/text.json
--rw-r--r--   0        0        0    97258 2023-04-16 14:18:41.934841 mimesis-8.0.0/mimesis/data/sv/address.json
--rw-r--r--   0        0        0      508 2023-04-16 14:18:41.934841 mimesis-8.0.0/mimesis/data/sv/datetime.json
--rw-r--r--   0        0        0     5035 2023-04-16 14:18:41.934841 mimesis-8.0.0/mimesis/data/sv/finance.json
--rw-r--r--   0        0        0     6863 2023-04-16 14:18:41.934841 mimesis-8.0.0/mimesis/data/sv/food.json
--rw-r--r--   0        0        0    32781 2023-04-16 14:18:41.934841 mimesis-8.0.0/mimesis/data/sv/person.json
--rw-r--r--   0        0        0    41878 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/sv/text.json
--rw-r--r--   0        0        0    12375 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/address.json
--rw-r--r--   0        0        0      508 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/datetime.json
--rw-r--r--   0        0        0    11988 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/finance.json
--rw-r--r--   0        0        0     1819 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/food.json
--rw-r--r--   0        0        0    29265 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/person.json
--rw-r--r--   0        0        0     8857 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/text.json
--rw-r--r--   0        0        0    54571 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/address.json
--rw-r--r--   0        0        0     6247 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/builtin.json
--rw-r--r--   0        0        0      790 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/datetime.json
--rw-r--r--   0        0        0     6981 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/finance.json
--rw-r--r--   0        0        0     9121 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/food.json
--rw-r--r--   0        0        0    52753 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/person.json
--rw-r--r--   0        0        0    21072 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/text.json
--rw-r--r--   0        0        0    10240 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/zh/address.json
--rw-r--r--   0        0        0      539 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/zh/datetime.json
--rw-r--r--   0        0        0     3604 2023-04-16 14:18:41.946841 mimesis-8.0.0/mimesis/data/zh/finance.json
--rw-r--r--   0        0        0     2301 2023-04-16 14:18:41.946841 mimesis-8.0.0/mimesis/data/zh/food.json
--rw-r--r--   0        0        0    96427 2023-04-16 14:18:41.946841 mimesis-8.0.0/mimesis/data/zh/person.json
--rw-r--r--   0        0        0    17796 2023-04-16 14:18:41.946841 mimesis-8.0.0/mimesis/data/zh/text.json
--rw-r--r--   0        0        0      377 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/entrypoints.py
--rw-r--r--   0        0        0     6827 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/enums.py
--rw-r--r--   0        0        0     1901 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/exceptions.py
--rw-r--r--   0        0        0      507 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/locales.py
--rw-r--r--   0        0        0     1450 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/__init__.py
--rw-r--r--   0        0        0     7754 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/address.py
--rw-r--r--   0        0        0     7676 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/base.py
--rw-r--r--   0        0        0     3058 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/binaryfile.py
--rw-r--r--   0        0        0     3190 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/choice.py
--rw-r--r--   0        0        0     2655 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/code.py
--rw-r--r--   0        0        0     3325 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/cryptographic.py
--rw-r--r--   0        0        0     8676 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/date.py
--rw-r--r--   0        0        0     2768 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/development.py
--rw-r--r--   0        0        0     2136 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/file.py
--rw-r--r--   0        0        0     3754 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/finance.py
--rw-r--r--   0        0        0     1712 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/food.py
--rw-r--r--   0        0        0     5534 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/generic.py
--rw-r--r--   0        0        0     3044 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/hardware.py
--rw-r--r--   0        0        0    15706 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/internet.py
--rw-r--r--   0        0        0     7042 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/numeric.py
--rw-r--r--   0        0        0     2746 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/path.py
--rw-r--r--   0        0        0     5199 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/payment.py
--rw-r--r--   0        0        0    13766 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/person.py
--rw-r--r--   0        0        0     2126 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/science.py
--rw-r--r--   0        0        0     4375 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/text.py
--rw-r--r--   0        0        0     1454 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/transport.py
--rw-r--r--   0        0        0        1 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/py.typed
--rw-r--r--   0        0        0     4502 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/random.py
--rw-r--r--   0        0        0    13900 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/schema.py
--rw-r--r--   0        0        0     1373 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/shortcuts.py
--rw-r--r--   0        0        0     1190 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/types.py
--rw-r--r--   0        0        0     2748 2023-04-16 14:18:20.078791 mimesis-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     8588 1970-01-01 00:00:00.000000 mimesis-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-04-30 12:40:15.227399 mimesis-9.0.0/LICENSE
+-rw-r--r--   0        0        0     7075 2023-04-30 12:40:15.227399 mimesis-9.0.0/README.rst
+-rw-r--r--   0        0        0     2361 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/__init__.py
+-rw-r--r--   0        0        0      552 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/builtins/__init__.py
+-rw-r--r--   0        0        0      428 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/builtins/base.py
+-rw-r--r--   0        0        0     3671 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/builtins/da.py
+-rw-r--r--   0        0        0     1776 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/builtins/en.py
+-rw-r--r--   0        0        0     1545 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/builtins/it.py
+-rw-r--r--   0        0        0     1535 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/builtins/nl.py
+-rw-r--r--   0        0        0     3281 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/builtins/pl.py
+-rw-r--r--   0        0        0     3354 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/builtins/pt_br.py
+-rw-r--r--   0        0        0     7496 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/builtins/ru.py
+-rw-r--r--   0        0        0     1084 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/builtins/uk.py
+-rw-r--r--   0        0        0      127 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/compat.py
+-rw-r--r--   0        0        0      403 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/data/__init__.py
+-rw-r--r--   0        0        0   182787 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/data/bin/sample.aac
+-rw-r--r--   0        0        0   385692 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/data/bin/sample.docx
+-rw-r--r--   0        0        0   115256 2023-04-30 12:40:15.235400 mimesis-9.0.0/mimesis/data/bin/sample.gif
+-rw-r--r--   0        0        0      269 2023-04-30 12:40:15.239400 mimesis-9.0.0/mimesis/data/bin/sample.gz
+-rw-r--r--   0        0        0    88187 2023-04-30 12:40:15.239400 mimesis-9.0.0/mimesis/data/bin/sample.jpg
+-rw-r--r--   0        0        0   281424 2023-04-30 12:40:15.239400 mimesis-9.0.0/mimesis/data/bin/sample.mov
+-rw-r--r--   0        0        0    67911 2023-04-30 12:40:15.239400 mimesis-9.0.0/mimesis/data/bin/sample.mp3
+-rw-r--r--   0        0        0   304520 2023-04-30 12:40:15.239400 mimesis-9.0.0/mimesis/data/bin/sample.mp4
+-rw-r--r--   0        0        0   414593 2023-04-30 12:40:15.243400 mimesis-9.0.0/mimesis/data/bin/sample.pdf
+-rw-r--r--   0        0        0   221697 2023-04-30 12:40:15.247401 mimesis-9.0.0/mimesis/data/bin/sample.png
+-rw-r--r--   0        0        0   223362 2023-04-30 12:40:15.247401 mimesis-9.0.0/mimesis/data/bin/sample.pptx
+-rw-r--r--   0        0        0     4857 2023-04-30 12:40:15.247401 mimesis-9.0.0/mimesis/data/bin/sample.xlsx
+-rw-r--r--   0        0        0      673 2023-04-30 12:40:15.247401 mimesis-9.0.0/mimesis/data/bin/sample.zip
+-rw-r--r--   0        0        0    79583 2023-04-30 12:40:37.690985 mimesis-9.0.0/mimesis/data/cs/address.json
+-rw-r--r--   0        0        0      515 2023-04-30 12:40:37.690985 mimesis-9.0.0/mimesis/data/cs/datetime.json
+-rw-r--r--   0        0        0     1340 2023-04-30 12:40:37.690985 mimesis-9.0.0/mimesis/data/cs/finance.json
+-rw-r--r--   0        0        0     1845 2023-04-30 12:40:37.690985 mimesis-9.0.0/mimesis/data/cs/food.json
+-rw-r--r--   0        0        0    33117 2023-04-30 12:40:37.690985 mimesis-9.0.0/mimesis/data/cs/person.json
+-rw-r--r--   0        0        0    49335 2023-04-30 12:40:37.694985 mimesis-9.0.0/mimesis/data/cs/text.json
+-rw-r--r--   0        0        0    82900 2023-04-30 12:40:37.694985 mimesis-9.0.0/mimesis/data/da/address.json
+-rw-r--r--   0        0        0      494 2023-04-30 12:40:37.694985 mimesis-9.0.0/mimesis/data/da/datetime.json
+-rw-r--r--   0        0        0     4656 2023-04-30 12:40:37.694985 mimesis-9.0.0/mimesis/data/da/finance.json
+-rw-r--r--   0        0        0     3873 2023-04-30 12:40:37.694985 mimesis-9.0.0/mimesis/data/da/food.json
+-rw-r--r--   0        0        0    23273 2023-04-30 12:40:37.698984 mimesis-9.0.0/mimesis/data/da/person.json
+-rw-r--r--   0        0        0    17323 2023-04-30 12:40:37.698984 mimesis-9.0.0/mimesis/data/da/text.json
+-rw-r--r--   0        0        0   251577 2023-04-30 12:40:37.706984 mimesis-9.0.0/mimesis/data/de/address.json
+-rw-r--r--   0        0        0      512 2023-04-30 12:40:37.706984 mimesis-9.0.0/mimesis/data/de/datetime.json
+-rw-r--r--   0        0        0     3497 2023-04-30 12:40:37.706984 mimesis-9.0.0/mimesis/data/de/finance.json
+-rw-r--r--   0        0        0     6237 2023-04-30 12:40:37.706984 mimesis-9.0.0/mimesis/data/de/food.json
+-rw-r--r--   0        0        0    18346 2023-04-30 12:40:37.706984 mimesis-9.0.0/mimesis/data/de/person.json
+-rw-r--r--   0        0        0   773143 2023-04-30 12:40:37.722984 mimesis-9.0.0/mimesis/data/de/text.json
+-rw-r--r--   0        0        0    73006 2023-04-30 12:40:37.722984 mimesis-9.0.0/mimesis/data/de-at/address.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.722984 mimesis-9.0.0/mimesis/data/de-at/datetime.json
+-rw-r--r--   0        0        0     4538 2023-04-30 12:40:37.726984 mimesis-9.0.0/mimesis/data/de-at/finance.json
+-rw-r--r--   0        0        0     2335 2023-04-30 12:40:37.726984 mimesis-9.0.0/mimesis/data/de-at/food.json
+-rw-r--r--   0        0        0    28622 2023-04-30 12:40:37.726984 mimesis-9.0.0/mimesis/data/de-at/person.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.726984 mimesis-9.0.0/mimesis/data/de-at/text.json
+-rw-r--r--   0        0        0    42841 2023-04-30 12:40:37.726984 mimesis-9.0.0/mimesis/data/de-ch/address.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.726984 mimesis-9.0.0/mimesis/data/de-ch/datetime.json
+-rw-r--r--   0        0        0     9750 2023-04-30 12:40:37.726984 mimesis-9.0.0/mimesis/data/de-ch/finance.json
+-rw-r--r--   0        0        0      152 2023-04-30 12:40:37.726984 mimesis-9.0.0/mimesis/data/de-ch/food.json
+-rw-r--r--   0        0        0    71143 2023-04-30 12:40:37.730985 mimesis-9.0.0/mimesis/data/de-ch/person.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.730985 mimesis-9.0.0/mimesis/data/de-ch/text.json
+-rw-r--r--   0        0        0    99824 2023-04-30 12:40:37.730985 mimesis-9.0.0/mimesis/data/el/address.json
+-rw-r--r--   0        0        0      817 2023-04-30 12:40:37.730985 mimesis-9.0.0/mimesis/data/el/datetime.json
+-rw-r--r--   0        0        0     2249 2023-04-30 12:40:37.730985 mimesis-9.0.0/mimesis/data/el/finance.json
+-rw-r--r--   0        0        0     4461 2023-04-30 12:40:37.730985 mimesis-9.0.0/mimesis/data/el/food.json
+-rw-r--r--   0        0        0    14494 2023-04-30 12:40:37.734984 mimesis-9.0.0/mimesis/data/el/person.json
+-rw-r--r--   0        0        0    10297 2023-04-30 12:40:37.734984 mimesis-9.0.0/mimesis/data/el/text.json
+-rw-r--r--   0        0        0    50488 2023-04-30 12:40:37.734984 mimesis-9.0.0/mimesis/data/en/address.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.734984 mimesis-9.0.0/mimesis/data/en/builtin.json
+-rw-r--r--   0        0        0      501 2023-04-30 12:40:37.734984 mimesis-9.0.0/mimesis/data/en/datetime.json
+-rw-r--r--   0        0        0    24968 2023-04-30 12:40:37.734984 mimesis-9.0.0/mimesis/data/en/finance.json
+-rw-r--r--   0        0        0    14076 2023-04-30 12:40:37.734984 mimesis-9.0.0/mimesis/data/en/food.json
+-rw-r--r--   0        0        0    64738 2023-04-30 12:40:37.738984 mimesis-9.0.0/mimesis/data/en/person.json
+-rw-r--r--   0        0        0   343508 2023-04-30 12:40:37.746984 mimesis-9.0.0/mimesis/data/en/text.json
+-rw-r--r--   0        0        0    68774 2023-04-30 12:40:37.746984 mimesis-9.0.0/mimesis/data/en-au/address.json
+-rw-r--r--   0        0        0       49 2023-04-30 12:40:37.746984 mimesis-9.0.0/mimesis/data/en-au/datetime.json
+-rw-r--r--   0        0        0   117507 2023-04-30 12:40:37.750985 mimesis-9.0.0/mimesis/data/en-au/finance.json
+-rw-r--r--   0        0        0      504 2023-04-30 12:40:37.750985 mimesis-9.0.0/mimesis/data/en-au/food.json
+-rw-r--r--   0        0        0    41658 2023-04-30 12:40:37.750985 mimesis-9.0.0/mimesis/data/en-au/person.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.750985 mimesis-9.0.0/mimesis/data/en-au/text.json
+-rw-r--r--   0        0        0    24229 2023-04-30 12:40:37.750985 mimesis-9.0.0/mimesis/data/en-ca/address.json
+-rw-r--r--   0        0        0       49 2023-04-30 12:40:37.750985 mimesis-9.0.0/mimesis/data/en-ca/datetime.json
+-rw-r--r--   0        0        0     3053 2023-04-30 12:40:37.750985 mimesis-9.0.0/mimesis/data/en-ca/finance.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.750985 mimesis-9.0.0/mimesis/data/en-ca/food.json
+-rw-r--r--   0        0        0    13729 2023-04-30 12:40:37.750985 mimesis-9.0.0/mimesis/data/en-ca/person.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.750985 mimesis-9.0.0/mimesis/data/en-ca/text.json
+-rw-r--r--   0        0        0    84033 2023-04-30 12:40:37.754984 mimesis-9.0.0/mimesis/data/en-gb/address.json
+-rw-r--r--   0        0        0       49 2023-04-30 12:40:37.754984 mimesis-9.0.0/mimesis/data/en-gb/datetime.json
+-rw-r--r--   0        0        0     9072 2023-04-30 12:40:37.754984 mimesis-9.0.0/mimesis/data/en-gb/finance.json
+-rw-r--r--   0        0        0     1316 2023-04-30 12:40:37.754984 mimesis-9.0.0/mimesis/data/en-gb/food.json
+-rw-r--r--   0        0        0    45054 2023-04-30 12:40:37.754984 mimesis-9.0.0/mimesis/data/en-gb/person.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.754984 mimesis-9.0.0/mimesis/data/en-gb/text.json
+-rw-r--r--   0        0        0    23805 2023-04-30 12:40:37.758984 mimesis-9.0.0/mimesis/data/es/address.json
+-rw-r--r--   0        0        0      561 2023-04-30 12:40:37.758984 mimesis-9.0.0/mimesis/data/es/datetime.json
+-rw-r--r--   0        0        0     2416 2023-04-30 12:40:37.758984 mimesis-9.0.0/mimesis/data/es/finance.json
+-rw-r--r--   0        0        0     4757 2023-04-30 12:40:37.758984 mimesis-9.0.0/mimesis/data/es/food.json
+-rw-r--r--   0        0        0    14143 2023-04-30 12:40:37.758984 mimesis-9.0.0/mimesis/data/es/person.json
+-rw-r--r--   0        0        0   128149 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/es/text.json
+-rw-r--r--   0        0        0    11619 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/es-mx/address.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/es-mx/datetime.json
+-rw-r--r--   0        0        0     2610 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/es-mx/finance.json
+-rw-r--r--   0        0        0     1081 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/es-mx/food.json
+-rw-r--r--   0        0        0    16998 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/es-mx/person.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/es-mx/text.json
+-rw-r--r--   0        0        0    21806 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/et/address.json
+-rw-r--r--   0        0        0      533 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/et/datetime.json
+-rw-r--r--   0        0        0     6635 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/et/finance.json
+-rw-r--r--   0        0        0     3683 2023-04-30 12:40:37.762984 mimesis-9.0.0/mimesis/data/et/food.json
+-rw-r--r--   0        0        0    33842 2023-04-30 12:40:37.766984 mimesis-9.0.0/mimesis/data/et/person.json
+-rw-r--r--   0        0        0    11545 2023-04-30 12:40:37.766984 mimesis-9.0.0/mimesis/data/et/text.json
+-rw-r--r--   0        0        0    13562 2023-04-30 12:40:37.766984 mimesis-9.0.0/mimesis/data/fa/address.json
+-rw-r--r--   0        0        0      665 2023-04-30 12:40:37.766984 mimesis-9.0.0/mimesis/data/fa/datetime.json
+-rw-r--r--   0        0        0     2589 2023-04-30 12:40:37.766984 mimesis-9.0.0/mimesis/data/fa/finance.json
+-rw-r--r--   0        0        0     6628 2023-04-30 12:40:37.766984 mimesis-9.0.0/mimesis/data/fa/food.json
+-rw-r--r--   0        0        0    56905 2023-04-30 12:40:37.766984 mimesis-9.0.0/mimesis/data/fa/person.json
+-rw-r--r--   0        0        0    11302 2023-04-30 12:40:37.766984 mimesis-9.0.0/mimesis/data/fa/text.json
+-rw-r--r--   0        0        0     5488 2023-04-30 12:40:37.770985 mimesis-9.0.0/mimesis/data/fi/address.json
+-rw-r--r--   0        0        0      542 2023-04-30 12:40:37.770985 mimesis-9.0.0/mimesis/data/fi/datetime.json
+-rw-r--r--   0        0        0     7886 2023-04-30 12:40:37.770985 mimesis-9.0.0/mimesis/data/fi/finance.json
+-rw-r--r--   0        0        0     3674 2023-04-30 12:40:37.770985 mimesis-9.0.0/mimesis/data/fi/food.json
+-rw-r--r--   0        0        0    26719 2023-04-30 12:40:37.770985 mimesis-9.0.0/mimesis/data/fi/person.json
+-rw-r--r--   0        0        0    57968 2023-04-30 12:40:37.770985 mimesis-9.0.0/mimesis/data/fi/text.json
+-rw-r--r--   0        0        0    39318 2023-04-30 12:40:37.774984 mimesis-9.0.0/mimesis/data/fr/address.json
+-rw-r--r--   0        0        0      529 2023-04-30 12:40:37.774984 mimesis-9.0.0/mimesis/data/fr/datetime.json
+-rw-r--r--   0        0        0     4390 2023-04-30 12:40:37.774984 mimesis-9.0.0/mimesis/data/fr/finance.json
+-rw-r--r--   0        0        0     7024 2023-04-30 12:40:37.774984 mimesis-9.0.0/mimesis/data/fr/food.json
+-rw-r--r--   0        0        0    46272 2023-04-30 12:40:37.774984 mimesis-9.0.0/mimesis/data/fr/person.json
+-rw-r--r--   0        0        0    37433 2023-04-30 12:40:37.774984 mimesis-9.0.0/mimesis/data/fr/text.json
+-rw-r--r--   0        0        0    13842 2023-04-30 12:40:37.778984 mimesis-9.0.0/mimesis/data/hu/address.json
+-rw-r--r--   0        0        0      515 2023-04-30 12:40:37.778984 mimesis-9.0.0/mimesis/data/hu/datetime.json
+-rw-r--r--   0        0        0      762 2023-04-30 12:40:37.778984 mimesis-9.0.0/mimesis/data/hu/finance.json
+-rw-r--r--   0        0        0     4302 2023-04-30 12:40:37.778984 mimesis-9.0.0/mimesis/data/hu/food.json
+-rw-r--r--   0        0        0    26944 2023-04-30 12:40:37.778984 mimesis-9.0.0/mimesis/data/hu/person.json
+-rw-r--r--   0        0        0    22876 2023-04-30 12:40:37.778984 mimesis-9.0.0/mimesis/data/hu/text.json
+-rw-r--r--   0        0        0      398 2023-04-30 12:40:15.271402 mimesis-9.0.0/mimesis/data/int/__init__.py
+-rw-r--r--   0        0        0    20986 2023-04-30 12:40:15.271402 mimesis-9.0.0/mimesis/data/int/address.py
+-rw-r--r--   0        0        0     2735 2023-04-30 12:40:15.271402 mimesis-9.0.0/mimesis/data/int/code.py
+-rw-r--r--   0        0        0     2223 2023-04-30 12:40:15.271402 mimesis-9.0.0/mimesis/data/int/common.py
+-rw-r--r--   0        0        0    27537 2023-04-30 12:40:15.271402 mimesis-9.0.0/mimesis/data/int/cryptographic.py
+-rw-r--r--   0        0        0    11625 2023-04-30 12:40:15.271402 mimesis-9.0.0/mimesis/data/int/datetime.py
+-rw-r--r--   0        0        0     7778 2023-04-30 12:40:15.271402 mimesis-9.0.0/mimesis/data/int/development.py
+-rw-r--r--   0        0        0    67892 2023-04-30 12:40:15.271402 mimesis-9.0.0/mimesis/data/int/file.py
+-rw-r--r--   0        0        0   264126 2023-04-30 12:40:15.275402 mimesis-9.0.0/mimesis/data/int/finance.py
+-rw-r--r--   0        0        0     5221 2023-04-30 12:40:15.275402 mimesis-9.0.0/mimesis/data/int/hardware.py
+-rw-r--r--   0        0        0    37473 2023-04-30 12:40:15.275402 mimesis-9.0.0/mimesis/data/int/internet.py
+-rw-r--r--   0        0        0      320 2023-04-30 12:40:15.275402 mimesis-9.0.0/mimesis/data/int/path.py
+-rw-r--r--   0        0        0      171 2023-04-30 12:40:15.275402 mimesis-9.0.0/mimesis/data/int/payment.py
+-rw-r--r--   0        0        0   140341 2023-04-30 12:40:15.275402 mimesis-9.0.0/mimesis/data/int/person.py
+-rw-r--r--   0        0        0      606 2023-04-30 12:40:15.275402 mimesis-9.0.0/mimesis/data/int/scientific.py
+-rw-r--r--   0        0        0      364 2023-04-30 12:40:15.275402 mimesis-9.0.0/mimesis/data/int/text.py
+-rw-r--r--   0        0        0    31498 2023-04-30 12:40:15.275402 mimesis-9.0.0/mimesis/data/int/transport.py
+-rw-r--r--   0        0        0   121675 2023-04-30 12:40:37.782984 mimesis-9.0.0/mimesis/data/is/address.json
+-rw-r--r--   0        0        0      546 2023-04-30 12:40:37.782984 mimesis-9.0.0/mimesis/data/is/datetime.json
+-rw-r--r--   0        0        0     1539 2023-04-30 12:40:37.782984 mimesis-9.0.0/mimesis/data/is/finance.json
+-rw-r--r--   0        0        0     1651 2023-04-30 12:40:37.782984 mimesis-9.0.0/mimesis/data/is/food.json
+-rw-r--r--   0        0        0    68768 2023-04-30 12:40:37.786984 mimesis-9.0.0/mimesis/data/is/person.json
+-rw-r--r--   0        0        0    51794 2023-04-30 12:40:37.786984 mimesis-9.0.0/mimesis/data/is/text.json
+-rw-r--r--   0        0        0   123349 2023-04-30 12:40:37.790984 mimesis-9.0.0/mimesis/data/it/address.json
+-rw-r--r--   0        0        0      142 2023-04-30 12:40:37.790984 mimesis-9.0.0/mimesis/data/it/builtin.json
+-rw-r--r--   0        0        0      535 2023-04-30 12:40:37.790984 mimesis-9.0.0/mimesis/data/it/datetime.json
+-rw-r--r--   0        0        0     5058 2023-04-30 12:40:37.790984 mimesis-9.0.0/mimesis/data/it/finance.json
+-rw-r--r--   0        0        0     5352 2023-04-30 12:40:37.790984 mimesis-9.0.0/mimesis/data/it/food.json
+-rw-r--r--   0        0        0    64650 2023-04-30 12:40:37.794984 mimesis-9.0.0/mimesis/data/it/person.json
+-rw-r--r--   0        0        0    77862 2023-04-30 12:40:37.794984 mimesis-9.0.0/mimesis/data/it/text.json
+-rw-r--r--   0        0        0    10631 2023-04-30 12:40:37.794984 mimesis-9.0.0/mimesis/data/ja/address.json
+-rw-r--r--   0        0        0      494 2023-04-30 12:40:37.794984 mimesis-9.0.0/mimesis/data/ja/datetime.json
+-rw-r--r--   0        0        0    23842 2023-04-30 12:40:37.794984 mimesis-9.0.0/mimesis/data/ja/finance.json
+-rw-r--r--   0        0        0    13902 2023-04-30 12:40:37.798984 mimesis-9.0.0/mimesis/data/ja/food.json
+-rw-r--r--   0        0        0    69460 2023-04-30 12:40:37.798984 mimesis-9.0.0/mimesis/data/ja/person.json
+-rw-r--r--   0        0        0    56672 2023-04-30 12:40:37.798984 mimesis-9.0.0/mimesis/data/ja/text.json
+-rw-r--r--   0        0        0    33301 2023-04-30 12:40:37.798984 mimesis-9.0.0/mimesis/data/kk/address.json
+-rw-r--r--   0        0        0      768 2023-04-30 12:40:37.802984 mimesis-9.0.0/mimesis/data/kk/datetime.json
+-rw-r--r--   0        0        0     6707 2023-04-30 12:40:37.802984 mimesis-9.0.0/mimesis/data/kk/finance.json
+-rw-r--r--   0        0        0       95 2023-04-30 12:40:37.802984 mimesis-9.0.0/mimesis/data/kk/food.json
+-rw-r--r--   0        0        0    28448 2023-04-30 12:40:37.802984 mimesis-9.0.0/mimesis/data/kk/person.json
+-rw-r--r--   0        0        0    14350 2023-04-30 12:40:37.802984 mimesis-9.0.0/mimesis/data/kk/text.json
+-rw-r--r--   0        0        0    30313 2023-04-30 12:40:37.802984 mimesis-9.0.0/mimesis/data/ko/address.json
+-rw-r--r--   0        0        0      492 2023-04-30 12:40:37.802984 mimesis-9.0.0/mimesis/data/ko/datetime.json
+-rw-r--r--   0        0        0    17722 2023-04-30 12:40:37.802984 mimesis-9.0.0/mimesis/data/ko/finance.json
+-rw-r--r--   0        0        0    12695 2023-04-30 12:40:37.802984 mimesis-9.0.0/mimesis/data/ko/food.json
+-rw-r--r--   0        0        0    39279 2023-04-30 12:40:37.806984 mimesis-9.0.0/mimesis/data/ko/person.json
+-rw-r--r--   0        0        0    68560 2023-04-30 12:40:37.806984 mimesis-9.0.0/mimesis/data/ko/text.json
+-rw-r--r--   0        0        0    60825 2023-04-30 12:40:37.810984 mimesis-9.0.0/mimesis/data/nl/address.json
+-rw-r--r--   0        0        0      507 2023-04-30 12:40:37.810984 mimesis-9.0.0/mimesis/data/nl/datetime.json
+-rw-r--r--   0        0        0     2771 2023-04-30 12:40:37.810984 mimesis-9.0.0/mimesis/data/nl/finance.json
+-rw-r--r--   0        0        0     7412 2023-04-30 12:40:37.810984 mimesis-9.0.0/mimesis/data/nl/food.json
+-rw-r--r--   0        0        0   109294 2023-04-30 12:40:37.814984 mimesis-9.0.0/mimesis/data/nl/person.json
+-rw-r--r--   0        0        0   202851 2023-04-30 12:40:37.818984 mimesis-9.0.0/mimesis/data/nl/text.json
+-rw-r--r--   0        0        0    53656 2023-04-30 12:40:37.818984 mimesis-9.0.0/mimesis/data/nl-be/address.json
+-rw-r--r--   0        0        0       31 2023-04-30 12:40:37.818984 mimesis-9.0.0/mimesis/data/nl-be/datetime.json
+-rw-r--r--   0        0        0     2303 2023-04-30 12:40:37.818984 mimesis-9.0.0/mimesis/data/nl-be/finance.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.818984 mimesis-9.0.0/mimesis/data/nl-be/food.json
+-rw-r--r--   0        0        0     1371 2023-04-30 12:40:37.818984 mimesis-9.0.0/mimesis/data/nl-be/person.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.818984 mimesis-9.0.0/mimesis/data/nl-be/text.json
+-rw-r--r--   0        0        0    40052 2023-04-30 12:40:37.822984 mimesis-9.0.0/mimesis/data/no/address.json
+-rw-r--r--   0        0        0      500 2023-04-30 12:40:37.822984 mimesis-9.0.0/mimesis/data/no/datetime.json
+-rw-r--r--   0        0        0     9731 2023-04-30 12:40:37.822984 mimesis-9.0.0/mimesis/data/no/finance.json
+-rw-r--r--   0        0        0     4479 2023-04-30 12:40:37.822984 mimesis-9.0.0/mimesis/data/no/food.json
+-rw-r--r--   0        0        0    43488 2023-04-30 12:40:37.822984 mimesis-9.0.0/mimesis/data/no/person.json
+-rw-r--r--   0        0        0    31334 2023-04-30 12:40:37.822984 mimesis-9.0.0/mimesis/data/no/text.json
+-rw-r--r--   0        0        0    80118 2023-04-30 12:40:37.826984 mimesis-9.0.0/mimesis/data/pl/address.json
+-rw-r--r--   0        0        0      567 2023-04-30 12:40:37.826984 mimesis-9.0.0/mimesis/data/pl/datetime.json
+-rw-r--r--   0        0        0    10830 2023-04-30 12:40:37.826984 mimesis-9.0.0/mimesis/data/pl/finance.json
+-rw-r--r--   0        0        0     4693 2023-04-30 12:40:37.826984 mimesis-9.0.0/mimesis/data/pl/food.json
+-rw-r--r--   0        0        0    27705 2023-04-30 12:40:37.826984 mimesis-9.0.0/mimesis/data/pl/person.json
+-rw-r--r--   0        0        0    65088 2023-04-30 12:40:37.830984 mimesis-9.0.0/mimesis/data/pl/text.json
+-rw-r--r--   0        0        0    19169 2023-04-30 12:40:37.830984 mimesis-9.0.0/mimesis/data/pt/address.json
+-rw-r--r--   0        0        0      563 2023-04-30 12:40:37.830984 mimesis-9.0.0/mimesis/data/pt/datetime.json
+-rw-r--r--   0        0        0     2572 2023-04-30 12:40:37.830984 mimesis-9.0.0/mimesis/data/pt/finance.json
+-rw-r--r--   0        0        0     4310 2023-04-30 12:40:37.830984 mimesis-9.0.0/mimesis/data/pt/food.json
+-rw-r--r--   0        0        0    38175 2023-04-30 12:40:37.830984 mimesis-9.0.0/mimesis/data/pt/person.json
+-rw-r--r--   0        0        0    25766 2023-04-30 12:40:37.834984 mimesis-9.0.0/mimesis/data/pt/text.json
+-rw-r--r--   0        0        0    94350 2023-04-30 12:40:37.834984 mimesis-9.0.0/mimesis/data/pt-br/address.json
+-rw-r--r--   0        0        0      564 2023-04-30 12:40:37.834984 mimesis-9.0.0/mimesis/data/pt-br/datetime.json
+-rw-r--r--   0        0        0    24208 2023-04-30 12:40:37.838984 mimesis-9.0.0/mimesis/data/pt-br/finance.json
+-rw-r--r--   0        0        0     3162 2023-04-30 12:40:37.838984 mimesis-9.0.0/mimesis/data/pt-br/food.json
+-rw-r--r--   0        0        0    63714 2023-04-30 12:40:37.838984 mimesis-9.0.0/mimesis/data/pt-br/person.json
+-rw-r--r--   0        0        0        2 2023-04-30 12:40:37.838984 mimesis-9.0.0/mimesis/data/pt-br/text.json
+-rw-r--r--   0        0        0   101129 2023-04-30 12:40:37.842984 mimesis-9.0.0/mimesis/data/ru/address.json
+-rw-r--r--   0        0        0    10949 2023-04-30 12:40:37.842984 mimesis-9.0.0/mimesis/data/ru/builtin.json
+-rw-r--r--   0        0        0      790 2023-04-30 12:40:37.842984 mimesis-9.0.0/mimesis/data/ru/datetime.json
+-rw-r--r--   0        0        0    22783 2023-04-30 12:40:37.842984 mimesis-9.0.0/mimesis/data/ru/finance.json
+-rw-r--r--   0        0        0    20262 2023-04-30 12:40:37.842984 mimesis-9.0.0/mimesis/data/ru/food.json
+-rw-r--r--   0        0        0    86369 2023-04-30 12:40:37.842984 mimesis-9.0.0/mimesis/data/ru/person.json
+-rw-r--r--   0        0        0    89215 2023-04-30 12:40:37.846984 mimesis-9.0.0/mimesis/data/ru/text.json
+-rw-r--r--   0        0        0    38882 2023-04-30 12:40:37.846984 mimesis-9.0.0/mimesis/data/sk/address.json
+-rw-r--r--   0        0        0      485 2023-04-30 12:40:37.846984 mimesis-9.0.0/mimesis/data/sk/datetime.json
+-rw-r--r--   0        0        0      816 2023-04-30 12:40:37.846984 mimesis-9.0.0/mimesis/data/sk/finance.json
+-rw-r--r--   0        0        0      284 2023-04-30 12:40:37.846984 mimesis-9.0.0/mimesis/data/sk/food.json
+-rw-r--r--   0        0        0     5828 2023-04-30 12:40:37.846984 mimesis-9.0.0/mimesis/data/sk/person.json
+-rw-r--r--   0        0        0      752 2023-04-30 12:40:37.846984 mimesis-9.0.0/mimesis/data/sk/text.json
+-rw-r--r--   0        0        0    97258 2023-04-30 12:40:37.850984 mimesis-9.0.0/mimesis/data/sv/address.json
+-rw-r--r--   0        0        0      508 2023-04-30 12:40:37.850984 mimesis-9.0.0/mimesis/data/sv/datetime.json
+-rw-r--r--   0        0        0     5035 2023-04-30 12:40:37.850984 mimesis-9.0.0/mimesis/data/sv/finance.json
+-rw-r--r--   0        0        0     6863 2023-04-30 12:40:37.850984 mimesis-9.0.0/mimesis/data/sv/food.json
+-rw-r--r--   0        0        0    32781 2023-04-30 12:40:37.854984 mimesis-9.0.0/mimesis/data/sv/person.json
+-rw-r--r--   0        0        0    41878 2023-04-30 12:40:37.854984 mimesis-9.0.0/mimesis/data/sv/text.json
+-rw-r--r--   0        0        0    12375 2023-04-30 12:40:37.854984 mimesis-9.0.0/mimesis/data/tr/address.json
+-rw-r--r--   0        0        0      508 2023-04-30 12:40:37.854984 mimesis-9.0.0/mimesis/data/tr/datetime.json
+-rw-r--r--   0        0        0    11988 2023-04-30 12:40:37.854984 mimesis-9.0.0/mimesis/data/tr/finance.json
+-rw-r--r--   0        0        0     1819 2023-04-30 12:40:37.854984 mimesis-9.0.0/mimesis/data/tr/food.json
+-rw-r--r--   0        0        0    29265 2023-04-30 12:40:37.858984 mimesis-9.0.0/mimesis/data/tr/person.json
+-rw-r--r--   0        0        0     8857 2023-04-30 12:40:37.858984 mimesis-9.0.0/mimesis/data/tr/text.json
+-rw-r--r--   0        0        0    54571 2023-04-30 12:40:37.858984 mimesis-9.0.0/mimesis/data/uk/address.json
+-rw-r--r--   0        0        0     6247 2023-04-30 12:40:37.858984 mimesis-9.0.0/mimesis/data/uk/builtin.json
+-rw-r--r--   0        0        0      790 2023-04-30 12:40:37.858984 mimesis-9.0.0/mimesis/data/uk/datetime.json
+-rw-r--r--   0        0        0     6981 2023-04-30 12:40:37.858984 mimesis-9.0.0/mimesis/data/uk/finance.json
+-rw-r--r--   0        0        0     9121 2023-04-30 12:40:37.858984 mimesis-9.0.0/mimesis/data/uk/food.json
+-rw-r--r--   0        0        0    52753 2023-04-30 12:40:37.858984 mimesis-9.0.0/mimesis/data/uk/person.json
+-rw-r--r--   0        0        0    21072 2023-04-30 12:40:37.862984 mimesis-9.0.0/mimesis/data/uk/text.json
+-rw-r--r--   0        0        0    10240 2023-04-30 12:40:37.862984 mimesis-9.0.0/mimesis/data/zh/address.json
+-rw-r--r--   0        0        0      539 2023-04-30 12:40:37.862984 mimesis-9.0.0/mimesis/data/zh/datetime.json
+-rw-r--r--   0        0        0     3604 2023-04-30 12:40:37.862984 mimesis-9.0.0/mimesis/data/zh/finance.json
+-rw-r--r--   0        0        0     2301 2023-04-30 12:40:37.862984 mimesis-9.0.0/mimesis/data/zh/food.json
+-rw-r--r--   0        0        0    96427 2023-04-30 12:40:37.862984 mimesis-9.0.0/mimesis/data/zh/person.json
+-rw-r--r--   0        0        0    17796 2023-04-30 12:40:37.862984 mimesis-9.0.0/mimesis/data/zh/text.json
+-rw-r--r--   0        0        0      377 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/entrypoints.py
+-rw-r--r--   0        0        0     6827 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/enums.py
+-rw-r--r--   0        0        0     1901 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/exceptions.py
+-rw-r--r--   0        0        0      869 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/keys.py
+-rw-r--r--   0        0        0      507 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/locales.py
+-rw-r--r--   0        0        0     1450 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/__init__.py
+-rw-r--r--   0        0        0     7764 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/address.py
+-rw-r--r--   0        0        0     7738 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/base.py
+-rw-r--r--   0        0        0     3058 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/binaryfile.py
+-rw-r--r--   0        0        0     3190 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/choice.py
+-rw-r--r--   0        0        0     2655 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/code.py
+-rw-r--r--   0        0        0     3325 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/cryptographic.py
+-rw-r--r--   0        0        0     8683 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/date.py
+-rw-r--r--   0        0        0     2768 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/development.py
+-rw-r--r--   0        0        0     2136 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/file.py
+-rw-r--r--   0        0        0     3758 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/finance.py
+-rw-r--r--   0        0        0     1713 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/food.py
+-rw-r--r--   0        0        0     5534 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/generic.py
+-rw-r--r--   0        0        0     3044 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/hardware.py
+-rw-r--r--   0        0        0    15706 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/internet.py
+-rw-r--r--   0        0        0     7042 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/numeric.py
+-rw-r--r--   0        0        0     2746 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/path.py
+-rw-r--r--   0        0        0     5152 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/payment.py
+-rw-r--r--   0        0        0    13459 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/person.py
+-rw-r--r--   0        0        0     2128 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/science.py
+-rw-r--r--   0        0        0     4383 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/text.py
+-rw-r--r--   0        0        0     1454 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/providers/transport.py
+-rw-r--r--   0        0        0        1 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/py.typed
+-rw-r--r--   0        0        0     4979 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/random.py
+-rw-r--r--   0        0        0    10996 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/schema.py
+-rw-r--r--   0        0        0     1373 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/shortcuts.py
+-rw-r--r--   0        0        0     1190 2023-04-30 12:40:15.299404 mimesis-9.0.0/mimesis/types.py
+-rw-r--r--   0        0        0     2756 2023-04-30 12:40:15.299404 mimesis-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8718 1970-01-01 00:00:00.000000 mimesis-9.0.0/PKG-INFO
```

### Comparing `mimesis-8.0.0/LICENSE` & `mimesis-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/README.rst` & `mimesis-9.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
 
 Python compatibility
 ---------------------
 
 Mimesis is compatible with Python, including PyPy, version 3.8 or higher. The Mimesis 4.1.3 is the last release that accommodates Python 3.6 and 3.7.
 
+To prevent unintended upgrades, it is higly advisable to always specify the version of mimesis that you are using by pinning it.
+
 Supported Features
 ------------------
 
 - **Easy**: A simple design and clear documentation for easy and swift data generation.
 - **Multilingual**: Mimesis generates data in a vast range of `languages <https://mimesis.name/en/latest/getting_started.html#supported-locales>`_.
 - **Performance**: Mimesis has excellent performance and is widely regarded as the fastest data generator among all Python solutions available.
 - **Data variety**: Mimesis supports a broad range of data providers, including names, addresses, phone numbers, email addresses, dates, times, and more, enabling users to generate data for various purposes.
```

### Comparing `mimesis-8.0.0/mimesis/__init__.py` & `mimesis-9.0.0/mimesis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Copyright (c) 2016 - 2023 Isaak Uchakaev (Likid Geimfari).
 Website: https://mimesis.name
 Email: <likid.geimfari@gmail.com>
 Repository: https://github.com/lk-geimfari/mimesis
 """
 
+from mimesis import keys
 from mimesis.enums import (
     Algorithm,
     AudioFile,
     CardType,
     CompressedFile,
     CountryCode,
     DocumentFile,
@@ -77,14 +78,16 @@
     "Person",
     "Science",
     "Text",
     "Transport",
     "Cryptographic",
     # Has all:
     "Generic",
+    # Keys:
+    "keys",
     # Schema:
     "Field",
     "Fieldset",
     "Schema",
     # Locale:
     "Locale",
     # Enums:
@@ -116,14 +119,14 @@
     "__description__",
     "__url__",
     "__author__",
     "__author_email__",
     "__license__",
 ]
 
-__version__ = "8.0.0"
+__version__ = "9.0.0"
 __title__ = "mimesis"
 __description__ = "Mimesis: Fake Data Generator."
 __url__ = "https://github.com/lk-geimfari/mimesis"
 __author__ = "Isaak Uchakaev (Likid Geimfari)"
 __author_email__ = "likid.geimfari@gmail.com"
 __license__ = "MIT License"
```

### Comparing `mimesis-8.0.0/mimesis/builtins/__init__.py` & `mimesis-9.0.0/mimesis/builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/builtins/da.py` & `mimesis-9.0.0/mimesis/builtins/da.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/builtins/en.py` & `mimesis-9.0.0/mimesis/builtins/en.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/builtins/it.py` & `mimesis-9.0.0/mimesis/builtins/it.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,21 +33,21 @@
         Example:
             RSSMRA66R05D612U
         """
         code = "".join(self.random.choices(string.ascii_uppercase, k=6))
 
         code += self.random.custom_code(mask="##")
 
-        month_codes = self.extract(["fiscal_code", "month_codes"])
+        month_codes = self._extract(["fiscal_code", "month_codes"])
         code += self.random.choice(month_codes)
 
         birth_day = self.random.randint(101, 131)
         self.validate_enum(gender, Gender)
         if gender == Gender.FEMALE:
             birth_day += 40
         code += str(birth_day)[1:]
 
-        city_letters = self.extract(["fiscal_code", "city_letters"])
+        city_letters = self._extract(["fiscal_code", "city_letters"])
         code += self.random.choice(city_letters)
         code += self.random.custom_code(mask="###@")
 
         return code
```

### Comparing `mimesis-8.0.0/mimesis/builtins/nl.py` & `mimesis-9.0.0/mimesis/builtins/nl.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/builtins/pl.py` & `mimesis-9.0.0/mimesis/builtins/pl.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/builtins/pt_br.py` & `mimesis-9.0.0/mimesis/builtins/pt_br.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/builtins/ru.py` & `mimesis-9.0.0/mimesis/builtins/ru.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         name: t.Final[str] = "russia_provider"
 
     def generate_sentence(self) -> str:
         """Generate sentence from the parts.
 
         :return: Sentence.
         """
-        sentences = self.extract(["sentence"])
+        sentences = self._extract(["sentence"])
         sentence = [
             self.random.choice(sentences[k]) for k in ("head", "p1", "p2", "tail")
         ]
         return " ".join(sentence)
 
     def patronymic(self, gender: t.Optional[Gender] = None) -> str:
         """Generate random patronymic name.
@@ -42,15 +42,15 @@
         :param gender: Gender of person.
         :return: Patronymic name.
 
         :Example:
             Алексеевна.
         """
         gender = self.validate_enum(gender, Gender)
-        patronymics: t.List[str] = self.extract(["patronymic", str(gender)])
+        patronymics: t.List[str] = self._extract(["patronymic", str(gender)])
         return self.random.choice(patronymics)
 
     def passport_series(self, year: t.Optional[int] = None) -> str:
         """Generate random series of passport.
 
         :param year: Year of manufacture.
         :type year: int or None
```

### Comparing `mimesis-8.0.0/mimesis/builtins/uk.py` & `mimesis-9.0.0/mimesis/builtins/uk.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,9 +26,9 @@
         """Generate random patronymic name.
 
         :param gender: Gender of person.
         :type gender: str or int
         :return: Patronymic name.
         """
         gender = self.validate_enum(gender, Gender)
-        patronymics: t.List[str] = self.extract(["patronymic", str(gender)])
+        patronymics: t.List[str] = self._extract(["patronymic", str(gender)])
         return self.random.choice(patronymics)
```

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.aac` & `mimesis-9.0.0/mimesis/data/bin/sample.aac`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.docx` & `mimesis-9.0.0/mimesis/data/bin/sample.docx`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.gif` & `mimesis-9.0.0/mimesis/data/bin/sample.gif`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.jpg` & `mimesis-9.0.0/mimesis/data/bin/sample.jpg`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.mov` & `mimesis-9.0.0/mimesis/data/bin/sample.mov`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.mp3` & `mimesis-9.0.0/mimesis/data/bin/sample.mp3`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.mp4` & `mimesis-9.0.0/mimesis/data/bin/sample.mp4`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.pdf` & `mimesis-9.0.0/mimesis/data/bin/sample.pdf`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.png` & `mimesis-9.0.0/mimesis/data/bin/sample.png`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.pptx` & `mimesis-9.0.0/mimesis/data/bin/sample.pptx`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.xlsx` & `mimesis-9.0.0/mimesis/data/bin/sample.xlsx`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/bin/sample.zip` & `mimesis-9.0.0/mimesis/data/bin/sample.zip`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/cs/address.json` & `mimesis-9.0.0/mimesis/data/cs/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/cs/datetime.json` & `mimesis-9.0.0/mimesis/data/cs/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/cs/finance.json` & `mimesis-9.0.0/mimesis/data/cs/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/cs/food.json` & `mimesis-9.0.0/mimesis/data/cs/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/cs/person.json` & `mimesis-9.0.0/mimesis/data/cs/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/cs/text.json` & `mimesis-9.0.0/mimesis/data/cs/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/da/address.json` & `mimesis-9.0.0/mimesis/data/da/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/da/finance.json` & `mimesis-9.0.0/mimesis/data/da/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/da/food.json` & `mimesis-9.0.0/mimesis/data/da/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/da/person.json` & `mimesis-9.0.0/mimesis/data/da/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/da/text.json` & `mimesis-9.0.0/mimesis/data/da/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de/address.json` & `mimesis-9.0.0/mimesis/data/de/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de/datetime.json` & `mimesis-9.0.0/mimesis/data/de/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de/finance.json` & `mimesis-9.0.0/mimesis/data/de/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de/food.json` & `mimesis-9.0.0/mimesis/data/de/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de/person.json` & `mimesis-9.0.0/mimesis/data/de/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de/text.json` & `mimesis-9.0.0/mimesis/data/de/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de-at/address.json` & `mimesis-9.0.0/mimesis/data/de-at/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de-at/finance.json` & `mimesis-9.0.0/mimesis/data/de-at/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de-at/food.json` & `mimesis-9.0.0/mimesis/data/de-at/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de-at/person.json` & `mimesis-9.0.0/mimesis/data/de-at/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de-ch/address.json` & `mimesis-9.0.0/mimesis/data/de-ch/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de-ch/finance.json` & `mimesis-9.0.0/mimesis/data/de-ch/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/de-ch/person.json` & `mimesis-9.0.0/mimesis/data/de-ch/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/el/address.json` & `mimesis-9.0.0/mimesis/data/el/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/el/datetime.json` & `mimesis-9.0.0/mimesis/data/el/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/el/finance.json` & `mimesis-9.0.0/mimesis/data/el/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/el/food.json` & `mimesis-9.0.0/mimesis/data/el/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/el/person.json` & `mimesis-9.0.0/mimesis/data/el/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/el/text.json` & `mimesis-9.0.0/mimesis/data/el/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en/address.json` & `mimesis-9.0.0/mimesis/data/en/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en/finance.json` & `mimesis-9.0.0/mimesis/data/en/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en/food.json` & `mimesis-9.0.0/mimesis/data/en/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en/person.json` & `mimesis-9.0.0/mimesis/data/en/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en/text.json` & `mimesis-9.0.0/mimesis/data/en/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en-au/address.json` & `mimesis-9.0.0/mimesis/data/en-au/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en-au/finance.json` & `mimesis-9.0.0/mimesis/data/en-au/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en-au/person.json` & `mimesis-9.0.0/mimesis/data/en-au/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en-ca/address.json` & `mimesis-9.0.0/mimesis/data/en-ca/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en-ca/finance.json` & `mimesis-9.0.0/mimesis/data/en-ca/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en-ca/person.json` & `mimesis-9.0.0/mimesis/data/en-ca/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en-gb/address.json` & `mimesis-9.0.0/mimesis/data/en-gb/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en-gb/finance.json` & `mimesis-9.0.0/mimesis/data/en-gb/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en-gb/food.json` & `mimesis-9.0.0/mimesis/data/en-gb/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/en-gb/person.json` & `mimesis-9.0.0/mimesis/data/en-gb/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/es/address.json` & `mimesis-9.0.0/mimesis/data/es/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/es/datetime.json` & `mimesis-9.0.0/mimesis/data/es/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/es/finance.json` & `mimesis-9.0.0/mimesis/data/es/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/es/food.json` & `mimesis-9.0.0/mimesis/data/es/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/es/person.json` & `mimesis-9.0.0/mimesis/data/es/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/es/text.json` & `mimesis-9.0.0/mimesis/data/es/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/es-mx/address.json` & `mimesis-9.0.0/mimesis/data/es-mx/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/es-mx/finance.json` & `mimesis-9.0.0/mimesis/data/es-mx/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/es-mx/food.json` & `mimesis-9.0.0/mimesis/data/es-mx/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/es-mx/person.json` & `mimesis-9.0.0/mimesis/data/es-mx/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/et/address.json` & `mimesis-9.0.0/mimesis/data/et/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/et/datetime.json` & `mimesis-9.0.0/mimesis/data/et/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/et/finance.json` & `mimesis-9.0.0/mimesis/data/et/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/et/food.json` & `mimesis-9.0.0/mimesis/data/et/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/et/person.json` & `mimesis-9.0.0/mimesis/data/et/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/et/text.json` & `mimesis-9.0.0/mimesis/data/et/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fa/address.json` & `mimesis-9.0.0/mimesis/data/fa/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fa/datetime.json` & `mimesis-9.0.0/mimesis/data/fa/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fa/finance.json` & `mimesis-9.0.0/mimesis/data/fa/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fa/food.json` & `mimesis-9.0.0/mimesis/data/fa/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fa/person.json` & `mimesis-9.0.0/mimesis/data/fa/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fa/text.json` & `mimesis-9.0.0/mimesis/data/fa/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fi/address.json` & `mimesis-9.0.0/mimesis/data/fi/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fi/datetime.json` & `mimesis-9.0.0/mimesis/data/fi/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fi/finance.json` & `mimesis-9.0.0/mimesis/data/fi/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fi/food.json` & `mimesis-9.0.0/mimesis/data/fi/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fi/person.json` & `mimesis-9.0.0/mimesis/data/fi/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fi/text.json` & `mimesis-9.0.0/mimesis/data/fi/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fr/address.json` & `mimesis-9.0.0/mimesis/data/fr/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fr/datetime.json` & `mimesis-9.0.0/mimesis/data/fr/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fr/finance.json` & `mimesis-9.0.0/mimesis/data/fr/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fr/food.json` & `mimesis-9.0.0/mimesis/data/fr/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fr/person.json` & `mimesis-9.0.0/mimesis/data/fr/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/fr/text.json` & `mimesis-9.0.0/mimesis/data/fr/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/hu/address.json` & `mimesis-9.0.0/mimesis/data/hu/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/hu/datetime.json` & `mimesis-9.0.0/mimesis/data/hu/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/hu/finance.json` & `mimesis-9.0.0/mimesis/data/hu/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/hu/food.json` & `mimesis-9.0.0/mimesis/data/hu/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/hu/person.json` & `mimesis-9.0.0/mimesis/data/hu/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/hu/text.json` & `mimesis-9.0.0/mimesis/data/hu/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/address.py` & `mimesis-9.0.0/mimesis/data/int/address.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/code.py` & `mimesis-9.0.0/mimesis/data/int/code.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/common.py` & `mimesis-9.0.0/mimesis/data/int/common.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/cryptographic.py` & `mimesis-9.0.0/mimesis/data/int/cryptographic.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/datetime.py` & `mimesis-9.0.0/mimesis/data/int/datetime.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/development.py` & `mimesis-9.0.0/mimesis/data/int/development.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/file.py` & `mimesis-9.0.0/mimesis/data/int/file.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/finance.py` & `mimesis-9.0.0/mimesis/data/int/finance.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/hardware.py` & `mimesis-9.0.0/mimesis/data/int/hardware.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/internet.py` & `mimesis-9.0.0/mimesis/data/int/internet.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/person.py` & `mimesis-9.0.0/mimesis/data/int/person.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/scientific.py` & `mimesis-9.0.0/mimesis/data/int/scientific.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/int/transport.py` & `mimesis-9.0.0/mimesis/data/int/transport.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/is/address.json` & `mimesis-9.0.0/mimesis/data/is/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/is/datetime.json` & `mimesis-9.0.0/mimesis/data/is/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/is/finance.json` & `mimesis-9.0.0/mimesis/data/is/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/is/food.json` & `mimesis-9.0.0/mimesis/data/is/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/is/person.json` & `mimesis-9.0.0/mimesis/data/is/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/is/text.json` & `mimesis-9.0.0/mimesis/data/is/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/it/address.json` & `mimesis-9.0.0/mimesis/data/it/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/it/datetime.json` & `mimesis-9.0.0/mimesis/data/it/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/it/finance.json` & `mimesis-9.0.0/mimesis/data/it/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/it/food.json` & `mimesis-9.0.0/mimesis/data/it/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/it/person.json` & `mimesis-9.0.0/mimesis/data/it/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/it/text.json` & `mimesis-9.0.0/mimesis/data/it/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ja/address.json` & `mimesis-9.0.0/mimesis/data/ja/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ja/finance.json` & `mimesis-9.0.0/mimesis/data/ja/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ja/food.json` & `mimesis-9.0.0/mimesis/data/ja/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ja/person.json` & `mimesis-9.0.0/mimesis/data/ja/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ja/text.json` & `mimesis-9.0.0/mimesis/data/ja/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/kk/address.json` & `mimesis-9.0.0/mimesis/data/kk/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/kk/datetime.json` & `mimesis-9.0.0/mimesis/data/kk/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/kk/finance.json` & `mimesis-9.0.0/mimesis/data/kk/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/kk/person.json` & `mimesis-9.0.0/mimesis/data/kk/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/kk/text.json` & `mimesis-9.0.0/mimesis/data/kk/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ko/address.json` & `mimesis-9.0.0/mimesis/data/ko/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ko/finance.json` & `mimesis-9.0.0/mimesis/data/ko/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ko/food.json` & `mimesis-9.0.0/mimesis/data/ko/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ko/person.json` & `mimesis-9.0.0/mimesis/data/ko/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ko/text.json` & `mimesis-9.0.0/mimesis/data/ko/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/nl/address.json` & `mimesis-9.0.0/mimesis/data/nl/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/nl/finance.json` & `mimesis-9.0.0/mimesis/data/nl/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/nl/food.json` & `mimesis-9.0.0/mimesis/data/nl/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/nl/person.json` & `mimesis-9.0.0/mimesis/data/nl/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/nl/text.json` & `mimesis-9.0.0/mimesis/data/nl/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/nl-be/address.json` & `mimesis-9.0.0/mimesis/data/nl-be/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/nl-be/finance.json` & `mimesis-9.0.0/mimesis/data/nl-be/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/nl-be/person.json` & `mimesis-9.0.0/mimesis/data/nl-be/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/no/address.json` & `mimesis-9.0.0/mimesis/data/no/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/no/finance.json` & `mimesis-9.0.0/mimesis/data/no/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/no/food.json` & `mimesis-9.0.0/mimesis/data/no/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/no/person.json` & `mimesis-9.0.0/mimesis/data/no/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/no/text.json` & `mimesis-9.0.0/mimesis/data/no/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pl/address.json` & `mimesis-9.0.0/mimesis/data/pl/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pl/datetime.json` & `mimesis-9.0.0/mimesis/data/pl/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pl/finance.json` & `mimesis-9.0.0/mimesis/data/pl/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pl/food.json` & `mimesis-9.0.0/mimesis/data/pl/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pl/person.json` & `mimesis-9.0.0/mimesis/data/pl/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pl/text.json` & `mimesis-9.0.0/mimesis/data/pl/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt/address.json` & `mimesis-9.0.0/mimesis/data/pt/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt/datetime.json` & `mimesis-9.0.0/mimesis/data/pt/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt/finance.json` & `mimesis-9.0.0/mimesis/data/pt/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt/food.json` & `mimesis-9.0.0/mimesis/data/pt/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt/person.json` & `mimesis-9.0.0/mimesis/data/pt/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt/text.json` & `mimesis-9.0.0/mimesis/data/pt/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt-br/address.json` & `mimesis-9.0.0/mimesis/data/pt-br/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt-br/datetime.json` & `mimesis-9.0.0/mimesis/data/pt-br/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt-br/finance.json` & `mimesis-9.0.0/mimesis/data/pt-br/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt-br/food.json` & `mimesis-9.0.0/mimesis/data/pt-br/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/pt-br/person.json` & `mimesis-9.0.0/mimesis/data/pt-br/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ru/address.json` & `mimesis-9.0.0/mimesis/data/ru/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ru/builtin.json` & `mimesis-9.0.0/mimesis/data/ru/builtin.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ru/datetime.json` & `mimesis-9.0.0/mimesis/data/ru/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ru/finance.json` & `mimesis-9.0.0/mimesis/data/ru/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ru/food.json` & `mimesis-9.0.0/mimesis/data/ru/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ru/person.json` & `mimesis-9.0.0/mimesis/data/ru/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/ru/text.json` & `mimesis-9.0.0/mimesis/data/ru/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/sk/address.json` & `mimesis-9.0.0/mimesis/data/sk/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/sk/finance.json` & `mimesis-9.0.0/mimesis/data/sk/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/sk/person.json` & `mimesis-9.0.0/mimesis/data/sk/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/sk/text.json` & `mimesis-9.0.0/mimesis/data/sk/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/sv/address.json` & `mimesis-9.0.0/mimesis/data/sv/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/sv/finance.json` & `mimesis-9.0.0/mimesis/data/sv/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/sv/food.json` & `mimesis-9.0.0/mimesis/data/sv/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/sv/person.json` & `mimesis-9.0.0/mimesis/data/sv/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/sv/text.json` & `mimesis-9.0.0/mimesis/data/sv/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/tr/address.json` & `mimesis-9.0.0/mimesis/data/tr/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/tr/finance.json` & `mimesis-9.0.0/mimesis/data/tr/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/tr/food.json` & `mimesis-9.0.0/mimesis/data/tr/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/tr/person.json` & `mimesis-9.0.0/mimesis/data/tr/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/tr/text.json` & `mimesis-9.0.0/mimesis/data/tr/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/uk/address.json` & `mimesis-9.0.0/mimesis/data/uk/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/uk/builtin.json` & `mimesis-9.0.0/mimesis/data/uk/builtin.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/uk/datetime.json` & `mimesis-9.0.0/mimesis/data/uk/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/uk/finance.json` & `mimesis-9.0.0/mimesis/data/uk/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/uk/food.json` & `mimesis-9.0.0/mimesis/data/uk/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/uk/person.json` & `mimesis-9.0.0/mimesis/data/uk/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/uk/text.json` & `mimesis-9.0.0/mimesis/data/uk/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/zh/address.json` & `mimesis-9.0.0/mimesis/data/zh/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/zh/datetime.json` & `mimesis-9.0.0/mimesis/data/zh/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/zh/finance.json` & `mimesis-9.0.0/mimesis/data/zh/finance.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/zh/food.json` & `mimesis-9.0.0/mimesis/data/zh/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/zh/person.json` & `mimesis-9.0.0/mimesis/data/zh/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/data/zh/text.json` & `mimesis-9.0.0/mimesis/data/zh/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/enums.py` & `mimesis-9.0.0/mimesis/enums.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/exceptions.py` & `mimesis-9.0.0/mimesis/exceptions.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/__init__.py` & `mimesis-9.0.0/mimesis/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/address.py` & `mimesis-9.0.0/mimesis/providers/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,44 +70,44 @@
         return str(self.random.randint(1, maximum))
 
     def street_name(self) -> str:
         """Get a random street name.
 
         :return: Street name.
         """
-        street_names: t.List[str] = self.extract(["street", "name"])
+        street_names: t.List[str] = self._extract(["street", "name"])
         return self.random.choice(street_names)
 
     def street_suffix(self) -> str:
         """Get a random street suffix.
 
         :return: Street suffix.
         """
-        suffixes: t.List[str] = self.extract(["street", "suffix"])
+        suffixes: t.List[str] = self._extract(["street", "suffix"])
         return self.random.choice(suffixes)
 
     def address(self) -> str:
         """Generate a random full address.
 
         :return: Full address.
         """
-        fmt: str = self.extract(["address_fmt"])
+        fmt: str = self._extract(["address_fmt"])
 
         st_num = self.street_number()
         st_name = self.street_name()
 
         if self.locale in SHORTENED_ADDRESS_FMT:
             return fmt.format(
                 st_num=st_num,
                 st_name=st_name,
             )
 
         if self.locale == "ja":
             return fmt.format(
-                self.random.choice(self.extract(["city"])),
+                self.random.choice(self._extract(["city"])),
                 # Generate list of random integers
                 # in amount of 3, from 1 to 100.
                 *self.random.randints(amount=3, a=1, b=100),
             )
 
         return fmt.format(
             st_num=st_num,
@@ -118,15 +118,15 @@
     def state(self, abbr: bool = False) -> str:
         """Get a random administrative district of country.
 
         :param abbr: Return ISO 3166-2 code.
         :return: Administrative district.
         """
         key = "abbr" if abbr else "name"
-        states: t.List[str] = self.extract(["state", key])
+        states: t.List[str] = self._extract(["state", key])
         return self.random.choice(states)
 
     def region(self, *args: t.Any, **kwargs: t.Any) -> str:
         """Get a random region.
 
         An alias for :meth:`~Address.state()`.
         """
@@ -154,15 +154,15 @@
         return self.state(*args, **kwargs)
 
     def postal_code(self) -> str:
         """Generate a postal code for current locale.
 
         :return: Postal code.
         """
-        return self.random.custom_code(self.extract(["postal_code_fmt"]))
+        return self.random.custom_code(self._extract(["postal_code_fmt"]))
 
     def zip_code(self) -> str:
         """Generate a zip code.
 
         An alias for :meth:`~Address.postal_code()`.
 
         :return: Zip code.
@@ -184,31 +184,31 @@
         return self.random.choice(COUNTRY_CODES[key])
 
     def default_country(self) -> str:
         """Get the country associated with the current locale.
 
         :return: The country associated with current locale.
         """
-        country: str = self.extract(["country", "current_locale"])
+        country: str = self._extract(["country", "current_locale"])
         return country
 
     def country(self) -> str:
         """Get a random country.
 
         :return: The Country.
         """
-        countries: t.List[str] = self.extract(["country", "name"])
+        countries: t.List[str] = self._extract(["country", "name"])
         return self.random.choice(countries)
 
     def city(self) -> str:
         """Get a random city.
 
         :return: City name.
         """
-        cities: t.List[str] = self.extract(["city"])
+        cities: t.List[str] = self._extract(["city"])
         return self.random.choice(cities)
 
     def _get_fs(self, key: str, dms: bool = False) -> t.Union[str, float]:
         """Get float number.
 
         :param key: Key (`lt` or `lg`).
         :param dms: DMS format.
@@ -252,15 +252,15 @@
 
     def continent(self, code: bool = False) -> str:
         """Get a random continent name or continent code.
 
         :param code: Return code of continent.
         :return: Continent name.
         """
-        codes: t.List[str] = self.extract(["continent"])
+        codes: t.List[str] = self._extract(["continent"])
 
         if code:
             codes = CONTINENT_CODES
 
         return self.random.choice(codes)
 
     def calling_code(self) -> str:
```

### Comparing `mimesis-8.0.0/mimesis/providers/base.py` & `mimesis-9.0.0/mimesis/providers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 from mimesis.locales import Locale, validate_locale
 from mimesis.types import JSON, MissingSeed, Seed
 
 __all__ = ["BaseDataProvider", "BaseProvider"]
 
 
 class BaseProvider:
-    """This is a base class for all providers."""
+    """This is a base class for all providers.
+
+
+    :attr: random: Instance of :class:`mimesis.random.Random`.
+    """
 
     class Meta:
         name: str
 
     def __init__(
         self,
         *,
@@ -71,15 +75,15 @@
 
         :param item: Item of enum object.
         :param enum: Enum object.
         :return: Value of item.
         :raises NonEnumerableError: if ``item`` not in ``enum``.
         """
         if item is None:
-            result = _random.get_random_item(enum, self.random)
+            result = self.random.choice_enum_item(enum)
         elif item and isinstance(item, enum):
             result = item
         else:
             raise NonEnumerableError(enum)
 
         return result.value
 
@@ -122,22 +126,21 @@
         :raises UnsupportedLocale: When locale not supported.
         :return: Nothing.
         """
 
         locale_obj = validate_locale(locale)
         self.locale = locale_obj.value
 
-    def extract(self, keys: t.List[str], default: t.Optional[t.Any] = None) -> t.Any:
+    def _extract(self, keys: t.List[str], default: t.Optional[t.Any] = None) -> t.Any:
         """Extracts nested values from JSON file by list of keys.
 
         :param keys: List of keys (order extremely matters).
         :param default: Default value.
         :return: Data.
         """
-
         if not keys:
             raise ValueError("The list of keys to extract cannot be empty.")
         try:
             return reduce(operator.getitem, keys, self._data)
         except (TypeError, KeyError):
             return default
```

### Comparing `mimesis-8.0.0/mimesis/providers/binaryfile.py` & `mimesis-9.0.0/mimesis/providers/binaryfile.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/choice.py` & `mimesis-9.0.0/mimesis/providers/choice.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/code.py` & `mimesis-9.0.0/mimesis/providers/code.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/cryptographic.py` & `mimesis-9.0.0/mimesis/providers/cryptographic.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/date.py` & `mimesis-9.0.0/mimesis/providers/date.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,25 +98,25 @@
     def day_of_week(self, abbr: bool = False) -> str:
         """Get a random day of week.
 
         :param abbr: Abbreviated day name.
         :return: Day of the week.
         """
         key = "abbr" if abbr else "name"
-        days: t.List[str] = self.extract(["day", key])
+        days: t.List[str] = self._extract(["day", key])
         return self.random.choice(days)
 
     def month(self, abbr: bool = False) -> str:
         """Get a random month.
 
         :param abbr: Abbreviated month name.
         :return: Month name.
         """
         key = "abbr" if abbr else "name"
-        months: t.List[str] = self.extract(["month", key])
+        months: t.List[str] = self._extract(["month", key])
         return self.random.choice(months)
 
     def year(self, minimum: int = 1990, maximum: int = _CURRENT_YEAR) -> int:
         """Generate a random year.
 
         :param minimum: Minimum value.
         :param maximum: Maximum value.
@@ -132,15 +132,15 @@
         return self.random.choice(ROMAN_NUMS)
 
     def periodicity(self) -> str:
         """Get a random periodicity string.
 
         :return: Periodicity.
         """
-        periodicity: t.List[str] = self.extract(["periodicity"])
+        periodicity: t.List[str] = self._extract(["periodicity"])
         return self.random.choice(periodicity)
 
     def date(self, start: int = 2000, end: int = _CURRENT_YEAR) -> Date:
         """Generate random date object.
 
         :param start: Minimum value of year.
         :param end: Maximum value of year.
@@ -159,15 +159,15 @@
             accepted in the current locale.
         :param kwargs: Keyword arguments for :meth:`~Datetime.date()`
         :return: Formatted date.
         """
         date_obj = self.date(**kwargs)
 
         if not fmt:
-            fmt = self.extract(["formats", "date"])
+            fmt = self._extract(["formats", "date"])
 
         return date_obj.strftime(fmt)
 
     def time(self) -> Time:
         """Generate a random time object.
 
         :return: ``datetime.time`` object.
@@ -186,15 +186,15 @@
         :param fmt: The format of time, if None then use standard
             accepted in the current locale.
         :return: String formatted time.
         """
         time_obj = self.time()
 
         if not fmt:
-            fmt = self.extract(["formats", "time"])
+            fmt = self._extract(["formats", "time"])
         return time_obj.strftime(fmt)
 
     def day_of_month(self) -> int:
         """Generate a random day of month, from 1 to 31.
 
         :return: Random value from 1 to 31.
         """
@@ -249,16 +249,16 @@
         :param fmt: Custom format (default is format for current locale)
         :param kwargs: Keyword arguments for :meth:`~Datetime.datetime()`
         :return: Formatted datetime string.
         """
         dt_obj = self.datetime(**kwargs)
 
         if not fmt:
-            date_fmt = self.extract(["formats", "date"])
-            time_fmt = self.extract(["formats", "time"])
+            date_fmt = self._extract(["formats", "date"])
+            time_fmt = self._extract(["formats", "time"])
             fmt = f"{date_fmt} {time_fmt}"
 
         return dt_obj.strftime(fmt)
 
     def timestamp(self, posix: bool = True, **kwargs: t.Any) -> t.Union[str, int]:
         """Generate random timestamp.
```

### Comparing `mimesis-8.0.0/mimesis/providers/development.py` & `mimesis-9.0.0/mimesis/providers/development.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/file.py` & `mimesis-9.0.0/mimesis/providers/file.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/finance.py` & `mimesis-9.0.0/mimesis/providers/finance.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,47 +34,47 @@
         name: t.Final[str] = "finance"
 
     def company(self) -> str:
         """Get a random company name.
 
         :return: Company name.
         """
-        names: t.List[str] = self.extract(["company", "name"])
+        names: t.List[str] = self._extract(["company", "name"])
 
         return self.random.choice(names)
 
     def company_type(self, abbr: bool = False) -> str:
         """Get a random type of business entity.
 
         :param abbr: Abbreviated company type.
         :return: Types of business entity.
         """
         key = "abbr" if abbr else "title"
 
-        company_types: t.List[str] = self.extract(["company", "type", key])
+        company_types: t.List[str] = self._extract(["company", "type", key])
         return self.random.choice(company_types)
 
     def currency_iso_code(self, allow_random: bool = False) -> str:
         """Get code of the currency for current locale.
 
         :param allow_random: Get a random ISO code.
         :return: Currency code.
         """
-        code: str = self.extract(["currency-code"])
+        code: str = self._extract(["currency-code"])
 
         if allow_random:
             return self.random.choice(CURRENCY_ISO_CODES)
         return code
 
     def bank(self) -> str:
         """Get a random bank name.
 
         :return: Bank name.
         """
-        banks: t.List[str] = self.extract(["banks"])
+        banks: t.List[str] = self._extract(["banks"])
         return self.random.choice(banks)
 
     def cryptocurrency_iso_code(self) -> str:
         """Get symbol of random cryptocurrency.
 
         :return: Symbol of cryptocurrency.
         """
```

### Comparing `mimesis-8.0.0/mimesis/providers/food.py` & `mimesis-9.0.0/mimesis/providers/food.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     class Meta:
         """Class for metadata."""
 
         name: t.Final[str] = "food"
 
     def _choice_from(self, key: str) -> str:
         """Choice random element."""
-        data: t.List[str] = self.extract([key])
+        data: t.List[str] = self._extract([key])
         return self.random.choice(data)
 
     def vegetable(self) -> str:
         """Get a random vegetable.
 
         :return: Vegetable name.
```

### Comparing `mimesis-8.0.0/mimesis/providers/generic.py` & `mimesis-9.0.0/mimesis/providers/generic.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/hardware.py` & `mimesis-9.0.0/mimesis/providers/hardware.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/internet.py` & `mimesis-9.0.0/mimesis/providers/internet.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/numeric.py` & `mimesis-9.0.0/mimesis/providers/numeric.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/path.py` & `mimesis-9.0.0/mimesis/providers/path.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/providers/payment.py` & `mimesis-9.0.0/mimesis/providers/payment.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from mimesis.data import CREDIT_CARD_NETWORKS
 from mimesis.enums import CardType, Gender
 from mimesis.exceptions import NonEnumerableError
 from mimesis.locales import Locale
 from mimesis.providers.base import BaseProvider
 from mimesis.providers.person import Person
-from mimesis.random import get_random_item
 from mimesis.shortcuts import luhn_checksum
 
 __all__ = ["Payment"]
 
 
 class Payment(BaseProvider):
     """Class that provides data related to payments."""
@@ -107,15 +106,15 @@
         :Example:
             4455 5299 1152 2450
         """
         length = 16
         regex = re.compile(r"(\d{4})(\d{4})(\d{4})(\d{4})")
 
         if card_type is None:
-            card_type = get_random_item(CardType, rnd=self.random)
+            card_type = self.random.choice_enum_item(CardType)
 
         if card_type == CardType.VISA:
             number = self.random.randint(4000, 4999)
         elif card_type == CardType.MASTER_CARD:
             number = self.random.choice(
                 [
                     self.random.randint(2221, 2720),
```

### Comparing `mimesis-8.0.0/mimesis/providers/person.py` & `mimesis-9.0.0/mimesis/providers/person.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,15 @@
     BLOOD_GROUPS,
     CALLING_CODES,
     EMAIL_DOMAINS,
     GENDER_SYMBOLS,
     USERNAMES,
 )
 from mimesis.enums import Gender, TitleType
-from mimesis.exceptions import NonEnumerableError
 from mimesis.providers.base import BaseDataProvider
-from mimesis.random import get_random_item
 
 __all__ = ["Person"]
 
 
 class Person(BaseDataProvider):
     """Class for generating personal data."""
 
@@ -73,15 +71,15 @@
         :param gender: Gender's enum object.
         :return: Name.
 
         :Example:
             John.
         """
         key = self.validate_enum(gender, Gender)
-        names: t.List[str] = self.extract(["names", key])
+        names: t.List[str] = self._extract(["names", key])
         return self.random.choice(names)
 
     def first_name(self, gender: t.Optional[Gender] = None) -> str:
         """Generate a random first name.
 
         ..note: An alias for self.name().
 
@@ -95,15 +93,15 @@
 
         :param gender: Gender's enum object.
         :return: Surname.
 
         :Example:
             Smith.
         """
-        surnames: t.Sequence[str] = self.extract(["surnames"])
+        surnames: t.Sequence[str] = self._extract(["surnames"])
 
         # Surnames separated by gender.
         if isinstance(surnames, dict):
             key = self.validate_enum(gender, Gender)
             surnames = surnames[key]
 
         return self.random.choice(surnames)
@@ -135,37 +133,29 @@
 
         :Example:
             PhD.
         """
         gender_key = self.validate_enum(gender, Gender)
         title_key = self.validate_enum(title_type, TitleType)
 
-        titles: t.List[str] = self.extract(["title", gender_key, title_key])
+        titles: t.List[str] = self._extract(["title", gender_key, title_key])
         return self.random.choice(titles)
 
     def full_name(
         self, gender: t.Optional[Gender] = None, reverse: bool = False
     ) -> str:
         """Generate a random full name.
 
         :param reverse: Return reversed full name.
         :param gender: Gender's enum object.
         :return: Full name.
 
         :Example:
             Johann Wolfgang.
         """
-        if gender is None:
-            gender = get_random_item(Gender, rnd=self.random)
-
-        if gender and isinstance(gender, Gender):
-            gender = gender
-        else:
-            raise NonEnumerableError(Gender)
-
         name = self.name(gender)
         surname = self.surname(gender)
         return f"{surname} {name}" if reverse else f"{name} {surname}"
 
     def username(
         self, mask: t.Optional[str] = None, drange: t.Tuple[int, int] = (1800, 2100)
     ) -> str:
@@ -269,15 +259,15 @@
 
         domain = self.random.choice(domains)
 
         if not domain.startswith("@"):
             domain = "@" + domain
 
         if unique:
-            name = self.random.randstr(unique)
+            name = self.random._randstr(unique)
         else:
             name = self.username(mask="ld")
 
         return f"{name}{domain}"
 
     def gender(self, iso5218: bool = False, symbol: bool = False) -> t.Union[str, int]:
         """Get a random gender.
@@ -298,15 +288,15 @@
         """
         if iso5218:
             return self.random.choice([0, 1, 2, 9])
 
         if symbol:
             return self.random.choice(GENDER_SYMBOLS)
 
-        genders: t.List[str] = self.extract(["gender"])
+        genders: t.List[str] = self._extract(["gender"])
         return self.random.choice(genders)
 
     def sex(self, *args: t.Any, **kwargs: t.Any) -> t.Union[str, int]:
         """An alias for method self.gender().
 
         See docstrings of method self.gender() for details.
 
@@ -355,60 +345,60 @@
         """Get a random job.
 
         :return: The name of job.
 
         :Example:
             Programmer.
         """
-        jobs: t.List[str] = self.extract(["occupation"])
+        jobs: t.List[str] = self._extract(["occupation"])
         return self.random.choice(jobs)
 
     def political_views(self) -> str:
         """Get a random political views.
 
         :return: Political views.
 
         :Example:
             Liberal.
         """
-        views: t.List[str] = self.extract(["political_views"])
+        views: t.List[str] = self._extract(["political_views"])
         return self.random.choice(views)
 
     def worldview(self) -> str:
         """Get a random worldview.
 
         :return: Worldview.
 
         :Example:
             Pantheism.
         """
-        views: t.List[str] = self.extract(["worldview"])
+        views: t.List[str] = self._extract(["worldview"])
         return self.random.choice(views)
 
     def views_on(self) -> str:
         """Get a random views on.
 
         :return: Views on.
 
         :Example:
             Negative.
         """
-        views: t.List[str] = self.extract(["views_on"])
+        views: t.List[str] = self._extract(["views_on"])
         return self.random.choice(views)
 
     def nationality(self, gender: t.Optional[Gender] = None) -> str:
         """Get a random nationality.
 
         :param gender: Gender.
         :return: Nationality.
 
         :Example:
             Russian
         """
-        nationalities: t.List[str] = self.extract(["nationality"])
+        nationalities: t.List[str] = self._extract(["nationality"])
 
         # Separated by gender
         if isinstance(nationalities, dict):
             key = self.validate_enum(gender, Gender)
             nationalities = nationalities[key]
 
         return self.random.choice(nationalities)
@@ -417,37 +407,37 @@
         """Get a random university.
 
         :return: University name.
 
         :Example:
             MIT.
         """
-        universities: t.List[str] = self.extract(["university"])
+        universities: t.List[str] = self._extract(["university"])
         return self.random.choice(universities)
 
     def academic_degree(self) -> str:
         """Get a random academic degree.
 
         :return: Degree.
 
         :Example:
             Bachelor.
         """
-        degrees: t.List[str] = self.extract(["academic_degree"])
+        degrees: t.List[str] = self._extract(["academic_degree"])
         return self.random.choice(degrees)
 
     def language(self) -> str:
         """Get a random language.
 
         :return: Random language.
 
         :Example:
             Irish.
         """
-        languages: t.List[str] = self.extract(["language"])
+        languages: t.List[str] = self._extract(["language"])
         return self.random.choice(languages)
 
     def phone_number(self, mask: str = "", placeholder: str = "#") -> str:
         """Generate a random phone number.
 
         :param mask: Mask for formatting number.
         :param placeholder: A placeholder for a mask (default is #).
@@ -455,15 +445,15 @@
 
         :Example:
             +7-(963)-409-11-22.
         """
         if not mask:
             code = self.random.choice(CALLING_CODES)
             default = f"{code}-(###)-###-####"
-            masks = self.extract(["telephone_fmt"], default=[default])
+            masks = self._extract(["telephone_fmt"], default=[default])
             mask = self.random.choice(masks)
 
         return self.random.custom_code(mask=mask, digit=placeholder)
 
     def telephone(self, *args: t.Any, **kwargs: t.Any) -> str:
         return self.phone_number(*args, **kwargs)
```

### Comparing `mimesis-8.0.0/mimesis/providers/science.py` & `mimesis-9.0.0/mimesis/providers/science.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 
         :param length: Length of block.
         :return: RNA sequence.
 
         :Example:
             AGUGACACAA
         """
-        return self.random.generate_string("UCGA", length)
+        return self.random._generate_string("UCGA", length)
 
     def dna_sequence(self, length: int = 10) -> str:
         """Generate a random DNA sequence.
 
         :param length: Length of block.
         :return: DNA sequence.
 
         :Example:
             GCTTTAGACC
         """
-        return self.random.generate_string("TCGA", length)
+        return self.random._generate_string("TCGA", length)
 
     def measure_unit(
         self,
         name: t.Optional[MeasureUnit] = None,
         symbol: bool = False,
     ) -> str:
         """Get unit name from International System of Units.
```

### Comparing `mimesis-8.0.0/mimesis/providers/text.py` & `mimesis-9.0.0/mimesis/providers/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,35 +30,35 @@
         """Get an alphabet for current locale.
 
         :param lower_case: Return alphabet in lower case.
         :return: Alphabet.
         """
         case = "uppercase" if not lower_case else "lowercase"
 
-        alpha: t.List[str] = self.extract(["alphabet", case])
+        alpha: t.List[str] = self._extract(["alphabet", case])
         return alpha
 
     def level(self) -> str:
         """Generate a random level of danger or something else.
 
         :return: Level.
 
         :Example:
             critical.
         """
-        levels: t.List[str] = self.extract(["level"])
+        levels: t.List[str] = self._extract(["level"])
         return self.random.choice(levels)
 
     def text(self, quantity: int = 5) -> str:
         """Generate the text.
 
         :param quantity: Quantity of sentences.
         :return: Text.
         """
-        text = self.extract(["text"])
+        text = self._extract(["text"])
         return " ".join(self.random.choices(text, k=quantity))
 
     def sentence(self) -> str:
         """Get a random sentence from text.
 
         :return: Sentence.
         """
@@ -76,15 +76,15 @@
 
         :param quantity: Quantity of words. Default is 5.
         :return: Word list.
 
         :Example:
             [science, network, god, octopus, love]
         """
-        words = self.extract(["words", "normal"])
+        words = self._extract(["words", "normal"])
         return self.random.choices(words, k=quantity)
 
     def word(self) -> str:
         """Get a random word.
 
         :return: Single word.
 
@@ -97,37 +97,37 @@
         """Get a random swear word.
 
         :return: Swear word.
 
         :Example:
             Damn.
         """
-        words: t.List[str] = self.extract(["words", "bad"])
+        words: t.List[str] = self._extract(["words", "bad"])
         return self.random.choice(words)
 
     def quote(self) -> str:
         """Get a random quote.
 
         :return: Quote from movie.
 
         :Example:
             "Bond... James Bond."
         """
-        quotes: t.List[str] = self.extract(["quotes"])
+        quotes: t.List[str] = self._extract(["quotes"])
         return self.random.choice(quotes)
 
     def color(self) -> str:
         """Get a random name of color.
 
         :return: Color name.
 
         :Example:
             Red.
         """
-        colors: t.List[str] = self.extract(["color"])
+        colors: t.List[str] = self._extract(["color"])
         return self.random.choice(colors)
 
     @staticmethod
     def _hex_to_rgb(color: str) -> t.Tuple[int, ...]:
         """Convert hex color to RGB format.
 
         :param color: Hex color.
@@ -167,9 +167,9 @@
         """Get a random answer in current language.
 
         :return: An answer.
 
         :Example:
             No
         """
-        answers: t.List[str] = self.extract(["answers"])
+        answers: t.List[str] = self._extract(["answers"])
         return self.random.choice(answers)
```

### Comparing `mimesis-8.0.0/mimesis/providers/transport.py` & `mimesis-9.0.0/mimesis/providers/transport.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/random.py` & `mimesis-9.0.0/mimesis/random.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 import random as random_module
 import string
 import typing as t
 import uuid
 
 from mimesis.types import MissingSeed, Seed
 
-__all__ = ["Random", "get_random_item", "random"]
+__all__ = ["Random", "random"]
 
 #: Different plugins (like `pytest-randomly`)
 #: can set custom values to a global seed,
 #: which are going to be the new default.
 global_seed: Seed = MissingSeed
 
 
 class Random(random_module.Random):
-    """Custom class for the possibility of extending.
+    """A custom random class.
 
-    The class is a subclass of the class :py:class:`random.Random`
-    from the module random of the standard library, which provides the custom methods.
+    This is a class that can be extended as needed.
+
+    It's a subclass of the random.Random class from the random
+    module in the standard library. The class includes additional
+    custom methods.
     """
 
     def randints(self, amount: int = 3, a: int = 1, b: int = 100) -> t.List[int]:
         """Generate list of random integers.
 
         :param amount: Amount of elements.
         :param a: Minimum value of range.
@@ -37,15 +40,15 @@
         :raises ValueError: if amount less or equal to zero.
         """
         if amount <= 0:
             raise ValueError("Amount out of range.")
 
         return [int(self.random() * (b - a)) + a for _ in range(amount)]
 
-    def generate_string(self, str_seq: str, length: int = 10) -> str:
+    def _generate_string(self, str_seq: str, length: int = 10) -> str:
         """Generate random string created from string sequence.
 
         :param str_seq: String sequence of letters or digits.
         :param length: Max value.
         :return: Single string.
         """
         return "".join(self.choices(str_seq, k=length))
@@ -59,15 +62,16 @@
         :return: Custom code.
         """
         char_code = ord(char)
         digit_code = ord(digit)
 
         if char_code == digit_code:
             raise ValueError(
-                "You cannot use the same placeholder for digits and chars!"
+                "The same placeholder cannot be "
+                "used for both numbers and characters."
             )
 
         def random_int(a: int, b: int) -> int:
             b = b - a
             return int(self.random() * b) + a
 
         _mask = mask.encode()
@@ -88,15 +92,15 @@
         :param a: Minimum value.
         :param b: Maximum value.
         :param precision: Round a number to a given
             precision in decimal digits, default is 15.
         """
         return round(a + (b - a) * self.random(), precision)
 
-    def randstr(self, unique: bool = False, length: t.Optional[int] = None) -> str:
+    def _randstr(self, unique: bool = False, length: t.Optional[int] = None) -> str:
         """Generate random string value.
 
         This method can be especially useful when you need to generate
         only unique values in your provider. Just pass parameter unique=True.
 
         Basically, this method is just a simple wrapper around :py:class:`uuid.UUID`.
 
@@ -114,23 +118,33 @@
         characters = string.ascii_letters + string.digits
         return "".join(self.choices(characters, k=length))
 
     def randbytes(self, n: int = 16) -> bytes:
         """Generate n random bytes."""
         return self.getrandbits(n * 8).to_bytes(n, "little")
 
+    def weighted_choice(self, choices: t.Dict[t.Any, float]) -> t.Any:
+        """Returns a random element according to the specified weights.
 
-def get_random_item(enum: t.Any, rnd: t.Optional[Random] = None) -> t.Any:
-    """Get random item of enum object.
+        :param choices: A dictionary where keys are choices and values are weights.
+        :raises ValueError: if choices is empty.
+        :return: Random key from dictionary.
+        """
+        if not choices:
+            raise ValueError("Choices cannot be empty.")
 
-    :param enum: Enum object.
-    :param rnd: Custom random object.
-    :return: Random item of enum.
-    """
-    if rnd and isinstance(rnd, Random):
-        return rnd.choice(list(enum))
-    return random_module.choice(list(enum))
+        population = list(choices.keys())
+        weights = list(choices.values())
+        return self.choices(population, weights=weights, k=1)[0]
+
+    def choice_enum_item(self, enum: t.Any) -> t.Any:
+        """Get random value of enum object.
+
+        :param enum: Enum object.
+        :return: Random value of enum.
+        """
+        return self.choice(list(enum))
 
 
 # Compat
 # See: https://github.com/lk-geimfari/mimesis/issues/469
 random = Random()
```

### Comparing `mimesis-8.0.0/mimesis/schema.py` & `mimesis-9.0.0/mimesis/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Implements classes for generating data by schema."""
 
 import csv
 import json
 import pickle
 import re
 import typing as t
-import warnings
 
 from mimesis.exceptions import FieldError, FieldsetError, SchemaError
 from mimesis.locales import Locale
 from mimesis.providers.base import BaseProvider
 from mimesis.providers.generic import Generic
 from mimesis.types import (
     JSON,
@@ -130,29 +129,37 @@
             - ``provider/name``
             - ``provider name``
 
         You can apply a *key function* to the result returned by
         the method, by passing a parameter **key** with a callable
         object which returns the final result.
 
+        The key function has the option to accept two parameters: **result** and **random**.
+        In case you require access to a random instance within the key function,
+        you must modify the function to accept both of them, where the first corresponds
+        to the method result and the second corresponds to the instance of random.
+
         :param name: Name of the method.
-        :param key: A key function (or any other callable object)
-            which will be applied to result.
+        :param key: A key function (any other callable object) which will be applied to result.
         :param kwargs: Kwargs of method.
         :return: Value which represented by method.
-        :raises ValueError: if provider not
-            supported or if field not defined.
+        :raises ValueError: if provider not supported or if field not defined.
         """
         if name is None:
             raise FieldError()
 
         result = self._lookup_method(name)(**kwargs)
 
         if key and callable(key):
-            return key(result)
+            try:
+                # If key function accepts two parameters
+                # then pass random instance to it.
+                return key(result, self._gen.random)  # type: ignore
+            except TypeError:
+                return key(result)
 
         return result
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__} <{self._gen.locale}>"
 
 
@@ -250,191 +257,96 @@
 
         return [self.perform(*args, **kwargs) for _ in range(iterations)]
 
 
 class Schema:
     """Class which return list of filled schemas."""
 
-    _MIN_ITERATIONS_VALUE: t.ClassVar[int] = 1
-
-    __slots__ = ("_schema",)
+    __slots__ = (
+        "_count",
+        "_schema",
+        "iterations",
+        "_min_iterations",
+    )
 
-    def __init__(self, schema: CallableSchema) -> None:
+    def __init__(self, schema: CallableSchema, iterations: int = 10) -> None:
         """Initialize schema.
 
+        :param iterations: Number of iterations.
+            This parameter is keyword-only. The default value is 10.
         :param schema: A schema (must be a callable object).
         """
         if schema and callable(schema):  # type: ignore[truthy-function]
             self._schema = schema
+            self._count = 0
+            self._min_iterations = 1
+            if iterations >= self._min_iterations:
+                self.iterations = iterations
+            else:
+                raise ValueError(
+                    f"Iterations must be greater than {self._min_iterations}"
+                )
         else:
             # This is just a better error message
             raise SchemaError()
 
-    def __mul__(self, other: int) -> t.List[JSON]:
-        """Multiplies the schema by the number of iterations.
-
-        Schema multiplication is not lazy, so it will be performed immediately (in fact,
-        you're using :meth:`~mimesis.schema.Schema.create` under the hood).
-
-        .. warning::
-
-            Multiplying the large and nested schema with a large number is obviously
-            a `stupid`_ idea, so **be reasonable** on choosing a multiplier.
-
-            .. _stupid: https://dictionary.cambridge.org/dictionary/english/stupid
-
-        Usage:
-
-        .. code-block:: python
-
-            schema = Schema(lambda: {
-                'email': _('username'),
-                'token': _('token_hex', key=lambda x: x[:8])
-            })
-            print(schema * 2)
-            print(2 * schema)
-
-        .. note::
-
-            Keep in mind the priority and order of multipliers.
-
-            Instead of doing this:
-
-            >>> schema * 2 * 10
-
-            Where you evaluate the schema 2 times and then multiply the resulting list 10 times, you should do this:
-
-            >>> schema * (2 * 10) # Evaluates the schema 20 times.
-
-            In other words, the first multiplier evaluetes the schema:
-
-            >>> 1 * schema * 3
-
-            The result will be:
-
-            .. code-block:: json
-
-                [
-                    {"email": "efforts1859@test.com", "token": "f4a29754"},
-                    {"email": "efforts1859@test.com", "token": "f4a29754"},
-                    {"email": "efforts1859@test.com", "token": "f4a29754"},
-                ]
-
-            Because schema is evaluated first (`1 * schema`), and then the second multiplier is
-            applied on the result of the first expression since.
-
-        :param other: The multiplier.
-        """
-        return self.create(other)
-
-    def __rmul__(self, other: int) -> t.List[JSON]:
-        return self.__mul__(other)
-
-    def to_csv(self, file_path: str, iterations: int = 100, **kwargs: t.Any) -> None:
+    def to_csv(self, file_path: str, **kwargs: t.Any) -> None:
         """Export a schema as a CSV file.
 
         :param file_path: File path.
-        :param iterations: The required number of rows.
         :param kwargs: The keyword arguments for :py:class:`csv.DictWriter` class.
 
         *New in version 5.3.0*
         """
-        data = self.create(iterations)
-        fieldnames = list(data[0])
-
+        data = self.create()
         with open(file_path, "w", encoding="utf-8", newline="") as fp:
+            fieldnames = list(data[0])
             dict_writer = csv.DictWriter(fp, fieldnames, **kwargs)
             dict_writer.writeheader()
             dict_writer.writerows(data)
 
-    def to_json(self, file_path: str, iterations: int = 100, **kwargs: t.Any) -> None:
+    def to_json(self, file_path: str, **kwargs: t.Any) -> None:
         """Export a schema as a JSON file.
 
         :param file_path: File path.
-        :param iterations: The required number of rows.
         :param kwargs: Extra keyword arguments for :py:func:`json.dump` class.
 
         *New in version 5.3.0*
         """
-        data = self.create(iterations)
         with open(file_path, "w", encoding="utf-8") as fp:
-            json.dump(data, fp, **kwargs)
+            json.dump(self.create(), fp, **kwargs)
 
-    def to_pickle(self, file_path: str, iterations: int = 100, **kwargs: t.Any) -> None:
+    def to_pickle(self, file_path: str, **kwargs: t.Any) -> None:
         """Export a schema as the pickled representation of the object to the file.
 
         :param file_path: File path.
-        :param iterations: The required number of rows.
         :param kwargs: Extra keyword arguments for :py:func:`pickle.dump` class.
 
         *New in version 5.3.0*
         """
-        data = self.create(iterations)
         with open(file_path, "wb") as fp:
-            pickle.dump(data, fp, **kwargs)
+            pickle.dump(self.create(), fp, **kwargs)
 
-    def create(self, iterations: int = 1) -> t.List[JSON]:
+    def create(self) -> t.List[JSON]:
         """Creates a list of a fulfilled schemas.
 
         .. note::
             This method evaluates immediately, so be careful on creating
             large datasets otherwise you're risking running out of memory.
 
             If you need a lazy version of this method, see :meth:`iterator`.
 
-        :param iterations: Number of iterations.
-        :return: List of fulfilled schemas.
-        """
-
-        if iterations < self._MIN_ITERATIONS_VALUE:
-            raise ValueError("The number of iterations must be greater than 0.")
-
-        return [self._schema() for _ in range(iterations)]
-
-    def loop(self) -> t.Iterator[JSON]:
-        """Fulfills a schema **infinitely** in a lazy way.
-
-        This method can be useful when you have dynamic conditions
-        on which the generation must depend and be interrupted accordingly.
-
-        Since the data provided by mimesis is limited, frequent
-        calls of this method may cause data duplication.
-
-        Before using this method, ask yourself: **Do I really need this**?
-        In most cases, the answer is: Nah, :meth:`iterator` is enough.
-
-        **Do not use** this method without **interrupt conditions**, otherwise,
-        you're risking running out of memory.
-
-        If you're accepting all risks below and want to suppress
-        the warnings then use :py:class:`warnings.catch_warnings`
-
-        .. warning::
-
-            **Never** (seriously) call :py:class:`list`, :py:class:`tuple`, :py:class:`set`
-            or any other callable which tries to evaluate the whole lazy object on this
-            method — **infinite** called infinite for a reason.
-
-        :return: An infinite iterator with fulfilled schemas.
-        """
-
-        warnings.warn(
-            "You're iterating over the infinite object! "
-            "The schema.loop() may cause a serious memory leak."
-            "Please, see: https://mimesis.name/en/latest/api.html#mimesis.schema.Schema.loop"
-        )
-
-        while True:
-            yield self._schema()
-
-    def iterator(self, iterations: int = 1) -> t.Iterator[JSON]:
-        """Fulfills schema in a lazy way.
-
-        :param iterations: Number of iterations.
         :return: List of fulfilled schemas.
         """
+        return [self._schema() for _ in range(self.iterations)]
 
-        if iterations < self._MIN_ITERATIONS_VALUE:
-            raise ValueError("The number of iterations must be greater than 0.")
-
-        for item in range(iterations):
-            yield self._schema()
+    def __next__(self) -> JSON:
+        """Return the next item from the iterator."""
+        if self._count < self.iterations:
+            self._count += 1
+            return self._schema()
+        raise StopIteration
+
+    def __iter__(self) -> "Schema":
+        """Return the iterator object itself."""
+        self._count = 0
+        return self
```

### Comparing `mimesis-8.0.0/mimesis/shortcuts.py` & `mimesis-9.0.0/mimesis/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/mimesis/types.py` & `mimesis-9.0.0/mimesis/types.py`

 * *Files identical despite different names*

### Comparing `mimesis-8.0.0/pyproject.toml` & `mimesis-9.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mimesis"
-version = "8.0.0"
+version = "9.0.0"
 description = "Mimesis: Fake Data Generator."
 authors = ["Isaak Uchakaev <likid.geimfari@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/lk-geimfari/mimesis"
 repository = "https://github.com/lk-geimfari/mimesis"
 documentation = "https://mimesis.name"
@@ -61,15 +61,15 @@
 black = "^22.10"
 autoflake = "^2.0"
 types-pytz = "^2023.3"
 taskipy = "^1.10.1"
 validators = "^0.20.0"
 pytest-repeat = "^0.9.1"
 memory-profiler = "^0.61.0"
-Sphinx = "^5.1.1"
+Sphinx = ">=5.1.1,<7.0.0"
 sphinx-copybutton = "^0.5.0"
 sphinx-autodoc-typehints = "^1.19.2"
 isort = "^5.12"
 
 [tool.poetry.plugins."pytest_randomly.random_seeder"]
 mimesis = "mimesis.entrypoints:pytest_randomly_reseed"
```

### Comparing `mimesis-8.0.0/PKG-INFO` & `mimesis-9.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimesis
-Version: 8.0.0
+Version: 9.0.0
 Summary: Mimesis: Fake Data Generator.
 Home-page: https://github.com/lk-geimfari/mimesis
 License: MIT
 Keywords: data,datascince,database,dummy,fake,faker,fixtures,generate,mimesis,mock,populate,testing
 Author: Isaak Uchakaev
 Author-email: likid.geimfari@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -87,14 +87,16 @@
 
 
 Python compatibility
 ---------------------
 
 Mimesis is compatible with Python, including PyPy, version 3.8 or higher. The Mimesis 4.1.3 is the last release that accommodates Python 3.6 and 3.7.
 
+To prevent unintended upgrades, it is higly advisable to always specify the version of mimesis that you are using by pinning it.
+
 Supported Features
 ------------------
 
 - **Easy**: A simple design and clear documentation for easy and swift data generation.
 - **Multilingual**: Mimesis generates data in a vast range of `languages <https://mimesis.name/en/latest/getting_started.html#supported-locales>`_.
 - **Performance**: Mimesis has excellent performance and is widely regarded as the fastest data generator among all Python solutions available.
 - **Data variety**: Mimesis supports a broad range of data providers, including names, addresses, phone numbers, email addresses, dates, times, and more, enabling users to generate data for various purposes.
```

