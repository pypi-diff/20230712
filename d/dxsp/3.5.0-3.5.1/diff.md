# Comparing `tmp/dxsp-3.5.0.tar.gz` & `tmp/dxsp-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.5.0.tar", max compression
+gzip compressed data, was "dxsp-3.5.1.tar", max compression
```

## Comparing `dxsp-3.5.0.tar` & `dxsp-3.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-11 21:24:25.568523 dxsp-3.5.0/LICENSE
--rw-r--r--   0        0        0     2697 2023-07-11 21:24:25.568523 dxsp-3.5.0/README.md
--rw-r--r--   0        0        0      115 2023-07-11 21:24:26.500525 dxsp-3.5.0/dxsp/__init__.py
--rw-r--r--   0        0        0      417 2023-07-11 21:24:25.568523 dxsp-3.5.0/dxsp/config.py
--rw-r--r--   0        0        0    10713 2023-07-11 21:24:25.568523 dxsp-3.5.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    17289 2023-07-11 21:24:25.568523 dxsp-3.5.0/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-11 21:24:25.568523 dxsp-3.5.0/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-11 21:24:25.568523 dxsp-3.5.0/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1773 2023-07-11 21:24:25.568523 dxsp-3.5.0/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      990 2023-07-11 21:24:25.568523 dxsp-3.5.0/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2328 2023-07-11 21:24:26.500525 dxsp-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-11 23:10:26.563298 dxsp-3.5.1/LICENSE
+-rw-r--r--   0        0        0     2697 2023-07-11 23:10:26.563298 dxsp-3.5.1/README.md
+-rw-r--r--   0        0        0      115 2023-07-11 23:10:27.251299 dxsp-3.5.1/dxsp/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-11 23:10:26.567298 dxsp-3.5.1/dxsp/config.py
+-rw-r--r--   0        0        0    10713 2023-07-11 23:10:26.567298 dxsp-3.5.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    17415 2023-07-11 23:10:26.567298 dxsp-3.5.1/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-11 23:10:26.567298 dxsp-3.5.1/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-11 23:10:26.567298 dxsp-3.5.1/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1773 2023-07-11 23:10:26.567298 dxsp-3.5.1/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      990 2023-07-11 23:10:26.567298 dxsp-3.5.1/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2328 2023-07-11 23:10:27.251299 dxsp-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-3.5.1/PKG-INFO
```

### Comparing `dxsp-3.5.0/LICENSE` & `dxsp-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.0/README.md` & `dxsp-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.0/dxsp/default_settings.toml` & `dxsp-3.5.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.0/dxsp/main.py` & `dxsp-3.5.1/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,22 +362,25 @@
 
     async def get_trading_asset_balance(self):
         trading_asset_balance = await self.get_token_balance(
             self.trading_asset_address)
         return trading_asset_balance if trading_asset_balance else 0
 
     async def get_account_position(self):
-        open_positions = 0
-        position = "📊 Position\n" + str(open_positions)
-        position += "\n" + str(await self.get_account_margin())
+        position = "📊 Position\n"
+        position += f"Opened: {str(await self.get_account_open_positions())}/n"
+        position += f"Margin: {str(await self.get_account_margin())}"
         return position
 
     async def get_account_margin(self):
         return 0
 
+    async def get_account_open_positions(self):
+        return 0
+
     async def get_account_pnl(self, period=24):
         """
         Create a profit and loss (PnL) 
         report for the account.
         """
         pnl_dict = await self.get_account_transactions(period)
         pnl_report = "".join(
@@ -421,11 +424,12 @@
             for entry in response["result"]:
                 token_symbol = entry.get("tokenSymbol")
                 value = int(entry.get("value", 0))
                 timestamp = int(entry.get("timeStamp", 0))
                 transaction_time = datetime.utcfromtimestamp(timestamp)
     
                 if transaction_time >= time_history_start and token_symbol:
-                    pnl_dict["tokenList"][token_symbol] = pnl_dict["tokenList"].get(token_symbol, 0) + value
+                    pnl_dict["tokenList"][token_symbol] = (
+                    pnl_dict["tokenList"].get(token_symbol, 0) + value)
                     pnl_dict["pnl"] += value
     
         return pnl_dict
```

### Comparing `dxsp-3.5.0/dxsp/protocols/oneinch.py` & `dxsp-3.5.1/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.0/dxsp/protocols/uniswap.py` & `dxsp-3.5.1/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.0/dxsp/protocols/zerox.py` & `dxsp-3.5.1/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.0/pyproject.toml` & `dxsp-3.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "3.5.0"
+version = "3.5.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.5.0/PKG-INFO` & `dxsp-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.5.0
+Version: 3.5.1
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
-Metadata-Version: 2.1 Name: dxsp Version: 3.5.0 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 3.5.1 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

