# Comparing `tmp/zwkit-0.4.8.tar.gz` & `tmp/zwkit-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zwkit-0.4.8.tar", last modified: Mon Mar 13 15:01:43 2023, max compression
+gzip compressed data, was "zwkit-0.4.9.tar", last modified: Mon Mar 13 18:15:59 2023, max compression
```

## Comparing `zwkit-0.4.8.tar` & `zwkit-0.4.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 15:01:43.735956 zwkit-0.4.8/
--rw-r--r--   0 summer     (501) staff       (20)    11357 2023-03-07 02:36:14.000000 zwkit-0.4.8/LICENSE
--rw-r--r--   0 summer     (501) staff       (20)      254 2023-03-13 15:01:43.736203 zwkit-0.4.8/PKG-INFO
-drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 15:01:43.726750 zwkit-0.4.8/data/
--rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-07 05:54:17.000000 zwkit-0.4.8/data/__init__.py
--rw-r--r--   0 summer     (501) staff       (20)    12651 2023-03-12 14:06:04.000000 zwkit-0.4.8/data/dataset.py
-drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 15:01:43.728760 zwkit-0.4.8/kit/
--rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-07 05:54:17.000000 zwkit-0.4.8/kit/__init__.py
--rw-r--r--   0 summer     (501) staff       (20)      402 2023-03-10 12:50:52.000000 zwkit-0.4.8/kit/date_kit.py
--rw-r--r--   0 summer     (501) staff       (20)     1301 2023-03-07 07:23:54.000000 zwkit-0.4.8/kit/num_kit.py
--rw-r--r--   0 summer     (501) staff       (20)      191 2023-03-11 12:58:12.000000 zwkit-0.4.8/kit/path_kit.py
--rw-r--r--   0 summer     (501) staff       (20)      477 2023-03-13 15:01:43.737234 zwkit-0.4.8/setup.cfg
--rw-r--r--   0 summer     (501) staff       (20)       99 2023-03-07 06:01:18.000000 zwkit-0.4.8/setup.py
-drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 15:01:43.730028 zwkit-0.4.8/zw_backtrader/
--rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-09 08:55:13.000000 zwkit-0.4.8/zw_backtrader/__init__.py
-drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 15:01:43.730419 zwkit-0.4.8/zw_backtrader/data/
--rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-09 11:13:39.000000 zwkit-0.4.8/zw_backtrader/data/__init__.py
--rw-r--r--   0 summer     (501) staff       (20)     1969 2023-03-10 08:00:27.000000 zwkit-0.4.8/zw_backtrader/demo.py
-drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 15:01:43.730986 zwkit-0.4.8/zw_backtrader/strategy/
--rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-09 09:38:40.000000 zwkit-0.4.8/zw_backtrader/strategy/__init__.py
--rw-r--r--   0 summer     (501) staff       (20)     7676 2023-03-11 12:29:12.000000 zwkit-0.4.8/zw_backtrader/strategy/strategy.py
-drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 15:01:43.732138 zwkit-0.4.8/zw_backtrader/trade/
--rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-11 08:58:46.000000 zwkit-0.4.8/zw_backtrader/trade/__init__.py
--rw-r--r--   0 summer     (501) staff       (20)      263 2023-03-11 09:14:03.000000 zwkit-0.4.8/zw_backtrader/trade/trade_detail.py
--rw-r--r--   0 summer     (501) staff       (20)      622 2023-03-09 13:20:49.000000 zwkit-0.4.8/zw_backtrader/zw_cerebro.py
--rw-r--r--   0 summer     (501) staff       (20)      640 2023-03-09 18:30:02.000000 zwkit-0.4.8/zw_backtrader/zw_option.py
-drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 15:01:43.735411 zwkit-0.4.8/zwkit.egg-info/
--rw-r--r--   0 summer     (501) staff       (20)      254 2023-03-13 15:01:43.000000 zwkit-0.4.8/zwkit.egg-info/PKG-INFO
--rw-r--r--   0 summer     (501) staff       (20)      566 2023-03-13 15:01:43.000000 zwkit-0.4.8/zwkit.egg-info/SOURCES.txt
--rw-r--r--   0 summer     (501) staff       (20)        1 2023-03-13 15:01:43.000000 zwkit-0.4.8/zwkit.egg-info/dependency_links.txt
--rw-r--r--   0 summer     (501) staff       (20)        1 2023-03-07 05:42:16.000000 zwkit-0.4.8/zwkit.egg-info/not-zip-safe
--rw-r--r--   0 summer     (501) staff       (20)       42 2023-03-13 15:01:43.000000 zwkit-0.4.8/zwkit.egg-info/requires.txt
--rw-r--r--   0 summer     (501) staff       (20)       23 2023-03-13 15:01:43.000000 zwkit-0.4.8/zwkit.egg-info/top_level.txt
+drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 18:15:59.947039 zwkit-0.4.9/
+-rw-r--r--   0 summer     (501) staff       (20)    11357 2023-03-07 02:36:14.000000 zwkit-0.4.9/LICENSE
+-rw-r--r--   0 summer     (501) staff       (20)      254 2023-03-13 18:15:59.947153 zwkit-0.4.9/PKG-INFO
+drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 18:15:59.939185 zwkit-0.4.9/data/
+-rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-07 05:54:17.000000 zwkit-0.4.9/data/__init__.py
+-rw-r--r--   0 summer     (501) staff       (20)    12771 2023-03-13 18:15:40.000000 zwkit-0.4.9/data/dataset.py
+drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 18:15:59.941153 zwkit-0.4.9/kit/
+-rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-07 05:54:17.000000 zwkit-0.4.9/kit/__init__.py
+-rw-r--r--   0 summer     (501) staff       (20)      402 2023-03-10 12:50:52.000000 zwkit-0.4.9/kit/date_kit.py
+-rw-r--r--   0 summer     (501) staff       (20)     1301 2023-03-07 07:23:54.000000 zwkit-0.4.9/kit/num_kit.py
+-rw-r--r--   0 summer     (501) staff       (20)      191 2023-03-11 12:58:12.000000 zwkit-0.4.9/kit/path_kit.py
+-rw-r--r--   0 summer     (501) staff       (20)      477 2023-03-13 18:15:59.947612 zwkit-0.4.9/setup.cfg
+-rw-r--r--   0 summer     (501) staff       (20)       99 2023-03-07 06:01:18.000000 zwkit-0.4.9/setup.py
+drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 18:15:59.943308 zwkit-0.4.9/zw_backtrader/
+-rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-09 08:55:13.000000 zwkit-0.4.9/zw_backtrader/__init__.py
+drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 18:15:59.943895 zwkit-0.4.9/zw_backtrader/data/
+-rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-09 11:13:39.000000 zwkit-0.4.9/zw_backtrader/data/__init__.py
+-rw-r--r--   0 summer     (501) staff       (20)     1969 2023-03-10 08:00:27.000000 zwkit-0.4.9/zw_backtrader/demo.py
+drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 18:15:59.944381 zwkit-0.4.9/zw_backtrader/strategy/
+-rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-09 09:38:40.000000 zwkit-0.4.9/zw_backtrader/strategy/__init__.py
+-rw-r--r--   0 summer     (501) staff       (20)     7676 2023-03-11 12:29:12.000000 zwkit-0.4.9/zw_backtrader/strategy/strategy.py
+drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 18:15:59.944890 zwkit-0.4.9/zw_backtrader/trade/
+-rw-r--r--   0 summer     (501) staff       (20)        0 2023-03-11 08:58:46.000000 zwkit-0.4.9/zw_backtrader/trade/__init__.py
+-rw-r--r--   0 summer     (501) staff       (20)      263 2023-03-11 09:14:03.000000 zwkit-0.4.9/zw_backtrader/trade/trade_detail.py
+-rw-r--r--   0 summer     (501) staff       (20)      622 2023-03-09 13:20:49.000000 zwkit-0.4.9/zw_backtrader/zw_cerebro.py
+-rw-r--r--   0 summer     (501) staff       (20)      640 2023-03-09 18:30:02.000000 zwkit-0.4.9/zw_backtrader/zw_option.py
+drwxr-xr-x   0 summer     (501) staff       (20)        0 2023-03-13 18:15:59.946817 zwkit-0.4.9/zwkit.egg-info/
+-rw-r--r--   0 summer     (501) staff       (20)      254 2023-03-13 18:15:59.000000 zwkit-0.4.9/zwkit.egg-info/PKG-INFO
+-rw-r--r--   0 summer     (501) staff       (20)      566 2023-03-13 18:15:59.000000 zwkit-0.4.9/zwkit.egg-info/SOURCES.txt
+-rw-r--r--   0 summer     (501) staff       (20)        1 2023-03-13 18:15:59.000000 zwkit-0.4.9/zwkit.egg-info/dependency_links.txt
+-rw-r--r--   0 summer     (501) staff       (20)        1 2023-03-07 05:42:16.000000 zwkit-0.4.9/zwkit.egg-info/not-zip-safe
+-rw-r--r--   0 summer     (501) staff       (20)       42 2023-03-13 18:15:59.000000 zwkit-0.4.9/zwkit.egg-info/requires.txt
+-rw-r--r--   0 summer     (501) staff       (20)       23 2023-03-13 18:15:59.000000 zwkit-0.4.9/zwkit.egg-info/top_level.txt
```

### Comparing `zwkit-0.4.8/LICENSE` & `zwkit-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zwkit-0.4.8/data/dataset.py` & `zwkit-0.4.9/data/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,15 +230,16 @@
     def execute(self):
         """
         执行特征工程
         :return:
         """
         symbol_list = self.data['ts_code'].unique()
         columns = self.data.columns
