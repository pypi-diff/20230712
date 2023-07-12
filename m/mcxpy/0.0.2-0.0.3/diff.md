# Comparing `tmp/mcxpy-0.0.2.tar.gz` & `tmp/mcxpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcxpy-0.0.2.tar", last modified: Mon Jul 10 18:39:45 2023, max compression
+gzip compressed data, was "mcxpy-0.0.3.tar", last modified: Wed Jul 12 17:41:31 2023, max compression
```

## Comparing `mcxpy-0.0.2.tar` & `mcxpy-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 18:39:45.750632 mcxpy-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-10 16:20:44.000000 mcxpy-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2873 2023-07-10 18:39:45.743631 mcxpy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2023-07-10 18:29:11.000000 mcxpy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 18:39:45.701620 mcxpy-0.0.2/mcxpy/
--rw-rw-rw-   0        0        0      405 2023-07-09 17:22:38.000000 mcxpy-0.0.2/mcxpy/__init__.py
--rw-rw-rw-   0        0        0      393 2023-07-09 17:22:53.000000 mcxpy-0.0.2/mcxpy/__init__.pyi
--rw-rw-rw-   0        0        0    13363 2023-07-09 17:33:24.000000 mcxpy-0.0.2/mcxpy/mcx.py
--rw-rw-rw-   0        0        0     1240 2023-07-09 17:23:32.000000 mcxpy-0.0.2/mcxpy/mcx.pyi
--rw-rw-rw-   0        0        0        0 2023-07-09 17:16:19.000000 mcxpy-0.0.2/mcxpy/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-10 18:39:45.740631 mcxpy-0.0.2/mcxpy.egg-info/
--rw-rw-rw-   0        0        0     2873 2023-07-10 18:39:45.000000 mcxpy-0.0.2/mcxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-07-10 18:39:45.000000 mcxpy-0.0.2/mcxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 18:39:45.000000 mcxpy-0.0.2/mcxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-10 18:39:45.000000 mcxpy-0.0.2/mcxpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 18:39:45.000000 mcxpy-0.0.2/mcxpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      609 2023-07-10 18:39:08.000000 mcxpy-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 18:39:45.751640 mcxpy-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 17:41:31.424373 mcxpy-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-10 16:20:44.000000 mcxpy-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3836 2023-07-12 17:41:31.418373 mcxpy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2193 2023-07-12 17:38:51.000000 mcxpy-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 17:41:31.369361 mcxpy-0.0.3/mcxpy/
+-rw-rw-rw-   0        0        0      471 2023-07-11 19:40:39.000000 mcxpy-0.0.3/mcxpy/__init__.py
+-rw-rw-rw-   0        0        0      459 2023-07-12 16:44:11.000000 mcxpy-0.0.3/mcxpy/__init__.pyi
+-rw-rw-rw-   0        0        0    20659 2023-07-12 16:39:33.000000 mcxpy-0.0.3/mcxpy/mcx.py
+-rw-rw-rw-   0        0        0     2278 2023-07-12 03:25:40.000000 mcxpy-0.0.3/mcxpy/mcx.pyi
+-rw-rw-rw-   0        0        0        0 2023-07-09 17:16:19.000000 mcxpy-0.0.3/mcxpy/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-12 17:41:31.405367 mcxpy-0.0.3/mcxpy.egg-info/
+-rw-rw-rw-   0        0        0     3836 2023-07-12 17:41:31.000000 mcxpy-0.0.3/mcxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-12 17:41:31.000000 mcxpy-0.0.3/mcxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 17:41:31.000000 mcxpy-0.0.3/mcxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-07-12 17:41:31.000000 mcxpy-0.0.3/mcxpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-12 17:41:31.000000 mcxpy-0.0.3/mcxpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      609 2023-07-12 17:40:19.000000 mcxpy-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-12 17:41:31.425377 mcxpy-0.0.3/setup.cfg
```

### Comparing `mcxpy-0.0.2/LICENSE` & `mcxpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcxpy-0.0.2/mcxpy/mcx.py` & `mcxpy-0.0.3/mcxpy/mcx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import requests
 import pandas as pd
 from datetime import datetime, date, timedelta
 import re
