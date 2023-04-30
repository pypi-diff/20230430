# Comparing `tmp/dxsp-1.4.3.tar.gz` & `tmp/dxsp-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.4.3.tar", max compression
+gzip compressed data, was "dxsp-1.4.4.tar", max compression
```

## Comparing `dxsp-1.4.3.tar` & `dxsp-1.4.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-04-30 18:22:43.816883 dxsp-1.4.3/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-30 18:22:43.816883 dxsp-1.4.3/README.md
--rw-r--r--   0        0        0       38 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-04-30 18:22:44.588894 dxsp-1.4.3/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/config.py
--rw-r--r--   0        0        0      564 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28463 2023-04-30 18:22:43.816883 dxsp-1.4.3/dxsp/main.py
--rw-r--r--   0        0        0     1015 2023-04-30 18:22:44.588894 dxsp-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-30 18:59:27.426097 dxsp-1.4.4/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-30 18:59:27.426097 dxsp-1.4.4/README.md
+-rw-r--r--   0        0        0       38 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-04-30 18:59:28.206128 dxsp-1.4.4/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/config.py
+-rw-r--r--   0        0        0      564 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28465 2023-04-30 18:59:27.426097 dxsp-1.4.4/dxsp/main.py
+-rw-r--r--   0        0        0     1015 2023-04-30 18:59:28.206128 dxsp-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     4028 1970-01-01 00:00:00.000000 dxsp-1.4.4/PKG-INFO
```

### Comparing `dxsp-1.4.3/LICENSE` & `dxsp-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.3/README.md` & `dxsp-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.3/dxsp/assets/blockchains.py` & `dxsp-1.4.4/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.3/dxsp/default_settings.toml` & `dxsp-1.4.4/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.4.3/dxsp/main.py` & `dxsp-1.4.4/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,18 @@
                  w3: Web3 = None,
                  protocol_type: str = None,
                  dex_exchange: str = None,
                  dex_router: str = None,
                  base_trading_symbol: str = None,
                  amount_trading_option: int = 1,
                  ):
-        """build a web3 object for swap activity"""
+        """build a web3 object for swap"""
         self.logger = logging.getLogger(__name__)
         self.logger.info("DexSwap version: %s", __version__)
-        self.logger.info("Initializing DexSwap object for %s on %s", wallet_address, chain_id)
+        self.logger.info("Initializing DexSwap for %s on %s", wallet_address, chain_id)
 
         self.chain_id = int(chain_id)
         self.logger.debug("self.chain_id %s", self.chain_id)
         if self.chain_id  is None:
             self.logger.warning("self.chain_id not setup")
             return
         blockchain = blockchains[self.chain_id ]
@@ -134,48 +134,48 @@
         response = requests.get(url,params =params,headers=headers)
         #self.logger.debug(f"response _get {response}")
         return response.json()
 
     async def get_quote(self, symbol):
         self.logger.debug(f"get_quote {symbol}")
         asset_in_address = await self.search_contract(symbol)
-        self.logger.debug(f"asset_in_address {asset_in_address}")
+        self.logger.debug("asset_in_address %s", asset_in_address)
         asset_out_symbol = self.base_trading_symbol
         asset_out_address = await self.search_contract(asset_out_symbol)
-        self.logger.debug(f"asset_out_address {asset_out_address}")
+        self.logger.debug("asset_out_address %s",asset_out_address)
         if asset_out_address is None:
             self.logger.debug(f"No Valid Contract {symbol}")
             return
         # asset_out_contract = await self.get_token_contract(asset_out_symbol)
         # asset_out_decimals = asset_out_contract.functions.decimals().call()
         # self.logger.debug(f"asset_out_decimals {asset_out_decimals}")
         try:
             if self.protocol_type == "1inch":
                 asset_out_amount = self.w3.to_wei(1,'ether') #1USDC()
-                self.logger.debug(f"asset_out_amount {asset_out_amount}")
+                self.logger.debug("asset_out_amount %s",asset_out_amount)
                 quote_url = f"{self.dex_url}/quote?fromTokenAddress={asset_in_address}&toTokenAddress={asset_out_address}&amount={asset_out_amount}"
                 quote = await self._get(quote_url)
-                self.logger.debug(f"quote {quote}")
+                self.logger.debug("quote %s" quote)
                 raw_quote = quote['toTokenAmount']
