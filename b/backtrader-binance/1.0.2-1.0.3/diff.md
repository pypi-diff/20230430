# Comparing `tmp/backtrader_binance-1.0.2.tar.gz` & `tmp/backtrader_binance-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtrader_binance-1.0.2.tar", last modified: Fri Apr 21 11:27:07 2023, max compression
+gzip compressed data, was "backtrader_binance-1.0.3.tar", last modified: Sun Apr 30 08:00:37 2023, max compression
```

## Comparing `backtrader_binance-1.0.2.tar` & `backtrader_binance-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:27:07.315417 backtrader_binance-1.0.2/
--rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_binance-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    23238 2023-04-21 11:27:07.316416 backtrader_binance-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    21996 2023-04-21 11:23:24.000000 backtrader_binance-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 11:27:07.310416 backtrader_binance-1.0.2/backtrader_binance/
--rw-rw-rw-   0        0        0       40 2021-06-25 01:58:20.000000 backtrader_binance-1.0.2/backtrader_binance/__init__.py
--rw-rw-rw-   0        0        0     6397 2023-04-05 12:42:51.000000 backtrader_binance-1.0.2/backtrader_binance/binance_broker.py
--rw-rw-rw-   0        0        0     5048 2023-04-05 03:54:03.000000 backtrader_binance-1.0.2/backtrader_binance/binance_feed.py
--rw-rw-rw-   0        0        0     6566 2023-04-06 06:34:54.000000 backtrader_binance-1.0.2/backtrader_binance/binance_store.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:27:07.315417 backtrader_binance-1.0.2/backtrader_binance.egg-info/
--rw-rw-rw-   0        0        0    23238 2023-04-21 11:27:07.000000 backtrader_binance-1.0.2/backtrader_binance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-04-21 11:27:07.000000 backtrader_binance-1.0.2/backtrader_binance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:27:07.000000 backtrader_binance-1.0.2/backtrader_binance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-21 11:27:07.000000 backtrader_binance-1.0.2/backtrader_binance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-21 11:27:07.000000 backtrader_binance-1.0.2/backtrader_binance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 11:27:07.316416 backtrader_binance-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2163 2023-04-21 11:27:05.000000 backtrader_binance-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:00:37.121945 backtrader_binance-1.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_binance-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0    23238 2023-04-30 08:00:37.121945 backtrader_binance-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    21996 2023-04-21 11:23:24.000000 backtrader_binance-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 08:00:37.116949 backtrader_binance-1.0.3/backtrader_binance/
+-rw-rw-rw-   0        0        0       40 2021-06-25 01:58:20.000000 backtrader_binance-1.0.3/backtrader_binance/__init__.py
+-rw-rw-rw-   0        0        0     6397 2023-04-05 12:42:51.000000 backtrader_binance-1.0.3/backtrader_binance/binance_broker.py
+-rw-rw-rw-   0        0        0     5048 2023-04-05 03:54:03.000000 backtrader_binance-1.0.3/backtrader_binance/binance_feed.py
+-rw-rw-rw-   0        0        0     6586 2023-04-30 07:50:22.000000 backtrader_binance-1.0.3/backtrader_binance/binance_store.py
+drwxrwxrwx   0        0        0        0 2023-04-30 08:00:37.120945 backtrader_binance-1.0.3/backtrader_binance.egg-info/
+-rw-rw-rw-   0        0        0    23238 2023-04-30 08:00:37.000000 backtrader_binance-1.0.3/backtrader_binance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-04-30 08:00:37.000000 backtrader_binance-1.0.3/backtrader_binance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 08:00:37.000000 backtrader_binance-1.0.3/backtrader_binance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-30 08:00:37.000000 backtrader_binance-1.0.3/backtrader_binance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-30 08:00:37.000000 backtrader_binance-1.0.3/backtrader_binance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-30 08:00:37.122945 backtrader_binance-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2163 2023-04-30 07:55:31.000000 backtrader_binance-1.0.3/setup.py
```

### Comparing `backtrader_binance-1.0.2/LICENSE` & `backtrader_binance-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.2/PKG-INFO` & `backtrader_binance-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtrader_binance
-Version: 1.0.2
+Version: 1.0.3
 Summary: Binance API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_binance
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_binance/blob/master/README.md
 Keywords: trading,development
```

### Comparing `backtrader_binance-1.0.2/README.md` & `backtrader_binance-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.2/backtrader_binance/binance_broker.py` & `backtrader_binance-1.0.3/backtrader_binance/binance_broker.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.2/backtrader_binance/binance_feed.py` & `backtrader_binance-1.0.3/backtrader_binance/binance_feed.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.2/backtrader_binance/binance_store.py` & `backtrader_binance-1.0.3/backtrader_binance/binance_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         (TimeFrame.Minutes, 720): KLINE_INTERVAL_12HOUR,
         (TimeFrame.Days, 1): KLINE_INTERVAL_1DAY,
         (TimeFrame.Days, 3): KLINE_INTERVAL_3DAY,
         (TimeFrame.Weeks, 1): KLINE_INTERVAL_1WEEK,
         (TimeFrame.Months, 1): KLINE_INTERVAL_1MONTH,
     }
 
-    def __init__(self, api_key, api_secret, coin_target, testnet=False, retries=5):  # coin_refer, coin_target
-        self.binance = Client(api_key, api_secret, testnet=testnet)
+    def __init__(self, api_key, api_secret, coin_target, testnet=False, retries=5, tld='com'):  # coin_refer, coin_target
+        self.binance = Client(api_key, api_secret, testnet=testnet, tld=tld)
         self.binance_socket = ThreadedWebsocketManager(api_key, api_secret, testnet=testnet)
         self.binance_socket.daemon = True
         self.binance_socket.start()
         # self.coin_refer = coin_refer
         self.coin_target = coin_target  # USDT
         # self.symbol = coin_refer + coin_target
         self.symbols = []  # symbols
```

### Comparing `backtrader_binance-1.0.2/backtrader_binance.egg-info/PKG-INFO` & `backtrader_binance-1.0.3/backtrader_binance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtrader-binance
-Version: 1.0.2
+Version: 1.0.3
 Summary: Binance API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_binance
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_binance/blob/master/README.md
 Keywords: trading,development
```

### Comparing `backtrader_binance-1.0.2/setup.py` & `backtrader_binance-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the relevant file
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='backtrader_binance',
-      version='1.0.2',
+      version='1.0.3',
       author='wiseplat',
       author_email='oshpagin@gmail.com',
       license='MIT License',
       description='Binance API integration with Backtrader',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/WISEPLAT/backtrader_binance',
```

