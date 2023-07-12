# Comparing `tmp/stock_market_bytetheory-1.0.3.tar.gz` & `tmp/stock_market_bytetheory-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stock_market_bytetheory-1.0.3.tar", last modified: Sun May 14 19:34:16 2023, max compression
+gzip compressed data, was "stock_market_bytetheory-1.0.4.tar", last modified: Wed Jul 12 18:17:16 2023, max compression
```

## Comparing `stock_market_bytetheory-1.0.3.tar` & `stock_market_bytetheory-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-14 19:34:16.387317 stock_market_bytetheory-1.0.3/
--rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-03-31 18:16:25.000000 stock_market_bytetheory-1.0.3/LICENSE
--rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-05-14 19:34:16.387412 stock_market_bytetheory-1.0.3/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-03-31 22:41:33.000000 stock_market_bytetheory-1.0.3/README.md
--rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-03-31 18:46:07.000000 stock_market_bytetheory-1.0.3/pyproject.toml
--rw-r--r--   0 robertblom   (501) staff       (20)      587 2023-05-14 19:34:16.387755 stock_market_bytetheory-1.0.3/setup.cfg
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-14 19:34:16.380504 stock_market_bytetheory-1.0.3/src/
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-14 19:34:16.381716 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/
--rw-r--r--   0 robertblom   (501) staff       (20)     5191 2023-05-14 19:29:32.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/SP500History.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2169 2023-04-25 19:21:06.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/SectorIndustryTickerParser.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2281 2023-04-26 18:36:16.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/TickerLevelDataParser.py
--rw-r--r--   0 robertblom   (501) staff       (20)      231 2023-04-25 19:59:08.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-14 19:34:16.387206 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/
--rw-r--r--   0 robertblom   (501) staff       (20)  5204000 2023-03-31 20:35:29.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/SP500_ind.csv
--rw-r--r--   0 robertblom   (501) staff       (20)    60623 2023-04-24 21:18:29.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/SP_500.xml
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-24 20:04:28.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-05-14 19:34:16.382637 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/
--rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-05-14 19:34:16.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)      577 2023-05-14 19:34:16.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/SOURCES.txt
--rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-05-14 19:34:16.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/dependency_links.txt
--rw-r--r--   0 robertblom   (501) staff       (20)       24 2023-05-14 19:34:16.000000 stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/top_level.txt
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-07-12 18:17:16.222904 stock_market_bytetheory-1.0.4/
+-rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-03-31 18:16:25.000000 stock_market_bytetheory-1.0.4/LICENSE
+-rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-07-12 18:17:16.223002 stock_market_bytetheory-1.0.4/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-03-31 22:41:33.000000 stock_market_bytetheory-1.0.4/README.md
+-rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-03-31 18:46:07.000000 stock_market_bytetheory-1.0.4/pyproject.toml
+-rw-r--r--   0 robertblom   (501) staff       (20)      587 2023-07-12 18:17:16.223607 stock_market_bytetheory-1.0.4/setup.cfg
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-07-12 18:17:16.208380 stock_market_bytetheory-1.0.4/src/
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-07-12 18:17:16.210086 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/
+-rw-r--r--   0 robertblom   (501) staff       (20)     5191 2023-05-14 19:29:32.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/SP500History.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2169 2023-04-25 19:21:06.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/SectorIndustryTickerParser.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2281 2023-04-26 18:36:16.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/TickerLevelDataParser.py
+-rw-r--r--   0 robertblom   (501) staff       (20)      231 2023-04-25 19:59:08.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-07-12 18:17:16.222789 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/data/
+-rw-r--r--   0 robertblom   (501) staff       (20)  5204000 2023-03-31 20:35:29.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/data/SP500_ind.csv
+-rw-r--r--   0 robertblom   (501) staff       (20)    60120 2023-07-12 18:15:00.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/data/SP_500.xml
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-24 20:04:28.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/data/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-07-12 18:17:16.210581 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory.egg-info/
+-rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-07-12 18:17:16.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory.egg-info/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)      577 2023-07-12 18:17:16.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory.egg-info/SOURCES.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-07-12 18:17:16.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory.egg-info/dependency_links.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)       24 2023-07-12 18:17:16.000000 stock_market_bytetheory-1.0.4/src/stock_market_bytetheory.egg-info/top_level.txt
```

### Comparing `stock_market_bytetheory-1.0.3/LICENSE` & `stock_market_bytetheory-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.3/setup.cfg` & `stock_market_bytetheory-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stock_market_bytetheory
-version = 1.0.3
+version = 1.0.4
 author = Robbie Blom
 description = Provides some sample stock data and helpers for supporting a stock samples app
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/SP500History.py` & `stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/SP500History.py`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/SectorIndustryTickerParser.py` & `stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/SectorIndustryTickerParser.py`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/TickerLevelDataParser.py` & `stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/TickerLevelDataParser.py`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/SP500_ind.csv` & `stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/data/SP500_ind.csv`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/SP_500.xml` & `stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/data/SP_500.xml`

 * *Files 0% similar despite different names*

#### Comparing `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory/data/SP_500.xml` & `stock_market_bytetheory-1.0.4/src/stock_market_bytetheory/data/SP_500.xml`

```diff
@@ -29,16 +29,15 @@
   <symbol ticker="MO" name="Altria Group Inc" type="stock" sector="Consumer Staples" industry="Tobacco"/>
   <symbol ticker="AMZN" name="Amazon.com Inc" type="stock" sector="Consumer Discretionary" industry="Internet Retail"/>
   <symbol ticker="AEE" name="Ameren Corp" type="stock" sector="Utilities" industry="Multi-Utilities &amp; Unregulated Power"/>
   <symbol ticker="AEP" name="American Electric Power" type="stock" sector="Utilities" industry="Electric Utilities"/>
   <symbol ticker="AXP" name="American Express Co" type="stock" sector="Financials" industry="Consumer Finance"/>
   <symbol ticker="AMT" name="American Tower Corp A" type="stock" sector="Financials" industry="REITs"/>
   <symbol ticker="AMP" name="Ameriprise Financial" type="stock" sector="Financials" industry="Diversified Financial Services"/>
