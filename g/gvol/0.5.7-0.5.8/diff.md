# Comparing `tmp/gvol-0.5.7.tar.gz` & `tmp/gvol-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvol-0.5.7.tar", max compression
+gzip compressed data, was "gvol-0.5.8.tar", max compression
```

## Comparing `gvol-0.5.7.tar` & `gvol-0.5.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1132 2023-03-17 16:07:05.923117 gvol-0.5.7/README.md
--rw-r--r--   0        0        0       86 2023-03-17 16:07:05.923117 gvol-0.5.7/gvol/__init__.py
--rw-r--r--   0        0        0    53169 2023-03-17 16:07:05.923117 gvol-0.5.7/gvol/client.py
--rw-r--r--   0        0        0    36166 2023-03-17 16:07:05.923117 gvol-0.5.7/gvol/queries.py
--rw-r--r--   0        0        0     1785 2023-03-17 16:07:05.923117 gvol-0.5.7/gvol/types.py
--rw-r--r--   0        0        0     1411 2023-03-17 16:07:05.923117 gvol-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 gvol-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1132 2023-07-12 07:52:55.074125 gvol-0.5.8/README.md
+-rw-r--r--   0        0        0       86 2023-07-12 07:52:55.074125 gvol-0.5.8/gvol/__init__.py
+-rw-r--r--   0        0        0    55510 2023-07-12 07:52:55.074125 gvol-0.5.8/gvol/client.py
+-rw-r--r--   0        0        0    36960 2023-07-12 07:52:55.074125 gvol-0.5.8/gvol/queries.py
+-rw-r--r--   0        0        0     1766 2023-07-12 07:52:55.074125 gvol-0.5.8/gvol/types.py
+-rw-r--r--   0        0        0     1411 2023-07-12 07:52:55.078125 gvol-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gvol-0.5.8/PKG-INFO
```

### Comparing `gvol-0.5.7/README.md` & `gvol-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `gvol-0.5.7/gvol/client.py` & `gvol-0.5.8/gvol/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,16 +155,16 @@
                 "symbol": symbol,
                 "exchange": exchange,
             },
         )
 
     def options_dvol_index(
         self,
-        exchange: types.ExchangeEnumType,
-        symbol: types.SymbolEnumType,
+        exchange: types.ExchangeDeribit,
+        symbol: types.BTCOrETHEnumType,
         interval: types.String,
         dateStart: types.String,
         dateEnd: types.String,
     ) -> Dict:
         """
         The DVol index is a VIX like volatility index built and maintained by Deribit.com
         The 30-day volatility index supports both BTC and ETH.
@@ -236,15 +236,15 @@
         """
         return self._client.execute(
             gql(queries.options_trades),
             variable_values={"date": date, "exchange": exchange},
         )
 
     def options_trades_orderbook_details(
-        self, exchange: types.ExchangeEnumType, symbol: types.SymbolEnumType, dateStart: types.String, dateEnd: types.String 
+        self, exchange: types.ExchangeDeribit, symbol: types.BTCOrETHEnumType, dateStart: types.String, dateEnd: types.String 
     ) -> Dict:
         """This query will return the trades with useful information about the orderbook at the time of the trade.
 
         Args:
             {
             "exchange": "deribit",
             "symbol": "BTC", 
@@ -489,16 +489,16 @@
                 "dateEnd": dateEnd,
                 "interval": interval,
             },
         )
 
     def futures_basis_hist(
         self,
-        exchange: types.ExchangeEnumType,
-        symbol: types.SymbolEnumType,
+        exchange: types.ExchangeDeribit,
+        symbol: types.BTCOrETHEnumType,
         expiration: types.String,
         dateStart: types.String,
         dateEnd: types.String,
     ) -> Dict:
         """Historical intraday traded weighted basis
 
         Args:
@@ -617,17 +617,17 @@
                 "ivShift": ivShift,
                 "symbol": symbol
             },
         )
 
     def options_greeks_minute(
         self,
-        exchange: types.ExchangeEnumType,
+        exchange: types.ExchangeDeribit,
         dateTime: types.String,
-        symbol: types.SymbolEnumType
+        symbol: types.BTCOrETHEnumType
     ) -> Dict:
         """
       Explanation:
         This endpoint returns a volatility surface represented by option strike prices.
         This is a "model-free" volatility surface, meaning no interpolation or fitting of any kind is present.
         Mark IV is determined by Deribit's internal risk-engine, which is proprietary formulation that is built upon a smoothing process. Deribit's internal fitting.
         Option greeks and implied volatility are based on the future (forward) price, also known as the underlying and Deribit "marks".
@@ -679,17 +679,17 @@
                 "dateTime": dateTime,
                 "symbol": symbol
             },
         )
 
     def options_greeks_hour(
         self,
-        exchange: types.ExchangeEnumType,
+        exchange: types.ExchangeDeribit,
         date: types.String,
-        symbol: types.SymbolEnumType,
+        symbol: types.BTCOrETHEnumType,
         interval: types.String
     ) -> Dict:
         """
       Explanation:
         This endpoint returns a volatility surface represented by option strike prices.
         This is a "model-free" volatility surface, meaning no interpolation or fitting of any kind is present.
         Mark IV is determined by Deribit's internal risk-engine, which is proprietary formulation that is built upon a smoothing process. Deribit's internal fitting.
@@ -743,60 +743,60 @@
                 "exchange": exchange,
                 "date": date,
                 "symbol": symbol,
                 "interval": interval
             },
         )
 
-    def spot_prices_lite(
-        self,
-        symbol: types.SymbolEnumType,
-    ) -> Dict:
-        """
-      Explanation:
-       Inputs:
-        Currency Symbol: Top 100 coins
-
-        Why do traders like this endpoint?
-        This endpoint is a building block for spot and vol. traders alike.
-        Use this endpoint to compare multiple coin prices.
-
-        Calculation:
-        OHLC: are calculated at midnight UTC.
-
-        Endpoint Output Details:
-        Granularity: Daily
-        Dataset: 1-year of OHLC for various crypto-currencies.
-        Date: Unix Format
-
-        Args:
-            {
-            "symbol": "SOL"
-            }
-        Returns:
-            {
-            "date": "1656288000000",
-            "currency": "SOL",
-            "open": 39.38,
-            "high": 41.22,
-            "low": 37.96,
-            "close": 38.46
-            }
-        """
-        return self._client.execute(
-            gql(queries.spot_prices_lite),
-            variable_values={
-                "symbol": symbol,
-            },
-        )
+    # def spot_prices_lite(
+    #     self,
+    #     symbol: types.SymbolEnumType,
+    # ) -> Dict:
+    #     """
+    #   Explanation:
+    #    Inputs:
+    #     Currency Symbol: Top 100 coins
+
+    #     Why do traders like this endpoint?
+    #     This endpoint is a building block for spot and vol. traders alike.
+    #     Use this endpoint to compare multiple coin prices.
+
+    #     Calculation:
+    #     OHLC: are calculated at midnight UTC.
+
+    #     Endpoint Output Details:
+    #     Granularity: Daily
+    #     Dataset: 1-year of OHLC for various crypto-currencies.
+    #     Date: Unix Format
+
+    #     Args:
+    #         {
+    #         "symbol": "SOL"
+    #         }
+    #     Returns:
+    #         {
+    #         "date": "1656288000000",
+    #         "currency": "SOL",
+    #         "open": 39.38,
+    #         "high": 41.22,
+    #         "low": 37.96,
+    #         "close": 38.46
+    #         }
+    #     """
+    #     return self._client.execute(
+    #         gql(queries.spot_prices_lite),
+    #         variable_values={
+    #             "symbol": symbol,
+    #         },
+    #     )
 
     def options_atm_constant_lite(
         self,
-        exchange: types.ExchangeEnumType,
-        symbol: types.SymbolEnumType,
+        exchange: types.ExchangeDeribit,
+        symbol: types.BTCOrETHEnumType,
     ) -> Dict:
         """
       Explanation:
        Why do traders like this endpoint?
         It's an industry axiom that the at-the-money (ATM) volatility chart is often viewed as the "truest" option volatility, because options that are ATM have the most embedded optionality.
         Fixed maturity ATM volatility ensures that users are analyzing an identical product overtime.
         This endpoint provides various fixed maturities (7-day, 30-day, 60-day, 90-day, 180-day), enabling users to measure the "term structure" throughout time.
@@ -840,16 +840,16 @@
                 "exchange": exchange,
                 "symbol": symbol,
             },
         )
 
     def options_skew_constant_lite(
         self,
-        exchange: types.ExchangeEnumType,
-        symbol: types.SymbolEnumType,
+        exchange: types.ExchangeDeribit,
+        symbol: types.BTCOrETHEnumType,
     ) -> Dict:
         """
       Explanation:
         Why do traders like this endpoint?
         When moving out into the "wings" of options (aka. farther out-of-the-money options) implied volatilities begin to differ between equidistant options.
         In this case, distance is measured by delta (Δ).
         The reason for this difference in implied volatility is due to "Volatility Path". Meaning, the option market might expect higher volatility/momentum during a market crash of 20% versus a market rally of 20% (or down to the -Δ25 versus up to the Δ25).
@@ -910,15 +910,15 @@
                 "symbol": symbol,
             },
         )
 
 
     def futures_orderbook(
         self,
-        exchange: types.ExchangeEnumType,
+        exchange: types.String,
     ) -> Dict:
         """
       Explanation:
         Inputs:
         Exchange: Deribit, Bit.com, Okex, DyDx, FTX
 
         Why do traders like this endpoint?
@@ -935,19 +935,14 @@
 
         open interest returned in coin: deribit
 
         Endpoint Output Details:
         Granularity: 100ms (1-minute for dydx)
         Date: Unix Format
 
-        Need More? info@genesisvolatility.io
-        API LITE Plus: Rate limit increase (10 per SECOND) $178/mo
-        GVol API Pro: 30/SEC rate, fitted + model-free surfaces, intraday granularity extended histories $11,000/year
-        GVol Enterprise API: GVol API Pro + Daily Raw data S3 bucket downloads $14,999/yea
-
         Args:
             {
             "exchange": "dydx"
             }
         Returns:
             {
             "date": "1656418050139",
@@ -970,26 +965,23 @@
                 "exchange": exchange,
             },
         )
 
 
     def futures_perps_table(
         self, 
-        exchange: types.ExchangeEnumType,
+        exchange: types.String,
     ) -> Dict:
         """
         Dataset: Returns the futures perpetual "table" information
 
+        Exchanges: deribit, dydx
+
         Date: Unix Format
         Granularity: 100ms
-
-        Need More? info@genesisvolatility.io
-        API LITE Plus: Rate limit increase (10 per SECOND) $178/mo
-        GVol API Pro: 30/SEC rate, fitted + model-free surfaces, intraday granularity extended histories $11,000/year
-        GVol Enterprise API: GVol API Pro + Daily Raw data S3 bucket downloads $14,999/year
         
         Args:
             {
             "exchange": "deribit"
             }
         Returns:
             {
@@ -1030,18 +1022,15 @@
     ) -> Dict:
         """
         Dataset: Returns the futures "table" information
 
         Date: Unix Format
         Granularity: 100ms
 
-        Need More? info@genesisvolatility.io
-        API LITE Plus: Rate limit increase (10 per SECOND) $178/mo
-        GVol API Pro: 30/SEC rate, fitted + model-free surfaces, intraday granularity extended histories $11,000/year
-        GVol Enterprise API: GVol API Pro + Daily Raw data S3 bucket downloads $14,999/year
+
         
         Args:
             {
             "exchange": "deribit"
             }
         Returns:
             {
@@ -1454,15 +1443,15 @@
         """
         return self._client.execute(
             gql(queries.options_atm_skew_spot),
             variable_values={"symbol":symbol, "dateStart":dateStart, "dateEnd":dateEnd},
         )
 
     def options_deribit_volume_detailed_daily(
-        self, exchange: types.ExchangeEnumType, dateStart: types.String, dateEnd: types.String, 
+        self, exchange: types.ExchangeDeribit, dateStart: types.String, dateEnd: types.String, 
     ) -> Dict:
         """This query will return the Deribit daily volumes detailed and open interest with putcall ratio.
 
         Args:
             {
             "exchange": "deribit",
             "dateStart": "2016-01-01",
@@ -1492,15 +1481,15 @@
         return self._client.execute(
             gql(queries.options_deribit_volume_detailed_daily),
             variable_values={"exchange":exchange, "dateStart":dateStart, "dateEnd":dateEnd},
         )
     
 
     def options_cumulative_net_volumes(
-        self,  symbol: types.BTCOrETHEnumType, exchange: types.Deribit, days: types.Float, showActiveExpirations: types.Boolean, tradeType: types.TradeTypeEnum
+        self,  symbol: types.BTCOrETHEnumType, exchange: types.ExchangeDeribit, days: types.Float, showActiveExpirations: types.Boolean, tradeType: types.TradeTypeEnum
     ) -> Dict:
         """
         This endpoint returns the cumulative net volumes of trades for the last "n" days selected.
         For calculating the "net" volume (aka the volume traded with the sign of the initiator) we use our proprietary algorithm composed from several heuristics which use the orderbook previous of the trade at millisecond granularity. You can read more about this here Gvol Direction.
 
         The endpoint is completed with some useful filters, such as:
             tradeType = ALL/block/onScreen
@@ -1526,17 +1515,56 @@
             }
         """
         return self._client.execute(
             gql(queries.options_cumulative_net_volumes),
             variable_values={"symbol":symbol, "exchange":exchange, "days":days, "showActiveExpirations":showActiveExpirations, "tradeType":tradeType}
         )
 
+    def options_cumulative_net_volumes_hist(
+        self,  symbol: types.BTCOrETHEnumType, exchange: types.ExchangeDeribit, dateStart: types.String, dateEnd: types.String, showActiveExpirations: types.Boolean, tradeType: types.TradeTypeEnum
+    ) -> Dict:
+        """
+        This endpoint returns the cumulative net volumes of trades for the date range selected (dateStart/dateEnd).
+
+        For calculating the "net" volume (aka the volume traded with the sign of the initiator) we use our proprietary algorithm composed from several heuristics which use the orderbook previous of the trade at millisecond granularity. You can read more about this here Gvol Direction.
+
+        The endpoint is completed with some useful filters, such as:
+        - tradeType = ALL/block/onScreen
+        - showActiveExpirations:
+        - true = endpoint returns only trades for active expirations
+        - false = endpoint returns all the trades even for expired expirations.
 
+        Args:
+            {
+            "symbol": "BTC",
+            "dateStart": "2023-06-01",
+            "dateEnd": "2023-06-04",
+            "exchange": "deribit",
+            "trade": "all",
+            "showActiveExpirations": true
+            }
+            
+        Returns:
+            {
+            "date": "1685923200000",
+            "strike": 48000,
+            "cumulative": 1.9,
+            "cumulativeGamma": 0,
+            "cumulativeVega": 7.92,
+            "cumulativeDelta": 0.03,
+            "indexPrice": 27125.03
+            }
+        """
+        return self._client.execute(
+            gql(queries.options_cumulative_net_volumes_hist),
+            variable_values={"symbol":symbol, "exchange":exchange, "dateStart":dateStart, "dateEnd":dateEnd, "showActiveExpirations":showActiveExpirations, "tradeType":tradeType}
+        )
+    
     def options_cumulative_net_positioning(
-        self,  symbol: types.BTCOrETHEnumType, exchange: types.Deribit, dateStart: types.String
+        self,  symbol: types.BTCOrETHEnumType, exchange: types.ExchangeDeribit, dateStart: types.String
     ) -> Dict:
         """
         This endpoint returns the cumulative net positioning of traders for the period from the dateStart parameter. It means that positioning is assumed "zero" at the dateStart.
         This endpoint starts from 7th November 2022.
         This endpoint could be seen as the other side of the gamma exposure of dealers (Gvol Gex).
 
         Args:
@@ -1554,7 +1582,42 @@
                 "indexPrice": 23134
             }
         """
         return self._client.execute(
             gql(queries.options_cumulative_net_positioning),
             variable_values={"symbol":symbol, "exchange":exchange, "dateStart":dateStart}   
         )
+    
+    def options_cumulative_net_positioning_hist(
+        self,  symbol: types.BTCOrETHEnumType, exchange: types.ExchangeDeribit, dateStart: types.String, dateEnd: types.String
+    ) -> Dict:
+        """
+        This endpoint returns the cumulative net oi for the date range selected (dateStart/dateEnd)
+
+        The cumulative net oi is the incremental change in the open interest according to the trades flow using our proprietary "taker detection".
+
+        When a strike is positive means that has been bought from traders, when is negative has been sold.
+
+        To the other side of positioning, there are the dealers with their inventory.
+
+        For not losing information cutting some open interest forming process it's strongly adviced to start from 1st November 2022.
+
+        Args:
+        {
+        "symbol": "BTC",
+        "exchange": "deribit",
+        "dateStart": "2023-03-01"
+        "dateEnd": "2023-04-01"
+        }
+            
+        Returns:
+            {
+                "date": "1677628800000",
+                "strike": 5000,
+                "netInv": 0,
+                "indexPrice": 23134
+            }
+        """
+        return self._client.execute(
+            gql(queries.options_cumulative_net_positioning_hist),
+            variable_values={"symbol":symbol, "exchange":exchange, "dateStart":dateStart, "dateEnd":dateEnd}    
+        )
```

