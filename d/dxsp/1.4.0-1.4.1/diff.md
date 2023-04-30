# Comparing `tmp/dxsp-1.4.0.tar.gz` & `tmp/dxsp-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.4.0.tar", max compression
+gzip compressed data, was "dxsp-1.4.1.tar", max compression
```

## Comparing `dxsp-1.4.0.tar` & `dxsp-1.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-04-30 12:29:17.434830 dxsp-1.4.0/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-30 12:29:17.434830 dxsp-1.4.0/README.md
--rw-r--r--   0        0        0       38 2023-04-30 12:29:17.438830 dxsp-1.4.0/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-04-30 12:29:18.318831 dxsp-1.4.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-30 12:29:17.438830 dxsp-1.4.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-04-30 12:29:17.438830 dxsp-1.4.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      368 2023-04-30 12:29:17.438830 dxsp-1.4.0/dxsp/config.py
--rw-r--r--   0        0        0      545 2023-04-30 12:29:17.438830 dxsp-1.4.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28265 2023-04-30 12:29:17.438830 dxsp-1.4.0/dxsp/main.py
--rw-r--r--   0        0        0      994 2023-04-30 12:29:18.318831 dxsp-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 dxsp-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-30 15:29:27.673239 dxsp-1.4.1/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-30 15:29:27.677239 dxsp-1.4.1/README.md
+-rw-r--r--   0        0        0       38 2023-04-30 15:29:27.677239 dxsp-1.4.1/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-04-30 15:29:28.529249 dxsp-1.4.1/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-30 15:29:27.677239 dxsp-1.4.1/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-04-30 15:29:27.677239 dxsp-1.4.1/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      368 2023-04-30 15:29:27.677239 dxsp-1.4.1/dxsp/config.py
+-rw-r--r--   0        0        0      545 2023-04-30 15:29:27.677239 dxsp-1.4.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28391 2023-04-30 15:29:27.677239 dxsp-1.4.1/dxsp/main.py
+-rw-r--r--   0        0        0     1006 2023-04-30 15:29:28.529249 dxsp-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4139 1970-01-01 00:00:00.000000 dxsp-1.4.1/PKG-INFO
```

### Comparing `dxsp-1.4.0/LICENSE` & `dxsp-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.0/README.md` & `dxsp-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.0/dxsp/assets/blockchains.py` & `dxsp-1.4.1/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.0/dxsp/default_settings.toml` & `dxsp-1.4.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.0/dxsp/main.py` & `dxsp-1.4.1/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import json
 import requests
 import logging
 
 from web3 import Web3
 from pycoingecko import CoinGeckoAPI
-#from ping3 import ping
+from ping3 import ping
 
 from dxsp.config import settings
 from dxsp import __version__
 from dxsp.assets.blockchains import blockchains
 
 class DexSwap:
 
@@ -98,14 +98,16 @@
             if (
                 self.dex_exchange is None
                 or self.dex_exchange != blockchain["uniswap_v3"]
             ):
                 self.router = blockchain["uniswap_v2"]
             else:
                 self.router = blockchain["uniswap_v3"]
+        else:
+            self.router = self.dex_router 
         self.logger.debug(f"self.router {self.router}")
 
         self.name = "TBD"
         self.logger.debug(f"self.name {self.name}")        
 
         self.base_trading_symbol = base_trading_symbol
         if self.base_trading_symbol is None:
@@ -193,20 +195,22 @@
         if order_type == 'market':
             self.logger.debug(f"execute_order {order_type}")
             return
         if order_type == 'limit':
             self.logger.debug(f"execute_order {order_type}")
             return
 
