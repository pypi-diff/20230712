# Comparing `tmp/ln-markets-2.0.1.tar.gz` & `tmp/ln-markets-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ln-markets-2.0.1.tar", last modified: Mon May 29 17:44:18 2023, max compression
+gzip compressed data, was "ln-markets-2.0.2.tar", last modified: Wed Jul 12 15:07:51 2023, max compression
```

## Comparing `ln-markets-2.0.1.tar` & `ln-markets-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-05-29 17:44:18.117904 ln-markets-2.0.1/
--rw-rw-r--   0 romain    (1000) romain    (1000)     1067 2022-05-10 09:43:34.000000 ln-markets-2.0.1/LICENSE
--rw-rw-r--   0 romain    (1000) romain    (1000)    19538 2023-05-29 17:44:18.117904 ln-markets-2.0.1/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)    18701 2023-05-29 17:42:35.000000 ln-markets-2.0.1/README.md
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-05-29 17:44:18.113904 ln-markets-2.0.1/ln_markets.egg-info/
--rw-rw-r--   0 romain    (1000) romain    (1000)    19538 2023-05-29 17:44:18.000000 ln-markets-2.0.1/ln_markets.egg-info/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)      309 2023-05-29 17:44:18.000000 ln-markets-2.0.1/ln_markets.egg-info/SOURCES.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2023-05-29 17:44:18.000000 ln-markets-2.0.1/ln_markets.egg-info/dependency_links.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       26 2023-05-29 17:44:18.000000 ln-markets-2.0.1/ln_markets.egg-info/requires.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       10 2023-05-29 17:44:18.000000 ln-markets-2.0.1/ln_markets.egg-info/top_level.txt
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-05-29 17:44:18.117904 ln-markets-2.0.1/lnmarkets/
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-10 09:43:34.000000 ln-markets-2.0.1/lnmarkets/__init__.py
--rw-rw-r--   0 romain    (1000) romain    (1000)    12695 2023-05-29 17:42:35.000000 ln-markets-2.0.1/lnmarkets/rest.py
--rw-rw-r--   0 romain    (1000) romain    (1000)     2349 2023-05-29 17:42:35.000000 ln-markets-2.0.1/lnmarkets/websockets.py
--rw-rw-r--   0 romain    (1000) romain    (1000)      104 2022-05-10 09:43:34.000000 ln-markets-2.0.1/pyproject.toml
--rw-rw-r--   0 romain    (1000) romain    (1000)       89 2023-05-29 17:44:18.117904 ln-markets-2.0.1/setup.cfg
--rw-rw-r--   0 romain    (1000) romain    (1000)     1192 2023-05-29 17:43:55.000000 ln-markets-2.0.1/setup.py
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-05-29 17:44:18.117904 ln-markets-2.0.1/tests/
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-10 09:43:34.000000 ln-markets-2.0.1/tests/test_node_state.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-07-12 15:07:51.019231 ln-markets-2.0.2/
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1067 2022-05-10 09:43:34.000000 ln-markets-2.0.2/LICENSE
+-rw-rw-r--   0 romain    (1000) romain    (1000)    19592 2023-07-12 15:07:51.019231 ln-markets-2.0.2/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)    18755 2023-07-12 15:06:50.000000 ln-markets-2.0.2/README.md
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-07-12 15:07:51.015231 ln-markets-2.0.2/ln_markets.egg-info/
+-rw-rw-r--   0 romain    (1000) romain    (1000)    19592 2023-07-12 15:07:51.000000 ln-markets-2.0.2/ln_markets.egg-info/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)      309 2023-07-12 15:07:51.000000 ln-markets-2.0.2/ln_markets.egg-info/SOURCES.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2023-07-12 15:07:51.000000 ln-markets-2.0.2/ln_markets.egg-info/dependency_links.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       26 2023-07-12 15:07:51.000000 ln-markets-2.0.2/ln_markets.egg-info/requires.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       10 2023-07-12 15:07:51.000000 ln-markets-2.0.2/ln_markets.egg-info/top_level.txt
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-07-12 15:07:51.019231 ln-markets-2.0.2/lnmarkets/
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-10 09:43:34.000000 ln-markets-2.0.2/lnmarkets/__init__.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)    12695 2023-05-29 17:42:35.000000 ln-markets-2.0.2/lnmarkets/rest.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)     2359 2023-07-12 15:06:50.000000 ln-markets-2.0.2/lnmarkets/websockets.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)      104 2022-05-10 09:43:34.000000 ln-markets-2.0.2/pyproject.toml
+-rw-rw-r--   0 romain    (1000) romain    (1000)       89 2023-07-12 15:07:51.019231 ln-markets-2.0.2/setup.cfg
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1192 2023-07-12 15:06:50.000000 ln-markets-2.0.2/setup.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2023-07-12 15:07:51.019231 ln-markets-2.0.2/tests/
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-10 09:43:34.000000 ln-markets-2.0.2/tests/test_node_state.py
```

### Comparing `ln-markets-2.0.1/LICENSE` & `ln-markets-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ln-markets-2.0.1/PKG-INFO` & `ln-markets-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ln-markets
-Version: 2.0.1
+Version: 2.0.2
 Summary: LN Markets API python implementation
 Home-page: https://github.com/ln-markets/api-python
 Author: Romain ROUPHAEL
 License: MIT
 Keywords: lnmarkets trading rest api bitcoin lightning network futures options
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,24 +24,26 @@
 A simple way to connect your Python application to [LN Markets](https://lnmarkets.com/)!
 
 ## Install
 
 You can install this package with pip:
 ```shell
 pip3 install ln-markets
+```
 
-## Usage
+## Use
 
-You can import rest class from ln_markets
+You can import the rest class from lnmarkets
 ```python
 from lnmarkets import rest
 ```
-And the websocket one as well!
+And the websocket class as well
 ```python
 from lnmarkets import websockets
+```
 
 ## Authentication
 
 > For authentication you need your api **key** **secret** and **passphrase**
 
 Without you will not bet able to authenticate
 
@@ -63,15 +65,15 @@
 lnm.connect()
 ```
 
 > Check [examples](examples/websocket/README.md) for more details as you'll need to extend this class most of the time.
 
 ### Subscription
 
-You can subscribe to LNM Markets public event such as futures bid offer, index and options data.
+You can subscribe to LNM Markets public event such as futures last price ('futures:btc_usd:last-price') and index ('futures:btc_usd:index').
 
 ## REST API
 
 ### Configuration
 
 Use the LNMarketsRest and your key / passphrase to instanciate a new api connector:
```

### Comparing `ln-markets-2.0.1/README.md` & `ln-markets-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 A simple way to connect your Python application to [LN Markets](https://lnmarkets.com/)!
 
 ## Install
 
 You can install this package with pip:
 ```shell
 pip3 install ln-markets
+```
 
-## Usage
+## Use
 
-You can import rest class from ln_markets
+You can import the rest class from lnmarkets
 ```python
 from lnmarkets import rest
 ```
-And the websocket one as well!
+And the websocket class as well
 ```python
 from lnmarkets import websockets
+```
 
 ## Authentication
 
 > For authentication you need your api **key** **secret** and **passphrase**
 
 Without you will not bet able to authenticate
 
@@ -42,15 +44,15 @@
 lnm.connect()
 ```
 
 > Check [examples](examples/websocket/README.md) for more details as you'll need to extend this class most of the time.
 
 ### Subscription
 
-You can subscribe to LNM Markets public event such as futures bid offer, index and options data.
+You can subscribe to LNM Markets public event such as futures last price ('futures:btc_usd:last-price') and index ('futures:btc_usd:index').
 
 ## REST API
 
 ### Configuration
 
 Use the LNMarketsRest and your key / passphrase to instanciate a new api connector:
```

### Comparing `ln-markets-2.0.1/ln_markets.egg-info/PKG-INFO` & `ln-markets-2.0.2/ln_markets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ln-markets
-Version: 2.0.1
+Version: 2.0.2
 Summary: LN Markets API python implementation
 Home-page: https://github.com/ln-markets/api-python
 Author: Romain ROUPHAEL
 License: MIT
 Keywords: lnmarkets trading rest api bitcoin lightning network futures options
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -24,24 +24,26 @@
 A simple way to connect your Python application to [LN Markets](https://lnmarkets.com/)!
 
 ## Install
 
 You can install this package with pip:
 ```shell
 pip3 install ln-markets
+```
 
-## Usage
+## Use
 
-You can import rest class from ln_markets
+You can import the rest class from lnmarkets
 ```python
 from lnmarkets import rest
 ```
-And the websocket one as well!
+And the websocket class as well
 ```python
 from lnmarkets import websockets
+```
 
 ## Authentication
 
 > For authentication you need your api **key** **secret** and **passphrase**
 
 Without you will not bet able to authenticate
 
@@ -63,15 +65,15 @@
 lnm.connect()
 ```
 
 > Check [examples](examples/websocket/README.md) for more details as you'll need to extend this class most of the time.
 
 ### Subscription
 
-You can subscribe to LNM Markets public event such as futures bid offer, index and options data.
+You can subscribe to LNM Markets public event such as futures last price ('futures:btc_usd:last-price') and index ('futures:btc_usd:index').
 
 ## REST API
 
 ### Configuration
 
 Use the LNMarketsRest and your key / passphrase to instanciate a new api connector:
```

### Comparing `ln-markets-2.0.1/lnmarkets/rest.py` & `ln-markets-2.0.2/lnmarkets/rest.py`

 * *Files identical despite different names*

### Comparing `ln-markets-2.0.1/lnmarkets/websockets.py` & `ln-markets-2.0.2/lnmarkets/websockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             on_error = self.on_error,
         )
         self.ws.run_forever()
     
     def subscribe(self, params):
         payload = {
             "jsonrpc": "2.0",
-            "method": "subscribe",
+            "method": "v1/public/subscribe",
             "id": secrets.token_bytes(4).hex(),
             "params": params
         }
 
         self.ws.send(json.dumps(payload))
 
     def unsubscribe(self, params):
```

### Comparing `ln-markets-2.0.1/setup.py` & `ln-markets-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ln-markets',
-    version='2.0.1',
+    version='2.0.2',
     packages=['lnmarkets'],
     description='LN Markets API python implementation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ln-markets/api-python',
     author='Romain ROUPHAEL',
     license='MIT',
```

