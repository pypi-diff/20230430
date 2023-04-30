# Comparing `tmp/sharetop-1.0.2.tar.gz` & `tmp/sharetop-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharetop-1.0.2.tar", last modified: Sun Apr 30 13:35:14 2023, max compression
+gzip compressed data, was "sharetop-1.0.3.tar", last modified: Sun Apr 30 13:59:36 2023, max compression
```

## Comparing `sharetop-1.0.2.tar` & `sharetop-1.0.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.343973 sharetop-1.0.2/
--rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    39033 2023-04-30 13:35:14.343973 sharetop-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    37774 2023-04-29 10:56:21.000000 sharetop-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-30 13:35:14.343973 sharetop-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.246222 sharetop-1.0.2/sharetop/
--rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.0.2/sharetop/__init__.py
--rw-rw-rw-   0        0        0      386 2023-04-30 13:35:02.000000 sharetop-1.0.2/sharetop/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.291674 sharetop-1.0.2/sharetop/api/
--rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.0.2/sharetop/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.293537 sharetop-1.0.2/sharetop/application/
--rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.0.2/sharetop/application/__init__.py
--rw-rw-rw-   0        0        0     4157 2023-04-30 13:28:10.000000 sharetop-1.0.2/sharetop/application/base.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.297234 sharetop-1.0.2/sharetop/core/
--rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.0.2/sharetop/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.304887 sharetop-1.0.2/sharetop/core/bond/
--rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.0.2/sharetop/core/bond/__init__.py
--rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.0.2/sharetop/core/bond/config.py
--rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.0.2/sharetop/core/bond/get_bond_info.py
--rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.0.2/sharetop/core/bond/get_bond_public_info.py
--rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.0.2/sharetop/core/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.307726 sharetop-1.0.2/sharetop/core/common/
--rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.0.2/sharetop/core/common/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.0.2/sharetop/core/common/config.py
--rw-rw-rw-   0        0        0    12266 2023-04-27 15:28:32.000000 sharetop-1.0.2/sharetop/core/common/getter.py
--rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.0.2/sharetop/core/config.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.321313 sharetop-1.0.2/sharetop/core/fund/
--rw-rw-rw-   0        0        0      707 2023-04-25 21:15:03.000000 sharetop-1.0.2/sharetop/core/fund/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.0.2/sharetop/core/fund/config.py
--rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.0.2/sharetop/core/fund/fund_list.py
--rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.0.2/sharetop/core/fund/get_fund_base_info.py
--rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.0.2/sharetop/core/fund/get_fund_history_data.py
--rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.0.2/sharetop/core/fund/get_fund_industry_info.py
--rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.0.2/sharetop/core/fund/get_fund_invest_info.py
--rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.0.2/sharetop/core/fund/get_fund_real_time.py
--rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.0.2/sharetop/core/fund/get_period_change_info.py
--rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.0.2/sharetop/core/fund/get_types_percentage_info.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.323606 sharetop-1.0.2/sharetop/core/futures/
--rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.0.2/sharetop/core/futures/__init__.py
--rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.0.2/sharetop/core/futures/get_futures_info.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.331253 sharetop-1.0.2/sharetop/core/stock/
--rw-rw-rw-   0        0        0      491 2023-04-25 21:15:03.000000 sharetop-1.0.2/sharetop/core/stock/__init__.py
--rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.0.2/sharetop/core/stock/bill_monitor.py
--rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.0.2/sharetop/core/stock/config.py
--rw-rw-rw-   0        0        0    14300 2023-04-27 15:24:55.000000 sharetop-1.0.2/sharetop/core/stock/getter.py
--rw-rw-rw-   0        0        0    10125 2023-04-28 01:45:42.000000 sharetop-1.0.2/sharetop/core/stock/quarterly_report.py
--rw-rw-rw-   0        0        0    10050 2023-04-27 15:28:32.000000 sharetop-1.0.2/sharetop/core/stock/rank_list.py
--rw-rw-rw-   0        0        0     6341 2023-04-27 13:30:47.000000 sharetop-1.0.2/sharetop/core/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.334877 sharetop-1.0.2/sharetop/crawl/
--rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.0.2/sharetop/crawl/__init__.py
--rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.0.2/sharetop/crawl/base.py
--rw-rw-rw-   0        0        0     2704 2023-04-24 00:30:13.000000 sharetop-1.0.2/sharetop/crawl/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.336761 sharetop-1.0.2/sharetop/parser/
--rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.0.2/sharetop/parser/__init__.py
--rw-rw-rw-   0        0        0      419 2023-04-10 00:57:53.000000 sharetop-1.0.2/sharetop/parser/base.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.339946 sharetop-1.0.2/sharetop/test/
--rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.0.2/sharetop/test/__init__.py
--rw-rw-rw-   0        0        0      261 2023-04-30 13:20:34.000000 sharetop-1.0.2/sharetop/test/test1.py
-drwxrwxrwx   0        0        0        0 2023-04-30 13:35:14.289507 sharetop-1.0.2/sharetop.egg-info/
--rw-rw-rw-   0        0        0    39033 2023-04-30 13:35:14.000000 sharetop-1.0.2/sharetop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1501 2023-04-30 13:35:14.000000 sharetop-1.0.2/sharetop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 13:35:14.000000 sharetop-1.0.2/sharetop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-30 13:35:14.000000 sharetop-1.0.2/sharetop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-30 13:35:14.000000 sharetop-1.0.2/sharetop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.691547 sharetop-1.0.3/
+-rw-rw-rw-   0        0        0     1066 2023-04-26 14:07:21.000000 sharetop-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    39033 2023-04-30 13:59:36.656552 sharetop-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    37774 2023-04-29 10:56:21.000000 sharetop-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-30 13:59:36.691547 sharetop-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-29 06:50:50.000000 sharetop-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.116289 sharetop-1.0.3/sharetop/
+-rw-rw-rw-   0        0        0      202 2023-04-26 04:55:09.000000 sharetop-1.0.3/sharetop/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-04-30 13:59:33.000000 sharetop-1.0.3/sharetop/__version__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.182171 sharetop-1.0.3/sharetop/api/
+-rw-rw-rw-   0        0        0      148 2023-04-26 00:55:53.000000 sharetop-1.0.3/sharetop/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.196872 sharetop-1.0.3/sharetop/application/
+-rw-rw-rw-   0        0        0       33 2023-04-21 11:53:52.000000 sharetop-1.0.3/sharetop/application/__init__.py
+-rw-rw-rw-   0        0        0     4146 2023-04-30 13:59:24.000000 sharetop-1.0.3/sharetop/application/base.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.205594 sharetop-1.0.3/sharetop/core/
+-rw-rw-rw-   0        0        0        0 2023-04-08 05:23:09.000000 sharetop-1.0.3/sharetop/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.303960 sharetop-1.0.3/sharetop/core/bond/
+-rw-rw-rw-   0        0        0      758 2023-04-25 21:15:03.000000 sharetop-1.0.3/sharetop/core/bond/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-24 04:28:03.000000 sharetop-1.0.3/sharetop/core/bond/config.py
+-rw-rw-rw-   0        0        0     9356 2023-04-26 00:46:59.000000 sharetop-1.0.3/sharetop/core/bond/get_bond_info.py
+-rw-rw-rw-   0        0        0    19572 2023-04-26 00:53:29.000000 sharetop-1.0.3/sharetop/core/bond/get_bond_public_info.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 05:06:06.000000 sharetop-1.0.3/sharetop/core/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.329184 sharetop-1.0.3/sharetop/core/common/
+-rw-rw-rw-   0        0        0      188 2023-04-27 15:24:55.000000 sharetop-1.0.3/sharetop/core/common/__init__.py
+-rw-rw-rw-   0        0        0     6271 2023-04-24 05:04:06.000000 sharetop-1.0.3/sharetop/core/common/config.py
+-rw-rw-rw-   0        0        0    12266 2023-04-30 13:59:24.000000 sharetop-1.0.3/sharetop/core/common/getter.py
+-rw-rw-rw-   0        0        0      750 2023-04-09 05:42:43.000000 sharetop-1.0.3/sharetop/core/config.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.480328 sharetop-1.0.3/sharetop/core/fund/
+-rw-rw-rw-   0        0        0      707 2023-04-25 21:15:03.000000 sharetop-1.0.3/sharetop/core/fund/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-22 11:35:14.000000 sharetop-1.0.3/sharetop/core/fund/config.py
+-rw-rw-rw-   0        0        0     2509 2023-04-26 00:53:29.000000 sharetop-1.0.3/sharetop/core/fund/fund_list.py
+-rw-rw-rw-   0        0        0     1471 2023-04-26 00:53:29.000000 sharetop-1.0.3/sharetop/core/fund/get_fund_base_info.py
+-rw-rw-rw-   0        0        0     2377 2023-04-27 15:28:32.000000 sharetop-1.0.3/sharetop/core/fund/get_fund_history_data.py
+-rw-rw-rw-   0        0        0     3601 2023-04-27 01:02:03.000000 sharetop-1.0.3/sharetop/core/fund/get_fund_industry_info.py
+-rw-rw-rw-   0        0        0     5387 2023-04-27 15:28:32.000000 sharetop-1.0.3/sharetop/core/fund/get_fund_invest_info.py
+-rw-rw-rw-   0        0        0     1466 2023-04-22 03:27:53.000000 sharetop-1.0.3/sharetop/core/fund/get_fund_real_time.py
+-rw-rw-rw-   0        0        0     2401 2023-04-26 00:53:29.000000 sharetop-1.0.3/sharetop/core/fund/get_period_change_info.py
+-rw-rw-rw-   0        0        0     2336 2023-04-26 00:53:29.000000 sharetop-1.0.3/sharetop/core/fund/get_types_percentage_info.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.515791 sharetop-1.0.3/sharetop/core/futures/
+-rw-rw-rw-   0        0        0      272 2023-04-27 14:23:26.000000 sharetop-1.0.3/sharetop/core/futures/__init__.py
+-rw-rw-rw-   0        0        0     9922 2023-04-28 01:45:42.000000 sharetop-1.0.3/sharetop/core/futures/get_futures_info.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.591429 sharetop-1.0.3/sharetop/core/stock/
+-rw-rw-rw-   0        0        0      491 2023-04-25 21:15:03.000000 sharetop-1.0.3/sharetop/core/stock/__init__.py
+-rw-rw-rw-   0        0        0     4606 2023-04-28 01:45:42.000000 sharetop-1.0.3/sharetop/core/stock/bill_monitor.py
+-rw-rw-rw-   0        0        0     1163 2023-04-13 13:52:05.000000 sharetop-1.0.3/sharetop/core/stock/config.py
+-rw-rw-rw-   0        0        0    14300 2023-04-27 15:24:55.000000 sharetop-1.0.3/sharetop/core/stock/getter.py
+-rw-rw-rw-   0        0        0    10088 2023-04-30 13:59:24.000000 sharetop-1.0.3/sharetop/core/stock/quarterly_report.py
+-rw-rw-rw-   0        0        0    10010 2023-04-30 13:59:24.000000 sharetop-1.0.3/sharetop/core/stock/rank_list.py
+-rw-rw-rw-   0        0        0     6341 2023-04-27 13:30:47.000000 sharetop-1.0.3/sharetop/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.626407 sharetop-1.0.3/sharetop/crawl/
+-rw-rw-rw-   0        0        0       29 2023-04-09 23:19:21.000000 sharetop-1.0.3/sharetop/crawl/__init__.py
+-rw-rw-rw-   0        0        0      683 2023-04-09 23:19:21.000000 sharetop-1.0.3/sharetop/crawl/base.py
+-rw-rw-rw-   0        0        0     2704 2023-04-24 00:30:13.000000 sharetop-1.0.3/sharetop/crawl/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.652329 sharetop-1.0.3/sharetop/parser/
+-rw-rw-rw-   0        0        0       27 2023-04-10 00:54:05.000000 sharetop-1.0.3/sharetop/parser/__init__.py
+-rw-rw-rw-   0        0        0      419 2023-04-10 00:57:53.000000 sharetop-1.0.3/sharetop/parser/base.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.655192 sharetop-1.0.3/sharetop/test/
+-rw-rw-rw-   0        0        0        0 2023-04-29 10:57:35.000000 sharetop-1.0.3/sharetop/test/__init__.py
+-rw-rw-rw-   0        0        0      261 2023-04-30 13:54:58.000000 sharetop-1.0.3/sharetop/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-04-30 13:59:36.179856 sharetop-1.0.3/sharetop.egg-info/
+-rw-rw-rw-   0        0        0    39033 2023-04-30 13:59:36.000000 sharetop-1.0.3/sharetop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1501 2023-04-30 13:59:36.000000 sharetop-1.0.3/sharetop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 13:59:36.000000 sharetop-1.0.3/sharetop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-30 13:59:36.000000 sharetop-1.0.3/sharetop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-30 13:59:36.000000 sharetop-1.0.3/sharetop.egg-info/top_level.txt
```

### Comparing `sharetop-1.0.2/LICENSE` & `sharetop-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/PKG-INFO` & `sharetop-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.0.2
+Version: 1.0.3
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-1.0.2/README.md` & `sharetop-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/setup.py` & `sharetop-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/application/base.py` & `sharetop-1.0.3/sharetop/application/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         data = self.json_data['data']
         if not data:
             columns.insert(0, '代码')
             columns.insert(0, '名称')
             return pd.DataFrame(columns=columns)
         deal_fields_list = ["f43", "f169", "f44", "f45", "f46", "f60", "f71", "f164", "f167", "f170", "f171"]
         data = self.deal_fields(data, deal_fields_list)
