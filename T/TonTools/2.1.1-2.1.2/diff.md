# Comparing `tmp/TonTools-2.1.1.tar.gz` & `tmp/TonTools-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TonTools-2.1.1.tar", last modified: Sat Jul  1 13:19:37 2023, max compression
+gzip compressed data, was "dist/TonTools-2.1.2.tar", last modified: Wed Jul 12 18:15:16 2023, max compression
```

## Comparing `TonTools-2.1.1.tar` & `TonTools-2.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-01 13:19:37.806505 TonTools-2.1.1/
--rw-r--r--   0 maxankurb   (501) staff       (20)     1071 2023-03-09 07:49:38.000000 TonTools-2.1.1/LICENSE
--rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-07-01 13:19:37.806196 TonTools-2.1.1/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)    11720 2023-07-01 13:13:19.000000 TonTools-2.1.1/README.md
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-01 13:19:37.797068 TonTools-2.1.1/TonTools/
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-01 13:19:37.801349 TonTools-2.1.1/TonTools/Contracts/
--rw-r--r--   0 maxankurb   (501) staff       (20)     5376 2023-07-01 13:03:20.000000 TonTools-2.1.1/TonTools/Contracts/Contract.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     3909 2023-06-06 11:47:34.000000 TonTools-2.1.1/TonTools/Contracts/Jetton.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     5661 2023-03-01 07:15:23.000000 TonTools-2.1.1/TonTools/Contracts/NFT.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     6091 2023-03-29 17:48:14.000000 TonTools-2.1.1/TonTools/Contracts/Wallet.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     1336 2023-05-22 11:16:39.000000 TonTools-2.1.1/TonTools/Contracts/utils.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-01 13:19:37.805796 TonTools-2.1.1/TonTools/Providers/
--rw-r--r--   0 maxankurb   (501) staff       (20)    21420 2023-06-06 11:47:34.000000 TonTools-2.1.1/TonTools/Providers/DtonClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    15041 2023-03-01 08:22:28.000000 TonTools-2.1.1/TonTools/Providers/LsClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    10949 2023-05-22 11:16:39.000000 TonTools-2.1.1/TonTools/Providers/TonApiClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)    16477 2023-07-01 13:07:06.000000 TonTools-2.1.1/TonTools/Providers/TonCenterClient.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     4437 2023-07-01 12:59:15.000000 TonTools-2.1.1/TonTools/Providers/_orbs_ton_access.py
--rw-r--r--   0 maxankurb   (501) staff       (20)     2569 2023-07-01 12:46:44.000000 TonTools-2.1.1/TonTools/Providers/utils.py
--rw-r--r--   0 maxankurb   (501) staff       (20)      323 2023-05-22 11:16:39.000000 TonTools-2.1.1/TonTools/__init__.py
-drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-01 13:19:37.799027 TonTools-2.1.1/TonTools.egg-info/
--rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-07-01 13:19:37.000000 TonTools-2.1.1/TonTools.egg-info/PKG-INFO
--rw-r--r--   0 maxankurb   (501) staff       (20)      553 2023-07-01 13:19:37.000000 TonTools-2.1.1/TonTools.egg-info/SOURCES.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-07-01 13:19:37.000000 TonTools-2.1.1/TonTools.egg-info/dependency_links.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)      114 2023-07-01 13:19:37.000000 TonTools-2.1.1/TonTools.egg-info/requires.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       47 2023-07-01 13:19:37.000000 TonTools-2.1.1/TonTools.egg-info/top_level.txt
--rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-07-01 13:19:37.806592 TonTools-2.1.1/setup.cfg
--rw-r--r--   0 maxankurb   (501) staff       (20)      513 2023-07-01 13:17:10.000000 TonTools-2.1.1/setup.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-12 18:15:16.801103 TonTools-2.1.2/
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1071 2023-03-09 07:49:38.000000 TonTools-2.1.2/LICENSE
+-rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-07-12 18:15:16.782609 TonTools-2.1.2/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)    11720 2023-07-01 13:13:19.000000 TonTools-2.1.2/README.md
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-12 18:15:12.620212 TonTools-2.1.2/TonTools/
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-12 18:15:16.694485 TonTools-2.1.2/TonTools/Contracts/
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5376 2023-07-01 13:03:20.000000 TonTools-2.1.2/TonTools/Contracts/Contract.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     3909 2023-06-06 11:47:34.000000 TonTools-2.1.2/TonTools/Contracts/Jetton.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     5661 2023-03-01 07:15:23.000000 TonTools-2.1.2/TonTools/Contracts/NFT.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     6091 2023-03-29 17:48:14.000000 TonTools-2.1.2/TonTools/Contracts/Wallet.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     1336 2023-05-22 11:16:39.000000 TonTools-2.1.2/TonTools/Contracts/utils.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-12 18:15:16.763034 TonTools-2.1.2/TonTools/Providers/
+-rw-r--r--   0 maxankurb   (501) staff       (20)    21442 2023-07-12 18:14:06.000000 TonTools-2.1.2/TonTools/Providers/DtonClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    15041 2023-03-01 08:22:28.000000 TonTools-2.1.2/TonTools/Providers/LsClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    10949 2023-05-22 11:16:39.000000 TonTools-2.1.2/TonTools/Providers/TonApiClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)    16477 2023-07-01 13:07:06.000000 TonTools-2.1.2/TonTools/Providers/TonCenterClient.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     4437 2023-07-01 12:59:15.000000 TonTools-2.1.2/TonTools/Providers/_orbs_ton_access.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)     2569 2023-07-01 12:46:44.000000 TonTools-2.1.2/TonTools/Providers/utils.py
+-rw-r--r--   0 maxankurb   (501) staff       (20)      323 2023-05-22 11:16:39.000000 TonTools-2.1.2/TonTools/__init__.py
+drwxr-xr-x   0 maxankurb   (501) staff       (20)        0 2023-07-12 18:15:16.675881 TonTools-2.1.2/TonTools.egg-info/
+-rw-r--r--   0 maxankurb   (501) staff       (20)      202 2023-07-12 18:15:12.000000 TonTools-2.1.2/TonTools.egg-info/PKG-INFO
+-rw-r--r--   0 maxankurb   (501) staff       (20)      553 2023-07-12 18:15:12.000000 TonTools-2.1.2/TonTools.egg-info/SOURCES.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)        1 2023-07-12 18:15:12.000000 TonTools-2.1.2/TonTools.egg-info/dependency_links.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)      114 2023-07-12 18:15:12.000000 TonTools-2.1.2/TonTools.egg-info/requires.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       47 2023-07-12 18:15:12.000000 TonTools-2.1.2/TonTools.egg-info/top_level.txt
+-rw-r--r--   0 maxankurb   (501) staff       (20)       38 2023-07-12 18:15:16.808286 TonTools-2.1.2/setup.cfg
+-rw-r--r--   0 maxankurb   (501) staff       (20)      513 2023-07-12 18:14:30.000000 TonTools-2.1.2/setup.py
```

### Comparing `TonTools-2.1.1/LICENSE` & `TonTools-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/README.md` & `TonTools-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools/Contracts/Contract.py` & `TonTools-2.1.2/TonTools/Contracts/Contract.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools/Contracts/Jetton.py` & `TonTools-2.1.2/TonTools/Contracts/Jetton.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools/Contracts/NFT.py` & `TonTools-2.1.2/TonTools/Contracts/NFT.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools/Contracts/Wallet.py` & `TonTools-2.1.2/TonTools/Contracts/Wallet.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools/Contracts/utils.py` & `TonTools-2.1.2/TonTools/Contracts/utils.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools/Providers/DtonClient.py` & `TonTools-2.1.2/TonTools/Providers/DtonClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,14 +309,15 @@
             ['address', 'workchain'], parsed_nft_collection_address_workchain=Address(collection.address).wc,
             parsed_nft_collection_address_address=Address(collection.address).hash_part.hex().upper(),
             parsed_nft_true_nft_in_collection=1, order_by="parsed_nft_index"
         )
         result = []
         for item in data:
             result.append(NftItem(self._process_address(self.get_addr_from_wc_hex(item['workchain'], item['address'])), self))