-  <symbol ticker="ABC" name="AmerisourceBergen Corp" type="stock" sector="Health Care" industry="Health Care Distribution &amp; Services"/>
-  <symbol ticker="AME" name="Ametek" type="stock" sector="Industrials" industry="Electrical Components and Equipment"/>
+  <symbol ticker="ABC" name="AmerisourceBergen Corp" type="stock" sector="Health Care" industry="Health Care Distributors &amp; Services"/>
   <symbol ticker="AMGN" name="Amgen Inc" type="stock" sector="Health Care" industry="Biotechnology"/>
   <symbol ticker="APH" name="Amphenol Corp A" type="stock" sector="Industrials" industry="Electrical Components &amp; Equipment"/>
   <symbol ticker="APC" name="Anadarko Petroleum Corp" type="stock" sector="Energy" industry="Oil &amp; Gas Exploration &amp; Production"/>
   <symbol ticker="ADI" name="Analog Devices, Inc." type="stock" sector="Information Technology" industry="Semiconductors"/>
   <symbol ticker="AON" name="Aon plc" type="stock" sector="Financials" industry="Insurance Brokers"/>
   <symbol ticker="APA" name="Apache Corporation" type="stock" sector="Energy" industry="Oil &amp; Gas Exploration &amp; Production"/>
   <symbol ticker="AAPL" name="Apple Inc." type="stock" sector="Information Technology" industry="Computer Hardware"/>
@@ -122,15 +121,14 @@
   <symbol ticker="COP" name="ConocoPhillips" type="stock" sector="Energy" industry="Integrated Oil &amp; Gas"/>
   <symbol ticker="CNX" name="CONSOL Energy Inc." type="stock" sector="Energy" industry="Oil &amp; Gas Exploration &amp; Production"/>
   <symbol ticker="ED" name="Consolidated Edison" type="stock" sector="Utilities" industry="Multi-Utilities &amp; Unregulated Power"/>
   <symbol ticker="STZ" name="Constellation Brands" type="stock" sector="Consumer Staples" industry="Distillers &amp; Vintners"/>
   <symbol ticker="GLW" name="Corning Inc." type="stock" sector="Industrials" industry="Construction &amp; Engineering"/>
   <symbol ticker="COST" name="Costco Co." type="stock" sector="Consumer Staples" industry="Hypermarkets &amp; Super Centers"/>
   <symbol ticker="COV" name="Covidien plc" type="stock" sector="Health Care" industry="Health Care Equipment &amp; Services"/>
-  <symbol ticker="CCI" name="Crown Castle International Corp." type="stock" sector="Telecommunications Services" industry="Wireless Telecommunications Services"/>
   <symbol ticker="CSX" name="CSX Corp." type="stock" sector="Industrials" industry="Railroads"/>
   <symbol ticker="CMI" name="Cummins Inc." type="stock" sector="Industrials" industry="Industrial Machinery"/>
   <symbol ticker="CVS" name="CVS Caremark Corp." type="stock" sector="Consumer Staples" industry="Drug Retail"/>
   <symbol ticker="DHI" name="D. R. Horton" type="stock" sector="Consumer Discretionary" industry="Construction"/>
   <symbol ticker="DHR" name="Danaher Corp." type="stock" sector="Industrials" industry="Industrial Machinery"/>
   <symbol ticker="DRI" name="Darden Restaurants" type="stock" sector="Consumer Discretionary" industry="Restaurants"/>
   <symbol ticker="DVA" name="DaVita Inc." type="stock" sector="Health Care" industry="Health Care Facilities"/>
