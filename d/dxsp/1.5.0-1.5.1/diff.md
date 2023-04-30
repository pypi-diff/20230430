# Comparing `tmp/dxsp-1.5.0.tar.gz` & `tmp/dxsp-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.5.0.tar", max compression
+gzip compressed data, was "dxsp-1.5.1.tar", max compression
```

## Comparing `dxsp-1.5.0.tar` & `dxsp-1.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-04-30 19:15:08.567402 dxsp-1.5.0/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-30 19:15:08.567402 dxsp-1.5.0/README.md
--rw-r--r--   0        0        0       38 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-04-30 19:15:09.539409 dxsp-1.5.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/config.py
--rw-r--r--   0        0        0      564 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28465 2023-04-30 19:15:08.567402 dxsp-1.5.0/dxsp/main.py
--rw-r--r--   0        0        0     1015 2023-04-30 19:15:09.539409 dxsp-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-30 20:46:32.534129 dxsp-1.5.1/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-30 20:46:32.534129 dxsp-1.5.1/README.md
+-rw-r--r--   0        0        0       38 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-04-30 20:46:33.422140 dxsp-1.5.1/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/config.py
+-rw-r--r--   0        0        0      564 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    27903 2023-04-30 20:46:32.534129 dxsp-1.5.1/dxsp/main.py
+-rw-r--r--   0        0        0     1015 2023-04-30 20:46:33.422140 dxsp-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.5.1/PKG-INFO
```

### Comparing `dxsp-1.5.0/LICENSE` & `dxsp-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.0/README.md` & `dxsp-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.0/dxsp/assets/blockchains.py` & `dxsp-1.5.1/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.0/dxsp/default_settings.toml` & `dxsp-1.5.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.5.0/dxsp/main.py` & `dxsp-1.5.1/dxsp/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """
  DEX SWAP Main
 """
-import os
 import json
-import requests
 import logging
+import os
 
-from web3 import Web3
-from pycoingecko import CoinGeckoAPI
-from ping3 import ping
-
-from dxsp.config import settings
+import requests
 from dxsp import __version__
 from dxsp.assets.blockchains import blockchains
+from dxsp.config import settings
+from ping3 import ping
+from pycoingecko import CoinGeckoAPI
+from web3 import Web3
+
 
 class DexSwap:
     """Do a swap."""
 
     def __init__(self,
                  chain_id: int = 1, 
-                 wallet_address: str = None,
-                 private_key: str = None,
-                 block_explorer_api: str = None,
-                 block_explorer_url: str = None,
-                 rpc: str = None,
-                 w3: Web3 = None,
-                 protocol_type: str = None,
-                 dex_exchange: str = None,
-                 dex_router: str = None,
-                 base_trading_symbol: str = None,
+                 wallet_address: str | None = None,
+                 private_key: str | None = None,
+                 block_explorer_api: str | None = None,
+                 block_explorer_url: str | None = None,
+                 rpc: str | None = None,
+                 w3: Web3 | None = None,
+                 protocol_type: str | None = None,
+                 dex_exchange: str | None = None,
+                 dex_router: str | None = None,
+                 base_trading_symbol: str | None = None,
                  amount_trading_option: int = 1,
                  ):
         """build a web3 object for swap"""
         self.logger = logging.getLogger(__name__)
         self.logger.info("DexSwap version: %s", __version__)
         self.logger.info("Initializing DexSwap for %s on %s", wallet_address, chain_id)
 
@@ -132,44 +132,44 @@
         headers = { "User-Agent": "Mozilla/5.0" }
         self.logger.debug("_get url %s",url)
         response = requests.get(url,params =params,headers=headers)
         #self.logger.debug(f"response _get {response}")
         return response.json()
 
     async def get_quote(self, symbol):