-from typing import Literal, Union, NewType, List, Tuple
+from typing import Literal, Union, NewType, List
+from functools import lru_cache
 
 DateFormat = NewType(name="%d-%m-%Y", tp=str)
 DateFormat_2 = NewType(name="%Y%m%d", tp=str)
 DateFormat_3 = NewType(name="%d%b%Y", tp=str)
 
 urls = {
     "base_url" : "https://www.mcxindia.com",
@@ -17,15 +18,19 @@
         "gainers" : "/backpage.aspx/GetGainer",
         "losers" : "/backpage.aspx/GetLosers",
         "activeoptions" : "/backpage.aspx/GetMostActiveOptionsContractsByValue",
         "activecontracts" : "/backpage.aspx/GetMostActiveContractByValueFilter",
         "heatmap" : "/backpage.aspx/GetHeatMap",
         "optionchain" : "/backpage.aspx/GetOptionChain",
         "pcr" : "/backpage.aspx/GetCommoditywisePutCallRatio",
-        "pcr_expirywise" : "/backpage.aspx/GetExpirywisePutCallRatio"
+        "pcr_expirywise" : "/backpage.aspx/GetExpirywisePutCallRatio",
+        "icomdex_details" : "/backpage.aspx/GetMCXIComdexIndicesDetails",
+        "icomdex_historical" : "/backpage.aspx/GetMCXIComdexIndicesHistory",
+        "getquote" : "/BackPage.aspx/GetQuote",
+        "optionquote" : "/BackPage.aspx/GetQuoteOption"
     },
 }
 
 
 headers = {
     "Accept": "application/json, text/javascript, */*; q=0.01",
     "Accept-Language": "en-GB,en-US;q=0.9,en;q=0.8",
@@ -79,26 +84,52 @@
 
             ist_datetime = datetime.utcfromtimestamp(timestamp_ms / 1000) + timedelta(hours=5, minutes=30)
             return ist_datetime
         return None
     except Exception as e:
         print(f"Error :: {e}")
 
+@lru_cache(maxsize=None)
+def get_session(url: str) -> requests.Session:
+    s = requests.Session()
+    s.headers.update(headers)
+    res = s.get(url)
+    return s
+
+def fallback_fetch(base_url: str, url: str, data: dict=None, retry=1) -> dict:
+    try:
+        session = get_session(base_url)
+        res = session.post(url=url, json=data)
+        res.raise_for_status()
+        if res.status_code == 200:
+            res_data = res.json()
+            return res_data
+    except requests.exceptions.RequestException:
+        if retry <= 3:
+            get_session.cache_clear()
+            fallback_fetch(base_url=base_url, url=url, data=data, retry=retry+1)
+    except Exception as e:
+        print(f"Error :: {e}")
+
 def mcxfetch(config_key: Literal["bhavcopy","marketwatch","circulars","gainers","losers","activeoptions",
-                                 "activecontracts","heatmap","optionchain","pcr", "pcr_expirywise"],
+                                 "activecontracts","heatmap","optionchain","pcr", "pcr_expirywise",
+                                 "icomdex_details", "icomdex_historical", "getquote", "optionquote"],
             data: dict=None) -> dict:
     try:
         base_url = urls['base_url']
         url = base_url + urls['routes'][config_key]
         response = requests.post(url, headers=headers, json=data)
         response.raise_for_status()
         if response.status_code == 200:
             res_data = response.json()
             return res_data
