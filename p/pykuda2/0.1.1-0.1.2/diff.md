# Comparing `tmp/pykuda2-0.1.1.tar.gz` & `tmp/pykuda2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykuda2-0.1.1.tar", max compression
+gzip compressed data, was "pykuda2-0.1.2.tar", max compression
```

## Comparing `pykuda2-0.1.1.tar` & `pykuda2-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1079 2023-04-17 17:54:48.089774 pykuda2-0.1.1/LICENSE
--rw-r--r--   0        0        0      220 2023-04-29 17:24:46.960487 pykuda2-0.1.1/README.md
--rw-r--r--   0        0        0      643 2023-04-10 15:02:27.716925 pykuda2-0.1.1/pykuda2/__init__.py
--rw-r--r--   0        0        0    13111 2023-04-29 12:20:49.931535 pykuda2-0.1.1/pykuda2/base.py
--rw-r--r--   0        0        0      249 2023-03-28 14:27:15.707706 pykuda2-0.1.1/pykuda2/exceptions.py
--rw-r--r--   0        0        0     3124 2023-04-30 00:14:25.238824 pykuda2-0.1.1/pykuda2/kuda.py
--rw-r--r--   0        0        0    11458 2023-04-28 10:50:55.010172 pykuda2-0.1.1/pykuda2/utils.py
--rw-r--r--   0        0        0        0 2023-03-28 23:10:17.676968 pykuda2-0.1.1/pykuda2/wrappers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-28 23:10:41.728988 pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/__init__.py
--rw-r--r--   0        0        0    10357 2023-04-29 16:52:55.541312 pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/accounts.py
--rw-r--r--   0        0        0     9065 2023-04-29 14:41:14.962004 pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/billing_and_betting.py
--rw-r--r--   0        0        0    13516 2023-04-29 14:41:14.938665 pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/card.py
--rw-r--r--   0        0        0     6547 2023-04-29 14:44:39.428125 pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/gift_card.py
--rw-r--r--   0        0        0     9514 2023-04-29 14:44:39.444793 pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/instant_settlement_service.py
--rw-r--r--   0        0        0    21854 2023-04-29 14:52:12.971156 pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/savings.py
--rw-r--r--   0        0        0    22617 2023-04-29 16:40:40.823535 pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/transaction.py
--rw-r--r--   0        0        0        0 2023-03-28 23:10:32.769446 pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/__init__.py
--rw-r--r--   0        0        0    10246 2023-04-29 14:18:43.688686 pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/accounts.py
--rw-r--r--   0        0        0     9024 2023-04-29 14:18:43.685352 pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/billing_and_betting.py
--rw-r--r--   0        0        0    12967 2023-04-29 14:41:15.008683 pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/card.py
--rw-r--r--   0        0        0     6484 2023-04-29 13:57:51.924011 pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/gift_card.py
--rw-r--r--   0        0        0     9449 2023-04-29 14:18:43.745351 pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/instant_settlement_service.py
--rw-r--r--   0        0        0    21647 2023-04-29 14:18:39.992082 pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/savings.py
--rw-r--r--   0        0        0    22454 2023-04-29 16:40:40.843535 pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/transaction.py
--rw-r--r--   0        0        0      749 2023-04-30 00:14:25.225492 pykuda2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 pykuda2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-04-17 17:54:48.089774 pykuda2-0.1.2/LICENSE
+-rw-r--r--   0        0        0      220 2023-04-29 17:24:46.960487 pykuda2-0.1.2/README.md
+-rw-r--r--   0        0        0      643 2023-04-10 15:02:27.716925 pykuda2-0.1.2/pykuda2/__init__.py
+-rw-r--r--   0        0        0    13111 2023-04-29 12:20:49.931535 pykuda2-0.1.2/pykuda2/base.py
+-rw-r--r--   0        0        0      249 2023-03-28 14:27:15.707706 pykuda2-0.1.2/pykuda2/exceptions.py
+-rw-r--r--   0        0        0     3124 2023-04-30 00:14:25.238824 pykuda2-0.1.2/pykuda2/kuda.py
+-rw-r--r--   0        0        0    11472 2023-04-30 16:14:45.424849 pykuda2-0.1.2/pykuda2/utils.py
+-rw-r--r--   0        0        0        0 2023-03-28 23:10:17.676968 pykuda2-0.1.2/pykuda2/wrappers/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-28 23:10:41.728988 pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/__init__.py
+-rw-r--r--   0        0        0    10357 2023-04-29 16:52:55.541312 pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/accounts.py
+-rw-r--r--   0        0        0     9924 2023-04-30 16:09:22.525382 pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/billing_and_betting.py
+-rw-r--r--   0        0        0    13516 2023-04-29 14:41:14.938665 pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/card.py
+-rw-r--r--   0        0        0     7745 2023-04-30 16:09:22.545382 pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/gift_card.py
+-rw-r--r--   0        0        0     9937 2023-04-30 16:09:22.565382 pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/instant_settlement_service.py
+-rw-r--r--   0        0        0    24243 2023-04-30 16:09:22.552049 pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/savings.py
+-rw-r--r--   0        0        0    25006 2023-04-30 16:14:45.408182 pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/transaction.py
+-rw-r--r--   0        0        0        0 2023-03-28 23:10:32.769446 pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/__init__.py
+-rw-r--r--   0        0        0    10246 2023-04-29 14:18:43.688686 pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/accounts.py
+-rw-r--r--   0        0        0     9825 2023-04-30 16:09:22.578715 pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/billing_and_betting.py
+-rw-r--r--   0        0        0    12967 2023-04-29 14:41:15.008683 pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/card.py
+-rw-r--r--   0        0        0     7682 2023-04-30 16:09:22.555382 pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/gift_card.py
+-rw-r--r--   0        0        0     9872 2023-04-30 16:09:22.562049 pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/instant_settlement_service.py
+-rw-r--r--   0        0        0    24036 2023-04-30 16:09:22.585382 pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/savings.py
+-rw-r--r--   0        0        0    24843 2023-04-30 16:14:45.428182 pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/transaction.py
+-rw-r--r--   0        0        0      790 2023-04-30 15:44:28.397531 pykuda2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 pykuda2-0.1.2/PKG-INFO
```

### Comparing `pykuda2-0.1.1/LICENSE` & `pykuda2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pykuda2-0.1.1/pykuda2/__init__.py` & `pykuda2-0.1.2/pykuda2/__init__.py`

 * *Files identical despite different names*

### Comparing `pykuda2-0.1.1/pykuda2/base.py` & `pykuda2-0.1.2/pykuda2/base.py`

 * *Files identical despite different names*

### Comparing `pykuda2-0.1.1/pykuda2/kuda.py` & `pykuda2-0.1.2/pykuda2/kuda.py`

 * *Files identical despite different names*

### Comparing `pykuda2-0.1.1/pykuda2/utils.py` & `pykuda2-0.1.2/pykuda2/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         long_code: The beneficiary's long code.
         reference: A unique identifier for the transfer.
     """
 
     account_number: str
     account_name: str
     beneficiary_bank_code: str
-    amount: int
+    amount: Union[int, float]
     bank_code: str
     narration: str
     bank_name: str
     long_code: str
     reference: str
 
     def to_dict(self) -> dict:
```

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/accounts.py` & `pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/accounts.py`

 * *Files identical despite different names*

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/billing_and_betting.py` & `pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/billing_and_betting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Optional, Union
 
 from pykuda2.base import BaseAsyncAPIWrapper
 from pykuda2.utils import BillType, ServiceType, APIResponse
 
 
 class AsyncBillingAndBetting(BaseAsyncAPIWrapper):
     async def get_bill_type_options(
@@ -68,24 +68,27 @@
             service_type=ServiceType.VERIFY_BILL_CUSTOMER,
             data=data,
             request_reference=request_reference,
         )
 
     async def purchase_bill(
         self,
-        amount: int,
+        amount: Union[int, float],
         bill_item_identifier: str,
         customer_identifier: str,
         phone_number: Optional[str] = None,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Purchase a bill from your main account.
 
         Args:
-            amount: Bill amount.
+            amount: Bill amount. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             bill_item_identifier: The Kuda bill unique identifier
             customer_identifier: The customer's unique identifier
             phone_number: The customer's phone number It is not required
                 if you're purchasing airtime.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
@@ -107,25 +110,28 @@
             data=data,
             request_reference=request_reference,
         )
 
     async def purchase_bill_from_virtual_account(
         self,
         tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         bill_item_identifier: str,
         phone_number: str,
         customer_identifier: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Purchase a bill from your virtual account.
 
         Args:
             tracking_reference: The customer virtual account Identifier.
-            amount: Bill amount.
+            amount: Bill amount. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             bill_item_identifier: The Kuda bill unique identifier
             customer_identifier: The customer's unique identifier
             phone_number: The customer's phone number It is not required
                 if you're purchasing airtime.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
@@ -154,14 +160,15 @@
         bill_request_ref: Optional[str],
         bill_response_reference: Optional[str],
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieve the status of a bill purchase.
 
         Args:
+            bill_request_ref: The bill request reference.
             bill_response_reference: The bill reference gotten from purchasing the bill.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
```

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/card.py` & `pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/card.py`

 * *Files identical despite different names*

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/gift_card.py` & `pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/gift_card.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-from typing import Optional
+from typing import Optional, Union
 
-from pykuda2.base import BaseAsyncAPIWrapper
+from pykuda2.base import BaseAPIWrapper
 from pykuda2.utils import ServiceType, APIResponse
 
 
-class AsyncGiftCard(BaseAsyncAPIWrapper):
-    async def get_gift_cards(self, request_reference: Optional[str] = None) -> APIResponse:
+class GiftCard(BaseAPIWrapper):
+    def get_gift_cards(self, request_reference: Optional[str] = None) -> APIResponse:
         """Retrieves a curated list of gift cards supported by Kuda.
 
         Args:
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.GET_GIFT_CARD, request_reference=request_reference
         )
 
