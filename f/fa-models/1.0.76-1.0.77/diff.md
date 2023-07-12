# Comparing `tmp/fa-models-1.0.76.tar.gz` & `tmp/fa-models-1.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.76.tar", last modified: Tue Jul 11 09:56:36 2023, max compression
+gzip compressed data, was "fa-models-1.0.77.tar", last modified: Wed Jul 12 07:34:30 2023, max compression
```

## Comparing `fa-models-1.0.76.tar` & `fa-models-1.0.77.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.237990 fa-models-1.0.76/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-11 09:56:36.237990 fa-models-1.0.76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-11 09:56:06.000000 fa-models-1.0.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.233989 fa-models-1.0.76/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-11 09:56:36.000000 fa-models-1.0.76/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-11 09:56:36.000000 fa-models-1.0.76/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:56:36.000000 fa-models-1.0.76/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 09:56:36.000000 fa-models-1.0.76/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 09:56:36.000000 fa-models-1.0.76/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.233989 fa-models-1.0.76/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.233989 fa-models-1.0.76/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/investor_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.233989 fa-models-1.0.76/famodels/models/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/market/public_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/signal_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-11 09:56:06.000000 fa-models-1.0.76/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-11 09:56:27.000000 fa-models-1.0.76/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:56:36.237990 fa-models-1.0.76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-11 09:56:06.000000 fa-models-1.0.76/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:56:36.233989 fa-models-1.0.76/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-11 09:56:06.000000 fa-models-1.0.76/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-11 09:56:06.000000 fa-models-1.0.76/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.687567 fa-models-1.0.77/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-12 07:34:30.687567 fa-models-1.0.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-12 07:33:53.000000 fa-models-1.0.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.683566 fa-models-1.0.77/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-12 07:34:30.000000 fa-models-1.0.77/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-12 07:34:30.000000 fa-models-1.0.77/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 07:34:30.000000 fa-models-1.0.77/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-12 07:34:30.000000 fa-models-1.0.77/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 07:34:30.000000 fa-models-1.0.77/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.683566 fa-models-1.0.77/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.687567 fa-models-1.0.77/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/investor_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.687567 fa-models-1.0.77/famodels/models/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/market/public_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/signal_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-12 07:33:53.000000 fa-models-1.0.77/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-12 07:34:20.000000 fa-models-1.0.77/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 07:34:30.687567 fa-models-1.0.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-12 07:33:53.000000 fa-models-1.0.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 07:34:30.687567 fa-models-1.0.77/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-12 07:33:53.000000 fa-models-1.0.77/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-12 07:33:53.000000 fa-models-1.0.77/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.76/PKG-INFO` & `fa-models-1.0.77/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.76
+Version: 1.0.77
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.76/README.md` & `fa-models-1.0.77/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.76/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.77/fa_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.76
+Version: 1.0.77
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.76/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.77/fa_models.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 fa_models.egg-info/top_level.txt
 famodels/__init__.py
 famodels/models/__init__.py
 famodels/models/algorithm.py
 famodels/models/direction.py
 famodels/models/investor.py
 famodels/models/investor_statement.py
-famodels/models/order.py
-famodels/models/order_type.py
 famodels/models/person.py
 famodels/models/processed_signal.py
 famodels/models/side.py
 famodels/models/signal_provider.py
 famodels/models/trade.py
 famodels/models/trading_signal.py
 famodels/models/virtual_order.py
```

### Comparing `fa-models-1.0.76/famodels/models/algorithm.py` & `fa-models-1.0.77/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.76/famodels/models/investor.py` & `fa-models-1.0.77/famodels/models/investor.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,17 +41,27 @@
 
 class Fund(EmbeddedJsonModel):
     id:str = Field(index=True)
     name:str = Field(index=True)    
     compounding: str = Field(index=True, default="true")
     """Marks the investment as to be compounded with every trade. CAUTION: Due to redis-om model restrictions this could not be a boolean as it's value suggests. The workaround is a str with values 'true' and 'false'. Default is 'true'. Will bechanged as soon the redis-om library has enhanced."""
     subscriptions: Optional[List[Subscription]]  
