# Comparing `tmp/sharetop-1.0.1.tar.gz` & `tmp/sharetop-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-1.0.1.tar", last modified: Fri Apr 28 01:46:04 2023, max compression
+gzip compressed data, was "sharetop-1.0.2.tar", last modified: Sun Apr 30 13:35:14 2023, max compression
```

## Comparing `sharetop-1.0.1.tar` & `sharetop-1.0.2.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.921975 sharetop-1.0.1/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    39117 2023-04-28 01:46:04.920942 sharetop-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    37909 2023-04-28 01:45:42.000000 sharetop-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 01:46:04.921975 sharetop-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1169 2023-04-27 23:46:58.000000 sharetop-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.846324 sharetop-1.0.1/sharetop/
--rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.0.1/sharetop/__init__.py
--rw-rw-rw-   0        0        0      386 2023-04-28 01:45:42.000000 sharetop-1.0.1/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.876739 sharetop-1.0.1/sharetop/api/
--rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.0.1/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.879737 sharetop-1.0.1/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.0.1/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4165 2023-04-21 13:29:45.000000 sharetop-1.0.1/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.883776 sharetop-1.0.1/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.0.1/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.891139 sharetop-1.0.1/sharetop/core/bond/
--rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.0.1/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.0.1/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.0.1/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.0.1/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.0.1/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.894135 sharetop-1.0.1/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.0.1/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.0.1/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    12266 2023-04-27 15:28:32.000000 sharetop-1.0.1/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.0.1/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.906938 sharetop-1.0.1/sharetop/core/fund/
--rw-rw-rw-   0        0        0      707 2023-04-25 21:15:03.000000 sharetop-1.0.1/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.0.1/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.0.1/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.0.1/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.0.1/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.0.1/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.0.1/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.0.1/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.0.1/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.0.1/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.908942 sharetop-1.0.1/sharetop/core/futures/
--rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.0.1/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.0.1/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.912938 sharetop-1.0.1/sharetop/core/stock/
--rw-rw-rw-   0        0        0      491 2023-04-25 21:15:03.000000 sharetop-1.0.1/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.0.1/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.0.1/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    14300 2023-04-27 15:24:55.000000 sharetop-1.0.1/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10125 2023-04-28 01:45:42.000000 sharetop-1.0.1/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10050 2023-04-27 15:28:32.000000 sharetop-1.0.1/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0     6341 2023-04-27 13:30:47.000000 sharetop-1.0.1/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.914937 sharetop-1.0.1/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.0.1/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.0.1/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     2704 2023-04-24 00:30:13.000000 sharetop-1.0.1/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.919939 sharetop-1.0.1/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.0.1/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0      419 2023-04-10 00:57:53.000000 sharetop-1.0.1/sharetop/parser/base.py
-drwxrwxrwx   0        0        0        0 2023-04-28 01:46:04.874744 sharetop-1.0.1/sharetop.egg-info/
--rw-rw-rw-   0        0        0    39117 2023-04-28 01:46:04.000000 sharetop-1.0.1/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1452 2023-04-28 01:46:04.000000 sharetop-1.0.1/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 01:46:04.000000 sharetop-1.0.1/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-28 01:46:04.000000 sharetop-1.0.1/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-28 01:46:04.000000 sharetop-1.0.1/sharetop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.343973 sharetop-1.0.2/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    39033 2023-04-30 13:35:14.343973 sharetop-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    37774 2023-04-29 10:56:21.000000 sharetop-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 13:35:14.343973 sharetop-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.246222 sharetop-1.0.2/sharetop/
+-rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.0.2/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-04-30 13:35:02.000000 sharetop-1.0.2/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.291674 sharetop-1.0.2/sharetop/api/
+-rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.0.2/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.293537 sharetop-1.0.2/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.0.2/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4157 2023-04-30 13:28:10.000000 sharetop-1.0.2/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.297234 sharetop-1.0.2/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.0.2/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.304887 sharetop-1.0.2/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.0.2/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.0.2/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.0.2/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.0.2/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.0.2/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.307726 sharetop-1.0.2/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.0.2/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.0.2/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    12266 2023-04-27 15:28:32.000000 sharetop-1.0.2/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.0.2/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.321313 sharetop-1.0.2/sharetop/core/fund/
+-rw-rw-rw-   0        0        0      707 2023-04-25 21:15:03.000000 sharetop-1.0.2/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.0.2/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.0.2/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.0.2/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.0.2/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.0.2/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.0.2/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.0.2/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.0.2/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.0.2/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.323606 sharetop-1.0.2/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.0.2/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.0.2/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.331253 sharetop-1.0.2/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      491 2023-04-25 21:15:03.000000 sharetop-1.0.2/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.0.2/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.0.2/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    14300 2023-04-27 15:24:55.000000 sharetop-1.0.2/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10125 2023-04-28 01:45:42.000000 sharetop-1.0.2/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10050 2023-04-27 15:28:32.000000 sharetop-1.0.2/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0     6341 2023-04-27 13:30:47.000000 sharetop-1.0.2/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.334877 sharetop-1.0.2/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.0.2/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.0.2/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     2704 2023-04-24 00:30:13.000000 sharetop-1.0.2/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.336761 sharetop-1.0.2/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.0.2/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0      419 2023-04-10 00:57:53.000000 sharetop-1.0.2/sharetop/parser/base.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.339946 sharetop-1.0.2/sharetop/test/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.0.2/sharetop/test/__init__.py
+-rw-rw-rw-   0        0        0      261 2023-04-30 13:20:34.000000 sharetop-1.0.2/sharetop/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.289507 sharetop-1.0.2/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    39033 2023-04-30 13:35:14.000000 sharetop-1.0.2/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1501 2023-04-30 13:35:14.000000 sharetop-1.0.2/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 13:35:14.000000 sharetop-1.0.2/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-30 13:35:14.000000 sharetop-1.0.2/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 13:35:14.000000 sharetop-1.0.2/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-1.0.1/LICENSE` & `sharetop-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/PKG-INFO` & `sharetop-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
 
 [![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/sharetop)
 [![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/sharetop)
-[![Pypi-Install](https://img.shields.io/pypi/dm/sharetop.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypi.python.org/pypi/sharetop)
-[![Github Stars](https://img.shields.io/github/stars/sharetop/sharetop.svg?style=social&label=Star&maxAge=60)](https://github.com/nrliangxy/sharetop)
 
-[`sharetop`](https://github.com/nrliangxy/sharetop) 是由个人打造的用于获取股票、基金、期货数据的免费开源 Python 库，你可以使用它很方便地获取数据以便更好地服务于个人的交易系统需求。
+[`sharetop`](https://github.com/nrliangxy/sharetop) 为个人或者机构提供准确详细的市场数据。用于获取经济市场相关的股票，基金，期货数据，也可以获取具体的行业数据，例如，猪肉周期相关数据，石油进出口数据等。
 
 - [`Source Code`](https://github.com/nrliangxy/sharetop)
 
 ---
 
 ## Installation
 
@@ -179,15 +178,15 @@
 4600  688148   芳源股份  -10.57    31.3   34.39    31.3    33.9    -3.7  26.07  0.56   220.01  188415   620632512.0   35.0   15923562000   2261706043  1.688148   沪A
 4601  300034   钢研高纳  -10.96   43.12   46.81   42.88    46.5   -5.31   7.45  1.77    59.49  323226  1441101824.0  48.43   20959281094  18706911861  0.300034   深A
 4602  300712   永福股份  -13.71    96.9  110.94    95.4   109.0   -15.4   6.96  1.26   511.21  126705  1265152928.0  112.3   17645877600  17645877600  0.300712   深A
 
 [4603 rows x 18 columns]
 ```
 
-- 获取单只股或者多只最新状况
+- 获取单只股或者多只最新股价情况
 
 ```python
 >>> import sharetop as sp
 >>> stock_code = '30033'
 >>> sp.stock.get_real_time_data(stock_code)
         股票名称    股票代码     最新价    最高价    最低价  ...  市盈率(TTM)    市净率     涨跌值  涨跌幅(%)  振幅(%)
 0  同花顺  300033  174.92  198.0  172.3  ...     55.27  15.63 -0.2009   -10.3  13.18
@@ -537,10 +536,11 @@
 1528  动力煤主力  ZCM  2021-08-23  796.8  836.6  843.8  796.8  82954  6.850341e+09  5.97  6.28  49.4  0.0
 
 [1529 rows x 13 columns]
 ```
 
 
 ## Contact
+- 对市场感兴趣的同学可以联系我，对互联网金融感兴趣的同学可以联系我，对市场行业相关数据感兴趣的同学可以联系我，对数据有需求的同学可以联系我。欢迎志同道合的同学联系我
+- 微信：share_top
+<img src="static/sharetop.jpg" width="350">
 
-[![Github](https://img.shields.io/badge/Github-blue?style=social&logo=github)](https://github.com/nrliangxy)
-[![Email](https://img.shields.io/badge/Email-blue)](mailto:nrliangxy@foxmail.com)
```

### Comparing `sharetop-1.0.1/README.md` & `sharetop-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 ## Introduction
 
 [![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/sharetop)
 [![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/sharetop)
-[![Pypi-Install](https://img.shields.io/pypi/dm/sharetop.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypi.python.org/pypi/sharetop)
-[![Github Stars](https://img.shields.io/github/stars/sharetop/sharetop.svg?style=social&label=Star&maxAge=60)](https://github.com/nrliangxy/sharetop)
 
-[`sharetop`](https://github.com/nrliangxy/sharetop) 是由个人打造的用于获取股票、基金、期货数据的免费开源 Python 库，你可以使用它很方便地获取数据以便更好地服务于个人的交易系统需求。
+[`sharetop`](https://github.com/nrliangxy/sharetop) 为个人或者机构提供准确详细的市场数据。用于获取经济市场相关的股票，基金，期货数据，也可以获取具体的行业数据，例如，猪肉周期相关数据，石油进出口数据等。
 
 - [`Source Code`](https://github.com/nrliangxy/sharetop)
 
 ---
 
 ## Installation
 
@@ -160,15 +158,15 @@
 4600  688148   芳源股份  -10.57    31.3   34.39    31.3    33.9    -3.7  26.07  0.56   220.01  188415   620632512.0   35.0   15923562000   2261706043  1.688148   沪A
 4601  300034   钢研高纳  -10.96   43.12   46.81   42.88    46.5   -5.31   7.45  1.77    59.49  323226  1441101824.0  48.43   20959281094  18706911861  0.300034   深A
 4602  300712   永福股份  -13.71    96.9  110.94    95.4   109.0   -15.4   6.96  1.26   511.21  126705  1265152928.0  112.3   17645877600  17645877600  0.300712   深A
 
 [4603 rows x 18 columns]
 ```
 
-- 获取单只股或者多只最新状况
+- 获取单只股或者多只最新股价情况
 
 ```python
 >>> import sharetop as sp
 >>> stock_code = '30033'
 >>> sp.stock.get_real_time_data(stock_code)
         股票名称    股票代码     最新价    最高价    最低价  ...  市盈率(TTM)    市净率     涨跌值  涨跌幅(%)  振幅(%)
 0  同花顺  300033  174.92  198.0  172.3  ...     55.27  15.63 -0.2009   -10.3  13.18
@@ -518,10 +516,11 @@
 1528  动力煤主力  ZCM  2021-08-23  796.8  836.6  843.8  796.8  82954  6.850341e+09  5.97  6.28  49.4  0.0
 
 [1529 rows x 13 columns]
 ```
 
 
 ## Contact
+- 对市场感兴趣的同学可以联系我，对互联网金融感兴趣的同学可以联系我，对市场行业相关数据感兴趣的同学可以联系我，对数据有需求的同学可以联系我。欢迎志同道合的同学联系我
+- 微信：share_top
+<img src="static/sharetop.jpg" width="350">
 
-[![Github](https://img.shields.io/badge/Github-blue?style=social&logo=github)](https://github.com/nrliangxy)
-[![Email](https://img.shields.io/badge/Email-blue)](mailto:nrliangxy@foxmail.com)
```

### Comparing `sharetop-1.0.1/setup.py` & `sharetop-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,12 +22,13 @@
     keywords=about['__keywords__'],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     packages=find_packages(),
     install_requires=require,
     project_urls=about['__project_urls__'],
 )
```

### Comparing `sharetop-1.0.1/sharetop/application/base.py` & `sharetop-1.0.2/sharetop/application/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def deal_real_time_data(self, columns, fields_k_v):
         data = self.json_data['data']
         if not data:
             columns.insert(0, '代码')
             columns.insert(0, '名称')
             return pd.DataFrame(columns=columns)
-        deal_fields_list = ["f43", "f169", "f44", "f45", "f46", "f60", "f71", "f164", "f167", "f169", "f170", "f171"]
+        deal_fields_list = ["f43", "f169", "f44", "f45", "f46", "f60", "f71", "f164", "f167", "f170", "f171"]
         data = self.deal_fields(data, deal_fields_list)
         r = {v: data[k] for k, v in fields_k_v.items() if data.get(k)}
         return pd.DataFrame([r])
 
     def deal_market_realtime(self, columns):
         df = pd.DataFrame(self.json_data['data']['diff'])
         df = df.rename(columns=columns)
```

### Comparing `sharetop-1.0.1/sharetop/core/bond/__init__.py` & `sharetop-1.0.2/sharetop/core/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/bond/config.py` & `sharetop-1.0.2/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/bond/get_bond_info.py` & `sharetop-1.0.2/sharetop/core/bond/get_bond_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/bond/get_bond_public_info.py` & `sharetop-1.0.2/sharetop/core/bond/get_bond_public_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/cache.py` & `sharetop-1.0.2/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/common/config.py` & `sharetop-1.0.2/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/common/getter.py` & `sharetop-1.0.2/sharetop/core/common/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/config.py` & `sharetop-1.0.2/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/fund/__init__.py` & `sharetop-1.0.2/sharetop/core/fund/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/fund/fund_list.py` & `sharetop-1.0.2/sharetop/core/fund/fund_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/fund/get_fund_base_info.py` & `sharetop-1.0.2/sharetop/core/fund/get_fund_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/fund/get_fund_history_data.py` & `sharetop-1.0.2/sharetop/core/fund/get_fund_history_data.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-1.0.2/sharetop/core/fund/get_fund_industry_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-1.0.2/sharetop/core/fund/get_fund_invest_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/fund/get_fund_real_time.py` & `sharetop-1.0.2/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/fund/get_period_change_info.py` & `sharetop-1.0.2/sharetop/core/fund/get_period_change_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-1.0.2/sharetop/core/fund/get_types_percentage_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/futures/get_futures_info.py` & `sharetop-1.0.2/sharetop/core/futures/get_futures_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/stock/bill_monitor.py` & `sharetop-1.0.2/sharetop/core/stock/bill_monitor.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/stock/config.py` & `sharetop-1.0.2/sharetop/core/stock/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/stock/getter.py` & `sharetop-1.0.2/sharetop/core/stock/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/stock/quarterly_report.py` & `sharetop-1.0.2/sharetop/core/stock/quarterly_report.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/stock/rank_list.py` & `sharetop-1.0.2/sharetop/core/stock/rank_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/core/utils.py` & `sharetop-1.0.2/sharetop/core/utils.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/crawl/base.py` & `sharetop-1.0.2/sharetop/crawl/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop/crawl/settings.py` & `sharetop-1.0.2/sharetop/crawl/settings.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.1/sharetop.egg-info/PKG-INFO` & `sharetop-1.0.2/sharetop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
 
 [![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/sharetop)
 [![Pypi Package](https://img.shields.io/pypi/v/sharetop.svg?maxAge=60)](https://pypi.python.org/pypi/sharetop)
-[![Pypi-Install](https://img.shields.io/pypi/dm/sharetop.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypi.python.org/pypi/sharetop)
-[![Github Stars](https://img.shields.io/github/stars/sharetop/sharetop.svg?style=social&label=Star&maxAge=60)](https://github.com/nrliangxy/sharetop)
 
-[`sharetop`](https://github.com/nrliangxy/sharetop) 是由个人打造的用于获取股票、基金、期货数据的免费开源 Python 库，你可以使用它很方便地获取数据以便更好地服务于个人的交易系统需求。
+[`sharetop`](https://github.com/nrliangxy/sharetop) 为个人或者机构提供准确详细的市场数据。用于获取经济市场相关的股票，基金，期货数据，也可以获取具体的行业数据，例如，猪肉周期相关数据，石油进出口数据等。
 
 - [`Source Code`](https://github.com/nrliangxy/sharetop)
 
 ---
 
 ## Installation
 
@@ -179,15 +178,15 @@
 4600  688148   芳源股份  -10.57    31.3   34.39    31.3    33.9    -3.7  26.07  0.56   220.01  188415   620632512.0   35.0   15923562000   2261706043  1.688148   沪A
 4601  300034   钢研高纳  -10.96   43.12   46.81   42.88    46.5   -5.31   7.45  1.77    59.49  323226  1441101824.0  48.43   20959281094  18706911861  0.300034   深A
 4602  300712   永福股份  -13.71    96.9  110.94    95.4   109.0   -15.4   6.96  1.26   511.21  126705  1265152928.0  112.3   17645877600  17645877600  0.300712   深A
 
 [4603 rows x 18 columns]
 ```
 
-- 获取单只股或者多只最新状况
+- 获取单只股或者多只最新股价情况
 
 ```python
 >>> import sharetop as sp
 >>> stock_code = '30033'
 >>> sp.stock.get_real_time_data(stock_code)
         股票名称    股票代码     最新价    最高价    最低价  ...  市盈率(TTM)    市净率     涨跌值  涨跌幅(%)  振幅(%)
 0  同花顺  300033  174.92  198.0  172.3  ...     55.27  15.63 -0.2009   -10.3  13.18
@@ -537,10 +536,11 @@
 1528  动力煤主力  ZCM  2021-08-23  796.8  836.6  843.8  796.8  82954  6.850341e+09  5.97  6.28  49.4  0.0
 
 [1529 rows x 13 columns]
 ```
 
 
 ## Contact
+- 对市场感兴趣的同学可以联系我，对互联网金融感兴趣的同学可以联系我，对市场行业相关数据感兴趣的同学可以联系我，对数据有需求的同学可以联系我。欢迎志同道合的同学联系我
+- 微信：share_top
+<img src="static/sharetop.jpg" width="350">
 
-[![Github](https://img.shields.io/badge/Github-blue?style=social&logo=github)](https://github.com/nrliangxy)
-[![Email](https://img.shields.io/badge/Email-blue)](mailto:nrliangxy@foxmail.com)
```

### Comparing `sharetop-1.0.1/sharetop.egg-info/SOURCES.txt` & `sharetop-1.0.2/sharetop.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -40,8 +40,10 @@
 sharetop/core/stock/getter.py
 sharetop/core/stock/quarterly_report.py
 sharetop/core/stock/rank_list.py
 sharetop/crawl/__init__.py
 sharetop/crawl/base.py
 sharetop/crawl/settings.py
 sharetop/parser/__init__.py
-sharetop/parser/base.py
+sharetop/parser/base.py
+sharetop/test/__init__.py
+sharetop/test/test1.py
```