-        for symbol in symbol_list:
+        for index,symbol in enumerate(symbol_list):
+            print("数据进度百分比:%s" % (index / len(symbol_list) * 100), end='\r', flush=True)
             symbol_data = pd.DataFrame(self.data[self.data['ts_code'] == symbol])
             symbol_data.reset_index(drop=True, inplace=True)
             for func in self.features_list:
                 func(symbol_data)
             # 将symbol_data 按照旧列和新列分成2个数据集
             symbol_data_left = symbol_data[columns]
             symbol_data_right = symbol_data[symbol_data.columns[~symbol_data.columns.isin(symbol_data_left.columns)]]
```

### Comparing `zwkit-0.4.8/kit/num_kit.py` & `zwkit-0.4.9/kit/num_kit.py`

 * *Files identical despite different names*

### Comparing `zwkit-0.4.8/zw_backtrader/demo.py` & `zwkit-0.4.9/zw_backtrader/demo.py`

 * *Files identical despite different names*

### Comparing `zwkit-0.4.8/zw_backtrader/strategy/strategy.py` & `zwkit-0.4.9/zw_backtrader/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `zwkit-0.4.8/zw_backtrader/zw_cerebro.py` & `zwkit-0.4.9/zw_backtrader/zw_cerebro.py`

 * *Files identical despite different names*

### Comparing `zwkit-0.4.8/zw_backtrader/zw_option.py` & `zwkit-0.4.9/zw_backtrader/zw_option.py`

 * *Files identical despite different names*

### Comparing `zwkit-0.4.8/zwkit.egg-info/SOURCES.txt` & `zwkit-0.4.9/zwkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