+    investment_ratio: float = Field(index=False, default=None)
+    """ The ratio of the total assets this investment can manage. It is a number between 1 and 0. 
+        The ratio-balancer will consume this value, the total assets, the fixed_max_amount to compute the max_amount.
+    None means: as much as one can."""
     number_of_positions: int = Field(index=False, default=5)
+    """ Number of positions this fund allows. 
+        Do not mistaken it for trade-positions, a signal provider uses to scale-in and out on positions with a shared TP/SL."""
+    fixed_max_amount: float = Field(index=False, default=None)
+    """This can be optional set by the investor. The max_amount can NEVER be higher than the fixed_max_amount."""
     max_amount: Optional[float]
-    """The max amount in quote currency to invest. e.g. 10'000 (USDT)."""
+    """The max amount in quote currency to invest. e.g. 10'000 (USDT)
+    It is computed possible in real time by the ratio-balancer triggered by events like: new or deleted funds, closed orders, investor statements, depositing money, withdrawing money, change of fixed_max_amount.
+    """
     
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="fund"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
     def add_subscription(self, subscription):
```

### Comparing `fa-models-1.0.76/famodels/models/investor_statement.py` & `fa-models-1.0.77/famodels/models/investor_statement.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.76/famodels/models/market/public_trade.py` & `fa-models-1.0.77/famodels/models/market/public_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.76/famodels/models/person.py` & `fa-models-1.0.77/famodels/models/person.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.76/famodels/models/processed_signal.py` & `fa-models-1.0.77/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.76/famodels/models/signal_provider.py` & `fa-models-1.0.77/famodels/models/signal_provider.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.76/famodels/models/trading_signal.py` & `fa-models-1.0.77/famodels/models/trading_signal.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,17 +26,20 @@
     """The ID of the provider, who emitted the signal."""
     algo_id: str = Field(index=True)
     """Provide the id of your algorithm id (you might have more than one algorithm), which is sending a signal. """
     provider_signal_id: Optional[str]
     """You can use this correlation id as your own 'signal id' of your internal system. 
     #Do not mistaken this correlation id with the trade correlation id."""    
     provider_trade_id: str = Field(index=True)
-    """FA Models describes a Trade as a buy and a sell (not soley a buy or a sell). 
-    # Every trade is expected to consist of at least one buy order and zero or more sell orders. 
-    # Thus, the trade_correlation_id is mandatory. Use this correlation id to link your signals to a trade. All updates provided by the system will hold the trade id."""    
+    """ FA Models describes a Trade as a buy and a sell (not soley a buy or a sell). 
+        Every trade is expected to consist of at least one buy order and zero or more sell orders. 
+        Thus, the provider_trade_id is mandatory if a provider wants to scale in and out on positions. 
+        E.g. one can send one long signal with a provider_trade_id 77 and another long signal a few hours later also with the provider_trade_id 77. 
+        Provided that the position_size_in_percentage is less than 100 on the first one.
+        All updates provided by the system will hold the trade id."""    
     is_hot_signal: int = Field(default=0, index=True)
     """By default, every signal is marked as a cold signal. Thus, set to 0. That is a paper-trading signal and will only be processed for forward-performance testing. 
     Hot signals are suggested to be processed by the order engines - provided all other requirements for hot trading are fulfilled.
     Set 1 (not true) to this value to suggest a hot trade."""    
     market: str = Field(index=True)
     """The market you want to trade. e.g. BTC/USDT"""
     exchange: str = Field(index=True)
```

### Comparing `fa-models-1.0.76/famodels/models/virtual_order.py` & `fa-models-1.0.77/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.76/pyproject.toml` & `fa-models-1.0.77/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.76"
+version = "1.0.77"
 description = "A simple library of trading models."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.76"
+current_version = "1.0.77"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.76/setup.py` & `fa-models-1.0.77/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.76/tests/test_investor.py` & `fa-models-1.0.77/tests/test_investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.76/tests/test_processed_trading_signal.py` & `fa-models-1.0.77/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

