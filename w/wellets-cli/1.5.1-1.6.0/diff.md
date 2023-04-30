# Comparing `tmp/wellets_cli-1.5.1.tar.gz` & `tmp/wellets_cli-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wellets_cli-1.5.1.tar", max compression
+gzip compressed data, was "wellets_cli-1.6.0.tar", max compression
```

## Comparing `wellets_cli-1.5.1.tar` & `wellets_cli-1.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1211 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/LICENSE
--rw-r--r--   0        0        0      990 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/pyproject.toml
--rw-r--r--   0        0        0        6 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/VERSION
--rw-r--r--   0        0        0       46 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/__init__.py
--rw-r--r--   0        0        0      137 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/__main__.py
--rw-r--r--   0        0        0    14811 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/api.py
--rw-r--r--   0        0        0     1047 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/auth.py
--rw-r--r--   0        0        0      335 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/base.py
--rw-r--r--   0        0        0      973 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/chart.py
--rw-r--r--   0        0        0     1281 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/cli.py
--rw-r--r--   0        0        0        0 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/__init__.py
--rw-r--r--   0        0        0     8501 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/accumulation.py
--rw-r--r--   0        0        0     6479 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/asset.py
--rw-r--r--   0        0        0     1333 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/currency.py
--rw-r--r--   0        0        0     1896 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/investment.py
--rw-r--r--   0        0        0      666 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/login.py
--rw-r--r--   0        0        0    10997 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/portfolio.py
--rw-r--r--   0        0        0     1394 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/register.py
--rw-r--r--   0        0        0     6878 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/transaction.py
--rw-r--r--   0        0        0     3571 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/transfer.py
--rw-r--r--   0        0        0     6192 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/wallet.py
--rw-r--r--   0        0        0      187 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/commands/whoami.py
--rw-r--r--   0        0        0      393 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/config.py
--rw-r--r--   0        0        0     4176 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/model.py
--rw-r--r--   0        0        0      479 2023-04-24 20:39:50.752089 wellets_cli-1.5.1/wellets_cli/prompt.py
--rw-r--r--   0        0        0     9108 2023-04-24 20:39:50.756089 wellets_cli-1.5.1/wellets_cli/question.py
--rw-r--r--   0        0        0     4250 2023-04-24 20:39:50.756089 wellets_cli-1.5.1/wellets_cli/util.py
--rw-r--r--   0        0        0     6647 2023-04-24 20:39:50.756089 wellets_cli-1.5.1/wellets_cli/validator.py
--rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 wellets_cli-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/LICENSE
+-rw-r--r--   0        0        0      990 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/VERSION
+-rw-r--r--   0        0        0       46 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/__main__.py
+-rw-r--r--   0        0        0    15278 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/api.py
+-rw-r--r--   0        0        0     1047 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/auth.py
+-rw-r--r--   0        0        0      335 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/base.py
+-rw-r--r--   0        0        0     2702 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/chart.py
+-rw-r--r--   0        0        0     1281 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/cli.py
+-rw-r--r--   0        0        0        0 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/__init__.py
+-rw-r--r--   0        0        0     8501 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/accumulation.py
+-rw-r--r--   0        0        0     8582 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/asset.py
+-rw-r--r--   0        0        0     1333 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/currency.py
+-rw-r--r--   0        0        0     1896 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/investment.py
+-rw-r--r--   0        0        0      666 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/login.py
+-rw-r--r--   0        0        0    10997 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/portfolio.py
+-rw-r--r--   0        0        0     1394 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/register.py
+-rw-r--r--   0        0        0     6878 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/transaction.py
+-rw-r--r--   0        0        0     3571 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/transfer.py
+-rw-r--r--   0        0        0     6192 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/wallet.py
+-rw-r--r--   0        0        0      187 2023-04-30 13:53:20.270775 wellets_cli-1.6.0/wellets_cli/commands/whoami.py
+-rw-r--r--   0        0        0      393 2023-04-30 13:53:20.274775 wellets_cli-1.6.0/wellets_cli/config.py
+-rw-r--r--   0        0        0     4333 2023-04-30 13:53:20.274775 wellets_cli-1.6.0/wellets_cli/model.py
+-rw-r--r--   0        0        0      479 2023-04-30 13:53:20.274775 wellets_cli-1.6.0/wellets_cli/prompt.py
+-rw-r--r--   0        0        0     9108 2023-04-30 13:53:20.274775 wellets_cli-1.6.0/wellets_cli/question.py
+-rw-r--r--   0        0        0     4250 2023-04-30 13:53:20.274775 wellets_cli-1.6.0/wellets_cli/util.py
+-rw-r--r--   0        0        0     6647 2023-04-30 13:53:20.274775 wellets_cli-1.6.0/wellets_cli/validator.py
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 wellets_cli-1.6.0/PKG-INFO
```

### Comparing `wellets_cli-1.5.1/LICENSE` & `wellets_cli-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/pyproject.toml` & `wellets_cli-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wellets_cli"
-version = "1.5.1"
+version = "1.6.0"
 description = "wellets-cli is the command line interface for Wellets, a crypto-oriented financial management tool that allows you to keep under control your money."
 authors = ["lparolari"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-dotenv = "^0.20.0"
 requests = "^2.28.1"
```

### Comparing `wellets_cli-1.5.1/wellets_cli/api.py` & `wellets_cli-1.6.0/wellets_cli/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     User,
     UserCurrency,
     UserSettings,
     Wallet,
     WalletAverageLoadPrice,
     WalletHistory,
     AssetHistory,
+    KLines,
 )
 
 base_url = lambda: settings.api_url
 
 
 class APIError(ValueError):
     pass