-        r = {v: data[k] for k, v in fields_k_v.items() if data.get(k)}
+        r = {v: data.get(k) for k, v in fields_k_v.items()}
         return pd.DataFrame([r])
 
     def deal_market_realtime(self, columns):
         df = pd.DataFrame(self.json_data['data']['diff'])
         df = df.rename(columns=columns)
         df: pd.DataFrame = df[columns.values()]
         df['行情ID'] = df['市场编号'].astype(str) + '.' + df['代码'].astype(str)
```

### Comparing `sharetop-1.0.2/sharetop/core/bond/__init__.py` & `sharetop-1.0.3/sharetop/core/bond/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/bond/config.py` & `sharetop-1.0.3/sharetop/core/bond/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/bond/get_bond_info.py` & `sharetop-1.0.3/sharetop/core/bond/get_bond_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/bond/get_bond_public_info.py` & `sharetop-1.0.3/sharetop/core/bond/get_bond_public_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/cache.py` & `sharetop-1.0.3/sharetop/core/cache.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/common/config.py` & `sharetop-1.0.3/sharetop/core/common/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/common/getter.py` & `sharetop-1.0.3/sharetop/core/common/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/config.py` & `sharetop-1.0.3/sharetop/core/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/fund/__init__.py` & `sharetop-1.0.3/sharetop/core/fund/__init__.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/fund/fund_list.py` & `sharetop-1.0.3/sharetop/core/fund/fund_list.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/fund/get_fund_base_info.py` & `sharetop-1.0.3/sharetop/core/fund/get_fund_base_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/fund/get_fund_history_data.py` & `sharetop-1.0.3/sharetop/core/fund/get_fund_history_data.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/fund/get_fund_industry_info.py` & `sharetop-1.0.3/sharetop/core/fund/get_fund_industry_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/fund/get_fund_invest_info.py` & `sharetop-1.0.3/sharetop/core/fund/get_fund_invest_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/fund/get_fund_real_time.py` & `sharetop-1.0.3/sharetop/core/fund/get_fund_real_time.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/fund/get_period_change_info.py` & `sharetop-1.0.3/sharetop/core/fund/get_period_change_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/fund/get_types_percentage_info.py` & `sharetop-1.0.3/sharetop/core/fund/get_types_percentage_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/futures/get_futures_info.py` & `sharetop-1.0.3/sharetop/core/futures/get_futures_info.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/stock/bill_monitor.py` & `sharetop-1.0.3/sharetop/core/stock/bill_monitor.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/stock/config.py` & `sharetop-1.0.3/sharetop/core/stock/config.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/stock/getter.py` & `sharetop-1.0.3/sharetop/core/stock/getter.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/core/stock/quarterly_report.py` & `sharetop-1.0.3/sharetop/core/stock/quarterly_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,14 @@
             ('sty', 'ALL'),
             ('token', '894050c76af8597a853f5b408b759f5d'),
             # ! 只选沪深A股
             ('filter', f'(SECURITY_TYPE_CODE in ("058001001","058001008")){date}'),
         )
         url = "".join(quarterly_report_url_list)
         response = requests_obj.get(url, params, user_agent=True)