-        self.logger.debug(f"get_quote {symbol}")
+        self.logger.debug("get_quote %s",symbol)
         asset_in_address = await self.search_contract(symbol)
         self.logger.debug("asset_in_address %s", asset_in_address)
         asset_out_symbol = self.base_trading_symbol
         asset_out_address = await self.search_contract(asset_out_symbol)
         self.logger.debug("asset_out_address %s",asset_out_address)
         if asset_out_address is None:
-            self.logger.debug(f"No Valid Contract {symbol}")
+            self.logger.warning("No Valid Contract %s",symbol)
             return
         # asset_out_contract = await self.get_token_contract(asset_out_symbol)
         # asset_out_decimals = asset_out_contract.functions.decimals().call()
         # self.logger.debug(f"asset_out_decimals {asset_out_decimals}")
         try:
             if self.protocol_type == "1inch":
                 asset_out_amount = self.w3.to_wei(1,'ether') #1USDC()
                 self.logger.debug("asset_out_amount %s",asset_out_amount)
                 quote_url = f"{self.dex_url}/quote?fromTokenAddress={asset_in_address}&toTokenAddress={asset_out_address}&amount={asset_out_amount}"
                 quote = await self._get(quote_url)
-                self.logger.debug("quote %s" quote)
+                self.logger.debug("quote %s",quote)
                 raw_quote = quote['toTokenAmount']
                 self.logger.debug("raw_quote %s",raw_quote)
                 asset_quote_decimals = quote['fromToken']['decimals']
                 self.logger.debug("asset_quote_decimals %s", asset_quote_decimals)
                 quote_readable = self.w3.from_wei(int(raw_quote),'wei') /(10 ** asset_quote_decimals)
-                self.logger.debug(f"quote_readable {quote_readable}")
+                self.logger.debug("quote_readable %s",quote_readable)
                 return round(quote_readable,2)
             if self.protocol_type in ["uniswap_v2","uniswap_v3"]:
                 return
         except Exception as e:
-            self.logger.debug(f"error get_quote {e}")
+            self.logger.error("get_quote %s", e)
             return
 
     async def execute_order(self,direction,instrument,stop_loss=10000,take_profit=10000,quantity=1,amount_trading_option=1,order_type='swap'):
         self.logger.debug("execute_order %s %s %s",direction,instrument, order_type)
         if order_type == 'swap':
             self.logger.debug("execute_order %s",order_type)
             try:
@@ -215,34 +215,34 @@
             asset_out_address = await self.search_contract(asset_out_symbol)
             asset_out_contract = await self.get_token_contract(asset_out_symbol)
             self.logger.debug("asset_out_address %s %s",asset_out_address,asset_out_symbol)
             if asset_out_contract is None:
                 return
             asset_out_decimals=asset_out_contract.functions.decimals().call()
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
-            self.logger.debug(f"asset_out_balance {asset_out_balance} {asset_out_symbol}")
+            self.logger.debug("asset_out_balance %s",asset_out_balance)
             if asset_out_balance == 0:
-                self.logger.debug(f"No Money on {asset_out_balance} balance: {asset_out_balance}")
+                self.logger.warning("No Money")
                 return 
             #ASSETS IN 
             asset_in_address = await self.search_contract(asset_in_symbol)
-            self.logger.debug(f"asset_out_address {asset_out_address} {asset_in_symbol}")
+            self.logger.debug("asset_in_address %s", asset_in_address)
             if asset_in_address is None:
                 return
 
             #AMOUNT
             asset_out_decimals = asset_out_contract.functions.decimals().call()
-            self.logger.debug(f"asset_out_decimals {asset_out_decimals}")
+            self.logger.debug("asset_out_decimals %s",asset_out_decimals)
             asset_out_amount = amount * 10 ** asset_out_decimals
             slippage = slippage_tolerance_percentage # defaulted to 2% slippage if not given
-            self.logger.debug(f"slippage {slippage}")
+            self.logger.debug("slippage %s",slippage)
             asset_out_amount_converted = self.w3.to_wei(amount,'ether')
 
             transaction_amount = int((asset_out_amount_converted *(slippage/100)))
