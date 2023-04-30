# Comparing `tmp/hledger_lots-0.1.6.tar.gz` & `tmp/hledger_lots-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hledger_lots-0.1.6.tar", last modified: Mon Apr 24 18:35:21 2023, max compression
+gzip compressed data, was "hledger_lots-0.2.0.tar", last modified: Sun Apr 30 16:22:23 2023, max compression
```

## Comparing `hledger_lots-0.1.6.tar` & `hledger_lots-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.094962 hledger_lots-0.1.6/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-24 18:35:21.094962 hledger_lots-0.1.6/PKG-INFO
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.084962 hledger_lots-0.1.6/docs/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4733 2023-04-19 21:08:59.000000 hledger_lots-0.1.6/docs/README.md
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.087962 hledger_lots-0.1.6/hledger_lots/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/hledger_lots/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/hledger_lots/__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2957 2023-04-23 02:50:39.000000 hledger_lots-0.1.6/hledger_lots/avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2631 2023-04-23 18:16:23.000000 hledger_lots-0.1.6/hledger_lots/avg_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/hledger_lots/checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)    10816 2023-04-24 18:30:26.000000 hledger_lots-0.1.6/hledger_lots/cli.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2023-04-23 02:50:39.000000 hledger_lots-0.1.6/hledger_lots/fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3157 2023-04-23 18:16:23.000000 hledger_lots-0.1.6/hledger_lots/fifo_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      969 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/hledger_lots/files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/hledger_lots/hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4326 2023-04-24 13:24:22.000000 hledger_lots-0.1.6/hledger_lots/info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2758 2023-04-24 18:30:26.000000 hledger_lots-0.1.6/hledger_lots/lib.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3749 2023-04-24 18:30:26.000000 hledger_lots-0.1.6/hledger_lots/prices_yahoo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     9399 2023-04-24 18:30:26.000000 hledger_lots-0.1.6/hledger_lots/prompt.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.089962 hledger_lots-0.1.6/hledger_lots.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5073 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/PKG-INFO
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1026 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/entry_points.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       78 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/requires.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       40 2023-04-24 18:35:21.000000 hledger_lots-0.1.6/hledger_lots.egg-info/top_level.txt
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1255 2023-04-24 18:34:19.000000 hledger_lots-0.1.6/pyproject.toml
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-24 18:35:21.094962 hledger_lots-0.1.6/setup.cfg
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.091962 hledger_lots-0.1.6/tests/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/__init__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/lots_data.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test__main__.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4562 2023-04-23 02:50:39.000000 hledger_lots-0.1.6/tests/test_avg.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3241 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test_checks.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2565 2023-04-23 02:50:39.000000 hledger_lots-0.1.6/tests/test_fifo.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2305 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test_files.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test_hl.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test_info.py
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.1.6/tests/test_lib.py
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.084962 hledger_lots-0.1.6/venv/
-drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-24 18:35:21.093962 hledger_lots-0.1.6/venv/bin/
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2html.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2html4.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2html5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2latex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2man.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2odt.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2s5.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2xetex.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rst2xml.py
--rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.1.6/venv/bin/rstpep2html.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.383155 hledger_lots-0.2.0/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5729 2023-04-30 16:22:23.382155 hledger_lots-0.2.0/PKG-INFO
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.366155 hledger_lots-0.2.0/docs/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5389 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/docs/README.md
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.369155 hledger_lots-0.2.0/hledger_lots/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/hledger_lots/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       85 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/hledger_lots/__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2957 2023-04-23 02:50:39.000000 hledger_lots-0.2.0/hledger_lots/avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2719 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/avg_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1393 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/hledger_lots/checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)    13624 2023-04-30 16:17:25.000000 hledger_lots-0.2.0/hledger_lots/cli.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3732 2023-04-23 02:50:39.000000 hledger_lots-0.2.0/hledger_lots/fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3245 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/fifo_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      913 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1709 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/hledger_lots/hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4318 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2758 2023-04-24 18:30:26.000000 hledger_lots-0.2.0/hledger_lots/lib.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3749 2023-04-24 18:30:26.000000 hledger_lots-0.2.0/hledger_lots/prices_yahoo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     7340 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/prompt.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4158 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/prompt_buy.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3374 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/hledger_lots/prompt_sell.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.370155 hledger_lots-0.2.0/hledger_lots.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5729 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1081 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        1 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/entry_points.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       78 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/requires.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       45 2023-04-30 16:22:23.000000 hledger_lots-0.2.0/hledger_lots.egg-info/top_level.txt
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     1255 2023-04-30 16:20:54.000000 hledger_lots-0.2.0/pyproject.toml
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       38 2023-04-30 16:22:23.383155 hledger_lots-0.2.0/setup.cfg
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.378155 hledger_lots-0.2.0/tests/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)        0 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/__init__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     5566 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/lots_data.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)      192 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/test__main__.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     4562 2023-04-23 02:50:39.000000 hledger_lots-0.2.0/tests/test_avg.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3205 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/tests/test_checks.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2565 2023-04-23 02:50:39.000000 hledger_lots-0.2.0/tests/test_fifo.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)       60 2023-04-30 16:01:03.000000 hledger_lots-0.2.0/tests/test_files.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/test_hl.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3068 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/test_info.py
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     2136 2023-04-18 19:22:25.000000 hledger_lots-0.2.0/tests/test_lib.py
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.365155 hledger_lots-0.2.0/venv/
+drwxr-xr-x   0 eduardo   (1000) eduardo   (1000)        0 2023-04-30 16:22:23.382155 hledger_lots-0.2.0/venv/bin/
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      627 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      749 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1094 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      826 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      649 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      815 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)     1753 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      634 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      670 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      906 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      635 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 eduardo   (1000) eduardo   (1000)      703 2023-04-18 19:23:23.000000 hledger_lots-0.2.0/venv/bin/rstpep2html.py
```

### Comparing `hledger_lots-0.1.6/PKG-INFO` & `hledger_lots-0.2.0/docs/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,76 @@
-Metadata-Version: 2.1
-Name: hledger_lots
-Version: 0.1.6
-License: MIT License
-Project-URL: homepage, https://github.com/edkedk99/hledger-lots
-Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
-Project-URL: repository, https://github.com/edkedk99/hledger-lots
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-# Introduction
+# Hledger-lots
 
 ![automatic lots](img/meme.jpg)
 
