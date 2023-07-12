# Comparing `tmp/finops-0.2.4.tar.gz` & `tmp/finops-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.2.4.tar", last modified: Fri Jul  7 22:57:59 2023, max compression
+gzip compressed data, was "finops-0.2.5.tar", last modified: Wed Jul 12 15:33:47 2023, max compression
```

## Comparing `finops-0.2.4.tar` & `finops-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:57:59.009552 finops-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-07 22:57:46.000000 finops-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 22:57:59.009552 finops-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-07 22:57:46.000000 finops-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:57:59.005552 finops-0.2.4/finops/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-07 22:57:46.000000 finops-0.2.4/finops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-07-07 22:57:46.000000 finops-0.2.4/finops/codal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-07 22:57:46.000000 finops-0.2.4/finops/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-07 22:57:46.000000 finops-0.2.4/finops/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-07 22:57:46.000000 finops-0.2.4/finops/tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-07 22:57:46.000000 finops-0.2.4/finops/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:57:59.009552 finops-0.2.4/finops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:57:46.000000 finops-0.2.4/finops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 22:57:46.000000 finops-0.2.4/finops/utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-07-07 22:57:46.000000 finops-0.2.4/finops/utils/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-07 22:57:46.000000 finops-0.2.4/finops/utils/scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-07 22:57:46.000000 finops-0.2.4/finops/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:57:59.009552 finops-0.2.4/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-07 22:57:58.000000 finops-0.2.4/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-07 22:57:58.000000 finops-0.2.4/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 22:57:58.000000 finops-0.2.4/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 22:57:58.000000 finops-0.2.4/finops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 22:57:58.000000 finops-0.2.4/finops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 22:57:59.009552 finops-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-07 22:57:46.000000 finops-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:57:59.009552 finops-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:57:46.000000 finops-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-07 22:57:46.000000 finops-0.2.4/tests/test_tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-07 22:57:46.000000 finops-0.2.4/tests/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 22:57:59.009552 finops-0.2.4/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 22:57:46.000000 finops-0.2.4/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-07 22:57:46.000000 finops-0.2.4/tests/test_utils/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-07 22:57:46.000000 finops-0.2.4/tests/test_utils/test_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:47.041742 finops-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-12 15:33:36.000000 finops-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-12 15:33:47.041742 finops-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-12 15:33:36.000000 finops-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:47.037742 finops-0.2.5/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-12 15:33:36.000000 finops-0.2.5/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-07-12 15:33:36.000000 finops-0.2.5/finops/codal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-12 15:33:36.000000 finops-0.2.5/finops/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-12 15:33:36.000000 finops-0.2.5/finops/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-12 15:33:36.000000 finops-0.2.5/finops/tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-12 15:33:36.000000 finops-0.2.5/finops/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:47.037742 finops-0.2.5/finops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:36.000000 finops-0.2.5/finops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-12 15:33:36.000000 finops-0.2.5/finops/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-07-12 15:33:36.000000 finops-0.2.5/finops/utils/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-12 15:33:36.000000 finops-0.2.5/finops/utils/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-12 15:33:36.000000 finops-0.2.5/finops/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:47.037742 finops-0.2.5/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-12 15:33:46.000000 finops-0.2.5/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-12 15:33:47.000000 finops-0.2.5/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:33:46.000000 finops-0.2.5/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 15:33:46.000000 finops-0.2.5/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-12 15:33:46.000000 finops-0.2.5/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:33:47.041742 finops-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-12 15:33:36.000000 finops-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:47.037742 finops-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:36.000000 finops-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-07-12 15:33:36.000000 finops-0.2.5/tests/test_tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-12 15:33:36.000000 finops-0.2.5/tests/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:47.041742 finops-0.2.5/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:36.000000 finops-0.2.5/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-12 15:33:36.000000 finops-0.2.5/tests/test_utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-12 15:33:36.000000 finops-0.2.5/tests/test_utils/test_scraper.py
```

### Comparing `finops-0.2.4/LICENSE` & `finops-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/PKG-INFO` & `finops-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.2.4/README.md` & `finops-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/finops/codal.py` & `finops-0.2.5/finops/codal.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/finops/config.py` & `finops-0.2.5/finops/config.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/finops/tehran_stock_exchange.py` & `finops-0.2.5/finops/tehran_stock_exchange.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import requests
 import concurrent
 import pandas as pd
