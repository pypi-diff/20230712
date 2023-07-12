# Comparing `tmp/dxsp-3.5.2.tar.gz` & `tmp/dxsp-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.5.2.tar", max compression
+gzip compressed data, was "dxsp-3.5.3.tar", max compression
```

## Comparing `dxsp-3.5.2.tar` & `dxsp-3.5.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-12 13:47:40.714739 dxsp-3.5.2/LICENSE
--rw-r--r--   0        0        0     2697 2023-07-12 13:47:40.714739 dxsp-3.5.2/README.md
--rw-r--r--   0        0        0      115 2023-07-12 13:47:41.526757 dxsp-3.5.2/dxsp/__init__.py
--rw-r--r--   0        0        0      417 2023-07-12 13:47:40.714739 dxsp-3.5.2/dxsp/config.py
--rw-r--r--   0        0        0    10713 2023-07-12 13:47:40.714739 dxsp-3.5.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0    17442 2023-07-12 13:47:40.714739 dxsp-3.5.2/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-12 13:47:40.714739 dxsp-3.5.2/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-12 13:47:40.714739 dxsp-3.5.2/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     1773 2023-07-12 13:47:40.714739 dxsp-3.5.2/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      990 2023-07-12 13:47:40.714739 dxsp-3.5.2/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2328 2023-07-12 13:47:41.526757 dxsp-3.5.2/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-3.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-12 15:44:17.017563 dxsp-3.5.3/LICENSE
+-rw-r--r--   0        0        0     2697 2023-07-12 15:44:17.017563 dxsp-3.5.3/README.md
+-rw-r--r--   0        0        0      115 2023-07-12 15:44:17.929569 dxsp-3.5.3/dxsp/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-12 15:44:17.017563 dxsp-3.5.3/dxsp/config.py
+-rw-r--r--   0        0        0    10713 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    17576 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     1773 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      990 2023-07-12 15:44:17.021563 dxsp-3.5.3/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2328 2023-07-12 15:44:17.929569 dxsp-3.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 dxsp-3.5.3/PKG-INFO
```

### Comparing `dxsp-3.5.2/LICENSE` & `dxsp-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.2/README.md` & `dxsp-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.2/dxsp/default_settings.toml` & `dxsp-3.5.3/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.2/dxsp/main.py` & `dxsp-3.5.3/dxsp/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,19 +172,26 @@
         except Exception as error:
             raise error
 
     async def calculate_sell_amount(self, sell_token_address, quantity):
         """Returns amount based on risk percentage."""
         sell_balance = await self.get_token_balance(sell_token_address)
         sell_contract = await self.get_token_contract(sell_token_address)
-        sell_decimals = (sell_contract.functions.decimals().call() 
-        if sell_contract is not None else 18)
+        sell_decimals = (
+            sell_contract.functions.decimals().call()
+            if sell_contract is not None else 18)
         risk_percentage = settings.trading_risk_amount
-        return (sell_balance / 
-        (risk_percentage * 10 ** sell_decimals)) * (float(quantity) / 100)
+
+        # Check for division by zero
+        if risk_percentage * 10 ** sell_decimals == 0:
+            return 0
+
+        return ((sell_balance / (risk_percentage * 10 ** sell_decimals))
+         * (float(quantity) / 100))
+
 
     async def get_confirmation(self, transactionHash):
         """Returns trade confirmation."""
         try:
             transaction = self.w3.eth.get_transaction(transactionHash)
             block = self.w3.eth.get_block(transaction["blockNumber"])
             return {
```

### Comparing `dxsp-3.5.2/dxsp/protocols/oneinch.py` & `dxsp-3.5.3/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.2/dxsp/protocols/uniswap.py` & `dxsp-3.5.3/dxsp/protocols/uniswap.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.2/dxsp/protocols/zerox.py` & `dxsp-3.5.3/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.5.2/pyproject.toml` & `dxsp-3.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dxsp"
-version = "3.5.2"
+version = "3.5.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.5.2/PKG-INFO` & `dxsp-3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.5.2
+Version: 3.5.3
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
-Metadata-Version: 2.1 Name: dxsp Version: 3.5.2 Summary: DXSP (DeX SwaP), A
+Metadata-Version: 2.1 Name: dxsp Version: 3.5.3 Summary: DXSP (DeX SwaP), A
 defi swap helper package. Swap made easy. License: MIT Author: mraniki Author-
 email: 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: pycoingecko (>=3.1.0,<4.0.0) Requires-Dist:
 uniswap-python (>=0.7.0,<0.8.0) Requires-Dist: web3 (>=6.4.0,<7.0.0) Project-
```