-    except (requests.HTTPError,Exception) as e:
+    except requests.HTTPError:
+        res = fallback_fetch(base_url=base_url, url=url, data=data)
+        return res
+    except Exception as e:
         print(f"Error :: {e}")
 
 def mcx_bhavcopy(bhavdate: Union[DateFormat, datetime, date]) -> pd.DataFrame:    
     try:
         fdate = format_date(bhavdate)
         
         data = {
@@ -298,14 +329,15 @@
             df['Expiry'] = pd.to_datetime(df['Expiry'], format="%d%b%Y", dayfirst=True, errors="coerce")
         reorderd_columns = ['Symbol', 'Date', 'Expiry', 'Ratio']
         df = df[reorderd_columns]
         return df
     except Exception as e:
         print(f"Error :: {e}")
 
+'''
 def mcx_expiry(commodity: Literal['COPPER', 'CRUDEOIL', 'GOLD', 'GOLDM', 'NATURALGAS', 
                                   'NICKEL', 'SILVER', 'SILVERM','ZINC']='CRUDEOIL',
                 expirytype : Literal['current', 'next', 'far', 'all']='current'
                 ) -> Union[datetime,List[datetime]]:
     try:
         exp_df = mcx_pcr(expirywise=True)
         com_df = exp_df[exp_df['Symbol'] == commodity]
@@ -319,8 +351,121 @@
             return exp_list[2]
         elif expirytype == "all":
             return exp_list
         else:
             print("Please input correct parameters.")
     except Exception as e:
         print(f"Error :: {e}")
+'''
+def mcx_expiry(commodity: Literal["ALUMINI", "ALUMINIUM", "COPPER", "COTTONCNDY", "CRUDEOIL", "CRUDEOILM", "GOLD", "GOLDGUINEA",
+                                    "GOLDM", "GOLDPETAL", "KAPAS", "LEAD", "LEADMINI", "MCXBULLDEX", "MCXENRGDEX", "MCXMETLDEX",
+                                    "MENTHAOIL", "NATGASMINI", "NATURALGAS", "NICKEL", "SILVER", "SILVERM", "SILVERMIC", "ZINC",
+                                    "ZINCMINI"]='CRUDEOIL',
+                instrument: Literal["option", "future"]="option",
+                expirytype: Literal['current', 'next', 'far', 'all']='current'
+                ) -> Union[datetime,List[datetime]]:
+    
+    try:
+        df = mcx_marketwatch()
+        if instrument == "option":
+            inst = "OPTFUT"
+        elif instrument == "future":
+            inst = "FUTCOM"
+        exp_list = df.query(f"Symbol in ['{commodity}'] and InstrumentName in ['{inst}']")['Expiry'].unique()
+        exp_dates = sorted([item.to_pydatetime() for item in exp_list])
+        if expirytype == "current":
+            return exp_dates[0]
+        elif expirytype == "next":
+            return exp_dates[1]
+        elif expirytype == "far":
+            return exp_dates[2]
+        elif expirytype == "all":
+            return exp_dates
+        else:
+            print("Please input correct parameters.")
+    except Exception as e:
+        print(f"Error :: {e}")
+
+def mcx_icomdexindices(datatype: Literal["today", "historical"]="today",
+                       start_date: Union[DateFormat, datetime, date]=None,
+                       end_date: Union[DateFormat, datetime, date]=None
+                       ) -> pd.DataFrame:    
+    try:
+        if datatype == "today":
+            data = {
+                "Instrument_Identifier": "0",
+                "Lang" : "en"
+                } 
+            res = mcxfetch(config_key="icomdex_details", data=data)
+        elif datatype == "historical":
+            if start_date is not None and end_date is not None:
+                stdt = format_date(dateobj=start_date)
+                enddt = format_date(dateobj=end_date)
+                data = {
+                    "Index": "0", 
+                    "StartDate": stdt, 
+                    "EndDate": enddt, 
+                    "Lang": "en"
+                    }
+                res = mcxfetch(config_key='icomdex_historical', data=data)
+            else:
+                print("Please enter start_date and end_date for historical data.")
+                return            
+        df = pd.DataFrame(res["d"]["Data"])
+        df = df.drop(columns=['__type']) 
+        return df
+    except Exception as e:
+        print(f"Error :: {e}")
 
+def mcx_quote(commodity: Literal["ALUMINI", "ALUMINIUM", "COPPER", "COTTONCNDY", "CRUDEOIL", "CRUDEOILM", "GOLD", "GOLDGUINEA",
+                                    "GOLDM", "GOLDPETAL", "KAPAS", "LEAD", "LEADMINI", "MCXBULLDEX", "MCXENRGDEX", "MCXMETLDEX",
+                                    "MENTHAOIL", "NATGASMINI", "NATURALGAS", "NICKEL", "SILVER", "SILVERM", "SILVERMIC", "ZINC",
+                                    "ZINCMINI"],
+                instrument: Literal["option", "future"], 
+                expiry: Union[DateFormat, datetime, date], 
+                optiontype: Literal["CE", "PE"]= None,
+                strikeprice: Union[str, int, float]= None,
+                outputtype: Literal["quote", "bidask"]="quote" 
+                ) -> pd.DataFrame:
+    try:
+        exp_date = format_date(dateobj=expiry, isExpiry=True)
+        if instrument == "future":
+            data = {
+                "Commodity": commodity, 
+                "Expiry": exp_date
+                }
+            res = mcxfetch(config_key="getquote", data=data)
+        elif instrument == "option":
+
+            data = {
+                "Commodity": commodity,
+                "Expiry": exp_date, 
+                "OptionType": optiontype, 
+                "StrikPrice": str(strikeprice)
+            }
+            res = mcxfetch(config_key="optionquote", data=data)
+        if outputtype == "quote":
+            df = pd.DataFrame(res['d']['Data']).drop('QuoteBid', axis=1)
+            if instrument == "future":
+                df = df.drop(columns=['__type', 'Productdesc', 'ParentName'])
+                reorderd_columns = ["Symbol", "Category", "ExpiryDate", "PreviousClose", "Open", "High", "Low", "LTP", "TotalBuyQty", 
+                                    "TotalsellQty", "Volume", "AveragePrice", "PercentChange", "AbsoluteChange","UnderlineValue", "OpenInterest", 
+                                    "ChangeInOpenInterest", "LifeTimeHigh", "LifeTimeLow", "DailyVolatility", "PriceQuoteUnit", "TradingUnit",  "VaR"]
+                df = df[reorderd_columns]
+            elif instrument == "option":
+                df = df.drop(columns=['ExtensionData', 'Productdesc', 'ParentName'])
+                reorderd_columns = ["Symbol","InstrumentName", "Category", "ExpiryDate", "PreviousClose", "Open","High", 
+                                    "Low", "LTP", "TotalBuyQty", "TotalsellQty", "Volume", "AveragePrice","PercentChange", 
+                                    "AbsoluteChange", "UnderlineValue", "OptionType", "StrikePrice", "OpenInterest", 
+                                    "ChangeInOpenInterest", "LifeTimeHigh", "LifeTimeLow", "DailyVolatility", 
+                                    "PriceQuoteUnit", "TradingUnit", "VaR"]
+                df = df[reorderd_columns]
+            df["ExpiryDate"] = pd.to_datetime(df["ExpiryDate"], format="%d-%b-%Y", dayfirst=True, errors='coerce')
+        elif outputtype == "bidask":
+            df = pd.DataFrame(res['d']['Data'][0]['QuoteBid'])
+            df.insert(0, "Symbol", commodity) 
+            if instrument == "option":
+                df = df.drop(columns=["ExtensionData"])       
+        df.insert(0, "Timestamp",convert_to_ist(res['d']['Summary']['AsOn']))
+        return df
+    except Exception as e:
+        print(f"Error :: {e}")
```

### Comparing `mcxpy-0.0.2/pyproject.toml` & `mcxpy-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mcxpy"
-version = "0.0.2"
+version = "0.0.3"
 description = "For fetching mcx data"
 authors = [{ name = "Tapan Hazarika" }]
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = ["pandas>=2.0.0","requests"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

