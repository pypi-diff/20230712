# Comparing `tmp/talkytrend-1.7.2.tar.gz` & `tmp/talkytrend-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.7.2.tar", max compression
+gzip compressed data, was "talkytrend-1.7.3.tar", max compression
```

## Comparing `talkytrend-1.7.2.tar` & `talkytrend-1.7.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-11 18:01:43.390880 talkytrend-1.7.2/LICENSE
--rw-r--r--   0        0        0     3446 2023-07-11 18:01:43.390880 talkytrend-1.7.2/README.md
--rw-r--r--   0        0        0     2476 2023-07-11 18:01:44.338887 talkytrend-1.7.2/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-11 18:01:44.338887 talkytrend-1.7.2/talkytrend/__init__.py
--rw-r--r--   0        0        0      706 2023-07-11 18:01:43.390880 talkytrend-1.7.2/talkytrend/config.py
--rw-r--r--   0        0        0     2232 2023-07-11 18:01:43.390880 talkytrend-1.7.2/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     7807 2023-07-11 18:01:43.390880 talkytrend-1.7.2/talkytrend/main.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-12 13:59:39.697182 talkytrend-1.7.3/LICENSE
+-rw-r--r--   0        0        0     3446 2023-07-12 13:59:39.697182 talkytrend-1.7.3/README.md
+-rw-r--r--   0        0        0     2476 2023-07-12 13:59:40.517257 talkytrend-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-12 13:59:40.517257 talkytrend-1.7.3/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-12 13:59:39.697182 talkytrend-1.7.3/talkytrend/config.py
+-rw-r--r--   0        0        0     2232 2023-07-12 13:59:39.697182 talkytrend-1.7.3/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     7304 2023-07-12 13:59:39.697182 talkytrend-1.7.3/talkytrend/main.py
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.7.3/PKG-INFO
```

### Comparing `talkytrend-1.7.2/LICENSE` & `talkytrend-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.2/README.md` & `talkytrend-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.2/pyproject.toml` & `talkytrend-1.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "talkytrend"
-version = "1.7.2"
+version = "1.7.3"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.7.2/talkytrend/config.py` & `talkytrend-1.7.3/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.2/talkytrend/default_settings.toml` & `talkytrend-1.7.3/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.2/talkytrend/main.py` & `talkytrend-1.7.3/talkytrend/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,32 +11,29 @@
 from tradingview_ta import TA_Handler
 from talkytrend import __version__
 from talkytrend.config import settings
 
 
 class TalkyTrend:
     def __init__(self):
-        try:
-            self.logger = logging.getLogger("TalkyTrend")
-            self.enabled = settings.talkytrend_enabled
-            if not self.enabled:
-                return
-            self.mode = settings.talkytrend_mode
-            self.assets = settings.assets
-            self.asset_signals = {}
-            self.economic_calendar = settings.economic_calendar
-            self.news_url = (
-                f"{settings.news_url}{settings.news_api_key}"
-                if settings.news_api_key
-                else settings.news_url
-            )
-            self.live_tv = settings.live_tv_url
-            print(self.news_url)
-        except Exception as error:
-            self.logger.error("TalkyTrend init error %s", error)
+        self.logger = logging.getLogger("TalkyTrend")
+        self.enabled = settings.talkytrend_enabled
+        if not self.enabled:
+            return
+        self.mode = settings.talkytrend_mode
+        self.assets = settings.assets
+        self.asset_signals = {}
+        self.economic_calendar = settings.economic_calendar
+        self.news_url = (
+            f"{settings.news_url}{settings.news_api_key}"
+            if settings.news_api_key
+            else settings.news_url
+        )
+        self.live_tv = settings.live_tv_url
+
 
     async def fetch_analysis(
         self,
         asset_id,
         exchange,
         screener,
         interval):
@@ -59,54 +56,49 @@
                 return "⏬"
             else:
                 return "▶️"
         except Exception as error:
             self.logger.error("event %s", error)
 
     async def check_signal(self):