@@ -617,7 +618,26 @@
     if not response.ok:
         print(response.status_code)
         raise APIError(response.json())
 
     history = response.json()
     history = [AssetHistory(**h) for h in history]
     return history
+
+
+def get_currency_history(params: dict, headers: dict) -> List[KLines]:
+    currency_id = params.pop("currency_id")
+
+    response = requests.get(
+        f"{base_url()}/currencies/{currency_id}/klines",
+        params=params,
+        headers=headers,
+    )
+
+    if not response.ok:
+        print(response.status_code)
+        raise APIError(response.json())
+
+    history = response.json()
+    history = [KLines(**h) for h in history]
+
+    return history
```

### Comparing `wellets_cli-1.5.1/wellets_cli/auth.py` & `wellets_cli-1.6.0/wellets_cli/auth.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/cli.py` & `wellets_cli-1.6.0/wellets_cli/cli.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/commands/accumulation.py` & `wellets_cli-1.6.0/wellets_cli/commands/accumulation.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/commands/asset.py` & `wellets_cli-1.6.0/wellets_cli/commands/asset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,24 @@
+from datetime import timedelta
+
 import click
 from tabulate import tabulate
 
 import wellets_cli.api as api
 from wellets_cli.auth import get_auth_token
-from wellets_cli.chart import show_chart, plot_balance, mk_fig
+from wellets_cli.chart import (
+    mk_fig,
+    plot_allocation,
+    plot_balance,
+    plot_exposition,
+    plot_position,
+    plot_price,
+    show_chart,
+    xdate_fmt,
+)
 from wellets_cli.config import settings
 from wellets_cli.model import Asset, AssetAllocation, AssetEntry
 from wellets_cli.question import asset_question, date_range_question, interval_question
 from wellets_cli.util import change_val, change_value, get_by_id, make_headers, pp
 
 
 @click.group()
@@ -95,14 +106,18 @@
             "allocation\n(%)": f"{pp(allocation.allocation, 1, percent=True)}",
         }
 
     data = [get_row_value(allocation) for allocation in allocations]
 
     print(tabulate(data, headers="keys"))
 
+    fig = mk_fig()
+    fig = plot_allocation(fig, allocations)
+    fig = show_chart(fig)
+
 
 @asset.command(name="total-balance")
 @click.option("--auth-token")
 def show_total_asset_balance(auth_token):
     auth_token = auth_token or get_auth_token()
     headers = make_headers(auth_token)
 