@@ -278,15 +276,14 @@
   <symbol ticker="LMT" name="Lockheed Martin Corp." type="stock" sector="Industrials" industry="Aerospace &amp; Defense"/>
   <symbol ticker="L" name="Loews Corp." type="stock" sector="Financials" industry="Multi-Sector Holdings"/>
   <symbol ticker="LO" name="Lorillard Inc." type="stock" sector="Consumer Staples" industry="Tobacco"/>
   <symbol ticker="LOW" name="Lowe's Cos." type="stock" sector="Consumer Discretionary" industry="Home Improvement Retail"/>
   <symbol ticker="LSI" name="LSI Corporation" type="stock" sector="Information Technology" industry="Semiconductors"/>
   <symbol ticker="LYB" name="LyondellBasell" type="stock" sector="Materials" industry="Diversified Chemicals"/>
   <symbol ticker="MTB" name="M&amp;T Bank Corp." type="stock" sector="Financials" industry="Banks"/>
-  <symbol ticker="MAC" name="Macerich" type="stock" sector="Financials" industry="Retail REITs"/>
   <symbol ticker="M" name="Macy's Inc." type="stock" sector="Consumer Discretionary" industry="Department Stores"/>
   <symbol ticker="MRO" name="Marathon Oil Corp." type="stock" sector="Energy" industry="Oil &amp; Gas Exploration &amp; Production"/>
   <symbol ticker="MPC" name="Marathon Petroleum" type="stock" sector="Energy" industry="Oil &amp; Gas Refining &amp; Marketing &amp; Transportation"/>
   <symbol ticker="MAR" name="Marriott Int'l." type="stock" sector="Consumer Discretionary" industry="Hotels, Resorts &amp; Cruise Lines"/>
   <symbol ticker="MMC" name="Marsh &amp; McLennan" type="stock" sector="Financials" industry="Insurance Brokers"/>
   <symbol ticker="MAS" name="Masco Corp." type="stock" sector="Industrials" industry="Building Products"/>
   <symbol ticker="MA" name="Mastercard Inc." type="stock" sector="Information Technology" industry="Internet Software &amp; Services"/>
@@ -320,15 +317,14 @@
   <symbol ticker="NTAP" name="NetApp" type="stock" sector="Information Technology" industry="Internet Software &amp; Services"/>
   <symbol ticker="NFLX" name="NetFlix Inc." type="stock" sector="Information Technology" industry="Internet Software &amp; Services"/>
   <symbol ticker="NWL" name="Newell Rubbermaid Co." type="stock" sector="Consumer Discretionary" industry="Housewares &amp; Specialties"/>
   <symbol ticker="NFX" name="Newfield Exploration Co" type="stock" sector="Energy" industry="Oil &amp; Gas Exploration &amp; Production"/>
   <symbol ticker="NEM" name="Newmont Mining Corp. (Hldg. Co.)" type="stock" sector="Materials" industry="Gold"/>
   <symbol ticker="NWSA" name="News Corporation" type="stock" sector="Consumer Discretionary" industry="Publishing"/>
   <symbol ticker="NEE" name="NextEra Energy Resources" type="stock" sector="Utilities" industry="Multi-Utilities &amp; Unregulated Power"/>
-  <symbol ticker="NLSN" name="Nielsen Holdings" type="stock" sector="Industrials" industry="Research &amp; Consulting Services"/>
   <symbol ticker="NKE" name="NIKE Inc." type="stock" sector="Consumer Discretionary" industry="Apparel, Accessories &amp; Luxury Goods"/>
   <symbol ticker="NI" name="NiSource Inc." type="stock" sector="Utilities" industry="Multi-Utilities &amp; Unregulated Power"/>
   <symbol ticker="NE" name="Noble Corp" type="stock" sector="Energy" industry="Oil &amp; Gas Drilling"/>
   <symbol ticker="NBL" name="Noble Energy Inc" type="stock" sector="Energy" industry="Oil &amp; Gas Exploration &amp; Production"/>
   <symbol ticker="JWN" name="Nordstrom" type="stock" sector="Consumer Discretionary" industry="Department Stores"/>
   <symbol ticker="NSC" name="Norfolk Southern Corp." type="stock" sector="Industrials" industry="Railroads"/>
   <symbol ticker="NTRS" name="Northern Trust Corp." type="stock" sector="Financials" industry="Diversified Financial Services"/>
```

### Comparing `stock_market_bytetheory-1.0.3/src/stock_market_bytetheory.egg-info/SOURCES.txt` & `stock_market_bytetheory-1.0.4/src/stock_market_bytetheory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

