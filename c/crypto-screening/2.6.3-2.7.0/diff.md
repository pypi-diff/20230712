# Comparing `tmp/crypto-screening-2.6.3.tar.gz` & `tmp/crypto-screening-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-2.6.3.tar", last modified: Mon Jul 10 17:18:02 2023, max compression
+gzip compressed data, was "crypto-screening-2.7.0.tar", last modified: Wed Jul 12 05:48:46 2023, max compression
```

## Comparing `crypto-screening-2.6.3.tar` & `crypto-screening-2.7.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.744184 crypto-screening-2.6.3/
--rw-rw-rw-   0        0        0       98 2023-07-10 17:18:00.000000 crypto-screening-2.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-10 17:18:02.744184 crypto-screening-2.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.6.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.6.3/build.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.629648 crypto-screening-2.6.3/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.666652 crypto-screening-2.6.3/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.6.3/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.6.3/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    52089 2023-07-09 13:51:36.000000 crypto-screening-2.6.3/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    11824 2023-07-10 16:42:59.000000 crypto-screening-2.6.3/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.6.3/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    12514 2023-06-30 09:18:44.000000 crypto-screening-2.6.3/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.6.3/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.6.3/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.678210 crypto-screening-2.6.3/crypto_screening/market/
--rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.6.3/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.702183 crypto-screening-2.6.3/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.6.3/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.6.3/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.6.3/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.6.3/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.743183 crypto-screening-2.6.3/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.6.3/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.6.3/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.6.3/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.6.3/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.6.3/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-10 17:18:02.644647 crypto-screening-2.6.3/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-10 17:18:02.000000 crypto-screening-2.6.3/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1167 2023-07-10 17:18:02.000000 crypto-screening-2.6.3/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 17:18:02.000000 crypto-screening-2.6.3/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-07-10 17:18:02.000000 crypto-screening-2.6.3/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-10 17:18:02.000000 crypto-screening-2.6.3/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-10 17:18:00.000000 crypto-screening-2.6.3/pyproject.toml
--rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.6.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.6.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 17:18:02.744184 crypto-screening-2.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-10 17:17:46.000000 crypto-screening-2.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.501671 crypto-screening-2.7.0/
+-rw-rw-rw-   0        0        0       98 2023-07-12 05:48:44.000000 crypto-screening-2.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-12 05:48:46.501671 crypto-screening-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-2.7.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-2.7.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.395399 crypto-screening-2.7.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.427459 crypto-screening-2.7.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-2.7.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-2.7.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    54714 2023-07-12 05:47:33.000000 crypto-screening-2.7.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    18142 2023-07-12 05:47:33.000000 crypto-screening-2.7.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18974 2023-07-06 12:49:00.000000 crypto-screening-2.7.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    12669 2023-07-12 05:22:26.000000 crypto-screening-2.7.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-2.7.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5281 2023-07-06 12:49:43.000000 crypto-screening-2.7.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.437575 crypto-screening-2.7.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0     6010 2023-07-09 08:11:33.000000 crypto-screening-2.7.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.460608 crypto-screening-2.7.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-2.7.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-2.7.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-2.7.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6969 2023-07-04 21:21:42.000000 crypto-screening-2.7.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.500167 crypto-screening-2.7.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    13531 2023-07-04 21:23:28.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0     3255 2023-07-03 15:13:24.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    32767 2023-07-04 21:25:29.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    24982 2023-07-04 21:26:30.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0     5390 2023-07-03 15:12:27.000000 crypto-screening-2.7.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0     3839 2023-06-30 09:26:54.000000 crypto-screening-2.7.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-2.7.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-2.7.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     3857 2023-07-10 17:12:15.000000 crypto-screening-2.7.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-12 05:48:46.409003 crypto-screening-2.7.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-12 05:48:46.000000 crypto-screening-2.7.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-07-12 05:48:46.000000 crypto-screening-2.7.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 05:48:46.000000 crypto-screening-2.7.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-07-12 05:48:46.000000 crypto-screening-2.7.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-12 05:48:46.000000 crypto-screening-2.7.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-12 05:48:44.000000 crypto-screening-2.7.0/pyproject.toml
+-rw-rw-rw-   0        0        0      106 2023-07-06 12:50:05.000000 crypto-screening-2.7.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       71 2023-07-06 10:23:07.000000 crypto-screening-2.7.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 05:48:46.501671 crypto-screening-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-12 05:48:40.000000 crypto-screening-2.7.0/setup.py
```

### Comparing `crypto-screening-2.6.3/PKG-INFO` & `crypto-screening-2.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.6.3
+Version: 2.7.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.6.3/README.md` & `crypto-screening-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/build.py` & `crypto-screening-2.7.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/collect/assets.py` & `crypto-screening-2.7.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/collect/exchanges.py` & `crypto-screening-2.7.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/collect/market.py` & `crypto-screening-2.7.0/crypto_screening/collect/market.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,25 @@
 from represent import represent, Modifiers
 
 import numpy as np
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
-from crypto_screening.dataset import BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME
+from crypto_screening.dataset import (
+    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, dataset_to_json
+)
 from crypto_screening.symbols import symbol_to_parts, parts_to_symbol