-from finops.config import TICKERS_URL, USER_AGENT
+from finops.config import TICKERS_URL, USER_AGENT, SHAREHOLDER_DATA_COLUMNS
 from finops.utils.scraper import Scraper
 from finops.utils.preprocessor import Preprocessor
 from finops.ticker import Ticker
 
 
 class TehranStockExchange(Scraper, Preprocessor):
     def get_tickers(self) -> pd.DataFrame:
@@ -38,16 +38,31 @@
 
         :return: List of stock ticker indices.
         :rtype: list
         """
         stock_tickers_df = self.get_stock_tickers()
         tickers_index_list = stock_tickers_df.ticker_index.tolist()
         return tickers_index_list
+    
+    def get_price_histories(self, tickers_index_list, store_path):
+        """
+        Retrieves and stores the price history for multiple tickers.
+
+        :param tickers_index_list: List of ticker indices.
+        :type tickers_index_list: list
+        :param store_path: The path to store the price history.
+        :type store_path: str
+        """
+        if tickers_index_list is None:
+            tickers_index_list = self.get_stock_tickers_index_list()
+        price_history = self._load_or_create_csv(store_path, SHAREHOLDER_DATA_COLUMNS)
+        for ticker_index in tickers_index_list:
+            self._save_csv(Ticker(ticker_index).get_price_history(), store_path)
 
-    def _get_shareholder_data_thread(
+    def _get_shareholder_data_wrapper(
         self,
         ticker_index: str,
         start_date: pd.Timestamp,
         end_date: pd.Timestamp,
         store_path: str,
         log_path: str,
     ):
@@ -95,15 +110,15 @@
         :type n_threads: int, optional
         """
         if tickers_index_list is None:
             tickers_index_list = self.get_stock_tickers_index_list()
         with concurrent.futures.ThreadPoolExecutor(max_workers=n_threads) as executor:
             futures = [
                 executor.submit(
-                    self._get_shareholder_data_thread,
+                    self._get_shareholder_data_wrapper,
                     ticker_index,
                     start_date,
                     end_date,
                     store_path,
                     log_path,
                 )
                 for ticker_index in tickers_index_list
```

### Comparing `finops-0.2.4/finops/ticker.py` & `finops-0.2.5/finops/ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/finops/utils/downloader.py` & `finops-0.2.5/finops/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/finops/utils/preprocessor.py` & `finops-0.2.5/finops/utils/preprocessor.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/finops/utils/scraper.py` & `finops-0.2.5/finops/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/finops/utils/wrappers.py` & `finops-0.2.5/finops/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/finops.egg-info/PKG-INFO` & `finops-0.2.5/finops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `finops-0.2.4/finops.egg-info/SOURCES.txt` & `finops-0.2.5/finops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/setup.py` & `finops-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='finops',
-    version='0.2.4',
+    version='0.2.5',
     description='A Python package for financial operations.',
     author='Alireza Nilgaran',
     author_email='alireza.nilgaran@gmail.com',
     url='https://github.com/nixuri/FinOps',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `finops-0.2.4/tests/test_tehran_stock_exchange.py` & `finops-0.2.5/tests/test_tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/tests/test_ticker.py` & `finops-0.2.5/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/tests/test_utils/test_downloader.py` & `finops-0.2.5/tests/test_utils/test_downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.2.4/tests/test_utils/test_scraper.py` & `finops-0.2.5/tests/test_utils/test_scraper.py`

 * *Files identical despite different names*