@@ -192,7 +207,67 @@
     ]
 
     print(tabulate(data, headers="keys"))
 
     fig = mk_fig()
     fig = plot_balance(fig, history, label=asset.currency.acronym)
     fig = show_chart(fig, path)
+
+
+@asset.command(name="visualize")
+@click.option("-id", "--asset-id")
+@click.option("--auth-token")
+def visualize(asset_id, auth_token):
+    auth_token = auth_token or get_auth_token()
+    headers = make_headers(auth_token)
+
+    assets = api.get_assets(headers=headers)
+    base_currency = api.get_preferred_currency(headers=headers)
+
+    asset_id = asset_id or asset_question(assets=assets).execute()
+
+    asset: Asset = get_by_id(assets, asset_id)
+    currency = asset.currency
+    entries = asset.entries
+    exposition = api.get_asset_average_load_price(
+        params={"asset_id": asset_id},
+        headers=headers,
+    )
+
+    date_min = min([e.created_at for e in entries])
+    date_max = max([e.created_at for e in entries]) + timedelta(days=1)
+
+    history = api.get_currency_history(
+        {
+            "currency_id": asset.currency_id,
+            "interval": "1d",
+            "start_time": date_min.strftime("%Y-%m-%d"),
+            "end_time": date_max.strftime("%Y-%m-%d"),
+        },
+        headers=headers,
+    )
+
+    price_date = [h.open_time for h in history]
+    price = [
+        change_value(1 / h.close_price, base_currency.dollar_rate, 1) for h in history
+    ]
+
+    position_date = [e.created_at for e in entries]
+    position = [
+        change_value(e.dollar_rate, base_currency.dollar_rate, 1) for e in entries
+    ]
+    size_max = max([abs(e.value) for e in entries])
+    size = [abs(e.value) / size_max for e in entries]
+    kind = ["buy" if e.value >= 0 else "sell" for e in entries]
+
+    fig = mk_fig()
+    fig = plot_price(
+        fig,
+        price_date,
+        price,
+        label=currency.acronym,
+        ylabel=f"Price ({base_currency.acronym})",
+    )
+    fig = plot_exposition(fig, exposition.average_load_price)
+    fig = plot_position(fig, position_date, position, size, kind)
+    fig = xdate_fmt(fig)
+    show_chart(fig)
```

### Comparing `wellets_cli-1.5.1/wellets_cli/commands/currency.py` & `wellets_cli-1.6.0/wellets_cli/commands/currency.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/commands/investment.py` & `wellets_cli-1.6.0/wellets_cli/commands/investment.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/commands/login.py` & `wellets_cli-1.6.0/wellets_cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/commands/portfolio.py` & `wellets_cli-1.6.0/wellets_cli/commands/portfolio.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/commands/register.py` & `wellets_cli-1.6.0/wellets_cli/commands/register.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/commands/transaction.py` & `wellets_cli-1.6.0/wellets_cli/commands/transaction.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/commands/transfer.py` & `wellets_cli-1.6.0/wellets_cli/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/commands/wallet.py` & `wellets_cli-1.6.0/wellets_cli/commands/wallet.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/model.py` & `wellets_cli-1.6.0/wellets_cli/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -215,7 +215,16 @@
     timestamp: datetime
     balance: float
 
 
 class AssetHistory(BaseModel):
     timestamp: datetime
     balance: float
+
+
+class KLines(BaseModel):
+    open_time: datetime
+    open_price: float
+    high_price: float
+    low_price: float
+    close_price: float
+    volume: float
```

### Comparing `wellets_cli-1.5.1/wellets_cli/question.py` & `wellets_cli-1.6.0/wellets_cli/question.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/util.py` & `wellets_cli-1.6.0/wellets_cli/util.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/wellets_cli/validator.py` & `wellets_cli-1.6.0/wellets_cli/validator.py`

 * *Files identical despite different names*

### Comparing `wellets_cli-1.5.1/PKG-INFO` & `wellets_cli-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wellets-cli
-Version: 1.5.1
+Version: 1.6.0
 Summary: wellets-cli is the command line interface for Wellets, a crypto-oriented financial management tool that allows you to keep under control your money.
 Author: lparolari
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