-from crypto_screening.collect.screeners import find_screeners
-from crypto_screening.market.screeners.orderbook import create_orderbook_dataframe
+from crypto_screening.collect.screeners import (
+    find_screeners, screeners_to_assets_datasets,
+    screeners_to_symbols_datasets
+)
+from crypto_screening.market.screeners.orderbook import (
+    create_orderbook_dataframe
+)
 
 __all__ = [
     "validate_assets_market_state_prices_symbol",
     "assets_market_price",
     "is_symbol_in_assets_market_prices",
     "symbols_market_prices",
     "symbols_market_state",
@@ -786,14 +793,105 @@
         bids_volume=bids_volume, asks_volume=asks_volume
     )
 # end assets_market_state
 
 SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
 SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
 
+def dataset_to_data(dataset: pd.DataFrame) -> List[Tuple[dt.datetime, Dict[str, float]]]:
+    """
+    Converts the dataset into the data of the rows.
+
+    :param dataset: The dataset.
+
+    :return: The data structure.
+    """
+
+    data = dataset_to_json(dataset)
+
+    return [
+        (index, value)
+        for index, (_, value) in zip(dataset.index, data)
+    ]
+# end dataset_to_data
+
+def symbols_datasets_to_symbols_data(
+        datasets: Dict[str, Dict[str, pd.DataFrame]]
+) -> SymbolsMarketData:
+    """
+    Converts the datasets structure to the structure of the data rows.
+
+    :param datasets: The datasets to convert.
+
+    :return: The new data.
+    """
+
+    return {
+        exchange: {
+            symbol: dataset_to_data(dataset=dataset)
+            for symbol, dataset in symbols.items()
+        } for exchange, symbols in datasets.items()
+    }
+# end symbols_datasets_to_symbols_data
+
+def assets_datasets_to_assets_data(
+        datasets: Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
+) -> AssetsMarketData:
+    """
+    Converts the datasets structure to the structure of the data rows.
+
+    :param datasets: The datasets to convert.
+
+    :return: The new data.
+    """
+
+    return {
+        exchange: {
+            base: {
+                quote: dataset_to_data(dataset=dataset)
+                for quote, dataset in quotes.items()
+            } for base, quotes in bases.items()
+        } for exchange, bases in datasets.items()
+    }
+# end assets_datasets_to_assets_data
+
+def screeners_to_assets_data(
+        screeners: Iterable[BaseScreener],
+        separator: Optional[str] = None
+) -> AssetsMarketData:
+    """
+    Converts the datasets structure to the structure of the data rows.
+
+    :param screeners: The screeners to process.
+    :param separator: The separator for the symbols.
+
+    :return: The new data.
+    """
+
+    return assets_datasets_to_assets_data(
+        screeners_to_assets_datasets(
+            screeners=screeners, separator=separator
+        )
+    )
+# end screeners_to_assets_data
+
+def screeners_to_symbols_data(screeners: Iterable[BaseScreener]) -> SymbolsMarketData:
+    """
+    Converts the datasets structure to the structure of the data rows.
+
+    :param screeners: The screeners to process.
+
+    :return: The new data.
+    """
+
+    return symbols_datasets_to_symbols_data(
+        screeners_to_symbols_datasets(screeners=screeners)
+    )
+# end screeners_to_symbols_data
+
 @define(repr=False)
 @represent
 class SymbolsMarketState(SymbolsMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
```

### Comparing `crypto-screening-2.6.3/crypto_screening/collect/symbols.py` & `crypto-screening-2.7.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/dataset.py` & `crypto-screening-2.7.0/crypto_screening/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # dataset.py
 
 import os
 import json
 from pathlib import Path
 from typing import (
     Union, Optional, Tuple, Iterable,
-    Any, Callable, Dict
+    Any, Callable, Dict, List
 )
 
 import pandas as pd
 
 __all__ = [
     "row_to_dataset",
     "save_dataset",
@@ -215,35 +215,41 @@
         raise ValueError(
             f"Dataset must have length of {length}, "
             f"not: {len(dataset)}."
         )
     # end if
 # end validate_dataset
 
-def dataset_to_json(dataset: pd.DataFrame) -> Dict[str, Dict[str, Any]]:
+def dataset_to_json(dataset: pd.DataFrame) -> List[Union[str, Dict[str, Any]]]:
     """
     Converts the data of the dataset to json.
 
     :param dataset: The dataset to process.
 
     :return: The json representation of the data.
     """
 
-    return json.loads(dataset.to_json(orient='index'))
+    return list(json.loads(dataset.to_json(orient='index')).items())
 # end dataset_to_json
 
-def dataset_from_json(data: Dict[str, Dict[str, Any]]) -> pd.DataFrame:
+def dataset_from_json(
+        data: Union[Dict[str, Dict[str, Any]], List[Union[str, Dict[str, Any]]]]
+) -> pd.DataFrame:
     """
     Converts the data from json format into a dataframe object.
 
     :param data: The json data to process.
 
     :return: The data frame object.
     """
 
+    if isinstance(data, list):
+        data = dict(data)
+    # end if
+
     return pd.read_json(json.dumps(data), orient="index")
 # end dataset_from_json
 
 CSV_EXTENSION = "csv"
 JSON_EXTENSION = "json"
 DEFAULT_EXTENSION = CSV_EXTENSION
```

### Comparing `crypto-screening-2.6.3/crypto_screening/interval.py` & `crypto-screening-2.7.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/dynamic.py` & `crypto-screening-2.7.0/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/foundation/data.py` & `crypto-screening-2.7.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/foundation/protocols.py` & `crypto-screening-2.7.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/foundation/state.py` & `crypto-screening-2.7.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/foundation/waiting.py` & `crypto-screening-2.7.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/screeners/base.py` & `crypto-screening-2.7.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/screeners/container.py` & `crypto-screening-2.7.0/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-2.7.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-2.7.0/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/screeners/recorder.py` & `crypto-screening-2.7.0/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/market/waiting.py` & `crypto-screening-2.7.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/process.py` & `crypto-screening-2.7.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/symbols.py` & `crypto-screening-2.7.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening/validate.py` & `crypto-screening-2.7.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-2.7.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 2.6.3
+Version: 2.7.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-2.6.3/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-2.7.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-2.6.3/pyproject.toml` & `crypto-screening-2.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '2.6.3'
+version = '2.7.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-2.6.3/setup.py` & `crypto-screening-2.7.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='2.6.3',
+        version='2.7.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