### Comparing `gvol-0.5.7/gvol/queries.py` & `gvol-0.5.8/gvol/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1383,15 +1383,27 @@
 
 options_cumulative_net_volumes = """
 query NetVolumeGvolDirection($tradeType: TradeTypeEnum, $days: Float, $symbol: SymbolEnumType, $exchange: ExchangeEnumType, $showActiveExpirations: Boolean)
  {genericNetVolumeGvolDirection(symbol: $symbol, tradeType: $tradeType, days: $days, exchange: $exchange, showActiveExpirations: $showActiveExpirations) 
  {date strike cumulative indexPrice}}
 """
 
+options_cumulative_net_volumes_hist = """
+query HistoricalNetVolumeApi($symbol: SymbolEnumType, $dateStart: String, $dateEnd: String $exchange: ExchangeEnumType, $trade: TradeEnumType, $showActiveExpirations: Boolean)
+{HistoricalNetVolumeApi(symbol: $symbol, dateStart: $dateStart, dateEnd: $dateEnd exchange: $exchange, trade: $trade, showActiveExpirations: $showActiveExpirations) 
+{date strike cumulative cumulativeGamma cumulativeVega cumulativeDelta indexPrice} }
+"""
+
 options_cumulative_net_positioning = """
 query NetPositioning( $symbol: SymbolEnumType, $exchange: ExchangeEnumType, $dateStart: String) 
 {genericNetPositioningGvolDirection(symbol: $symbol, exchange: $exchange, dateStart: $dateStart) 
 { date
    strike
    netInv
    indexPrice}}
+"""
+
+options_cumulative_net_positioning_hist = """
+query HistoricalNetPositioningApi($symbol: SymbolEnumType, $dateStart: String, $dateEnd: String $exchange: ExchangeEnumType)
+{HistoricalNetPositioningApi(symbol: $symbol, dateStart: $dateStart, dateEnd: $dateEnd exchange: $exchange) 
+{date strike netInv indexPrice } }
 """
