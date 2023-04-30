# Comparing `tmp/dxsp-1.2.9.tar.gz` & `tmp/dxsp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.2.9.tar", max compression
+gzip compressed data, was "dxsp-1.3.0.tar", max compression
```

## Comparing `dxsp-1.2.9.tar` & `dxsp-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-04-18 19:02:16.965228 dxsp-1.2.9/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-18 19:02:16.965228 dxsp-1.2.9/README.md
--rw-r--r--   0        0        0      136 2023-04-18 19:02:17.621240 dxsp-1.2.9/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-18 19:02:16.965228 dxsp-1.2.9/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8675 2023-04-18 19:02:16.965228 dxsp-1.2.9/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    28389 2023-04-18 19:02:16.965228 dxsp-1.2.9/dxsp/main.py
--rw-r--r--   0        0        0      960 2023-04-18 19:02:17.621240 dxsp-1.2.9/pyproject.toml
--rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 dxsp-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-30 11:46:27.483602 dxsp-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-30 11:46:27.483602 dxsp-1.3.0/README.md
+-rw-r--r--   0        0        0       38 2023-04-30 11:46:27.483602 dxsp-1.3.0/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-04-30 11:46:28.123607 dxsp-1.3.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-30 11:46:27.483602 dxsp-1.3.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-04-30 11:46:27.483602 dxsp-1.3.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      368 2023-04-30 11:46:27.483602 dxsp-1.3.0/dxsp/config.py
+-rw-r--r--   0        0        0      545 2023-04-30 11:46:27.483602 dxsp-1.3.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28140 2023-04-30 11:46:27.483602 dxsp-1.3.0/dxsp/main.py
+-rw-r--r--   0        0        0     1006 2023-04-30 11:46:28.123607 dxsp-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4139 1970-01-01 00:00:00.000000 dxsp-1.3.0/PKG-INFO
```

### Comparing `dxsp-1.2.9/LICENSE` & `dxsp-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.9/README.md` & `dxsp-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.9/dxsp/assets/blockchains.py` & `dxsp-1.3.0/dxsp/assets/blockchains.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+
+# to be used https://github.com/ethereum-lists/chains/tree/master/_data/chains
+
+#https://raw.githubusercontent.com/ethereum-lists/chains/master/_data/chains/eip155-10.json
+#https://chainid.network/chains.json
+
+
 blockchains = {
     #  ETHEREUM
     1: {
         "block_explorer_url": "https://api.etherscan.io/api?",
         "rpc": "https://rpc.ankr.com/eth",
         "uniswap_v2": "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D",
         "uniswap_v3": "0x1f98431c8ad98523631ae4a59f267346ea31f984",
```

### Comparing `dxsp-1.2.9/dxsp/main.py` & `dxsp-1.3.0/dxsp/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from dxsp import __version__
-from dxsp.assets.blockchains import blockchains
-
 import os, json, requests, asyncio, logging
 
-from dotenv import load_dotenv
-
 from web3 import Web3
 from pycoingecko import CoinGeckoAPI
-
 from ping3 import ping
 
+from dxsp.config import settings
+from dxsp import __version__
+from dxsp.assets.blockchains import blockchains
+
+
 class DexSwap:
 
 
     def __init__(self,
                  chain_id: int = 1, 
                  wallet_address: str = None,
                  private_key: str = None,
@@ -160,15 +159,15 @@
                 return round(quote_readable,2)
             if self.protocol_type in ["uniswap_v2","uniswap_v3"]:
                 return
         except Exception as e:
             self.logger.debug(f"error get_quote {e}")
             return
 
-    async def execute_order(self,direction,symbol,stoploss=10000,takeprofit=10000,quantity=1,amount_trading_option=1,order_type='swap'):
+    async def execute_order(self,direction,symbol,stop_loss=10000,take_profit=10000,quantity=1,amount_trading_option=1,order_type='swap'):
         self.logger.debug(f"execute_order {direction} {symbol} {order_type}")
         if order_type == 'swap':
             self.logger.debug(f"execute_order {order_type}")
             try:
                 asset_out_symbol = self.base_trading_symbol if direction=="BUY" else symbol
                 asset_in_symbol = symbol if direction=="BUY" else self.base_trading_symbol
                 asset_out_contract = await self.get_token_contract(asset_out_symbol)
@@ -307,30 +306,25 @@
     #         output_dict = [x for x in assetplatform if x['chain_identifier'] == int(self.chain_id)]
     #         self.logger.debug(f"search_gecko_platform search {output_dict}")
     #         return output_dict[0]['id']
     #     except Exception as e:
     #         self.logger.debug(f"error search_gecko_platform {e}")
     #         return
 
-
     async def search_contract(self, token):
         self.logger.debug(f"search_contract {token}")
-        #📝tokenlist
-        main_list = 'https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json'
-        personal_list = os.getenv("DXSP_TOKEN_LIST", "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json")
-        test_token_list=os.getenv("DXSP_TEST_TOKEN_LIST", "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json")
 
         try:
-            token_contract = await self.get_contract_address(personal_list,token)
+            token_contract = await self.get_contract_address(settings.TOKEN_PERSONAL_LIST,token)
             self.logger.debug(f"personal_list {token} {token_contract}")
             if token_contract is None:
-                token_contract = await self.get_contract_address(test_token_list,token)
+                token_contract = await self.get_contract_address(settings.TOKEN_TESTNET_LIST,token)
                 self.logger.debug(f"test_token_list {token} {token_contract}")
             if token_contract is None:
-                token_contract = await self.get_contract_address(main_list,token)
+                token_contract = await self.get_contract_address(settings.TOKEN_MAINNET_LIST,token)
                 self.logger.debug(f"main_list {token} {token_contract}")
             if token_contract is None:
                 self.logger.debug(f"gecko search {token}")
                 token_contract = await self.search_gecko_contract(token)
             if token_contract is not None:
                 self.logger.debug(f"token_contract {token_contract}")
                 return self.w3.to_checksum_address(token_contract)
@@ -361,28 +355,26 @@
             return
 
     async def search_gecko_contract(self,token):
         self.logger.debug(f"🦎search_gecko_contract {token}")
         self.logger.debug(f"🦎self.gecko_platform {self.gecko_platform}")
         try:
             coin_info = await self.search_gecko(token)
-            #self.logger.debug(f"coin_info {coin_info}")
             if coin_info is not None:
                 coin_info['platforms'][f'{self.gecko_platform}']
                 self.logger.debug(f"🦎search_gecko_coin_info {coin_info} {token}")
                 return coin_info['platforms'][f'{self.gecko_platform}']
         except Exception as e:
             self.logger.debug(f"error search_gecko_contract {e}")
             return
 
     async def get_contract_address(self,token_list_url, symbol):
         self.logger.debug(f"get_contract_address {token_list_url} {symbol}")
         try: 
             token_list = await self._get(token_list_url)
-            #self.logger.debug(f"token_list {token_list}")
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and keyval['chainId'] == self.chain_id):
                     return keyval['address']
         except Exception as e:
             self.logger.debug(f"error get_contract_address {e}")
             return
@@ -478,21 +470,20 @@
             if resp['status']=="1":
                 self.logger.debug(f"ABI found {resp}")
                 abi = resp["result"]
                 return abi
             else:
                 self.logger.debug(f"No ABI identified Option B needed for contract {addr} on chain {self.chain_id}")
                 # https://github.com/tintinweb/smart-contract-sanctuary
+                #https://raw.githubusercontent.com/tintinweb/smart-contract-sanctuary-optimism/master/contracts/mainnet/1f/1F98431c8aD98523631AE4a59f267346ea31F984_UniswapV3Factory.sol
 
         except Exception as e:
             self.logger.debug(f"error get_abi {e}")
             return
 
-
-
 #####USERS
 
     async def get_wallet_auth():
         try:
             return
         except Exception as e:
             self.logger.error(msg=f"get_wallet_auth error: {e}")
```

### Comparing `dxsp-1.2.9/pyproject.toml` & `dxsp-1.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.2.9"
+version = "1.3.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
 "Changelog" =  "https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst"
 "Support" =  "https://github.com/mraniki/dxsp/discussions"
 "Issues" =  "https://github.com/mraniki/dxsp/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.9,<3.11"
 asyncio = "*"
-python-dotenv = "*"
-web3 = ">=6.*"
+web3 = ">=6.0.0"
 pycoingecko = "*"
 ping3 = "*"
 dynaconf = "*"
-many-abis = "*"
+web3client = ">=1.1.8"
+many-abis = ">=0.1.7"
+apollox-connector-python = "*"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = ["pyproject.toml:version","dxsp/__init__.py:__version__"]
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
-
-
```

### Comparing `dxsp-1.2.9/PKG-INFO` & `dxsp-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.2.9
+Version: 1.3.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: apollox-connector-python
 Requires-Dist: asyncio
 Requires-Dist: dynaconf
-Requires-Dist: many-abis
+Requires-Dist: many-abis (>=0.1.7)
 Requires-Dist: ping3
 Requires-Dist: pycoingecko
-Requires-Dist: python-dotenv
-Requires-Dist: web3 (>=6)
+Requires-Dist: web3 (>=6.0.0)
+Requires-Dist: web3client (>=1.1.8)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
```

