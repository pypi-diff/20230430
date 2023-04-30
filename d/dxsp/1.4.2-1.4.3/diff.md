# Comparing `tmp/dxsp-1.4.2.tar.gz` & `tmp/dxsp-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.4.2.tar", max compression
+gzip compressed data, was "dxsp-1.4.3.tar", max compression
```

## Comparing `dxsp-1.4.2.tar` & `dxsp-1.4.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-04-30 16:39:33.036173 dxsp-1.4.2/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-30 16:39:33.036173 dxsp-1.4.2/README.md
--rw-r--r--   0        0        0       38 2023-04-30 16:39:33.036173 dxsp-1.4.2/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-04-30 16:39:33.772182 dxsp-1.4.2/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-30 16:39:33.036173 dxsp-1.4.2/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-04-30 16:39:33.036173 dxsp-1.4.2/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-04-30 16:39:33.036173 dxsp-1.4.2/dxsp/config.py
--rw-r--r--   0        0        0      564 2023-04-30 16:39:33.036173 dxsp-1.4.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28429 2023-04-30 16:39:33.036173 dxsp-1.4.2/dxsp/main.py
--rw-r--r--   0        0        0     1015 2023-04-30 16:39:33.772182 dxsp-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-30 18:22:43.816883 dxsp-1.4.3/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-30 18:22:43.816883 dxsp-1.4.3/README.md
+-rw-r--r--   0        0        0       38 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-04-30 18:22:44.588894 dxsp-1.4.3/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/config.py
+-rw-r--r--   0        0        0      564 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28463 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/main.py
+-rw-r--r--   0        0        0     1015 2023-04-30 18:22:44.588894 dxsp-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.4.3/PKG-INFO
```

### Comparing `dxsp-1.4.2/LICENSE` & `dxsp-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.2/README.md` & `dxsp-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.2/dxsp/assets/blockchains.py` & `dxsp-1.4.3/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.2/dxsp/default_settings.toml` & `dxsp-1.4.3/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.2/dxsp/main.py` & `dxsp-1.4.3/dxsp/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,19 +524,20 @@
             bal_toptoken = await self.get_token_balance(i)
             if bal_toptoken:
                 msg += f"\n💵{bal_toptoken} {i}"
             # bal = round(ex.from_wei(bal,'ether'),5)
 
     async def get_account_balance(self):
         toptokens = ["USDT","USDC"]
-        for i in toptokens:
-            bal_toptoken = await self.get_token_balance(i)
-            if bal_toptoken:
-                msg += f"\n💵{bal_toptoken} {i}"
-                return msg
+        try:
+            for i in toptokens:
+                bal_toptoken = await self.get_token_balance(i)
+                if bal_toptoken:
+                    msg += f"\n💵{bal_toptoken} {i}"
+                    return msg
         except Exception as e:
             self.logger.error("get_account_balance error: %s", e)
             return 0
             # bal = round(ex.from_wei(bal,'ether'),5)
 
     async def get_account_position(self):
         self.logger.debug("get_account_position")
@@ -546,14 +547,15 @@
             # asset_position_contract = ex.eth.contract(address=asset_out_address, abi=asset_out_abi)
             # open_positions = asset_position_contract.functions.getOpenPositions(walletaddress).call()
             return
         except Exception as e:
             self.logger.error("get_account_position error: %s", e)
             return 0
 
+
     # async def fetch_account_dex(addr):
     #     url = block_explorer_url
     #     query = {'module':'account',
     #             'action':'tokenbalance',
     #             'contractaddress':addr,
     #             'address':walletaddress,
     #             'tag':'latest',
```

### Comparing `dxsp-1.4.2/pyproject.toml` & `dxsp-1.4.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.4.2"
+version = "1.4.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.4.2/PKG-INFO` & `dxsp-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.4.2
+Version: 1.4.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

