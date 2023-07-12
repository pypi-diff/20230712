# Comparing `tmp/dxsp-3.5.3.tar.gz` & `tmp/dxsp-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.5.3.tar", max compression
+gzip compressed data, was "dxsp-3.5.4.tar", max compression
```

## Comparing `dxsp-3.5.3.tar` & `dxsp-3.5.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-12 15:44:17.017563 dxsp-3.5.3/LICENSE
--rw-r--r--   0        0        0     2697 2023-07-12 15:44:17.017563 dxsp-3.5.3/README.md
--rw-r--r--   0        0        0      115 2023-07-12 15:44:17.929569 dxsp-3.5.3/dxsp/__init__.py
--rw-r--r--   0        0        0      417 2023-07-12 15:44:17.017563 dxsp-3.5.3/dxsp/config.py
--rw-r--r--   0        0        0    10713 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/default_settings.toml
--rw-r--r--   0        0        0    17576 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1773 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      990 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2328 2023-07-12 15:44:17.929569 dxsp-3.5.3/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-3.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-12 17:44:08.491625 dxsp-3.5.4/LICENSE
+-rw-r--r--   0        0        0     2697 2023-07-12 17:44:08.491625 dxsp-3.5.4/README.md
+-rw-r--r--   0        0        0      115 2023-07-12 17:44:09.419632 dxsp-3.5.4/dxsp/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/config.py
+-rw-r--r--   0        0        0    10713 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    17573 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1773 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      990 2023-07-12 17:44:08.491625 dxsp-3.5.4/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2328 2023-07-12 17:44:09.419632 dxsp-3.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-3.5.4/PKG-INFO
```

### Comparing `dxsp-3.5.3/LICENSE` & `dxsp-3.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.3/README.md` & `dxsp-3.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.3/dxsp/default_settings.toml` & `dxsp-3.5.4/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.3/dxsp/main.py` & `dxsp-3.5.4/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
  DEX SWAP Main
 """
 
 import logging
 from typing import Optional
 from datetime import datetime, timedelta
+import decimal
 import requests
 from pycoingecko import CoinGeckoAPI
 from web3 import Web3
 from web3.gas_strategies.time_based import medium_gas_price_strategy
 from dxsp import __version__
 from dxsp.config import settings
 
@@ -69,28 +70,30 @@
 
         except Exception as error:
             return f"⚠️ order execution: {error}"
 
     async def get_swap(self, sell_token: str, buy_token: str, quantity: int) -> None:
         """ Main swap function """
         try:
+            print("get_swap", quantity)
             await self.get_protocol()
             sell_token_address = sell_token
             if not sell_token.startswith("0x"):
                 sell_token_address = await self.search_contract_address(sell_token)
             buy_token_address = buy_token
             if not buy_token_address.startswith("0x"):
                 buy_token_address = await self.search_contract_address(buy_token)
             sell_amount = await self.calculate_sell_amount(sell_token_address, quantity)
             sell_token_amount_wei = sell_amount * (10 ** (
                 await self.get_token_decimals(sell_token_address)))
             await self.get_approve(sell_token_address)
 
             order_amount = int(
-                sell_token_amount_wei * (settings.dex_trading_slippage / 100))
+                sell_token_amount_wei * decimal.Decimal(
+                    (settings.dex_trading_slippage / 100)))
             order = await self.dex_swap.get_swap(
                 sell_token_address, buy_token_address, order_amount)
 
             if not order:
                 raise ValueError("swap order not executed")
 
             signed_order = await self.get_sign(order)
@@ -168,29 +171,26 @@
                 url, params=params, headers=headers, timeout=10)
             if response.status_code == 200:
                 return response.json()
 
         except Exception as error:
             raise error
 
+
+
     async def calculate_sell_amount(self, sell_token_address, quantity):
         """Returns amount based on risk percentage."""
         sell_balance = await self.get_token_balance(sell_token_address)
         sell_contract = await self.get_token_contract(sell_token_address)
         sell_decimals = (
             sell_contract.functions.decimals().call()
             if sell_contract is not None else 18)
         risk_percentage = settings.trading_risk_amount
-
-        # Check for division by zero
-        if risk_percentage * 10 ** sell_decimals == 0:
-            return 0
-
         return ((sell_balance / (risk_percentage * 10 ** sell_decimals))
-         * (float(quantity) / 100))
+                * (decimal.Decimal(quantity)/ 100)) 
 
 
     async def get_confirmation(self, transactionHash):
         """Returns trade confirmation."""
         try:
             transaction = self.w3.eth.get_transaction(transactionHash)
             block = self.w3.eth.get_block(transaction["blockNumber"])
```

### Comparing `dxsp-3.5.3/dxsp/protocols/oneinch.py` & `dxsp-3.5.4/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.3/dxsp/protocols/uniswap.py` & `dxsp-3.5.4/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.3/dxsp/protocols/zerox.py` & `dxsp-3.5.4/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.3/pyproject.toml` & `dxsp-3.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "3.5.3"
+version = "3.5.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.5.3/PKG-INFO` & `dxsp-3.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.5.3
+Version: 3.5.4
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dxsp Version: 3.5.3 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 3.5.4 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