```

### Comparing `gvol-0.5.7/gvol/types.py` & `gvol-0.5.8/gvol/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 BTCOrETHEnumType = Literal["BTC", "ETH"]
 BlockEnumType = Literal["any", "block", "nonBlock"]
 Boolean = bool
 Deribit = Literal['deribit']
 DaysBackEnumType = Literal["NINETY", "ONE_EIGHTY", "ONE_YEAR", "SIXTY", "THIRTY"]
 ExchangeEnumType = Literal[
-    "binance", "bitcom", "cme", "delta", "deribit", "ledgerx", "okex"
+    "deribit", "bitcom", "delta","ledgerx", "okex"
 ]
 ExchangeDeribit = Literal["deribit"]
 Float = float
 Int = int
 LiquidationEnumType = Literal["any", "liquidation", "nonLiquidation"]
 PutCallEnumType = Literal["C", "P"]
 String = str
```

### Comparing `gvol-0.5.7/pyproject.toml` & `gvol-0.5.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gvol"
-version = "0.5.7"
+version = "0.5.8"
 description = "GVol is a Python library to access the GVol API"
 authors = ["Denys Halenok <denys.halenok@gmail.com>"]
 
 readme = "README.md"
 
 homepage = "https://github.com/genesis-volatility/gvol-py"
 repository = "https://github.com/genesis-volatility/gvol-py"
```

### Comparing `gvol-0.5.7/PKG-INFO` & `gvol-0.5.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 Metadata-Version: 2.1
 Name: gvol
-Version: 0.5.7
+Version: 0.5.8
 Summary: GVol is a Python library to access the GVol API
 Home-page: https://github.com/genesis-volatility/gvol-py
 Author: Denys Halenok
 Author-email: denys.halenok@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Requires-Dist: gql[requests] (>=3.4.0,<4.0.0)
 Requires-Dist: sphinx (>=4.3.2,<5.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0) ; extra == "docs"
 Requires-Dist: typing-extensions (>=4.0.1,<5.0.0) ; python_version >= "3.7" and python_version < "3.8"
 Project-URL: Bug Tracker, https://github.com/genesis-volatility/gvol-py/issues
 Project-URL: Documentation, https://gvol.readthedocs.io/
```

