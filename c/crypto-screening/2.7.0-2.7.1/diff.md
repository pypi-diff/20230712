# Comparing `tmp/crypto-screening-2.7.0.tar.gz` & `tmp/crypto-screening-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.7.0.tar", last modified: Wed Jul 12 05:48:46 2023, max compression
+gzip compressed data, was "crypto-screening-2.7.1.tar", last modified: Wed Jul 12 05:52:16 2023, max compression
```

## Comparing `crypto-screening-2.7.0.tar` & `crypto-screening-2.7.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.501671 crypto-screening-2.7.0/
--rw-rw-rw-   0        0        0       98 2023-07-12 05:48:44.000000 crypto-screening-2.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-12 05:48:46.501671 crypto-screening-2.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.7.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.7.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.395399 crypto-screening-2.7.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.427459 crypto-screening-2.7.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.7.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.7.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    54714 2023-07-12 05:47:33.000000 crypto-screening-2.7.0/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.7.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.7.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.7.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.7.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.7.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.437575 crypto-screening-2.7.0/crypto_screening/market/
--rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.7.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.460608 crypto-screening-2.7.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.7.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.7.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.7.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.7.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.500167 crypto-screening-2.7.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.7.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.7.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.7.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.7.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.409003 crypto-screening-2.7.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-12 05:48:46.000000 crypto-screening-2.7.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-07-12 05:48:46.000000 crypto-screening-2.7.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 05:48:46.000000 crypto-screening-2.7.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-12 05:48:46.000000 crypto-screening-2.7.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-12 05:48:46.000000 crypto-screening-2.7.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-12 05:48:44.000000 crypto-screening-2.7.0/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.7.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.7.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 05:48:46.501671 crypto-screening-2.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-12 05:48:40.000000 crypto-screening-2.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.295759 crypto-screening-2.7.1/
+-rw-rw-rw-   0        0        0       98 2023-07-12 05:52:15.000000 crypto-screening-2.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-12 05:52:16.295759 crypto-screening-2.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.7.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.7.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.272786 crypto-screening-2.7.1/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.285745 crypto-screening-2.7.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.7.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.7.1/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    54885 2023-07-12 05:52:05.000000 crypto-screening-2.7.1/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.7.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.7.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.7.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.7.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.7.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.287745 crypto-screening-2.7.1/crypto_screening/market/
+-rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.7.1/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.290252 crypto-screening-2.7.1/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.7.1/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.7.1/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.7.1/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.7.1/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.294813 crypto-screening-2.7.1/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.7.1/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.7.1/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.7.1/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.7.1/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.7.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:52:16.282235 crypto-screening-2.7.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-12 05:52:16.000000 crypto-screening-2.7.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-07-12 05:52:16.000000 crypto-screening-2.7.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 05:52:16.000000 crypto-screening-2.7.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-12 05:52:16.000000 crypto-screening-2.7.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-12 05:52:16.000000 crypto-screening-2.7.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-12 05:52:15.000000 crypto-screening-2.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.7.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.7.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 05:52:16.295759 crypto-screening-2.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-12 05:52:12.000000 crypto-screening-2.7.1/setup.py
```

### Comparing `crypto-screening-2.7.0/PKG-INFO` & `crypto-screening-2.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.7.0
+Version: 2.7.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.7.0/README.md` & `crypto-screening-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/build.py` & `crypto-screening-2.7.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/collect/assets.py` & `crypto-screening-2.7.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/collect/exchanges.py` & `crypto-screening-2.7.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/collect/market.py` & `crypto-screening-2.7.1/crypto_screening/collect/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,20 @@
     "assets_screeners",
     "assets_market_datasets_to_assets_screeners",
     "assets_market_data_to_symbols_market_data",
     "add_symbols_data_to_screeners",
     "add_assets_data_to_screeners",
     "symbols_market_data_to_assets_market_data",
     "merge_symbols_market_data",
-    "merge_assets_market_data"
+    "merge_assets_market_data",
+    "dataset_to_data",
+    "symbols_datasets_to_symbols_data",
+    "assets_datasets_to_assets_data",
+    "screeners_to_symbols_data",
+    "screeners_to_assets_data"
 ]
 
 AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
 SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
 
 def is_exchange_in_market_prices(
         exchange: str,
```

### Comparing `crypto-screening-2.7.0/crypto_screening/collect/screeners.py` & `crypto-screening-2.7.1/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/collect/symbols.py` & `crypto-screening-2.7.1/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/dataset.py` & `crypto-screening-2.7.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/interval.py` & `crypto-screening-2.7.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/dynamic.py` & `crypto-screening-2.7.1/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/foundation/data.py` & `crypto-screening-2.7.1/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.7.1/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/foundation/state.py` & `crypto-screening-2.7.1/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.7.1/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/screeners/base.py` & `crypto-screening-2.7.1/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/screeners/container.py` & `crypto-screening-2.7.1/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.7.1/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.7.1/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.7.1/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/market/waiting.py` & `crypto-screening-2.7.1/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/process.py` & `crypto-screening-2.7.1/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/symbols.py` & `crypto-screening-2.7.1/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening/validate.py` & `crypto-screening-2.7.1/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.7.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.7.0
+Version: 2.7.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.7.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.7.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.7.0/pyproject.toml` & `crypto-screening-2.7.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.7.0'
+version = '2.7.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.7.0/setup.py` & `crypto-screening-2.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.7.0',
+        version='2.7.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