-    async def get_swap(self, 
-            asset_out_symbol: str, 
-            asset_in_symbol: str,
-            amount: int, 
-            slippage_tolerance_percentage = 2 
+    async def get_swap(
+                self, 
+                asset_out_symbol: str, 
+                asset_in_symbol: str,
+                amount: int, 
+                slippage_tolerance_percentage = 2 
         ):
+        """main swap function"""
 
         self.logger.debug(f"get_swap {asset_out_symbol} {asset_in_symbol} {amount}")
         try:
             
             #ASSET OUT 
             asset_out_address = await self.search_contract(asset_out_symbol)
             asset_out_contract = await self.get_token_contract(asset_out_symbol)
@@ -243,58 +247,58 @@
             if self.protocol_type in ["1inch"]:
                 swap_url = f"{self.dex_url}/swap?fromTokenAddress={asset_out_address}&toTokenAddress={asset_in_address}&amount={transaction_amount}&fromAddress={self.wallet_address}&slippage={slippage}"
                 swap_TX = await self._get(swap_url)
                 TX_status_code = swap_TX['statusCode']
                 if TX_status_code != 200:
                     return
             #UNISWAP V2
-            if self.protocol_type ['uniswap_v2']:
+            if self.protocol_type in ["uniswap_v2"]:
                 order_path_dex=[asset_out_address, asset_in_address]
                 router_abi = await self.get_abi(self.router)
                 router_instance = self.w3.eth.contract(address=self.w3.to_checksum_address(self.router), abi=self.router_abi)
                 deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
                 transaction_min_amount  = int(router_instance.functions.getAmountsOut(transaction_amount, order_path_dex).call()[1])
                 swap_TX = router_instance.functions.swapExactTokensForTokens(transaction_amount,transaction_min_amount,order_path_dex,self.wallet_address,deadline)
             #1INCH LIMIT
-            if self.protocol_type ["1inch_limit"]:
+            if self.protocol_type in ["1inch_limit"]:
                  return
                 # encoded_message = encode_structured_data(eip712_data)
                 # signed_message = await sign_transaction_dex(encoded_message)
                 # # this is the limit order that will be broadcast to the limit order API
                 # limit_order = {
                 #     "orderHash": signed_message.messageHash.hex(),
                 #     "signature": signed_message.signature.hex(),
                 #     "data": order_data,
                 # }
                 # limit_order_url = dex_1inch_limit_api + str(chain_id) +"/limit-order" # make sure to change the chain_id if you are not using ETH mainnet
                 # response = requests.post(url=limit_order_url,headers={"accept": "application/json, text/plain, */*", "content-type": "application/json"}, json=limit_order)
 
             #UNISWAP V3
-            if self.protocol_type ['uniswap_v3']:
+            if self.protocol_type in ['uniswap_v3']:
                 return
             if swap_TX:
                 self.logger.debug(f"swap_TX {swap_TX}")
                 signed_TX = await self.get_sign(swap_TX)
                 transaction_hash = str(self.w3.to_hex(signed_TX))
                 #transaction_results = await self.get_block_explorer_status(transaction_hash)
                 transaction_hash_details = self.w3.wait_for_transaction_receipt(transaction_hash, timeout=120, poll_latency=0.1)
-                if(transaction_hash_details['status'] == "1"):
+                if transaction_hash_details['status'] == "1":
                     transaction_blockNumber = transaction_hash_details['blockNumber']
                     transaction_receipt = self.w3.eth.get_transaction_receipt(transaction_hash)
                     transaction_block = self.w3.eth.get_block(blockNumber)
                     order={}
                     order['id'] = transaction_receipt['transactionHash']
                     order['timestamp'] = transaction_block['timestamp']
                     order['symbol'] = asset_out_symbol
                     order['contract'] = asset_out_address
                     order['amount'] = transaction_amount
                     order['fee'] = transaction_receipt['gasUsed']
-                    order['price'] = 'na'
-                    order['confirmation'] = 'na'
-                                #response+= f"\n➕ Size: {round(ex.from_wei(transaction_amount, 'ether'),5)}\n⚫️ Entry: {await fetch_gecko_asset_price(asset_in_symbol)}USD \nℹ️ {txHash}\n⛽️ {txHashDetail['gasUsed']}\n🗓️ {datetime.now()}"
+                    order['price'] = "TBD"
+                    order['confirmation'] = "TBD"
+                    #response+= f"\n➕ Size: {round(ex.from_wei(transaction_amount, 'ether'),5)}\n⚫️ Entry: {await fetch_gecko_asset_price(asset_in_symbol)}USD \nℹ️ {txHash}\n⛽️ {txHashDetail['gasUsed']}\n🗓️ {datetime.now()}"
             #logger.info(msg=f"{response}")
                     return order
         except Exception as e:
             self.logger.debug(f"error get_swap {e}")
             return
 
     async def get_block_explorer_status(self,txHash):
@@ -371,15 +375,15 @@
                 return coin_info['platforms'][f'{self.gecko_platform}']
         except Exception as e:
             self.logger.debug(f"error search_gecko_contract {e}")
             return
 
     async def get_contract_address(self,token_list_url, symbol):
         self.logger.debug(f"get_contract_address {token_list_url} {symbol}")
-        try: 
+        try:
             token_list = await self._get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and keyval['chainId'] == self.chain_id):
                     return keyval['address']
         except Exception as e:
             self.logger.debug(f"error get_contract_address {e}")