-            self.logger.debug(f"transaction_amount {transaction_amount}")
+            self.logger.debug("transaction_amount %s",transaction_amount)
 
             #VERIFY IF ASSET OUT IS APPROVED otherwise get it approved
             await self.get_approve(asset_out_address)
 
             #1INCH
             if self.protocol_type in ["1inch"]:
                 swap_url = f"{self.dex_url}/swap?fromTokenAddress={asset_out_address}&toTokenAddress={asset_in_address}&amount={transaction_amount}&fromAddress={self.wallet_address}&slippage={slippage}"
@@ -250,15 +250,15 @@
                 TX_status_code = swap_TX['statusCode']
                 if TX_status_code != 200:
                     return
             #UNISWAP V2
             if self.protocol_type in ["uniswap_v2"]:
                 order_path_dex=[asset_out_address, asset_in_address]
                 router_abi = await self.get_abi(self.router)
-                router_instance = self.w3.eth.contract(address=self.w3.to_checksum_address(self.router), abi=self.router_abi)
+                router_instance = self.w3.eth.contract(address=self.w3.to_checksum_address(self.router), abi=router_abi)
                 deadline = self.w3.eth.get_block("latest")["timestamp"] + 3600
                 transaction_min_amount  = int(router_instance.functions.getAmountsOut(transaction_amount, order_path_dex).call()[1])
                 swap_TX = router_instance.functions.swapExactTokensForTokens(transaction_amount,transaction_min_amount,order_path_dex,self.wallet_address,deadline)
             #1INCH LIMIT
             if self.protocol_type in ["1inch_limit"]:
                  return
                 # encoded_message = encode_structured_data(eip712_data)
@@ -272,43 +272,43 @@
                 # limit_order_url = dex_1inch_limit_api + str(chain_id) +"/limit-order" # make sure to change the chain_id if you are not using ETH mainnet
                 # response = requests.post(url=limit_order_url,headers={"accept": "application/json, text/plain, */*", "content-type": "application/json"}, json=limit_order)
 
             #UNISWAP V3
             if self.protocol_type in ['uniswap_v3']:
                 return
             if swap_TX:
-                self.logger.debug(f"swap_TX {swap_TX}")
+                self.logger.debug("swap_TX %s",swap_TX)
                 signed_TX = await self.get_sign(swap_TX)
                 transaction_hash = str(self.w3.to_hex(signed_TX))
                 #transaction_results = await self.get_block_explorer_status(transaction_hash)
                 transaction_hash_details = self.w3.wait_for_transaction_receipt(transaction_hash, timeout=120, poll_latency=0.1)
                 if transaction_hash_details['status'] == "1":
                     transaction_blockNumber = transaction_hash_details['blockNumber']
                     transaction_receipt = self.w3.eth.get_transaction_receipt(transaction_hash)
-                    transaction_block = self.w3.eth.get_block(blockNumber)
+                    transaction_block = self.w3.eth.get_block(transaction_blockNumber)
                     order={}
                     order['id'] = transaction_receipt['transactionHash']
                     order['timestamp'] = transaction_block['timestamp']
-                    order['symbol'] = asset_out_symbol
+                    order['instrument'] = asset_out_symbol
                     order['contract'] = asset_out_address
                     order['amount'] = transaction_amount
                     order['fee'] = transaction_receipt['gasUsed']
                     order['price'] = "TBD"
                     order['confirmation'] = "TBD"
                     #response+= f"\n➕ Size: {round(ex.from_wei(transaction_amount, 'ether'),5)}\n⚫️ Entry: {await fetch_gecko_asset_price(asset_in_symbol)}USD \nℹ️ {txHash}\n⛽️ {txHashDetail['gasUsed']}\n🗓️ {datetime.now()}"
             #logger.info(msg=f"{response}")
                     return order
         except Exception as e:
-            self.logger.debug(f"error get_swap {e}")
+            self.logger.error("get_swap %s",e)
             return
 
     async def get_block_explorer_status(self,txHash):