-        print("url:", response.url)
         # response = session.get(url, headers=EASTMONEY_REQUEST_HEADERS, params=params)
         items = jsonpath(response.json(), '$..data[:]')
         if not items:
             break
         df = pd.DataFrame(items)
         dfs.append(df)
         page += 1
```

### Comparing `sharetop-1.0.2/sharetop/core/stock/rank_list.py` & `sharetop-1.0.3/sharetop/core/stock/rank_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 
             url = ''.join(rank_list_list)
             response = requests_obj.get(
                 url, params, user_agent=False
             )
             if bar is None:
                 pages = jsonpath(response.json(), '$..pages')
-                print("pages:", pages)
                 if pages and pages[0] != 1:
                     total = pages[0]
                     bar = tqdm(total=int(total))
             if bar is not None:
                 bar.update()
 
             items = jsonpath(response.json(), '$..data[:]')
```

### Comparing `sharetop-1.0.2/sharetop/core/utils.py` & `sharetop-1.0.3/sharetop/core/utils.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/crawl/base.py` & `sharetop-1.0.3/sharetop/crawl/base.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop/crawl/settings.py` & `sharetop-1.0.3/sharetop/crawl/settings.py`

 * *Files identical despite different names*

### Comparing `sharetop-1.0.2/sharetop.egg-info/PKG-INFO` & `sharetop-1.0.3/sharetop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharetop
-Version: 1.0.2
+Version: 1.0.3
 Summary: Provide data related to the economic market
 Home-page: https://github.com/nrliangxy/sharetop
 Author: nrliangxy
 Author-email: nrliangxy@foxmail.com
 License: MIT
 Project-URL: Source, https://github.com/nrliangxy/sharetop
 Keywords: data,finance,quant,stock,fund,futures,share
```

### Comparing `sharetop-1.0.2/sharetop.egg-info/SOURCES.txt` & `sharetop-1.0.3/sharetop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