@@ -408,18 +412,18 @@
                 approval_response = await self._get(approval_URL)
         elif self.protocol_type in ["uniswap_v2","uniswap_v3"]:
             asset_out_abi= await self.get_abi(asset_out_address)
             asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)           
             approval_check = asset_out_contract.functions.allowance(self.w3.to_checksum_address(self.wallet_address), self.w3.to_checksum_address(self.router)).call()
             if (approval_check==0):
                 approved_amount = (self.w3.to_wei(2**64-1,'ether'))
-                asset_out_abi = await fetch_abi_dex(asset_out_address)
+                asset_out_abi = await self.get_abi(asset_out_address)
                 asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)
                 approval_TX = asset_out_contract.functions.approve(self.w3.to_checksum_address(self.router), approved_amount)
-                approval_txHash = await sign_transaction_dex(approval_TX)
+                approval_txHash = await self.get_sign(approval_TX)
                 approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(approval_txHash, timeout=120, poll_latency=0.1)
 
     async def get_sign(self, tx):
         self.logger.debug(f"get_sign {tx}")
         try:
             if self.protocol_type in ['uniswap_v2']:
                 tx_params = {
@@ -498,19 +502,19 @@
     async def get_token_balance(self, token):
         self.logger.debug(f"get_token_balance {token}")
         try:
             token_address = await self.search_contract(token)
             token_abi =  await self.get_abi(token_address)
             token_contract = self.w3.eth.contract(address=token_address, abi=token_abi)
             token_balance = token_contract.functions.balanceOf(self.wallet_address).call()
-            logger.debug(msg=f"token_address {token_address} token_balance {token_balance}")
+            self.logger.debug(msg=f"token_address {token_address} token_balance {token_balance}")
             # (ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
             return 0 if token_balance <=0 or token_balance is None else token_balance
         except Exception as e:
-            logger.error(msg=f"{token} get_token_balance error: {e}")
+            self.logger.error(msg=f"{token} get_token_balance error: {e}")
             return 0
 
     async def get_basecoin_balance(self):
         bal_base_trading_symbol = await self.get_token_balance(self.base_trading_symbol)
             # return round(ex.from_wei(await fetch_token_balance(basesymbol), 'ether'), 5)
         return bal_base_trading_symbol
         # bal = round(ex.from_wei(bal,'ether'),5)
@@ -536,15 +540,15 @@
         try:
             # asset_position_address= await search_contract(asset_out_symbol)
             # asset_position_abi= await fetch_abi_dex(asset_out_address)
             # asset_position_contract = ex.eth.contract(address=asset_out_address, abi=asset_out_abi)
             # open_positions = asset_position_contract.functions.getOpenPositions(walletaddress).call()
             return
         except Exception as e:
-            logger.error(msg=f"get_account_position error: {e}")
+            self. logger.error(msg=f"get_account_position error: {e}")
             return 0
 
     # async def fetch_account_dex(addr):
     #     url = block_explorer_url
     #     query = {'module':'account',
     #             'action':'tokenbalance',
     #             'contractaddress':addr,
@@ -572,8 +576,7 @@
 #         fetch_tokeninfo = gecko_api.get_coin_info_from_contract_address_by_id(id=f'{coin_platform}',contract_address=asset_in_address)
 #         logger.debug(msg=f"fetch_tokeninfo {fetch_tokeninfo}")
 #         asset_out_cg_quote = fetch_tokeninfo['market_data']['current_price']['usd']
 #         asset_out_cg_name = fetch_tokeninfo['name']
 #         return f"{asset_out_cg_name}\n🦎{asset_out_cg_quote} USD"
 #     except Exception:
 #         return
-
```

### Comparing `dxsp-1.4.0/pyproject.toml` & `dxsp-1.4.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.4.0"
+version = "1.4.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -17,14 +17,15 @@
 asyncio = "*"
 dynaconf = "*"
 web3 = ">=6.0.0"
 pycoingecko = "*"
 web3client = ">=1.1.8"
 many-abis = ">=0.1.7"
 apollox-connector-python = "*"
+ping3 = "*"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dxsp-1.4.0/PKG-INFO` & `dxsp-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.4.0
+Version: 1.4.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: apollox-connector-python
 Requires-Dist: asyncio
 Requires-Dist: dynaconf
 Requires-Dist: many-abis (>=0.1.7)
+Requires-Dist: ping3
 Requires-Dist: pycoingecko
 Requires-Dist: web3 (>=6.0.0)
 Requires-Dist: web3client (>=1.1.8)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
```