-        self.logger.debug(f"get_block_explorer_status {txHash}")
+        self.logger.debug("get_block_explorer_status %s",txHash)
         checkTransactionSuccessURL = f"{self.block_explorer_url}?module=transaction&action=gettxreceiptstatus&txhash={txHash}&apikey={self.block_explorer_api}"
-        checkTransactionRequest =  self.get(checkTransactionSuccessURL)
+        checkTransactionRequest =  self._get(checkTransactionSuccessURL)
         return checkTransactionRequest['status']
 
 ####CONTRACT SEARCH
 
     # async def search_gecko_platform(self):
     #     self.logger.debug("search_gecko_platform")
     #     try:
@@ -317,84 +317,84 @@
     #         self.logger.debug(f"search_gecko_platform search {output_dict}")
     #         return output_dict[0]['id']
     #     except Exception as e:
     #         self.logger.debug(f"error search_gecko_platform {e}")
     #         return
 
     async def search_contract(self, token):
-        self.logger.debug(f"search_contract {token}")
+        self.logger.debug("search_contract")
 
         try:
             token_contract = await self.get_contract_address(settings.TOKEN_PERSONAL_LIST,token)
-            self.logger.debug(f"personal_list {token} {token_contract}")
+            self.logger.debug("personal_list")
             if token_contract is None:
                 token_contract = await self.get_contract_address(settings.TOKEN_TESTNET_LIST,token)
-                self.logger.debug(f"test_token_list {token} {token_contract}")
+                self.logger.debug("test_token_list")
             if token_contract is None:
                 token_contract = await self.get_contract_address(settings.TOKEN_MAINNET_LIST,token)
-                self.logger.debug(f"main_list {token} {token_contract}")
+                self.logger.debug("main_list")
             if token_contract is None:
-                self.logger.debug(f"gecko search {token}")
+                self.logger.debug("gecko search")
                 token_contract = await self.search_gecko_contract(token)
             if token_contract is not None:
-                self.logger.debug(f"token_contract {token_contract}")
+                self.logger.debug("token_contract %s",token_contract)
                 return self.w3.to_checksum_address(token_contract)
             else:
-                self.logger.debug(f"no contract found for {token} on chain {self.chain_id}")
+                self.logger.debug("no contract found for %s",token)
         except Exception as e:
-            self.logger.debug(f"error search_contract {e} token {token} token_contract {token_contract}")
+            self.logger.error("search_contract %s",e)
             return
 
     async def search_gecko(self,token):
-        self.logger.debug(f"search_gecko {token}")
+        self.logger.debug("search_gecko %s",token)
         try:
             search_results = self.gecko_api.search(query=token)
             search_dict = search_results['coins']
             #self.logger.debug(f"search_dict {search_dict}")
             filtered_dict = [x for x in search_dict if x['symbol'] == token.upper()]
             api_dict = [ sub['api_symbol'] for sub in filtered_dict ]
-            self.logger.debug(f"api_dict {api_dict}")
+            self.logger.debug("api_dict %s",api_dict)
             for i in api_dict:
                 coin_dict = self.gecko_api.get_coin_by_id(i)
                 try:
                     if coin_dict['platforms'][f'{self.gecko_platform}'] is not None:
                         return coin_dict
                 except KeyError:
                     pass
         except Exception as e:
-            self.logger.debug(f"error search_gecko {e}")
+            self.logger.error("search_gecko %s", e)
             return
 
     async def search_gecko_contract(self,token):
-        self.logger.debug(f"🦎search_gecko_contract {token}")
-        self.logger.debug(f"🦎self.gecko_platform {self.gecko_platform}")
+        self.logger.debug("🦎search_gecko_contract %s", token)
+        self.logger.debug("🦎self.gecko_platform %s", self.gecko_platform)
         try:
             coin_info = await self.search_gecko(token)
             if coin_info is not None:
                 coin_info['platforms'][f'{self.gecko_platform}']