-    async def purchase_gift_card(
+    def purchase_gift_card(
         self,
-        amount: int,
+        amount: Union[int, float],
         customer_name: str,
         customer_mobile: str,
         customer_email: str,
         biller_identifier: str,
         note: Optional[str] = None,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Buy gift cards from the admin account
 
         Args:
-            amount: The gift card amount to be purchased. It could be in USD/ GBP/ EUR/ NGN/ AED , e.t.c.
+            amount: The gift card amount to be purchased. It could be in USD/ GBP/ EUR/ NGN/ AED , e.t.c. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             customer_name: Name of the customer receiving the gift card.
             customer_mobile: Mobile number of customer.
             customer_email: The email address of customer.
             biller_identifier: The Biller ID or identifier. You can find it in the `APIResponse` of
                 `self.gift_cards`.
             note: An optional gift card note.
             request_reference: a unique identifier for this api call.
@@ -57,36 +60,39 @@
             "amount": amount,
             "requestingCustomerName": customer_name,
             "requestingCustomerMobile": customer_mobile,
             "requestingCustomerEmail": customer_email,
             "billerIdentifier": biller_identifier,
             "note": note,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.ADMIN_BUY_GIFT_CARD,
             data=data,
             request_reference=request_reference,
         )
 
-    async def purchase_gift_card_from_virtual_account(
+    def purchase_gift_card_from_virtual_account(
         self,
         tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         customer_name: str,
         customer_mobile: str,
         customer_email: str,
         biller_identifier: str,
         note: Optional[str] = None,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Buy gift cards from the virtual account.
 
         Args:
             tracking_reference: The unique identifier of the virtual account.
-            amount: The gift card amount to be purchased. It could be in USD/ GBP/ EUR/ NGN/ AED , e.t.c.
+            amount: The gift card amount to be purchased. It could be in USD/ GBP/ EUR/ NGN/ AED , e.t.c. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             customer_name: Name of the customer receiving the gift card.
             customer_mobile: Mobile number of customer.
             customer_email: The email address of customer.
             biller_identifier: The Biller ID or identifier. You can find it in the `APIResponse` of
                 `self.gift_cards`.
             note: An optional gift card note.
             request_reference: a unique identifier for this api call.
@@ -104,36 +110,39 @@
             "amount": amount,
             "requestingCustomerName": customer_name,
             "requestingCustomerMobile": customer_mobile,
             "requestingCustomerEmail": customer_email,
             "billerIdentifier": biller_identifier,
             "note": note,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.BUY_GIFT_CARD,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_gift_card_status(
+    def get_gift_card_status(
         self,
         tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         customer_name: str,
         customer_mobile: str,
         customer_email: str,
         biller_identifier: str,
         note: Optional[str] = None,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves the status of all gift cards purchased.
 
         Args:
             tracking_reference: The unique identifier of the virtual account.
-            amount: The gift card amount to be purchased. It could be in USD/ GBP/ EUR/ NGN/ AED , e.t.c.
+            amount: The gift card amount to be purchased. It could be in USD/ GBP/ EUR/ NGN/ AED , e.t.c. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             customer_name: Name of the customer receiving the gift card.
             customer_mobile: Mobile number of customer.
             customer_email: The email address of customer.
             biller_identifier: The Biller ID or identifier. You can find it in the `APIResponse` of
                 `self.gift_cards`.
             note: An optional gift card note.
             request_reference: a unique identifier for this api call.
@@ -151,12 +160,12 @@
             "amount": amount,
             "requestingCustomerName": customer_name,
             "requestingCustomerMobile": customer_mobile,
             "requestingCustomerEmail": customer_email,
             "billerIdentifier": biller_identifier,
             "note": note,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.GIFT_CARD_TSQ,
             data=data,
             request_reference=request_reference,
         )
```

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/instant_settlement_service.py` & `pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/instant_settlement_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 from pykuda2 import Mode, ServiceType, APIResponse
 from pykuda2.base import BaseAsyncAPIWrapper
 from pykuda2.exceptions import TokenException
 
 
 class AsyncInstantSettlementService(BaseAsyncAPIWrapper):
     def __init__(self, secret_key: str, client_password: str, mode=Mode.DEVELOPMENT):
@@ -169,25 +171,28 @@
         payload = {"transactionId": transaction_id}
         return await self._api_call(
             service_type=ServiceType.NO_OP,
             data=payload,
             endpoint_path="/api/terminal/settlementstatus",
         )
 
-    async def log_transaction(self, amount: int, transaction_id: str, terminal_id: str) -> APIResponse:
+    async def log_transaction(self, amount: Union[int, float], transaction_id: str, terminal_id: str) -> APIResponse:
         """Logs a complete transaction.
 
         For complete transaction fulfilment, a user will call this method with the transaction amount
         that needs to be fulfilled. This way, the terminal management system is updated with the transaction
         status in real-time and completes settlement to the specified user's account.
 
         Logging a transaction sends a notification to Kuda which triggers instant settlement.
 
         Args:
-            amount: The transaction amount.
+            amount: The transaction amount. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             transaction_id: The transaction reference number or unique identifier.
             terminal_id: The terminal unique identifier.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
```

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/savings.py` & `pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/savings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Optional
+from typing import Optional, Union
 
-from pykuda2.base import BaseAsyncAPIWrapper
+from pykuda2.base import BaseAPIWrapper
 from pykuda2.utils import TransactionType, ServiceType, APIResponse
 
 
-class AsyncSavings(BaseAsyncAPIWrapper):
-    async def create_plain_savings_account(
+class Savings(BaseAPIWrapper):
+    def create_plain_savings_account(
         self,
         name: str,
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Create a Plain Savings Account.
 
@@ -27,21 +27,21 @@
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"Name": name, "TrackingReference": tracking_reference}
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.CREATE_PLAIN_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_plain_savings_account(
+    def get_plain_savings_account(
         self,
         tracking_reference: str,
         primary_account_number: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves a customers plain savings account
 
@@ -59,17 +59,17 @@
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "TrackingReference": tracking_reference,
             "PrimaryAccountNumber": primary_account_number,
         }
-        return await self._api_call(service_type=ServiceType.GET_PLAIN_SAVE, data=data)
+        return self._api_call(service_type=ServiceType.GET_PLAIN_SAVE, data=data)
 
-    async def get_plain_savings_accounts(
+    def get_plain_savings_accounts(
         self, tracking_reference: str, request_reference: Optional[str] = None
     ) -> APIResponse:
         """Retrieves all customers plain savings accounts
 
         Args:
             tracking_reference: Account transaction reference number of the savings you want to retrieve.
                 This parameter is for specific plain savings.
@@ -80,32 +80,35 @@
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"TrackingReference": tracking_reference}
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.GET_ALL_CUSTOMER_PLAIN_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    async def credit_or_debit_plain_savings_account(
+    def credit_or_debit_plain_savings_account(
         self,
-        amount: int,
+        amount: Union[int, float],
         narration: str,
         transaction_type: TransactionType,
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Adds or removes money from a plain savings account.
 
         Args:
-            amount: The amount to be added or removed.
+            amount: The amount to be added or removed. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             narration: The transaction description.
             transaction_type: The transaction type e.g. TransactionType.CREDIT.
             tracking_reference: Unique identifier for savings.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
@@ -117,21 +120,21 @@
         """
         data = {
             "Amount": amount,
             "Narration": narration,
             "TransactionType": transaction_type,
             "TrackingReference": tracking_reference,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.PLAIN_SAVE_DEBIT_CREDIT,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_plain_savings_account_transactions(
+    def get_plain_savings_account_transactions(
         self,
         page_size: int,
         page_number: int,
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves all plain savings account transaction data.
@@ -151,39 +154,42 @@
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "PageSize": page_size,
             "PageNumber": page_number,
             "TrackingReference": tracking_reference,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.RETRIEVE_PLAIN_SAVE_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    async def create_open_flexible_savings_account(
+    def create_open_flexible_savings_account(
         self,
         savings_tracking_reference: str,
         name: str,
         virtual_account_tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         duration: str,
         frequency: str,
         start_now: bool,
         start_date: Optional[str],
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Create an open savings plan.
 
         Args:
             savings_tracking_reference: The unique identifier for savings.
             name: Name of the savings plan.
             virtual_account_tracking_reference: Unique identifier for the associated virtual account.
-            amount: Amount to be saved.
+            amount: Amount to be saved. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             duration: Length of savings.
             frequency: How often the savings should happen.
             start_now: Flag to start the savings immediately.
             start_date: Starting date of the savings. Required if `start_now` is `False`.
                 Format (YYYY-MM-DD).
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
@@ -201,40 +207,43 @@
             "VirtualAccountTrackingReference": virtual_account_tracking_reference,
             "Amount": amount,
             "Duration": duration,
             "Frequency": frequency,
             "StartNow": start_now,
             "StartData": start_date,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.CREATE_OPEN_FLEXIBLE_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    async def pre_create_open_flexible_savings_account(
+    def pre_create_open_flexible_savings_account(
         self,
         savings_tracking_reference: str,
         name: str,
         virtual_account_tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         duration: str,
         frequency: str,
         start_now: bool,
         start_date: str,
         is_interest_earning: bool,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Pre create an Open Flexible Savings account.
 
         Args:
             savings_tracking_reference: The unique identifier for savings.
             name: Name of the savings plan.
             virtual_account_tracking_reference: Unique identifier for the associated virtual account.
-            amount: Amount to be saved.
+            amount: Amount to be saved. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             duration: Length of savings.
             frequency: How often the savings should happen.
             start_now: Flag to start the savings immediately.
             start_date: Starting date of the savings. Required if `start_now` is `False`.
                 Format (YYYY-MM-DD).
             is_interest_earning: Will the savings earn interest or not.
             request_reference: a unique identifier for this api call.
@@ -254,21 +263,21 @@
             "Amount": amount,
             "Duration": duration,
             "Frequency": frequency,
             "StartNow": start_now,
             "StartData": start_date,
             "IsInterestEarning": is_interest_earning,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.PRE_CREATE_OPEN_FLEXIBLE_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_open_flexible_savings_account(
+    def get_open_flexible_savings_account(
         self,
         tracking_reference: str,
         primary_account_number: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieve an open flexible savings account.
 
@@ -285,21 +294,21 @@
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "TrackingReference": tracking_reference,
             "PrimaryAccountNumber": primary_account_number,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.GET_OPEN_FLEXIBLE_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_open_flexible_savings_accounts(
+    def get_open_flexible_savings_accounts(
         self,
         tracking_reference: str,
         primary_account_number: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves all flexible savings account.
 
@@ -316,49 +325,52 @@
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "TrackingReference": tracking_reference,
             "PrimaryAccountNumber": primary_account_number,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.GET_ALL_CUSTOMER_OPEN_FLEXIBLE_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    async def withdrawal_from_flexible_savings_account(
+    def withdrawal_from_flexible_savings_account(
         self,
-        amount: int,
+        amount: Union[int, float],
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """
 
         Args:
-            amount: Amount to be removed.
+            amount: Amount to be removed. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             tracking_reference: Unique identifier for savings.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"Amount": amount, "TrackingReference": tracking_reference}
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.COMPLETE_OPEN_FLEXIBLE_SAVE_WITHDRAWAL,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_flexible_savings_account_transactions(
+    def get_flexible_savings_account_transactions(
         self,
         tracking_reference: str,
         page_size: int,
         page_number: int,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """
@@ -378,40 +390,43 @@
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "PageSize": page_size,
             "PageNumber": page_number,
             "TrackingReference": tracking_reference,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.RETRIEVE_OPEN_FLEXIBLE_SAVE_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    async def create_fixed_savings_account(
+    def create_fixed_savings_account(
         self,
         savings_tracking_reference: str,
         name: str,
         virtual_account_tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         duration: str,
         frequency: str,
         start_now: bool,
         start_date: str,
         is_interest_earning: bool,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Creates a fixed account.
 
         Args:
             savings_tracking_reference: The unique identifier for savings.
             name: Name of the savings plan.
             virtual_account_tracking_reference: Unique identifier for the associated virtual account.
-            amount: Amount to be saved.
+            amount: Amount to be saved. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             duration: Length of savings.
             frequency: How often the savings should happen.
             start_now: Flag to start the savings immediately.
             start_date: Starting date of the savings. Required if `start_now` is `False`.
                 Format (YYYY-MM-DD).
             is_interest_earning: Will the savings earn interest or not.
             request_reference: a unique identifier for this api call.
@@ -431,21 +446,21 @@
             "Amount": amount,
             "Duration": duration,
             "Frequency": frequency,
             "StartNow": start_now,
             "StartData": start_date,
             "IsInterestEarning": is_interest_earning,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.CREATE_FIXED_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_fixed_savings_account(
+    def get_fixed_savings_account(
         self,
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves a fixed savings account.
 
         Args:
@@ -459,21 +474,21 @@
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "SavingsId": tracking_reference,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.GET_FIXED_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_fixed_savings_accounts(
+    def get_fixed_savings_accounts(
         self, tracking_reference: str, request_reference: Optional[str] = None
     ) -> APIResponse:
         """Retrieves all fixed savings you want to retrieve.
 
         Args:
             tracking_reference: Account transaction reference number of the savings you want to retrieve.
             request_reference: a unique identifier for this api call.
@@ -483,49 +498,52 @@
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"TrackingReference": tracking_reference}
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.GET_ALL_CUSTOMER_FIXED_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    async def close_fixed_savings_account(
+    def close_fixed_savings_account(
         self,
-        amount: int,
+        amount: Union[int, float],
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """
 
         Args:
-            amount: amount to be removed.
+            amount: amount to be removed. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             tracking_reference: unique identifier for the savings.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"Amount": amount, "SavingsId": tracking_reference}
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.COMPLETE_FIXED_SAVE_WITHDRAWAL,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_fixed_savings_account_transactions(
+    def get_fixed_savings_account_transactions(
         self,
         tracking_reference: str,
         page_number: int,
         page_size: int,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves all fixed savings account transaction
@@ -545,12 +563,12 @@
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "PageNumber": page_number,
             "PageSize": page_size,
             "SavingsId": tracking_reference,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.RETRIEVE_FIXED_SAVE_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
```

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/async_wrappers/transaction.py` & `pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/transaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from typing import Optional
+from typing import Optional, Union
 
-from pykuda2.base import BaseAsyncAPIWrapper
-from pykuda2.utils import TransferInstruction, ServiceType, TransactionStatus, APIResponse
+from pykuda2.base import BaseAPIWrapper
+from pykuda2.utils import (
+    TransferInstruction,
+    ServiceType,
+    TransactionStatus,
+    APIResponse,
+)
 
 
-class AsyncTransaction(BaseAsyncAPIWrapper):
-    async def get_banks(self, request_reference: Optional[str] = None) -> APIResponse:
+class Transaction(BaseAPIWrapper):
+    def get_banks(self, request_reference: Optional[str] = None) -> APIResponse:
         """Retrieves all the banks available from NIPS
 
          In production, the list of banks and bank codes may change based on
          the responses gotten from NIBSS (Nigerian Interbank Settlement System).
 
          Args:
              request_reference: a unique identifier for this api call.
@@ -18,19 +23,19 @@
          Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.BANK_LIST, request_reference=request_reference
         )
 
-    async def confirm_transfer_recipient(
+    def confirm_transfer_recipient(
         self,
         beneficiary_account_number: str,
         beneficiary_bank_code: str,
         sender_tracking_reference: Optional[str],
         is_request_from_virtual_account: bool,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
@@ -57,26 +62,26 @@
         """
         data = {
             "beneficiaryAccountNumber": beneficiary_account_number,
             "beneficiaryBankCode": beneficiary_bank_code,
             "SenderTrackingReference": sender_tracking_reference,
             "isRequestFromVirtualAccount": is_request_from_virtual_account,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.NAME_ENQUIRY,
             data=data,
             request_reference=request_reference,
         )
 
-    async def fund_transfer(
+    def fund_transfer(
         self,
         beneficiary_account: str,
         beneficiary_bank_code: str,
         beneficiary_name: str,
-        amount: int,
+        amount: Union[int, float],
         narration: str,
         name_enquiry_session_id: str,
         sender_name: str,
         client_fee_charge: int = 0,
         client_account_number: Optional[str] = None,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
@@ -86,15 +91,18 @@
         Please, do not use sensitive data while doing test transactions so
         as not to save it in your sandbox environment.
 
         Args:
             beneficiary_account: Destination bank account number.
             beneficiary_bank_code: Destination bank code.
             beneficiary_name: Name of the recipient.
-            amount: Amount to be transferred.
+            amount: Amount to be transferred. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             narration: User defined reason for the transaction.
             name_enquiry_session_id: Session ID generated from the nameEnquiry request.
             sender_name: Name of the person sending money.
             client_fee_charge: It is an amount a client wishes to charge their customer
                 for a transfer being carried out.
             client_account_number: Account number of the client where the charged fee is
                 sent to.
@@ -115,47 +123,53 @@
             "beneficiaryName": beneficiary_name,
             "amount": amount,
             "narration": narration,
             "nameEnquirySessionID": name_enquiry_session_id,
             "senderName": sender_name,
             "clientFeeCharge": client_fee_charge,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.SINGLE_FUND_TRANSFER,
             data=data,
             request_reference=request_reference,
         )
 
-    async def virtual_account_fund_transfer(
+    def virtual_account_fund_transfer(
         self,
         tracking_reference: str,
         beneficiary_account: str,
-        amount: int,
+        amount: Union[int, float],
         beneficiary_name: str,
         narration: str,
         beneficiary_bank_code: str,
         sender_name: str,
         name_enquiry_id: str,
-        client_fee_charge: int = 0,
+        client_fee_charge: Union[int, float] = 0,
         client_account_number: Optional[str] = None,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Transfer money from a virtual account to another and any other Nigerian bank account.
 
         Args:
             tracking_reference: Unique identifier of the sender.
             beneficiary_account: Destination bank account number.
             beneficiary_bank_code: Destination bank code.
             beneficiary_name: Name of the recipient.
-            amount: Amount to be transferred.
+            amount: Amount to be transferred. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             narration: User defined reason for the transaction.
             name_enquiry_id: Session ID generated from the nameEnquiry request.
             sender_name: Name of the person sending money.
             client_fee_charge: It is an amount a client wishes to charge their customer
-                for a transfer being carried out.
+                for a transfer being carried out. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             client_account_number: Account number of the client where the charged fee is
                 sent to.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
@@ -172,21 +186,21 @@
             "beneficiaryBankCode": beneficiary_bank_code,
             "beneficiaryName": beneficiary_name,
             "senderName": sender_name,
             "nameEnquiryId": name_enquiry_id,
             "clientFeeCharge": client_fee_charge,
             "ClientAccountNumber": client_account_number,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.VIRTUAL_ACCOUNT_FUND_TRANSFER,
             data=data,
             request_reference=request_reference,
         )
 
-    async def process_transfers(
+    def process_transfers(
         self,
         fund_transfer_instructions: list[TransferInstruction],
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Allows you to send a list of transfer instructions to Kuda, to make the payments on your behalf.
 
         Args:
@@ -203,37 +217,40 @@
         """
         data = {
             "FundTransferInstructions": [
                 fund_transfer_instruction.to_dict()
                 for fund_transfer_instruction in fund_transfer_instructions
             ]
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.FUND_TRANSFER_INSTRUCTION,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_transfer_instructions(
+    def get_transfer_instructions(
         self,
         account_number: str,
         reference: str,
-        amount: int,
+        amount: Union[int, float],
         original_request_ref: str,
         status: TransactionStatus,
         page_number: int,
         page_size: int,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves transfer instructions and returns the status of the transaction.
 
         Args:
             account_number: The beneficiary’s account number.
             reference: The reference on the transfer instruction.
-            amount: The transaction amount.
+            amount: The transaction amount. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             original_request_ref: The request reference used in logging the instruction.
             status: The status of the transaction.
             page_size: This specifies the number of transfer instructions to be retrieved.
             page_number: This specifies the index of the paginated results retrieved.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
@@ -249,31 +266,31 @@
             "Reference": reference,
             "Amount": amount,
             "OriginalRequestRef": original_request_ref,
             "Status": status,
             "PageNumber": page_number,
             "PageSize": page_size,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.SEARCH_FUND_TRANSFER_INSTRUCTION,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_transaction_logs(
+    def get_transaction_logs(
         self,
         request_reference: str,
         response_reference: str,
         transaction_date: str,
         has_transaction_date_range_filter: bool,
         start_date: str,
         end_date: str,
         page_size: int,
         page_number: int,
-        fetch_successful_records: bool =False,
+        fetch_successful_records: bool=False,
     ) -> APIResponse:
         """Retrieves all transactions.
 
         Args:
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
             response_reference: Transaction response reference.
@@ -301,21 +318,21 @@
             "TransactionDate": transaction_date,
             "HasTransactionDateRangeFilter": has_transaction_date_range_filter,
             "StartDate": start_date,
             "EndDate": end_date,
             "PageSize": page_size,
             "PageNumber": page_number,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.RETRIEVE_TRANSACTION_LOGS,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_transaction_history(
+    def get_transaction_history(
         self, page_size: int, page_number: int, request_reference: Optional[str] = None
     ) -> APIResponse:
         """Retrieves a list of all main account transactions.
 
         Args:
             page_size: This specifies the number of transactions to be retrieved.
             page_number: This specifies the index of the paginated results retrieved.
@@ -326,21 +343,21 @@
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"pageSize": page_size, "pageNumber": page_number}
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.ADMIN_MAIN_ACCOUNT_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_filtered_transaction_history(
+    def get_filtered_transaction_history(
         self,
         page_size: int,
         page_number: int,
         start_date: str,
         end_date: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
@@ -363,21 +380,21 @@
         """
         data = {
             "pageSize": page_size,
             "pageNumber": page_number,
             "startDate": start_date,
             "endDate": end_date,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.ADMIN_MAIN_ACCOUNT_FILTERED_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_virtual_account_transaction_history(
+    def get_virtual_account_transaction_history(
         self,
         tracking_reference: str,
         page_size: int,
         page_number: int,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves a list of all virtual account transactions.
@@ -397,21 +414,21 @@
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "trackingReference": tracking_reference,
             "pageSize": page_size,
             "pageNumber": page_number,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.ADMIN_VIRTUAL_ACCOUNT_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_virtual_account_filtered_transaction_history(
+    def get_virtual_account_filtered_transaction_history(
         self,
         tracking_reference: str,
         page_size: int,
         page_number: int,
         start_date: str,
         end_date: str,
         request_reference: Optional[str] = None,
@@ -437,21 +454,21 @@
         data = {
             "trackingReference": tracking_reference,
             "pageSize": page_size,
             "pageNumber": page_number,
             "startDate": start_date,
             "endDate": end_date,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.ADMIN_VIRTUAL_ACCOUNT_FILTERED_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    async def get_status(
+    def get_status(
         self,
         is_third_party_bank_transfer: bool,
         transaction_request_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves the status of a transaction.
 
@@ -469,32 +486,35 @@
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "isThirdPartyBankTransfer": is_third_party_bank_transfer,
             "transactionRequestReference": transaction_request_reference,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.TRANSACTION_STATUS_QUERY,
             data=data,
             request_reference=request_reference,
         )
 
-    async def fund_virtual_account(
+    def fund_virtual_account(
         self,
         tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         narration: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Add funds to a virtual account.
 
         Args:
             tracking_reference: The virtual account tracking reference.
-            amount: The amount you want to fund your account.
+            amount: The amount you want to fund your account. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             narration: The additional description for the transaction.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
@@ -503,33 +523,36 @@
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "trackingReference": tracking_reference,
             "amount": amount,
             "narration": narration,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.FUND_VIRTUAL_ACCOUNT,
             data=data,
             request_reference=request_reference,
         )
 
-    async def withdraw_from_virtual_account(
+    def withdraw_from_virtual_account(
         self,
         tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         narration: str,
         client_fee_charge: int = 0,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Transfer funds from a virtual account to an associated Kuda account or to any other Nigerian Bank account.
 
         Args:
             tracking_reference: The virtual account tracking reference.
-            amount: The amount you want to fund your account.
+            amount: The amount you want to fund your account. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             narration: The additional description for the transaction.
             client_fee_charge: It is an amount a client wishes to charge their customer for a transfer
                 being carried out.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
@@ -541,12 +564,12 @@
         """
         data = {
             "trackingReference": tracking_reference,
             "amount": amount,
             "narration": narration,
             "ClientFeeCharge": client_fee_charge,
         }
-        return await self._api_call(
+        return self._api_call(
             service_type=ServiceType.WITHDRAW_VIRTUAL_ACCOUNT,
             data=data,
             request_reference=request_reference,
         )
```

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/accounts.py` & `pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/accounts.py`

 * *Files identical despite different names*

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/billing_and_betting.py` & `pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/billing_and_betting.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Optional, Union
 
 from pykuda2.base import BaseAPIWrapper
 from pykuda2.utils import BillType, ServiceType, APIResponse
 
 
 class BillingAndBetting(BaseAPIWrapper):
     def get_bill_type_options(
@@ -68,24 +68,27 @@
             service_type=ServiceType.VERIFY_BILL_CUSTOMER,
             data=data,
             request_reference=request_reference,
         )
 
     def purchase_bill(
         self,
-        amount: int,
+        amount: Union[int, float],
         bill_item_identifier: str,
         customer_identifier: str,
         phone_number: Optional[str] = None,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Purchase a bill from your main account.
 
         Args:
-            amount: Bill amount.
+            amount: Bill amount. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             bill_item_identifier: The Kuda bill unique identifier
             customer_identifier: The customer's unique identifier
             phone_number: The customer's phone number It is not required
                 if you're purchasing airtime.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
@@ -107,25 +110,28 @@
             data=data,
             request_reference=request_reference,
         )
 
     def purchase_bill_from_virtual_account(
         self,
         tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         bill_item_identifier: str,
         phone_number: str,
         customer_identifier: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Purchase a bill from your virtual account.
 
         Args:
             tracking_reference: The customer virtual account Identifier.
-            amount: Bill amount.
+            amount: Bill amount. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             bill_item_identifier: The Kuda bill unique identifier
             customer_identifier: The customer's unique identifier
             phone_number: The customer's phone number It is not required
                 if you're purchasing airtime.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
```

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/card.py` & `pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/card.py`

 * *Files identical despite different names*

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/instant_settlement_service.py` & `pykuda2-0.1.2/pykuda2/wrappers/sync_wrappers/instant_settlement_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Union
+
 from pykuda2 import Mode, ServiceType, APIResponse
 from pykuda2.base import BaseAPIWrapper
 
 from pykuda2.exceptions import TokenException
 
 
 class InstantSettlementService(BaseAPIWrapper):
@@ -172,26 +174,29 @@
         return self._api_call(
             service_type=ServiceType.NO_OP,
             data=payload,
             endpoint_path="/api/terminal/settlementstatus",
         )
 
     def log_transaction(
-        self, amount: int, transaction_id: str, terminal_id: str
+        self, amount: Union[int, float], transaction_id: str, terminal_id: str
     ) -> APIResponse:
         """Logs a complete transaction.
 
         For complete transaction fulfilment, a user will call this method with the transaction amount
         that needs to be fulfilled. This way, the terminal management system is updated with the transaction
         status in real-time and completes settlement to the specified user's account.
 
         Logging a transaction sends a notification to Kuda which triggers instant settlement.
 
         Args:
-            amount: The transaction amount.
+            amount: The transaction amount. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             transaction_id: The transaction reference number or unique identifier.
             terminal_id: The terminal unique identifier.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
```

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/savings.py` & `pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/savings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Optional
+from typing import Optional, Union
 
-from pykuda2.base import BaseAPIWrapper
+from pykuda2.base import BaseAsyncAPIWrapper
 from pykuda2.utils import TransactionType, ServiceType, APIResponse
 
 
-class Savings(BaseAPIWrapper):
-    def create_plain_savings_account(
+class AsyncSavings(BaseAsyncAPIWrapper):
+    async def create_plain_savings_account(
         self,
         name: str,
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Create a Plain Savings Account.
 
@@ -27,21 +27,21 @@
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"Name": name, "TrackingReference": tracking_reference}
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.CREATE_PLAIN_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_plain_savings_account(
+    async def get_plain_savings_account(
         self,
         tracking_reference: str,
         primary_account_number: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves a customers plain savings account
 
@@ -59,17 +59,17 @@
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "TrackingReference": tracking_reference,
             "PrimaryAccountNumber": primary_account_number,
         }
-        return self._api_call(service_type=ServiceType.GET_PLAIN_SAVE, data=data)
+        return await self._api_call(service_type=ServiceType.GET_PLAIN_SAVE, data=data)
 
-    def get_plain_savings_accounts(
+    async def get_plain_savings_accounts(
         self, tracking_reference: str, request_reference: Optional[str] = None
     ) -> APIResponse:
         """Retrieves all customers plain savings accounts
 
         Args:
             tracking_reference: Account transaction reference number of the savings you want to retrieve.
                 This parameter is for specific plain savings.
@@ -80,32 +80,35 @@
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"TrackingReference": tracking_reference}
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.GET_ALL_CUSTOMER_PLAIN_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    def credit_or_debit_plain_savings_account(
+    async def credit_or_debit_plain_savings_account(
         self,
-        amount: int,
+        amount: Union[int, float],
         narration: str,
         transaction_type: TransactionType,
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Adds or removes money from a plain savings account.
 
         Args:
-            amount: The amount to be added or removed.
+            amount: The amount to be added or removed. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             narration: The transaction description.
             transaction_type: The transaction type e.g. TransactionType.CREDIT.
             tracking_reference: Unique identifier for savings.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
@@ -117,21 +120,21 @@
         """
         data = {
             "Amount": amount,
             "Narration": narration,
             "TransactionType": transaction_type,
             "TrackingReference": tracking_reference,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.PLAIN_SAVE_DEBIT_CREDIT,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_plain_savings_account_transactions(
+    async def get_plain_savings_account_transactions(
         self,
         page_size: int,
         page_number: int,
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves all plain savings account transaction data.
@@ -151,39 +154,42 @@
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "PageSize": page_size,
             "PageNumber": page_number,
             "TrackingReference": tracking_reference,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.RETRIEVE_PLAIN_SAVE_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    def create_open_flexible_savings_account(
+    async def create_open_flexible_savings_account(
         self,
         savings_tracking_reference: str,
         name: str,
         virtual_account_tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         duration: str,
         frequency: str,
         start_now: bool,
         start_date: Optional[str],
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Create an open savings plan.
 
         Args:
             savings_tracking_reference: The unique identifier for savings.
             name: Name of the savings plan.
             virtual_account_tracking_reference: Unique identifier for the associated virtual account.
-            amount: Amount to be saved.
+            amount: Amount to be saved. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             duration: Length of savings.
             frequency: How often the savings should happen.
             start_now: Flag to start the savings immediately.
             start_date: Starting date of the savings. Required if `start_now` is `False`.
                 Format (YYYY-MM-DD).
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
@@ -201,40 +207,43 @@
             "VirtualAccountTrackingReference": virtual_account_tracking_reference,
             "Amount": amount,
             "Duration": duration,
             "Frequency": frequency,
             "StartNow": start_now,
             "StartData": start_date,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.CREATE_OPEN_FLEXIBLE_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    def pre_create_open_flexible_savings_account(
+    async def pre_create_open_flexible_savings_account(
         self,
         savings_tracking_reference: str,
         name: str,
         virtual_account_tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         duration: str,
         frequency: str,
         start_now: bool,
         start_date: str,
         is_interest_earning: bool,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Pre create an Open Flexible Savings account.
 
         Args:
             savings_tracking_reference: The unique identifier for savings.
             name: Name of the savings plan.
             virtual_account_tracking_reference: Unique identifier for the associated virtual account.
-            amount: Amount to be saved.
+            amount: Amount to be saved. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             duration: Length of savings.
             frequency: How often the savings should happen.
             start_now: Flag to start the savings immediately.
             start_date: Starting date of the savings. Required if `start_now` is `False`.
                 Format (YYYY-MM-DD).
             is_interest_earning: Will the savings earn interest or not.
             request_reference: a unique identifier for this api call.
@@ -254,21 +263,21 @@
             "Amount": amount,
             "Duration": duration,
             "Frequency": frequency,
             "StartNow": start_now,
             "StartData": start_date,
             "IsInterestEarning": is_interest_earning,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.PRE_CREATE_OPEN_FLEXIBLE_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_open_flexible_savings_account(
+    async def get_open_flexible_savings_account(
         self,
         tracking_reference: str,
         primary_account_number: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieve an open flexible savings account.
 
@@ -285,21 +294,21 @@
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "TrackingReference": tracking_reference,
             "PrimaryAccountNumber": primary_account_number,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.GET_OPEN_FLEXIBLE_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_open_flexible_savings_accounts(
+    async def get_open_flexible_savings_accounts(
         self,
         tracking_reference: str,
         primary_account_number: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves all flexible savings account.
 
@@ -316,49 +325,52 @@
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "TrackingReference": tracking_reference,
             "PrimaryAccountNumber": primary_account_number,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.GET_ALL_CUSTOMER_OPEN_FLEXIBLE_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    def withdrawal_from_flexible_savings_account(
+    async def withdrawal_from_flexible_savings_account(
         self,
-        amount: int,
+        amount: Union[int, float],
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """
 
         Args:
-            amount: Amount to be removed.
+            amount: Amount to be removed. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             tracking_reference: Unique identifier for savings.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"Amount": amount, "TrackingReference": tracking_reference}
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.COMPLETE_OPEN_FLEXIBLE_SAVE_WITHDRAWAL,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_flexible_savings_account_transactions(
+    async def get_flexible_savings_account_transactions(
         self,
         tracking_reference: str,
         page_size: int,
         page_number: int,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """
@@ -378,40 +390,43 @@
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "PageSize": page_size,
             "PageNumber": page_number,
             "TrackingReference": tracking_reference,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.RETRIEVE_OPEN_FLEXIBLE_SAVE_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    def create_fixed_savings_account(
+    async def create_fixed_savings_account(
         self,
         savings_tracking_reference: str,
         name: str,
         virtual_account_tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         duration: str,
         frequency: str,
         start_now: bool,
         start_date: str,
         is_interest_earning: bool,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Creates a fixed account.
 
         Args:
             savings_tracking_reference: The unique identifier for savings.
             name: Name of the savings plan.
             virtual_account_tracking_reference: Unique identifier for the associated virtual account.
-            amount: Amount to be saved.
+            amount: Amount to be saved. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             duration: Length of savings.
             frequency: How often the savings should happen.
             start_now: Flag to start the savings immediately.
             start_date: Starting date of the savings. Required if `start_now` is `False`.
                 Format (YYYY-MM-DD).
             is_interest_earning: Will the savings earn interest or not.
             request_reference: a unique identifier for this api call.
@@ -431,21 +446,21 @@
             "Amount": amount,
             "Duration": duration,
             "Frequency": frequency,
             "StartNow": start_now,
             "StartData": start_date,
             "IsInterestEarning": is_interest_earning,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.CREATE_FIXED_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_fixed_savings_account(
+    async def get_fixed_savings_account(
         self,
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves a fixed savings account.
 
         Args:
@@ -459,21 +474,21 @@
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "SavingsId": tracking_reference,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.GET_FIXED_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_fixed_savings_accounts(
+    async def get_fixed_savings_accounts(
         self, tracking_reference: str, request_reference: Optional[str] = None
     ) -> APIResponse:
         """Retrieves all fixed savings you want to retrieve.
 
         Args:
             tracking_reference: Account transaction reference number of the savings you want to retrieve.
             request_reference: a unique identifier for this api call.
@@ -483,49 +498,52 @@
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"TrackingReference": tracking_reference}
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.GET_ALL_CUSTOMER_FIXED_SAVE,
             data=data,
             request_reference=request_reference,
         )
 
-    def close_fixed_savings_account(
+    async def close_fixed_savings_account(
         self,
-        amount: int,
+        amount: Union[int, float],
         tracking_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """
 
         Args:
-            amount: amount to be removed.
+            amount: amount to be removed. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             tracking_reference: unique identifier for the savings.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"Amount": amount, "SavingsId": tracking_reference}
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.COMPLETE_FIXED_SAVE_WITHDRAWAL,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_fixed_savings_account_transactions(
+    async def get_fixed_savings_account_transactions(
         self,
         tracking_reference: str,
         page_number: int,
         page_size: int,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves all fixed savings account transaction
@@ -545,12 +563,12 @@
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "PageNumber": page_number,
             "PageSize": page_size,
             "SavingsId": tracking_reference,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.RETRIEVE_FIXED_SAVE_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
```

### Comparing `pykuda2-0.1.1/pykuda2/wrappers/sync_wrappers/transaction.py` & `pykuda2-0.1.2/pykuda2/wrappers/async_wrappers/transaction.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,15 @@
-from typing import Optional
+from typing import Optional, Union
 
-from pykuda2.base import BaseAPIWrapper
-from pykuda2.utils import (
-    TransferInstruction,
-    ServiceType,
-    TransactionStatus,
-    APIResponse,
-)
+from pykuda2.base import BaseAsyncAPIWrapper
+from pykuda2.utils import TransferInstruction, ServiceType, TransactionStatus, APIResponse
 
 
-class Transaction(BaseAPIWrapper):
-    def get_banks(self, request_reference: Optional[str] = None) -> APIResponse:
+class AsyncTransaction(BaseAsyncAPIWrapper):
+    async def get_banks(self, request_reference: Optional[str] = None) -> APIResponse:
         """Retrieves all the banks available from NIPS
 
          In production, the list of banks and bank codes may change based on
          the responses gotten from NIBSS (Nigerian Interbank Settlement System).
 
          Args:
              request_reference: a unique identifier for this api call.
@@ -23,19 +18,19 @@
          Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.BANK_LIST, request_reference=request_reference
         )
 
-    def confirm_transfer_recipient(
+    async def confirm_transfer_recipient(
         self,
         beneficiary_account_number: str,
         beneficiary_bank_code: str,
         sender_tracking_reference: Optional[str],
         is_request_from_virtual_account: bool,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
@@ -62,26 +57,26 @@
         """
         data = {
             "beneficiaryAccountNumber": beneficiary_account_number,
             "beneficiaryBankCode": beneficiary_bank_code,
             "SenderTrackingReference": sender_tracking_reference,
             "isRequestFromVirtualAccount": is_request_from_virtual_account,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.NAME_ENQUIRY,
             data=data,
             request_reference=request_reference,
         )
 
-    def fund_transfer(
+    async def fund_transfer(
         self,
         beneficiary_account: str,
         beneficiary_bank_code: str,
         beneficiary_name: str,
-        amount: int,
+        amount: Union[int, float],
         narration: str,
         name_enquiry_session_id: str,
         sender_name: str,
         client_fee_charge: int = 0,
         client_account_number: Optional[str] = None,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
@@ -91,15 +86,18 @@
         Please, do not use sensitive data while doing test transactions so
         as not to save it in your sandbox environment.
 
         Args:
             beneficiary_account: Destination bank account number.
             beneficiary_bank_code: Destination bank code.
             beneficiary_name: Name of the recipient.
-            amount: Amount to be transferred.
+            amount: Amount to be transferred. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             narration: User defined reason for the transaction.
             name_enquiry_session_id: Session ID generated from the nameEnquiry request.
             sender_name: Name of the person sending money.
             client_fee_charge: It is an amount a client wishes to charge their customer
                 for a transfer being carried out.
             client_account_number: Account number of the client where the charged fee is
                 sent to.
@@ -120,47 +118,53 @@
             "beneficiaryName": beneficiary_name,
             "amount": amount,
             "narration": narration,
             "nameEnquirySessionID": name_enquiry_session_id,
             "senderName": sender_name,
             "clientFeeCharge": client_fee_charge,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.SINGLE_FUND_TRANSFER,
             data=data,
             request_reference=request_reference,
         )
 
-    def virtual_account_fund_transfer(
+    async def virtual_account_fund_transfer(
         self,
         tracking_reference: str,
         beneficiary_account: str,
-        amount: int,
+        amount: Union[int, float],
         beneficiary_name: str,
         narration: str,
         beneficiary_bank_code: str,
         sender_name: str,
         name_enquiry_id: str,
-        client_fee_charge: int = 0,
+        client_fee_charge: Union[int, float] = 0,
         client_account_number: Optional[str] = None,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Transfer money from a virtual account to another and any other Nigerian bank account.
 
         Args:
             tracking_reference: Unique identifier of the sender.
             beneficiary_account: Destination bank account number.
             beneficiary_bank_code: Destination bank code.
             beneficiary_name: Name of the recipient.
-            amount: Amount to be transferred.
+            amount: Amount to be transferred. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             narration: User defined reason for the transaction.
             name_enquiry_id: Session ID generated from the nameEnquiry request.
             sender_name: Name of the person sending money.
             client_fee_charge: It is an amount a client wishes to charge their customer
-                for a transfer being carried out.
+                for a transfer being carried out. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             client_account_number: Account number of the client where the charged fee is
                 sent to.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
@@ -177,21 +181,21 @@
             "beneficiaryBankCode": beneficiary_bank_code,
             "beneficiaryName": beneficiary_name,
             "senderName": sender_name,
             "nameEnquiryId": name_enquiry_id,
             "clientFeeCharge": client_fee_charge,
             "ClientAccountNumber": client_account_number,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.VIRTUAL_ACCOUNT_FUND_TRANSFER,
             data=data,
             request_reference=request_reference,
         )
 
-    def process_transfers(
+    async def process_transfers(
         self,
         fund_transfer_instructions: list[TransferInstruction],
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Allows you to send a list of transfer instructions to Kuda, to make the payments on your behalf.
 
         Args:
@@ -208,37 +212,40 @@
         """
         data = {
             "FundTransferInstructions": [
                 fund_transfer_instruction.to_dict()
                 for fund_transfer_instruction in fund_transfer_instructions
             ]
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.FUND_TRANSFER_INSTRUCTION,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_transfer_instructions(
+    async def get_transfer_instructions(
         self,
         account_number: str,
         reference: str,
-        amount: int,
+        amount: Union[int, float],
         original_request_ref: str,
         status: TransactionStatus,
         page_number: int,
         page_size: int,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves transfer instructions and returns the status of the transaction.
 
         Args:
             account_number: The beneficiary’s account number.
             reference: The reference on the transfer instruction.
-            amount: The transaction amount.
+            amount: The transaction amount. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             original_request_ref: The request reference used in logging the instruction.
             status: The status of the transaction.
             page_size: This specifies the number of transfer instructions to be retrieved.
             page_number: This specifies the index of the paginated results retrieved.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
@@ -254,31 +261,31 @@
             "Reference": reference,
             "Amount": amount,
             "OriginalRequestRef": original_request_ref,
             "Status": status,
             "PageNumber": page_number,
             "PageSize": page_size,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.SEARCH_FUND_TRANSFER_INSTRUCTION,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_transaction_logs(
+    async def get_transaction_logs(
         self,
         request_reference: str,
         response_reference: str,
         transaction_date: str,
         has_transaction_date_range_filter: bool,
         start_date: str,
         end_date: str,
         page_size: int,
         page_number: int,
-        fetch_successful_records: bool=False,
+        fetch_successful_records: bool =False,
     ) -> APIResponse:
         """Retrieves all transactions.
 
         Args:
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
             response_reference: Transaction response reference.
@@ -306,21 +313,21 @@
             "TransactionDate": transaction_date,
             "HasTransactionDateRangeFilter": has_transaction_date_range_filter,
             "StartDate": start_date,
             "EndDate": end_date,
             "PageSize": page_size,
             "PageNumber": page_number,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.RETRIEVE_TRANSACTION_LOGS,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_transaction_history(
+    async def get_transaction_history(
         self, page_size: int, page_number: int, request_reference: Optional[str] = None
     ) -> APIResponse:
         """Retrieves a list of all main account transactions.
 
         Args:
             page_size: This specifies the number of transactions to be retrieved.
             page_number: This specifies the index of the paginated results retrieved.
@@ -331,21 +338,21 @@
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
 
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {"pageSize": page_size, "pageNumber": page_number}
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.ADMIN_MAIN_ACCOUNT_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_filtered_transaction_history(
+    async def get_filtered_transaction_history(
         self,
         page_size: int,
         page_number: int,
         start_date: str,
         end_date: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
@@ -368,21 +375,21 @@
         """
         data = {
             "pageSize": page_size,
             "pageNumber": page_number,
             "startDate": start_date,
             "endDate": end_date,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.ADMIN_MAIN_ACCOUNT_FILTERED_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_virtual_account_transaction_history(
+    async def get_virtual_account_transaction_history(
         self,
         tracking_reference: str,
         page_size: int,
         page_number: int,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves a list of all virtual account transactions.
@@ -402,21 +409,21 @@
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "trackingReference": tracking_reference,
             "pageSize": page_size,
             "pageNumber": page_number,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.ADMIN_VIRTUAL_ACCOUNT_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_virtual_account_filtered_transaction_history(
+    async def get_virtual_account_filtered_transaction_history(
         self,
         tracking_reference: str,
         page_size: int,
         page_number: int,
         start_date: str,
         end_date: str,
         request_reference: Optional[str] = None,
@@ -442,21 +449,21 @@
         data = {
             "trackingReference": tracking_reference,
             "pageSize": page_size,
             "pageNumber": page_number,
             "startDate": start_date,
             "endDate": end_date,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.ADMIN_VIRTUAL_ACCOUNT_FILTERED_TRANSACTIONS,
             data=data,
             request_reference=request_reference,
         )
 
-    def get_status(
+    async def get_status(
         self,
         is_third_party_bank_transfer: bool,
         transaction_request_reference: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Retrieves the status of a transaction.
 
@@ -474,32 +481,35 @@
         Raises:
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "isThirdPartyBankTransfer": is_third_party_bank_transfer,
             "transactionRequestReference": transaction_request_reference,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.TRANSACTION_STATUS_QUERY,
             data=data,
             request_reference=request_reference,
         )
 
-    def fund_virtual_account(
+    async def fund_virtual_account(
         self,
         tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         narration: str,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Add funds to a virtual account.
 
         Args:
             tracking_reference: The virtual account tracking reference.
-            amount: The amount you want to fund your account.
+            amount: The amount you want to fund your account. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             narration: The additional description for the transaction.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
             An `APIResponse` which is basically just a dataclass containing the data returned by the server as result
                 of calling this function.
@@ -508,33 +518,36 @@
             ConnectionException: when the request times out or in the absence of an internet connection.
         """
         data = {
             "trackingReference": tracking_reference,
             "amount": amount,
             "narration": narration,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.FUND_VIRTUAL_ACCOUNT,
             data=data,
             request_reference=request_reference,
         )
 
-    def withdraw_from_virtual_account(
+    async def withdraw_from_virtual_account(
         self,
         tracking_reference: str,
-        amount: int,
+        amount: Union[int, float],
         narration: str,
         client_fee_charge: int = 0,
         request_reference: Optional[str] = None,
     ) -> APIResponse:
         """Transfer funds from a virtual account to an associated Kuda account or to any other Nigerian Bank account.
 
         Args:
             tracking_reference: The virtual account tracking reference.
-            amount: The amount you want to fund your account.
+            amount: The amount you want to fund your account. Note care should be taken when performing calculations as money is involved.
+                a `Decimal` would have been the preferred type compared to `Union[int, float]` that was used.
+                it is advisable that static values are passed for this parameter. see
+                https://stackoverflow.com/questions/3730019/why-not-use-double-or-float-to-represent-currency
             narration: The additional description for the transaction.
             client_fee_charge: It is an amount a client wishes to charge their customer for a transfer
                 being carried out.
             request_reference: a unique identifier for this api call.
                 it is automatically generated if not provided.
 
         Returns:
@@ -546,12 +559,12 @@
         """
         data = {
             "trackingReference": tracking_reference,
             "amount": amount,
             "narration": narration,
             "ClientFeeCharge": client_fee_charge,
         }
-        return self._api_call(
+        return await self._api_call(
             service_type=ServiceType.WITHDRAW_VIRTUAL_ACCOUNT,
             data=data,
             request_reference=request_reference,
         )
```

### Comparing `pykuda2-0.1.1/PKG-INFO` & `pykuda2-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pykuda2
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: A developer friendly wrapper for Kuda API
 License: MIT
 Keywords: kuda,pykuda,kudapy
 Author: Jennifer
 Author-email: st.jennyandy@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