-                self.logger.debug(f"raw_quote {raw_quote}")
+                self.logger.debug("raw_quote %s",raw_quote)
                 asset_quote_decimals = quote['fromToken']['decimals']
-                self.logger.debug(f"asset_quote_decimals {asset_quote_decimals}")
+                self.logger.debug("asset_quote_decimals %s", asset_quote_decimals)
                 quote_readable = self.w3.from_wei(int(raw_quote),'wei') /(10 ** asset_quote_decimals)
                 self.logger.debug(f"quote_readable {quote_readable}")
                 return round(quote_readable,2)
             if self.protocol_type in ["uniswap_v2","uniswap_v3"]:
                 return
         except Exception as e:
             self.logger.debug(f"error get_quote {e}")
             return
 
     async def execute_order(self,direction,instrument,stop_loss=10000,take_profit=10000,quantity=1,amount_trading_option=1,order_type='swap'):
-        self.logger.debug(f"execute_order {direction} {instrument} {order_type}")
+        self.logger.debug("execute_order %s %s %s",direction,instrument, order_type)
         if order_type == 'swap':
-            self.logger.debug(f"execute_order {order_type}")
+            self.logger.debug("execute_order %s",order_type)
             try:
                 asset_out_symbol = self.base_trading_symbol if direction=="BUY" else instrument
                 asset_in_symbol = instrument if direction=="BUY" else self.base_trading_symbol
                 asset_out_contract = await self.get_token_contract(asset_out_symbol)
                 asset_out_decimals = asset_out_contract.functions.decimals().call()
                 asset_out_balance = await self.get_token_balance(asset_out_symbol)
                 if amount_trading_option == 1:
@@ -186,39 +186,39 @@
                 swap = self.get_swap(
                         asset_out_symbol,
                         asset_in_symbol,
                         asset_out_amount
                         )
 
             except Exception as e:
-                self.logger.debug(f"error execute_order {e}")
+                self.logger.debug("error execute_order %s",e)
                 return
 
         if order_type == 'market':
-            self.logger.debug(f"execute_order {order_type}")
+            self.logger.debug("execute_order %s", order_type)
             return
         if order_type == 'limit':
-            self.logger.debug(f"execute_order {order_type}")
+            self.logger.debug("execute_order %s", order_type)
             return
 
     async def get_swap(
                 self, 
                 asset_out_symbol: str, 
                 asset_in_symbol: str,
                 amount: int, 
                 slippage_tolerance_percentage = 2 
         ):
         """main swap function"""
 
-        self.logger.debug(f"get_swap {asset_out_symbol} {asset_in_symbol} {amount}")
+        self.logger.debug("get_swap %s %s %s", asset_out_symbol, asset_in_symbol, amount)
         try:
             #ASSET OUT 
             asset_out_address = await self.search_contract(asset_out_symbol)
             asset_out_contract = await self.get_token_contract(asset_out_symbol)
-            self.logger.debug(f"asset_out_address {asset_out_address} {asset_out_symbol}")
+            self.logger.debug("asset_out_address %s %s",asset_out_address,asset_out_symbol)
             if asset_out_contract is None:
                 return
             asset_out_decimals=asset_out_contract.functions.decimals().call()
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
             self.logger.debug(f"asset_out_balance {asset_out_balance} {asset_out_symbol}")
             if asset_out_balance == 0:
                 self.logger.debug(f"No Money on {asset_out_balance} balance: {asset_out_balance}")
@@ -392,21 +392,21 @@
     async def get_token_contract(self, token):
         self.logger.debug(f"get_token_contract {token}")
         try:
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
             return self.w3.eth.contract(address=token_address, abi=token_abi)
         except Exception as e:
-            self.logger.error(f"error  get_token_contract {e}")
+            self.logger.error("get_token_contract %s",e)
             return
 
 
 ####UTILS
     async def get_approve(self, asset_out_address: str, amount=None):
-        self.logger.debug(f"get_approve {asset_out_address}")
+        self.logger.debug("get_approve %s", asset_out_address)
         if self.protocol_type in ["1inch","1inch_limit"]:
             approval_check_URL = f"{self.dex_url}/approve/allowance?tokenAddress={asset_out_address}&walletAddress={self.wallet_address}"
             approval_response = await self._get(approval_check_URL)
             approval_check = approval_response['allowance']
             if (approval_check==0):
                 approval_URL = f"{self.dex_url}/approve/transaction?tokenAddress={asset_out_address}"
                 approval_response = await self._get(approval_URL)