-This script aims to help hledger's users to add transactions involving buying and selling commodities, which can be FOREX or investments assets, for example
+This package helps [hledger](https://hledger.org/) users to add and manage transactions involving buying and selling commodities like stock, currency, etc.
+
+## Features
+
+### Add transaction
+
+Instead of editing the journal file directly to add a commodity purchase or sale, answer some interactive prompts with the following benefits:
+
+- Validation of allowed values for each field
+- Fuzzy search completion using previous transaction data in the journal
+- Select the answer between possible values or autocomplete when only one answer is allowed.
+
+### Automatic Lots
 
-When you sell a commodity, you should use the cost and quantity from the purchase date, which is buried deep down in your journal file so you have hledger accounting the correct _Capital Gain_.
+The most convoluted aspect of using hledger for investment is to [manage lots](https://hledger.org/track-investments.html) because when selling a commodity, you need to use its cost, which is buried deep down in your journal, instead of the sale price, which is more easily available to add the correct profit/loss of the trade.
+
+To calculate the cost, there are some methods you can apply and hledger doesn't provide tools to do it, so you are on your own. Hledger-lots calculate the cost without the need to alocate each purchase to a specific subaccount or tag. When you use `hledger-lots sell`, it traverse the journal and arrive to the correct cost without additional information.
 
 You can choose between two diferrent methods to calculate the cost of selling lots:
 
 - **FIFO**: First In First Out
 - **AVERAGE COST**: Average Cost of all previous purchase. It is as if selling a proportional part of each previous sale.
 
-This package create a sale transaction according to information provided by the user and traverse the journal file to determine what quantity and lot prices should be used and generate a valid hledger transaction to be appended to the journal with additional helpful calculations as comment tags.
 
-When using this package, you don't need to create lots as subaccounts or tag, just add a purchase transaction as usual and when there is a sale, *hledger-lots* will generate the correct postings adding the cost for you, so you don't need to bother looking for this information.
+### Update Price
+
+After having the correct cost and result for selling a commodity, we want to follow the investment performance using market data. This package can download market price history from [Yahoo Finance](https://finance.yahoo.com/) and append [price directive](https://hledger.org/1.29/hledger.html#p-directive) to the journal just by following the required format when naming the commodity. More information [here](market_prices/)
+
+### Reports
+
+To get information about the commodities, there is more 2 commands:
 
-It also generate lots reports so the user can understand his situation with a commodity and check the correctness of the generated sell transaction, including market performance from *prices directives*, which can be automatically downloaded from [Yahoo Finance](https://finance.yahoo.com/).
+| command                          | description                                          |
+|----------------------------------|------------------------------------------------------|
+| [view](usage/#hledger-lots-view) | Get the lots and indicators for a specific commodity |
+| [list](usage/#hledger-lots-list) | Get the indicators for all commodities as a table    |
 
-To verify your transaction, this package can also check if your past sale has the correct cost.
+The indicators provided by these command are explained [here](#indicators).
 
 ## Documentation
 
 Documentation with usage information can be found [here](https://edkedk99.github.io/hledger-lots/)
 
-## Requirements
-
-- python
-- hledger
 
 ## Installation
 
+### Requirements
+
+- [python](https://www.python.org/)
+- [hledger](https://hledger.org/1.29/hledger.html#p-directive)
+
+### Command
+
 ```python
 pip install --upgrade hledger-lots
 ```
 
 ## Workflow
 
-1. Add purchase transaction as normal. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/test2022.journal)
-2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and print to stdout so you can add to the journal if everything is correct. *See transaction tags with interesting indicators about the current trade*
+1. Add purchase using the command [buy](usage/#buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
+2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
+3. View financial indicators for a specific commodity using [view](usage/#view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
 
 > By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
-   
-
-## Reports
-
-To get information about the commodities, there is more 2 commands:
-
-| command | description                                          |
-|---------|------------------------------------------------------|
-| view    | Get the lots and indicators for a specific commodity |
-| list   | Get the indicators for all commodities as a table    |
-
-
 
-If you add *price directives* for the commodity in a date after the last purchase, additional indicators will be shown related to the performance of the investment. See [indicators](#indicators) help for more detail and [market prices](market_prices) to download the prices from [Yahoo Finance](https://finance.yahoo.com/).
 
 ## Indicators
   
 ### Basic Indicators
 
 - Commodity Name
 - Total Quantity Purchased
@@ -84,19 +87,19 @@
 - Last Market Date
 - [XIRR](#xirr)
 
 ## XIRR
 
 The sale transaction gives you the calculated **xirr** as tag, which is the internal rate of return of an investment based on a specified series of irregularly spaced cash flows. This value is annual percentage rate following the 30/360US day count convention. It is a good metric to compare the investment return with a benchmark like the S&P or the T-Bill, for example.
 
-Note the benchmark can use another day count convention, so this comparison may not be 100% precise. This app may in the future offer others day count convention for **xirr** calculation.
+> Note the benchmark can use another day count convention, so this comparison may not be 100% precise. This app may in the future offer others day count convention for **xirr** calculation.
 
 ## Checks
 
 It is recommended to use the option *--check* to ensure you past selling transaction has the correct cost according to the choosen cost method. It can be enabled by setting the environment variable **HLEDGER_LOTS_CHECK** to "true". It can be disabled with the option *--no-check* or setting the environment variable **HLEDGER_LOTS_CHECK** to "false".
 
-At the moment the dafault is set to "false", but expect it to be turned to "true" in future releases.
+> At the moment the default is set to "false", but expect it to be turned to "true" in future releases.
 
 ## Limitations
 
 - No _short-selling_
 - Each commodity can have only one base currency. For example, it is not possible to buy AAPL with USD and later with EUR.
```

### Comparing `hledger_lots-0.1.6/docs/README.md` & `hledger_lots-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,86 @@
-# Introduction
+Metadata-Version: 2.1
+Name: hledger_lots
+Version: 0.2.0
+License: MIT License
+Project-URL: homepage, https://github.com/edkedk99/hledger-lots
+Project-URL: documentation, https://edkedk99.github.io/hledger-lots/
+Project-URL: repository, https://github.com/edkedk99/hledger-lots
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+# Hledger-lots
 
 ![automatic lots](img/meme.jpg)
 
-This script aims to help hledger's users to add transactions involving buying and selling commodities, which can be FOREX or investments assets, for example
+This package helps [hledger](https://hledger.org/) users to add and manage transactions involving buying and selling commodities like stock, currency, etc.
+
+## Features
+
+### Add transaction
+
+Instead of editing the journal file directly to add a commodity purchase or sale, answer some interactive prompts with the following benefits:
+
+- Validation of allowed values for each field
+- Fuzzy search completion using previous transaction data in the journal
+- Select the answer between possible values or autocomplete when only one answer is allowed.
+
+### Automatic Lots
 
-When you sell a commodity, you should use the cost and quantity from the purchase date, which is buried deep down in your journal file so you have hledger accounting the correct _Capital Gain_.
+The most convoluted aspect of using hledger for investment is to [manage lots](https://hledger.org/track-investments.html) because when selling a commodity, you need to use its cost, which is buried deep down in your journal, instead of the sale price, which is more easily available to add the correct profit/loss of the trade.
+
+To calculate the cost, there are some methods you can apply and hledger doesn't provide tools to do it, so you are on your own. Hledger-lots calculate the cost without the need to alocate each purchase to a specific subaccount or tag. When you use `hledger-lots sell`, it traverse the journal and arrive to the correct cost without additional information.
 
 You can choose between two diferrent methods to calculate the cost of selling lots:
 
 - **FIFO**: First In First Out
 - **AVERAGE COST**: Average Cost of all previous purchase. It is as if selling a proportional part of each previous sale.
 
-This package create a sale transaction according to information provided by the user and traverse the journal file to determine what quantity and lot prices should be used and generate a valid hledger transaction to be appended to the journal with additional helpful calculations as comment tags.
 
-When using this package, you don't need to create lots as subaccounts or tag, just add a purchase transaction as usual and when there is a sale, *hledger-lots* will generate the correct postings adding the cost for you, so you don't need to bother looking for this information.
+### Update Price
+
+After having the correct cost and result for selling a commodity, we want to follow the investment performance using market data. This package can download market price history from [Yahoo Finance](https://finance.yahoo.com/) and append [price directive](https://hledger.org/1.29/hledger.html#p-directive) to the journal just by following the required format when naming the commodity. More information [here](market_prices/)
+
+### Reports
+
+To get information about the commodities, there is more 2 commands:
 
-It also generate lots reports so the user can understand his situation with a commodity and check the correctness of the generated sell transaction, including market performance from *prices directives*, which can be automatically downloaded from [Yahoo Finance](https://finance.yahoo.com/).
+| command                          | description                                          |
+|----------------------------------|------------------------------------------------------|
+| [view](usage/#hledger-lots-view) | Get the lots and indicators for a specific commodity |
+| [list](usage/#hledger-lots-list) | Get the indicators for all commodities as a table    |
 
-To verify your transaction, this package can also check if your past sale has the correct cost.
+The indicators provided by these command are explained [here](#indicators).
 
 ## Documentation
 
 Documentation with usage information can be found [here](https://edkedk99.github.io/hledger-lots/)
 
-## Requirements
-
-- python
-- hledger
 
 ## Installation
 
+### Requirements
+
+- [python](https://www.python.org/)
+- [hledger](https://hledger.org/1.29/hledger.html#p-directive)
+
+### Command
+
 ```python
 pip install --upgrade hledger-lots
 ```
 
 ## Workflow
 
-1. Add purchase transaction as normal. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/test2022.journal)
-2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and print to stdout so you can add to the journal if everything is correct. *See transaction tags with interesting indicators about the current trade*
+1. Add purchase using the command [buy](usage/#buy) or edit the journal as usual using "@" notation. **Don't bother creating subaccounts or tags with unique lot name**. See the some examples [here](examples/data.journal)
+2. When you sell, use the command [sell](usage/#sell) instead of adding the transactions manually. Hledger-lots will generate the correct transaction and append to the selected journal if you confirm the transaction is correct. *See transaction tags with interesting indicators about the current trade*
+3. View financial indicators for a specific commodity using [view](usage/#view) or a summary of all commodities using [list](usage/$list). Optionally update market prices from [Yahoo Finance](https://finance.yahoo.com/) using the flag *--apend-prices-to [file path]*
 
 > By default the sale is created using *FIFO* method. Use the option flag "--avg-cost" to change it to *Average Cost*
-   
-
-## Reports
-
-To get information about the commodities, there is more 2 commands:
-
-| command | description                                          |
-|---------|------------------------------------------------------|
-| view    | Get the lots and indicators for a specific commodity |
-| list   | Get the indicators for all commodities as a table    |
-
-
 
-If you add *price directives* for the commodity in a date after the last purchase, additional indicators will be shown related to the performance of the investment. See [indicators](#indicators) help for more detail and [market prices](market_prices) to download the prices from [Yahoo Finance](https://finance.yahoo.com/).
 
 ## Indicators
   
 ### Basic Indicators
 
 - Commodity Name
 - Total Quantity Purchased
@@ -74,19 +97,19 @@
 - Last Market Date
 - [XIRR](#xirr)
 
 ## XIRR
 
 The sale transaction gives you the calculated **xirr** as tag, which is the internal rate of return of an investment based on a specified series of irregularly spaced cash flows. This value is annual percentage rate following the 30/360US day count convention. It is a good metric to compare the investment return with a benchmark like the S&P or the T-Bill, for example.
 
-Note the benchmark can use another day count convention, so this comparison may not be 100% precise. This app may in the future offer others day count convention for **xirr** calculation.
+> Note the benchmark can use another day count convention, so this comparison may not be 100% precise. This app may in the future offer others day count convention for **xirr** calculation.
 
 ## Checks
 
 It is recommended to use the option *--check* to ensure you past selling transaction has the correct cost according to the choosen cost method. It can be enabled by setting the environment variable **HLEDGER_LOTS_CHECK** to "true". It can be disabled with the option *--no-check* or setting the environment variable **HLEDGER_LOTS_CHECK** to "false".
 
-At the moment the dafault is set to "false", but expect it to be turned to "true" in future releases.
+> At the moment the default is set to "false", but expect it to be turned to "true" in future releases.
 
 ## Limitations
 
 - No _short-selling_
 - Each commodity can have only one base currency. For example, it is not possible to buy AAPL with USD and later with EUR.
```

### Comparing `hledger_lots-0.1.6/hledger_lots/avg.py` & `hledger_lots-0.2.0/hledger_lots/avg.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/hledger_lots/avg_info.py` & `hledger_lots-0.2.0/hledger_lots/avg_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from datetime import datetime
-from typing import Tuple
+from typing import Optional, Tuple
 
 from .avg import get_avg_cost
 from .info import AllInfo, Info, LotsInfo
 from .lib import dt_list2table
 
 
 class AvgInfo(Info):
-    def __init__(self, journals: Tuple[str, ...], commodity: str, check: bool):
+    def __init__(
+        self,
+        journals: Tuple[str, ...],
+        commodity: str,
+        check: bool,
+        no_desc: Optional[str] = None,
+    ):
         super().__init__(journals, commodity)
         self.check = check
         self.avg_lots = get_avg_cost(self.txns, self.check)
         self.table = dt_list2table(self.avg_lots)
 
     @property
     def info(self):
```

### Comparing `hledger_lots-0.1.6/hledger_lots/checks.py` & `hledger_lots-0.2.0/hledger_lots/checks.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/hledger_lots/cli.py` & `hledger_lots-0.2.0/hledger_lots/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import os
 from pathlib import Path
-from typing import Literal, Tuple
+from typing import Literal, Optional, Tuple
 
 import rich_click as click
 
 from .avg_info import AllAvgInfo, AvgInfo
 from .fifo_info import AllFifoInfo, FifoInfo
-from .files import get_default_file, get_file_path, get_files_comm
+from .files import get_file, get_files_comm
 from .info import AllInfo
 from .lib import default_fn_bool
 from .prices_yahoo import get_hledger_prices
-from .prompt import PromptSell, get_append_file
+from .prompt import get_append_file
+from .prompt_buy import PromptBuy
+from .prompt_sell import PromptSell
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 click.rich_click.USE_MARKDOWN = True
 click.rich_click.SHOW_ARGUMENTS = True
 click.rich_click.GROUP_ARGUMENTS_OPTIONS = True
 click.rich_click.MAX_WIDTH = 80
@@ -30,112 +32,106 @@
 click.rich_click.STYLE_OPTIONS_PANEL_BORDER = "dim"  # Possibly conceal
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 @click.option(
     "-f",
     "--file",
-    type=click.Path(),
     required=False,
-    callback=get_file_path,
     multiple=True,
     help="Inform the journal file path. If \"-\", read from stdin. Without this flag read from $LEDGER_FILE or ~/.hledger.journal in this order  or '-f-'.",
 )
 @click.version_option()
-def cli(file: str):  # pyright:ignore
+def cli(file: Optional[str] = None):  # pyright:ignore
     """
     Commands to apply FIFO(first-in-first-out) or AVERAGE COST accounting principles without manual management of lots. Useful for transactions involving buying and selling foreign currencies or stocks.
 
     To find out more, visit [https://github.com/edkedk99/hledger-lots](https://github.com/edkedk99/hledger-lots)
     """
 
 
 @click.command()
 @click.option(
     "-f",
     "--file",
-    type=click.Path(),
     required=False,
-    callback=get_file_path,
     multiple=True,
     help="Inform the journal file path. If \"-\", read from stdin. Without this flag read from $LEDGER_FILE or ~/.hledger.journal in this order  or '-f-'.",
 )
 @click.option(
     "-g",
     "--avg-cost",
     is_flag=True,
     default=default_fn_bool("HLEDGER_LOTS_AVG_COST", False),
     help='Change cost method to "average cost"". Can be set with env HLEDGER_LOTS_IS_AVG_COST=true|false. Default to false',
 )
 @click.option(
-    "-c",
-    "--commodity",
-    type=click.STRING,
-    prompt=True,
-    help="Commodity to get fifo lots",
-)
-@click.option(
     "-n",
     "--no-desc",
     type=click.STRING,
     default=lambda: os.environ.get("HLEDGER_LOTS_NO_DESC", None),
-    prompt=False,
     help="Description to be filtered out from calculation. Needed when closing journal with '--show-costs' option. Works like: not:desc:<value>. Will not be prompted if absent. If closed with default description, the value of this option should be: 'opening|closing balances'. Can be set with env HLEDGER_LOTS_NO_DESC",
 )
 @click.option(
     "--check/--no-check",
     default=default_fn_bool("HLEDGER_LOTS_CHECK", False),
-    help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=true|false. Default to false. Inthe future it will default to true",
-)
-@click.option(
-    "-p",
-    "--append-prices-to",
-    type=click.Path(),
-    default=lambda: os.environ.get("HLEDGER_APPEND_PRICES_TO", None),
-    prompt=False,
-    required=False,
-    help="Download market price and append to this option file value. Check the doc for info on how to set it up. Can be set with env HLEDGER_APPEND_PRICES_TO",
+    help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=true|false. Default to false. In the future it will default to true",
 )
-def view(
-    file: Tuple[str, ...],
+@click.pass_context
+def buy(
+    ctx: click.Context,  # pyright:ignore
     avg_cost: bool,
-    commodity: str,
     no_desc: str,
     check: bool,
-    append_prices_to: Path,
+    file: Tuple[str, ...],
 ):
     """
-    Report lots for a commodity.\r
+    Create a purchase transaction for a commodity by answering some prompts that tries to avoid errors with validation and using current journal data to filter possible answers and give informations that guides the user thru the process.\r
 
-    Show a report with lots for a commodity considering eventual past sale using FIFO or AVERAGE COST accounting principles.
+    ### Transaction postings
 
-    Also show some indicators about the lots and performance if there is prices in the journal after the last purchase. See the docs for details
+    - First posting: Negative amount on the cash account where the money was used to pay for the commodity
+
+    - Second Posting: Positive amount of the commodity being bought with its cost using \"@\" symbol
     """
 
-    journals = file or get_default_file()
+    journals = get_file(ctx, file)
+    prompt_buy = PromptBuy(journals, avg_cost, check, no_desc)
+    txn_print = prompt_buy.get_hl_txn()
+    click.echo("\n" + txn_print)
 
-    if append_prices_to:
-        get_hledger_prices(file, append_prices_to)
+    append_file = get_append_file(journals[0])
+    if append_file:
+        with open(append_file, "a") as f:
+            f.write("\n" + txn_print)
+    else:
+        click.echo("\n" + "Transaction not saved.")
 
+    commodity = prompt_buy.info["comm"]
     if avg_cost:
         info = AvgInfo(journals, commodity, check)
     else:
         info = FifoInfo(journals, commodity, check)
 
     click.echo(info.table)
     click.echo(info.info_txt)
 
+    if commodity.startswith("y."):
+        files_comm_str = " ".join(get_files_comm(journals))
+        click.echo(
+            f"To update prices from Yahoo finance, run:\n\n hledger-lots {files_comm_str} view -c {commodity} -p {journals[0]}"
+        )
+
 
 @click.command()
 @click.option(
     "-f",
     "--file",
     type=click.Path(),
     required=False,
-    callback=get_file_path,
     multiple=True,
     help="Inform the journal file path. If \"-\", read from stdin. Without this flag read from $LEDGER_FILE or ~/.hledger.journal in this order  or '-f-'.",
 )
 @click.option(
     "-g",
     "--avg-cost",
     is_flag=True,
@@ -153,34 +149,33 @@
     "--check/--no-check",
     default=default_fn_bool("HLEDGER_LOTS_CHECK", False),
     help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=true|false. Default to false. In the future it will default to true",
 )
 @click.pass_context
 def sell(
     ctx: click.Context,  # pyright:ignore
-    file: Tuple[str, ...],
     avg_cost: bool,
     no_desc: str,
     check: bool,
+    file: Tuple[str, ...],
 ):
     """
     Create a transaction with automatic FIFO or AVERAGE COST for a commodity by answering some prompts that tries to avoid errors with validation and using current journal data to filter possible answers give informations that guides the user thru the process.\r
 
     > This command also add transaction's comment with some indicators. See an example on "Output examples" page of the docs.
 
-    ## Transaction postings
+    ### Transaction postings
 
     - First posting: Positive amount on the 'base-currency' in the account that receives the product of the sale.
 
     - Multiple lot postings: Each posting represents a lot you are selling for the cost price on purchasing date, according to FIFO accounting principles or one postings in case of AVERAGE COST method.
 
     - Revenue posting: posting that represent Capital Gain or Loss as the difference between the total cost and the amount received on the base-currency.
     """
-
-    journals = file or get_default_file()
+    journals = get_file(ctx, file)
     prompt_sell = PromptSell(journals, avg_cost, check, no_desc)
 
     txn_print = prompt_sell.get_hl_txn()
     click.echo("\n" + txn_print)
 
     append_file = get_append_file(journals[0])
     if append_file:
@@ -201,21 +196,94 @@
     if commodity.startswith("y."):
         files_comm_str = " ".join(get_files_comm(journals))
         click.echo(
             f"To update prices from Yahoo finance, run:\n\n hledger-lots {files_comm_str} view -c {commodity} -p {journals[0]}"
         )
 
 
-@click.command(name="list")
+@click.command()
 @click.option(
     "-f",
     "--file",
+    required=False,
+    multiple=True,
+    help="Inform the journal file path. If \"-\", read from stdin. Without this flag read from $LEDGER_FILE or ~/.hledger.journal in this order  or '-f-'.",
+)
+@click.option(
+    "-g",
+    "--avg-cost",
+    is_flag=True,
+    default=default_fn_bool("HLEDGER_LOTS_AVG_COST", False),
+    help='Change cost method to "average cost"". Can be set with env HLEDGER_LOTS_IS_AVG_COST=true|false. Default to false',
+)
+@click.option(
+    "-c",
+    "--commodity",
+    type=click.STRING,
+    prompt=True,
+    help="Commodity to get fifo lots",
+)
+@click.option(
+    "-n",
+    "--no-desc",
+    type=click.STRING,
+    default=lambda: os.environ.get("HLEDGER_LOTS_NO_DESC", None),
+    prompt=False,
+    help="Description to be filtered out from calculation. Needed when closing journal with '--show-costs' option. Works like: not:desc:<value>. Will not be prompted if absent. If closed with default description, the value of this option should be: 'opening|closing balances'. Can be set with env HLEDGER_LOTS_NO_DESC",
+)
+@click.option(
+    "--check/--no-check",
+    default=default_fn_bool("HLEDGER_LOTS_CHECK", False),
+    help="Enable/Disable check on the commodities previous transactions to ensure it is following the choosen method. Can be set with env HLEDGER_LOTS_CHECK=true|false. Default to false. Inthe future it will default to true",
+)
+@click.option(
+    "-p",
+    "--append-prices-to",
     type=click.Path(),
+    default=lambda: os.environ.get("HLEDGER_APPEND_PRICES_TO", None),
+    prompt=False,
     required=False,
-    callback=get_file_path,
+    help="Download market price and append to this option file value. Check the doc for info on how to set it up. Can be set with env HLEDGER_APPEND_PRICES_TO",
+)
+@click.pass_context
+def view(
+    ctx: click.Context,
+    avg_cost: bool,
+    commodity: str,
+    no_desc: str,
+    check: bool,
+    append_prices_to: Path,
+    file: Tuple[str, ...],
+):
+    """
+    Report lots for a commodity.\r
+
+    Show a report with lots for a commodity considering eventual past sale using FIFO or AVERAGE COST accounting principles.
+
+    Also show some indicators about the lots and performance if there is prices in the journal after the last purchase. See the docs for details
+    """
+    journals = get_file(ctx, file)
+
+    if append_prices_to:
+        get_hledger_prices(journals, append_prices_to)
+
+    if avg_cost:
+        info = AvgInfo(journals, commodity, check, no_desc)
+    else:
+        info = FifoInfo(journals, commodity, check, no_desc)
+
+    click.echo(info.table)
+    click.echo(info.info_txt)
+
+
+@click.command(name="list")
+@click.option(
+    "-f",
+    "--file",
+    type=click.Path(),
     multiple=True,
     help="Inform the journal file path. If \"-\", read from stdin. Without this flag read from $LEDGER_FILE or ~/.hledger.journal in this order  or '-f-'.",
 )
 @click.option(
     "-g",
     "--avg-cost",
     is_flag=True,
@@ -247,47 +315,50 @@
     "--append-prices-to",
     type=click.Path(),
     default=lambda: os.environ.get("HLEDGER_APPEND_PRICES_TO", None),
     prompt=False,
     required=False,
     help="Download market price and append to this option file value. Check the doc for info on how to set it up. Can be set with env HLEDGER_LOTS_APPEND_PRICES_TO",
 )
+@click.pass_context
 def list_commodities(
-    file: Tuple[str, ...],
+    ctx: click.Context,
     avg_cost: bool,
     output_format: str,
     no_desc: Literal["plain", "pretty", "csv"],
     check: bool,
     append_prices_to: Path,
+    file: Tuple[str, ...],
 ):
     """
     List indicators for all your commodities in a tabular format sorted from higher to lower **XIRR**. It is advised to use full-screen of the terminal. See the docs for a list of indicators and output examples.
 
     It can output in three formats: *plain, pretty and csv*.
     """
 
-    journals = file or get_default_file()
+    journals = get_file(ctx, file)
     lots_info = AllInfo(journals, no_desc)
 
     if append_prices_to:
-        get_hledger_prices(file, append_prices_to)
+        get_hledger_prices(journals, append_prices_to)
 
     lots_info = (
-        AllAvgInfo(file, no_desc, check)
+        AllAvgInfo(journals, no_desc, check)
         if avg_cost
-        else AllFifoInfo(file, no_desc, check)
+        else AllFifoInfo(journals, no_desc, check)
     )
 
     if output_format == "pretty":
         table = lots_info.infos_table("mixed_grid")
     elif output_format == "csv":
         infos_io = lots_info.infos_csv()
         table = infos_io.read()
     else:
         table = lots_info.infos_table("plain")
 
     click.echo(table)
 
 
+cli.add_command(buy)
+cli.add_command(sell)
 cli.add_command(view)
 cli.add_command(list_commodities)
-cli.add_command(sell)
```

### Comparing `hledger_lots-0.1.6/hledger_lots/fifo.py` & `hledger_lots-0.2.0/hledger_lots/fifo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/hledger_lots/fifo_info.py` & `hledger_lots-0.2.0/hledger_lots/fifo_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from datetime import datetime
-from typing import Tuple
+from typing import Optional, Tuple
 
 from .checks import MultipleBaseCurrencies
 from .fifo import get_lots
 from .hl import hledger2txn
 from .info import AllInfo, Info, LotsInfo
 from .lib import dt_list2table, get_avg_fifo
 
 
 class FifoInfo(Info):
-    def __init__(self, journals: Tuple[str, ...], commodity: str, check: bool):
+    def __init__(
+        self,
+        journals: Tuple[str, ...],
+        commodity: str,
+        check: bool,
+        no_desc: Optional[str] = None,
+    ):
         super().__init__(journals, commodity)
         self.check = check
 
         self.lots = get_lots(self.txns, check)
         self.last_buy_date = self.lots[-1].date if len(self.lots) > 0 else None
 
         self.buy_lots = get_lots(self.txns, check)
```

### Comparing `hledger_lots-0.1.6/hledger_lots/files.py` & `hledger_lots-0.2.0/hledger_lots/files.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,38 +4,39 @@
 
 import click
 
 ENV_FILE = "LEDGER_FILE"
 default_path = Path.home() / ".hledger.journal"
 
 
-def get_default_file() -> Tuple[str, ...]:
-    file_env = os.getenv("LEDGER_FILE")
-    if file_env:
-        return (file_env,)
-    elif default_path.exists():
-        return (str(default_path),)
-    else:
-        raise click.BadOptionUsage("file", "File missing")
-
-
-def get_file_path(
-    ctx: click.Context, _param, value: Optional[Tuple[str, ...]]
-) -> Optional[Tuple[str, ...]]:  # type: ignore
-    if value:
-        return value
+def get_parent_file(ctx: click.Context):
+    parent = ctx.parent
+    if not parent:
+        return None
 
-    if not ctx.parent:
+    file_parent = parent.params.get("file")
+    if not file_parent:
         return None
+    file: Optional[Tuple[str, ...]] = file_parent
+    return file
+
+
+def get_file(ctx: click.Context, file: Tuple[str, ...]):
+    if len(file) > 0:
+        return file
+
+    parent_file = get_parent_file(ctx)
+    if parent_file:
+        return parent_file
 
-    filenames: Optional[Tuple] = ctx.parent.params.get("file")
-    if not filenames:
-        raise click.BadOptionUsage("file", "File missing")
+    env_file = os.getenv("LEDGER_FILE")
+    if env_file:
+        return (env_file,)
 
-    return filenames
+    raise click.BadOptionUsage("file", "File missing")
 
 
 def get_files_comm(file_path: Tuple[str, ...]) -> List[str]:
     files = []
     for file in file_path:
         files = [*files, "-f", file]
     return files
```

### Comparing `hledger_lots-0.1.6/hledger_lots/hl.py` & `hledger_lots-0.2.0/hledger_lots/hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/hledger_lots/info.py` & `hledger_lots-0.2.0/hledger_lots/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     if prices_str == "":
         return (None, None)
 
     prices_list = [row.split(" ", 3) for row in prices_str.split("\n") if row != ""]
 
     date_list = [
-        (row[1], re.sub(r"[a-zA-Z]|\,|\s", "", row[3]))
+        (row[1], re.sub(r"[^0-9.]", "", row[3]))
         for row in prices_list
         if row[2] == adjust_commodity(commodity)
     ]
 
     if len(date_list) == 0:
         return (None, None)
 
@@ -81,15 +81,14 @@
     ) -> None:
         self.journals = journals
         self.files_comm = get_files_comm(journals)
         self.commodity = commodity
         self.txns = hledger2txn(journals, commodity, no_desc)
 
         self.has_txn = len(self.txns) > 0
-
         self.last_price = get_last_price(self.files_comm, commodity)
 
         self.market_date, self.market_price = self.last_price
 
     def get_lots_xirr(self, last_buy_date: date):
         if self.market_date and self.market_price and self.market_date >= last_buy_date:
             xirr = get_xirr(self.market_price, self.market_date, self.txns)
```

### Comparing `hledger_lots-0.1.6/hledger_lots/lib.py` & `hledger_lots-0.2.0/hledger_lots/lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/hledger_lots/prices_yahoo.py` & `hledger_lots-0.2.0/hledger_lots/prices_yahoo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/hledger_lots/prompt.py` & `hledger_lots-0.2.0/hledger_lots/prompt.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,80 +2,92 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import List, Optional, Tuple
 
 import questionary
 from prompt_toolkit.shortcuts import CompleteStyle
 
-from . import avg, fifo
 from .avg_info import AllAvgInfo
 from .fifo_info import AllFifoInfo
 from .files import get_files_comm
-from .hl import hledger2txn
+from .info import LotsInfo
 
 
 class PromptError(BaseException):
     def __init__(self, message: str) -> None:
         self.message = message
         super().__init__(self.message)
 
 
 @dataclass
-class SellInfo:
+class Tradeinfo:
     date: str
     quantity: float
     commodity: str
     cash_account: str
-    revenue_account: str
     commodity_account: str
     price: float
     value: float
 
 
+def custom_autocomplete(name: str, choices: List[str]):
+    question = questionary.autocomplete(
+        f"{name} (TAB to autocomplete)",
+        choices=choices,
+        ignore_case=True,
+        match_middle=True,
+        style=questionary.Style([("answer", "fg:#f71b07")]),
+        complete_style=CompleteStyle.MULTI_COLUMN,
+    )
+    return question
+
+
 def get_append_file(default_file: str):
     confirm = questionary.confirm(
         "Add sale transaction to a journal", default=False, auto_enter=True
     ).ask()
 
     if confirm:
         file_append: str = questionary.path(
             "File to append transaction", default=default_file
         ).ask()
         comm = ["hledger", "-f", file_append, "check"]
         subprocess.run(comm, check=True)
         return file_append
 
 
-def custom_autocomplete(name: str, choices: List[str]):
-    question = questionary.autocomplete(
-        f"{name} (TAB to autocomplete)",
-        choices=choices,
-        ignore_case=True,
-        match_middle=True,
-        style=questionary.Style([("answer", "fg:#f71b07")]),
-        complete_style=CompleteStyle.MULTI_COLUMN,
-    )
-    return question
+def select_commodities_text(commodities: List[str]):
+    answer = questionary.select(
+        "Commodity",
+        choices=commodities,
+        use_shortcuts=True,
+    ).ask()
+    return answer
+
+
+def ask_commodities_text(commodities: List[str]):
+    answer: str = custom_autocomplete("Commodity", commodities).ask()
+    return answer
 
 
 def val_date(date: str):
     try:
         datetime.strptime(date, "%Y-%m-%d")
         return True
     except ValueError:
         return "Invalid date format"
 
 
-def val_qtty(answer: str, available: float):
+def val_sell_qtty(answer: str, available: float):
     try:
         answer_float = float(answer)
     except ValueError:
         return "Invalid number"
 
-    if answer_float < 0:
+    if answer_float <= 0:
         return "Quantity should be positive"
 
     if answer_float > available:
         return "Quantity should be less than available"
 
     return True
 
@@ -103,71 +115,66 @@
 
     if answer_float < 0:
         return "Amount should be positive"
 
     return True
 
 
-class PromptSell:
+class Prompt:
     def __init__(
         self,
         file: Tuple[str, ...],
         avg_cost: bool,
         check: bool,
         no_desc: Optional[str] = None,
     ) -> None:
         self.file = file
-        self.avg_cost = avg_cost
         self.check = check
         self.no_desc = no_desc
+        self.avg_cost = avg_cost
 
         self.files_comm = get_files_comm(file)
+        self.infos = self.get_infos()
+        self.commodities = [info["comm"] for info in self.get_infos()]
+
+    def run_hledger(self, *comm: str):
+        command = ["hledger", *self.files_comm, *comm, f"not:desc:{self.no_desc}"]
+        proc = subprocess.run(command, capture_output=True)
+        if proc.returncode != 0:
+            raise subprocess.SubprocessError(proc.stderr.decode("utf8"))
 
-        print(self.initial_info)
-        self.info = self.get_info()
+        result = proc.stdout.decode("utf8")
+        return result
 
-    def get_commodities_text(self, commodities: List[str]):
-        answer = questionary.select(
-            "Commodity",
-            choices=commodities,
-            use_shortcuts=True,
-        ).ask()
-        return answer
+    def run_hledger_no_query_desc(self, *comm: str):
+        command = ["hledger", *self.files_comm, *comm]
+        proc = subprocess.run(command, capture_output=True)
+        if proc.returncode != 0:
+            raise subprocess.SubprocessError(proc.stderr.decode("utf8"))
+
+        result = proc.stdout.decode("utf8")
+        return result
 
-    def get_info(self):
+    def get_infos(self):
         if self.avg_cost:
             infos = AllAvgInfo(self.file, self.no_desc or "", self.check)
         else:
             infos = AllFifoInfo(self.file, self.no_desc or "", self.check)
 
-        commodities = [info["comm"] for info in infos.infos if float(info["qtty"]) > 0]
-        commodity_text = self.get_commodities_text(commodities)
-        info = next(item for item in infos.infos if item["comm"] == commodity_text)
-        return info
-
-    def get_last_purchase(self):
-        commodity = self.info["comm"]
-
-        comm = ["hledger", *self.files_comm, "reg", f"cur:{commodity}", "amt:>0"]
-        reg_proc = subprocess.run(comm, capture_output=True)
-        reg_txt = reg_proc.stdout.decode("utf8")
-        rows_list = [row for row in reg_txt.split("\n") if row != ""]
-        last_date = rows_list[-1][0:10]
-        return last_date
+        valid_infos = [info for info in infos.infos if float(info["qtty"]) > 0]
+        return valid_infos
 
-    def get_accounts_list(self, *query: str):
-        command = ["hledger", *self.files_comm, *query]
-        proc = subprocess.run(command, capture_output=True)
-        if proc.returncode != 0:
-            stderr = proc.stderr.decode("utf8")
-            raise PromptError(stderr)
-
-        proc_list = proc.stdout.decode("utf8").split("\n")
-        proc_list = [row for row in proc_list if row != ""]
-        return proc_list
+    def get_last_purchase(self, info: LotsInfo):
+        commodity = info["comm"]
+        reg = self.run_hledger("reg", f"cur:{commodity}", "amt:>0")
+        rows_list = [row for row in reg.split("\n") if row != ""]
+
+        if len(rows_list) > 0:
+            last_date = rows_list[-1][0:10]
+            return last_date
 
     def get_append_file(self):
         default_file = self.file[0]
 
         confirm = questionary.confirm(
             "Add sale transaction to a journal", default=False, auto_enter=True
         ).ask()
@@ -176,75 +183,65 @@
             file_append: str = questionary.path(
                 "File to append transaction", default=default_file
             ).ask()
             comm = ["hledger", "-f", file_append, "check"]
             subprocess.run(comm, check=True)
             return file_append
 
-    def ask_date(self):
-        last_purchase = self.get_last_purchase()
+    def ask_date(self, last_purchase: Optional[str]):
+        last_purchase = last_purchase
 
         answer: str = questionary.text(
             f"Date YYYY-MM-DD",
             validate=val_date,
             instruction=f"(Last Purchase: {last_purchase})",
         ).ask()
         return answer
 
-    def ask_qtty(self):
-        available = float(self.info["qtty"])
+    def ask_sell_qtty(self, info: LotsInfo):
+        available = float(info["qtty"])
 
         answer_str: str = questionary.text(
             f"Quantity (available {available})",
-            validate=lambda answer: val_qtty(answer, available),
+            validate=lambda answer: val_sell_qtty(answer, available),
             instruction="",
         ).ask()
         return answer_str
 
-    def ask_price(self):
-        cost_str = self.info["avg_cost"].replace(",", ".")
+    def ask_price(self, info: LotsInfo):
+        cost_str = info["avg_cost"].replace(",", ".")
         cost = float(cost_str)
 
         answer_str: str = questionary.text(
             f"Price (avg cost: {cost})",
             validate=val_price,
             instruction="Empty to input total amount",
         ).ask()
         return answer_str
 
-    def ask_total(self, qtty: float):
-        available = qtty * float(self.info["avg_cost"])
+    def ask_total(self, qtty: float, info: LotsInfo):
+        available = qtty * float(info["avg_cost"])
         available_str = f"{available:,.2f}"
 
         answer_str: str = questionary.text(
             f"Total (available {available_str})",
             validate=val_total,
             instruction="Amount received",
         ).ask()
         return answer_str
 
     def ask_cash_account(self):
-        accts = self.get_accounts_list("accounts")
-
+        accts_txt = self.run_hledger("accounts")
+        accts = [acct for acct in accts_txt.split("\n") if acct != ""]
         answer: str = custom_autocomplete("Cash Account", accts).ask()
         return answer
 
-    def ask_commodity_account(self):
-        commodity = self.info["comm"]
-        accts = self.get_accounts_list("accounts", "note:Buy", f"cur:{commodity}")
-
-        answer: str = questionary.select(
-            "Commodity Account",
-            choices=accts,
-            use_shortcuts=True,
-        ).ask()
-        return answer
-
     def ask_revenue_account(self):
-        accts = self.get_accounts_list("accounts")
+        accts_txt = self.run_hledger("accounts")
+        accts = [acct for acct in accts_txt.split("\n") if acct != ""]
         answer: str = custom_autocomplete("Revenue Account", accts).ask()
         return answer
 
     @property
     def initial_info(self):
         cost_method_text = "Average Cost" if self.avg_cost else "Fifo"
         no_desc_text = self.no_desc or "None"
@@ -255,78 +252,7 @@
 
         result = f"""
 Files              : {files_text}
 Cost Method        : {cost_method_text} - {check_text}
 Remove description : {no_desc_text}
 """
         return result
-
-    def prompt(self):
-        commodity = self.info["comm"]
-        sell_date = self.ask_date()
-        qtty = float(self.ask_qtty())
-        price_str = self.ask_price()
-
-        if price_str == "":
-            value_str = self.ask_total(qtty)
-            value = float(value_str)
-            price = value / qtty
-        else:
-            price = float(price_str)
-            value = qtty * price
-
-        cash_acct = self.ask_cash_account()
-
-        if self.avg_cost:
-            commodity_acct = self.ask_commodity_account()
-        else:
-            commodity_acct = ""
-
-        revenue_acct = self.ask_revenue_account()
-
-        result = SellInfo(
-            date=sell_date,
-            quantity=qtty,
-            commodity=commodity,
-            cash_account=cash_acct,
-            revenue_account=revenue_acct,
-            commodity_account=commodity_acct,
-            price=price,
-            value=value,
-        )
-
-        return result
-
-    def get_hl_txn(self):
-        sell = self.prompt()
-        commodity = sell.commodity
-        adj_txns = hledger2txn(self.file, commodity, self.no_desc)
-
-        if self.avg_cost:
-            txn_print = avg.avg_sell(
-                txns=adj_txns,
-                date=sell.date,
-                qtty=sell.quantity,
-                cur=sell.commodity,
-                cash_account=sell.cash_account,
-                revenue_account=sell.revenue_account,
-                comm_account=sell.commodity_account,
-                value=sell.value,
-                check=self.check,
-            )
-        else:
-            sell_fifo = fifo.get_sell_lots(
-                lots=adj_txns,
-                sell_date=sell.date,
-                sell_qtty=sell.quantity,
-                check=self.check,
-            )
-            txn_print = fifo.txn2hl(
-                txns=sell_fifo,
-                date=sell.date,
-                cur=sell.commodity,
-                cash_account=sell.cash_account,
-                revenue_account=sell.revenue_account,
-                value=sell.value,
-            )
-
-        return txn_print
```

### Comparing `hledger_lots-0.1.6/hledger_lots.egg-info/SOURCES.txt` & `hledger_lots-0.2.0/hledger_lots.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 hledger_lots/fifo_info.py
 hledger_lots/files.py
 hledger_lots/hl.py
 hledger_lots/info.py
 hledger_lots/lib.py
 hledger_lots/prices_yahoo.py
 hledger_lots/prompt.py
+hledger_lots/prompt_buy.py
+hledger_lots/prompt_sell.py
 hledger_lots.egg-info/PKG-INFO
 hledger_lots.egg-info/SOURCES.txt
 hledger_lots.egg-info/dependency_links.txt
 hledger_lots.egg-info/entry_points.txt
 hledger_lots.egg-info/requires.txt
 hledger_lots.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `hledger_lots-0.1.6/pyproject.toml` & `hledger_lots-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 keyword = ["hledger","PTA", "investments", "accounting", "lots"]
 classifiers = [""]
 author = "Eduardo"
 author_email = "edkedk99@hotmail.com"
 
 [project]
 name = "hledger_lots"
-version = "0.1.6"
+version = "0.2.0"
 readme= "docs/README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 dependencies = [
 	     "click",
 	     "rich_click",
 	     "tabulate",
```

### Comparing `hledger_lots-0.1.6/tests/lots_data.py` & `hledger_lots-0.2.0/tests/lots_data.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/tests/test_avg.py` & `hledger_lots-0.2.0/tests/test_avg.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/tests/test_checks.py` & `hledger_lots-0.2.0/tests/test_checks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from hledger_lots.lib import AdjustedTxn
 import pytest
 from hledger_lots import checks
 
-# TODO: Test --check-no-check option
+
 class TestCheckShortSellPast:
     previous_buys = [
         AdjustedTxn(
             date="2022-01-01", price=100.0, base_cur="USD", qtty=50.0, acct="ABC"
         ),
         AdjustedTxn(
             date="2022-01-15", price=110.0, base_cur="USD", qtty=50.0, acct="ABC"
```

### Comparing `hledger_lots-0.1.6/tests/test_fifo.py` & `hledger_lots-0.2.0/tests/test_fifo.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/tests/test_hl.py` & `hledger_lots-0.2.0/tests/test_hl.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/tests/test_info.py` & `hledger_lots-0.2.0/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/tests/test_lib.py` & `hledger_lots-0.2.0/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2html.py` & `hledger_lots-0.2.0/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2html4.py` & `hledger_lots-0.2.0/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2html5.py` & `hledger_lots-0.2.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2latex.py` & `hledger_lots-0.2.0/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2man.py` & `hledger_lots-0.2.0/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2odt.py` & `hledger_lots-0.2.0/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2odt_prepstyles.py` & `hledger_lots-0.2.0/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2pseudoxml.py` & `hledger_lots-0.2.0/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2s5.py` & `hledger_lots-0.2.0/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2xetex.py` & `hledger_lots-0.2.0/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rst2xml.py` & `hledger_lots-0.2.0/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `hledger_lots-0.1.6/venv/bin/rstpep2html.py` & `hledger_lots-0.2.0/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