-        try:
-            signals = []
-            table = PrettyTable()
-            table.field_names = ["Asset","4h"]
-            for asset in self.assets:
-                current_signal = await self.fetch_analysis(
-                    asset_id=asset["id"],
-                    exchange=asset["exchange"],
-                    screener=asset["screener"],
-                    interval=asset["interval"]
-                )
-                if self.is_new_signal(asset["id"], asset["interval"], current_signal):
-                    signal_item = {
-                        "symbol": asset["id"],
-                        "interval": asset["interval"],
-                        "signal": current_signal
-                    }
-                    self.update_signal(asset["id"], asset["interval"], current_signal)
-                    table.add_row([asset["id"], current_signal])
-                    signals.append(signal_item)
-            return table.get_string()
-            # return table.get_html_string()
-        except Exception as error:
-            self.logger.error("check_signal %s", error)
-            return []
+        signals = []
+        table = PrettyTable()
+        table.field_names = ["Asset","4h"]
+        for asset in self.assets:
+            current_signal = await self.fetch_analysis(
+                asset_id=asset["id"],
+                exchange=asset["exchange"],
+                screener=asset["screener"],
+                interval=asset["interval"]
+            )
+            if self.is_new_signal(asset["id"], asset["interval"], current_signal):
+                signal_item = {
+                    "symbol": asset["id"],
+                    "interval": asset["interval"],
+                    "signal": current_signal
+                }
+                self.update_signal(asset["id"], asset["interval"], current_signal)
+                table.add_row([asset["id"], current_signal])
+                signals.append(signal_item)
+                return table.get_string()
 
     def is_new_signal(self, asset_id, interval, current_signal):
-        if self.asset_signals.get(asset_id):
-            if (
-                self.asset_signals[asset_id].get(interval)
-                and current_signal != self.asset_signals[asset_id][interval]
-            ):
-                self.asset_signals[asset_id][interval] = current_signal
-                return True
-        else:
-            self.asset_signals[asset_id] = {interval: current_signal}
+        if asset_id not in self.asset_signals:
+            self.asset_signals[asset_id] = {}
+        if interval not in self.asset_signals[asset_id]:
+            self.asset_signals[asset_id][interval] = current_signal
+            return True
+        elif current_signal != self.asset_signals[asset_id][interval]:
+            self.asset_signals[asset_id][interval] = current_signal
             return True
         return False
 
     def update_signal(self, asset_id, interval, current_signal):
+        if asset_id not in self.asset_signals:
+            self.asset_signals[asset_id] = {}
         self.asset_signals[asset_id][interval] = current_signal
 
     def get_asset_signals(self):
         return self.asset_signals
 
     async def fetch_key_events(self):
         def filter_events(data, today):
@@ -166,42 +158,39 @@
                         .get('rss')
                         .get('channel')['item'][0]
                     )
                     title = data['title']
                     link = data['link']
                     return f"📰 <a href='{link}'>{title}</a>"
         except aiohttp.ClientError as error:
-            self.logger.error("news %s", error)
+            self.logger.error("feed %s", error)
             return None
 
 
     async def check_fomc(self):
         event_dates = settings.fomc_decision_date
         current_date = date.today().isoformat()
         return any(event.startswith(current_date) for event in event_dates)
      
     async def allow_scanning(self, enable=True):
         return bool(enable)
 
     async def scanner(self):
         while await self.allow_scanning():
-            try:
-                if settings.enable_events:
-                    if await self.fetch_key_events() is not None:
-                        yield await self.fetch_key_events()
-                if settings.enable_news:
-                    if await self.fetch_key_news() is not None:
-                        yield await self.fetch_key_news()
-                if settings.enable_feed:
-                    if await self.fetch_key_feed() is not None:
-                        yield await self.fetch_key_feed()
-                if settings.enable_signals:
-                    if await self.check_signal() is not None:
-                        yield await self.check_signal()
+            if settings.enable_events:
+                if await self.fetch_key_events() is not None:
+                    yield await self.fetch_key_events()
+            if settings.enable_news:
+                if await self.fetch_key_news() is not None:
+                    yield await self.fetch_key_news()
+            if settings.enable_feed:
+                if await self.fetch_key_feed() is not None:
+                    yield await self.fetch_key_feed()
+            if settings.enable_signals:
+                if await self.check_signal() is not None:
+                    yield await self.check_signal()
 
-                await asyncio.sleep(settings.scanner_frequency)
+            await asyncio.sleep(settings.scanner_frequency)
 
-            except Exception as error:
-                raise error
 
     async def get_info(self):
         return f"{__class__.__name__} {__version__}" + "\n" + f"📺: {__version__}"
```

### Comparing `talkytrend-1.7.2/PKG-INFO` & `talkytrend-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.7.2
+Version: 1.7.3
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 1.7.2 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.7.3 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
```