-                self.logger.debug(f"🦎search_gecko_coin_info {coin_info} {token}")
+                self.logger.debug("🦎search_gecko_coin_info %s",token)
                 return coin_info['platforms'][f'{self.gecko_platform}']
         except Exception as e:
-            self.logger.debug(f"error search_gecko_contract {e}")
+            self.logger.error(f"error search_gecko_contract {e}")
             return
 
     async def get_contract_address(self,token_list_url, symbol):
-        self.logger.debug(f"get_contract_address {token_list_url} {symbol}")
+        self.logger.debug("get_contract_address %s %s",token_list_url, symbol)
         try:
             token_list = await self._get(token_list_url)
             token_search = token_list['tokens']
             for keyval in token_search:
                 if (keyval['symbol'] == symbol and keyval['chainId'] == self.chain_id):
                     return keyval['address']
         except Exception as e:
-            self.logger.debug(f"error get_contract_address {e}")
+            self.logger.debug("get_contract_address %s", e)
             return
 
     async def get_token_contract(self, token):
-        self.logger.debug(f"get_token_contract {token}")
+        self.logger.debug("get_token_contract %s",token)
         try:
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
             return self.w3.eth.contract(address=token_address, abi=token_abi)
         except Exception as e:
             self.logger.error("get_token_contract %s",e)
             return
@@ -421,23 +421,15 @@
                 approval_TX = asset_out_contract.functions.approve(self.w3.to_checksum_address(self.router), approved_amount)
                 approval_txHash = await self.get_sign(approval_TX)
                 approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(approval_txHash, timeout=120, poll_latency=0.1)
 
     async def get_sign(self, tx):
         self.logger.debug("get_sign %s", tx)
         try:
-            if self.protocol_type in ['uniswap_v2']:
-                tx_params = {
-                'from': self.wallet_address,
-                'gas': await self.get_gas(tx),
-                'gasPrice': await self.get_gasPrice(tx),
-                'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
-                }
-                tx = tx.build_transaction(tx_params)
-            elif self.protocol_type in ['uniswap_v3']:
+            if self.protocol_type in ['uniswap_v2','uniswap_v3']:
                 tx_params = {
                 'from': self.wallet_address,
                 'gas': await self.get_gas(tx),
                 'gasPrice': await self.get_gasPrice(tx),
                 'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
                 }
                 tx = tx.build_transaction(tx_params)
@@ -463,15 +455,15 @@
         self.logger.debug("get_gasPrice %s", tx)
         gasprice = self.w3.eth.generate_gas_price()
         return self.w3.to_wei(gasprice,'gwei')
 
     async def get_abi(self,addr):
         self.logger.debug("get_abi %s", addr)
         if self.block_explorer_api is None:
-            self.logger.debug("No block_explorer_api")
+            self.logger.warning("No block_explorer_api")
         try:
             params = {
                 "module": "contract",
                 "action": "getabi",
                 "address": addr,
                 "apikey": self.block_explorer_api }
             headers = { "User-Agent": "Mozilla/5.0" }
@@ -487,20 +479,20 @@
 
         except Exception as e:
             self.logger.error("error get_abi %s", e)
             return
 
 #####USERS
 
-    async def get_wallet_auth():
-        try:
-            return
-        except Exception as e:
-            self.logger.error("get_wallet_auth error: %s",e)
-            return
+    # async def get_wallet_auth(self):
+    #     try:
+    #         return
+    #     except Exception as e:
+    #         self.logger.error("get_wallet_auth error: %s",e)
+    #         return
 
     async def get_token_balance(self, token):
         self.logger.debug("get_token_balance %s", token)
         try:
             token_address = await self.search_contract(token)
             token_abi =  await self.get_abi(token_address)
             token_contract = self.w3.eth.contract(address=token_address, abi=token_abi)
```

### Comparing `dxsp-1.5.0/pyproject.toml` & `dxsp-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.5.0"
+version = "1.5.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.5.0/PKG-INFO` & `dxsp-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.5.0
+Version: 1.5.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