@@ -419,15 +419,15 @@
                 asset_out_abi = await self.get_abi(asset_out_address)
                 asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)
                 approval_TX = asset_out_contract.functions.approve(self.w3.to_checksum_address(self.router), approved_amount)
                 approval_txHash = await self.get_sign(approval_TX)
                 approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(approval_txHash, timeout=120, poll_latency=0.1)
 
     async def get_sign(self, tx):
-        self.logger.debug(f"get_sign {tx}")
+        self.logger.debug("get_sign %s", tx)
         try:
             if self.protocol_type in ['uniswap_v2']:
                 tx_params = {
                 'from': self.wallet_address,
                 'gas': await self.get_gas(tx),
                 'gasPrice': await self.get_gasPrice(tx),
                 'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
@@ -447,24 +447,24 @@
                 tx['nonce'] = self.w3.eth.get_transaction_count(self.wallet_address)
                 tx['value'] = int(tx['value'])
                 tx['gasPrice'] = await self.get_gasPrice(tx)
             signed = self.w3.eth.account.sign_transaction(tx, self.private_key)
             raw_tx = signed.rawTransaction
             return self.w3.eth.send_raw_transaction(raw_tx)
         except Exception as e:
-            self.logger.debug(f"error get_sign {e}")
+            self.logger.error(" get_sign %s", e)
             return
 
     async def get_gas(self, tx):
-        self.logger.debug(f"get_gas {tx}")
+        self.logger.debug("get_gas %s",tx)
         gasestimate= self.w3.eth.estimate_gas(tx) * 1.25
         return int(self.w3.to_wei(gasestimate,'wei'))
 
     async def get_gasPrice(self, tx):
-        self.logger.debug(f"get_gasPrice {tx}")
+        self.logger.debug("get_gasPrice %s", tx)
         gasprice = self.w3.eth.generate_gas_price()
         return self.w3.to_wei(gasprice,'gwei')
 
     async def get_abi(self,addr):
         self.logger.debug("get_abi %s", addr)
         if self.block_explorer_api is None:
             self.logger.debug("No block_explorer_api")
@@ -482,15 +482,15 @@
                 abi = resp["result"]
                 return abi
             self.logger.debug("No ABI identified Option B needed for contract %s on chain %s",addr,self.chain_id)
             # https://github.com/tintinweb/smart-contract-sanctuary
             #https://raw.githubusercontent.com/tintinweb/smart-contract-sanctuary-optimism/master/contracts/mainnet/1f/1F98431c8aD98523631AE4a59f267346ea31F984_UniswapV3Factory.sol
 
         except Exception as e:
-            self.logger.debug(f"error get_abi {e}")
+            self.logger.error("error get_abi %s", e)
             return
 
 #####USERS
 
     async def get_wallet_auth():
         try:
             return
@@ -536,26 +536,26 @@
                     return msg
         except Exception as e:
             self.logger.error("get_account_balance error: %s", e)
             return 0
             # bal = round(ex.from_wei(bal,'ether'),5)
 
     async def get_account_position(self):
-        self.logger.debug("get_account_position")
+        
         try:
+            self.logger.debug("get_account_position")
             # asset_position_address= await search_contract(asset_out_symbol)
             # asset_position_abi= await fetch_abi_dex(asset_out_address)
             # asset_position_contract = ex.eth.contract(address=asset_out_address, abi=asset_out_abi)
             # open_positions = asset_position_contract.functions.getOpenPositions(walletaddress).call()
             return
         except Exception as e:
             self.logger.error("get_account_position error: %s", e)
             return 0
 
-
     # async def fetch_account_dex(addr):
     #     url = block_explorer_url
     #     query = {'module':'account',
     #             'action':'tokenbalance',
     #             'contractaddress':addr,
     #             'address':walletaddress,
     #             'tag':'latest',
```

### Comparing `dxsp-1.4.3/pyproject.toml` & `dxsp-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.4.3"
+version = "1.4.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.4.3/PKG-INFO` & `dxsp-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.4.3
+Version: 1.4.4
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

