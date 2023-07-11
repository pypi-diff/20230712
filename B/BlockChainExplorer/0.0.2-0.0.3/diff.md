# Comparing `tmp/BlockChainExplorer-0.0.2.tar.gz` & `tmp/BlockChainExplorer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlockChainExplorer-0.0.2.tar", last modified: Thu Jun 29 01:24:07 2023, max compression
+gzip compressed data, was "BlockChainExplorer-0.0.3.tar", last modified: Tue Jul 11 22:28:03 2023, max compression
```

## Comparing `BlockChainExplorer-0.0.2.tar` & `BlockChainExplorer-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 01:24:07.041676 BlockChainExplorer-0.0.2/
--rw-rw-rw-   0        0        0     1089 2023-06-28 00:52:17.000000 BlockChainExplorer-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3579 2023-06-29 01:24:07.040677 BlockChainExplorer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1745 2023-06-28 02:24:53.000000 BlockChainExplorer-0.0.2/README.md
--rw-rw-rw-   0        0        0      739 2023-06-29 01:23:49.000000 BlockChainExplorer-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 01:24:07.041676 BlockChainExplorer-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 01:24:06.987676 BlockChainExplorer-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 01:24:07.001675 BlockChainExplorer-0.0.2/src/BlockChainExplorer/
--rw-rw-rw-   0        0        0     6008 2023-06-29 01:15:22.000000 BlockChainExplorer-0.0.2/src/BlockChainExplorer/BlockChainExplorer.py
--rw-rw-rw-   0        0        0        0 2023-06-28 00:28:53.000000 BlockChainExplorer-0.0.2/src/BlockChainExplorer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 01:24:07.037674 BlockChainExplorer-0.0.2/src/BlockChainExplorer.egg-info/
--rw-rw-rw-   0        0        0     3579 2023-06-29 01:24:06.000000 BlockChainExplorer-0.0.2/src/BlockChainExplorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-06-29 01:24:06.000000 BlockChainExplorer-0.0.2/src/BlockChainExplorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 01:24:06.000000 BlockChainExplorer-0.0.2/src/BlockChainExplorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 01:24:06.000000 BlockChainExplorer-0.0.2/src/BlockChainExplorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-29 01:24:06.000000 BlockChainExplorer-0.0.2/src/BlockChainExplorer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 22:28:03.436885 BlockChainExplorer-0.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-06-28 00:52:17.000000 BlockChainExplorer-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3579 2023-07-11 22:28:03.435885 BlockChainExplorer-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1745 2023-06-28 02:24:53.000000 BlockChainExplorer-0.0.3/README.md
+-rw-rw-rw-   0        0        0      739 2023-07-11 22:27:03.000000 BlockChainExplorer-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 22:28:03.437885 BlockChainExplorer-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 22:28:03.417882 BlockChainExplorer-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 22:28:03.423881 BlockChainExplorer-0.0.3/src/BlockChainExplorer/
+-rw-rw-rw-   0        0        0     6028 2023-07-10 02:20:53.000000 BlockChainExplorer-0.0.3/src/BlockChainExplorer/BlockChainExplorer.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 00:28:53.000000 BlockChainExplorer-0.0.3/src/BlockChainExplorer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 22:28:03.433882 BlockChainExplorer-0.0.3/src/BlockChainExplorer.egg-info/
+-rw-rw-rw-   0        0        0     3579 2023-07-11 22:28:03.000000 BlockChainExplorer-0.0.3/src/BlockChainExplorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-07-11 22:28:03.000000 BlockChainExplorer-0.0.3/src/BlockChainExplorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 22:28:03.000000 BlockChainExplorer-0.0.3/src/BlockChainExplorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-11 22:28:03.000000 BlockChainExplorer-0.0.3/src/BlockChainExplorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-11 22:28:03.000000 BlockChainExplorer-0.0.3/src/BlockChainExplorer.egg-info/top_level.txt
```

### Comparing `BlockChainExplorer-0.0.2/LICENSE.txt` & `BlockChainExplorer-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BlockChainExplorer-0.0.2/PKG-INFO` & `BlockChainExplorer-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlockChainExplorer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple package to access EVM blockchain explorers, currently supports Binance Smart Chain, Ethereum, Avalanche and Polygon
 Author-email: ManiacalEngineer <unhfireboy@yahoo.com>
 License: MIT License
         
         Copyright (c) 2023 Sean Bicknell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `BlockChainExplorer-0.0.2/README.md` & `BlockChainExplorer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `BlockChainExplorer-0.0.2/pyproject.toml` & `BlockChainExplorer-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BlockChainExplorer"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="ManiacalEngineer", email="unhfireboy@yahoo.com"},
 ]
 license = { file = "LICENSE.txt" }
 description = "Simple package to access EVM blockchain explorers, currently supports Binance Smart Chain, Ethereum, Avalanche and Polygon"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `BlockChainExplorer-0.0.2/src/BlockChainExplorer/BlockChainExplorer.py` & `BlockChainExplorer-0.0.3/src/BlockChainExplorer/BlockChainExplorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,19 +113,19 @@
 	def getContractCreation(self, address: str):
 		"""takes a single contract address as a string or a list of upto 5 contract addresses and returns the creator wallet and transaction hash as a list of dicts"""
 		if isinstance(address, list):
 			if not (len(address) > 5):
 				addressStr = address[0]
 				for addy in address:
 					addressStr += ', ' + addy
-				request_url = f"{self.chain}?module=contract&action=getcontractcreation&address={addressStr}&tag=latest&apikey={self.api_key}"
+				request_url = f"{self.chain}?module=contract&action=getcontractcreation&contractaddresses={addressStr}&tag=latest&apikey={self.api_key}"
 				response = requests.get(request_url).json()
 				return responseCheck(response)
 		else:
-			request_url = f"{self.chain}?module=contract&action=getcontractcreation&address={address}&tag=latest&apikey={self.api_key}"
+			request_url = f"{self.chain}?module=contract&action=getcontractcreation&contractaddresses={address}&tag=latest&apikey={self.api_key}"
 			response = requests.get(request_url).json()
 			return self.responseCheck(response)
 
 		return -1		
 
 	
 	def getInternalTransactionsByTx(self, tx: str):
```

### Comparing `BlockChainExplorer-0.0.2/src/BlockChainExplorer.egg-info/PKG-INFO` & `BlockChainExplorer-0.0.3/src/BlockChainExplorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlockChainExplorer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple package to access EVM blockchain explorers, currently supports Binance Smart Chain, Ethereum, Avalanche and Polygon
 Author-email: ManiacalEngineer <unhfireboy@yahoo.com>
 License: MIT License
         
         Copyright (c) 2023 Sean Bicknell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