+        return result
 
     async def get_transactions(self, address: str, limit: int = -1, limit_per_one_request: int = 150):
         transactions = await self.raw_get_transactions(
             fields=[
                 'gen_utime', 'total_fees_grams', 'hash', 'lt', 'compute_ph_success',
                 'action_ph_success', 'in_msg_created_lt', 'in_msg_src_addr_workchain_id',
                 'in_msg_src_addr_address_hex', 'in_msg_dest_addr_workchain_id', 'in_msg_dest_addr_address_hex',
```

### Comparing `TonTools-2.1.1/TonTools/Providers/LsClient.py` & `TonTools-2.1.2/TonTools/Providers/LsClient.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools/Providers/TonApiClient.py` & `TonTools-2.1.2/TonTools/Providers/TonApiClient.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools/Providers/TonCenterClient.py` & `TonTools-2.1.2/TonTools/Providers/TonCenterClient.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools/Providers/_orbs_ton_access.py` & `TonTools-2.1.2/TonTools/Providers/_orbs_ton_access.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools/Providers/utils.py` & `TonTools-2.1.2/TonTools/Providers/utils.py`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/TonTools.egg-info/SOURCES.txt` & `TonTools-2.1.2/TonTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TonTools-2.1.1/setup.py` & `TonTools-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 import setuptools
 
 requirements = ["tonsdk>=1.0.13", "ton>=0.26", "aiohttp>=3.8.1", "setuptools>=65.3.0", "requests>=2.28.1", "pytonlib>=0.0.46", "graphql-query==1.0.3"]
 
 setup(
     name='TonTools',
-    version='2.1.1',
+    version='2.1.2',
     packages=['TonTools', 'TonTools/Contracts', 'TonTools/Providers'],
     url='',
     license='MIT License',
     author='yungwine',
     author_email='cyrbatoff@gmail.com',
     description='Explore TON Blockchain with python',
     install_requires=requirements,
```

