# Comparing `tmp/w3bstream_client_python-0.4.5.tar.gz` & `tmp/w3bstream_client_python-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3bstream_client_python-0.4.5.tar", last modified: Fri Jul  7 19:37:00 2023, max compression
+gzip compressed data, was "w3bstream_client_python-0.4.6.tar", last modified: Wed Jul 12 19:38:36 2023, max compression
```

## Comparing `w3bstream_client_python-0.4.5.tar` & `w3bstream_client_python-0.4.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3078 2023-06-24 01:07:19.000000 w3bstream_client_python-0.4.5/.gitignore
--rw-r--r--   0 haaai     (1000) haaai     (1000)    11357 2023-06-24 01:07:19.000000 w3bstream_client_python-0.4.5/LICENSE
--rw-r--r--   0 haaai     (1000) haaai     (1000)      799 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      623 2023-07-07 19:34:25.000000 w3bstream_client_python-0.4.5/README.md
--rw-r--r--   0 haaai     (1000) haaai     (1000)      391 2023-07-07 19:33:48.000000 w3bstream_client_python-0.4.5/pyproject.toml
--rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/setup.cfg
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/src/
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/src/w3bstream_client_python/
--rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-07-07 17:50:45.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python/__init__.py
--rw-r--r--   0 haaai     (1000) haaai     (1000)     3840 2023-07-07 19:34:41.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python/client.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-07 19:37:00.892611 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      799 2023-07-07 19:37:00.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      375 2023-07-07 19:37:00.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-07-07 19:37:00.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       19 2023-07-07 19:37:00.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/requires.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-07-07 19:37:00.000000 w3bstream_client_python-0.4.5/src/w3bstream_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3078 2023-06-30 05:29:14.000000 w3bstream_client_python-0.4.6/.gitignore
+-rw-r--r--   0 haaai     (1000) haaai     (1000)    11357 2023-06-30 05:29:14.000000 w3bstream_client_python-0.4.6/LICENSE
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      886 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      709 2023-07-11 18:41:55.000000 w3bstream_client_python-0.4.6/README.md
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      391 2023-07-11 18:41:55.000000 w3bstream_client_python-0.4.6/pyproject.toml
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/setup.cfg
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/src/
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/src/w3bstream_client_python/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       67 2023-07-10 18:18:02.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python/__init__.py
+-rw-r--r--   0 haaai     (1000) haaai     (1000)     3833 2023-07-12 03:25:37.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python/client.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-07-12 19:38:35.994138 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      886 2023-07-12 19:38:35.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      375 2023-07-12 19:38:35.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-07-12 19:38:35.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       19 2023-07-12 19:38:35.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/requires.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-07-12 19:38:35.000000 w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/top_level.txt
```

### Comparing `w3bstream_client_python-0.4.5/.gitignore` & `w3bstream_client_python-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-0.4.5/LICENSE` & `w3bstream_client_python-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `w3bstream_client_python-0.4.5/PKG-INFO` & `w3bstream_client_python-0.4.6/src/w3bstream_client_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: w3bstream_client_python
-Version: 0.4.5
+Name: w3bstream-client-python
+Version: 0.4.6
 Summary: Official W3bstream Client for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # w3bstream-client-python
 
 The Python Client for W3bstream integration on server
@@ -28,7 +28,13 @@
 client = Client("http_route", "api_key")
 # device_id is the identity for the device
 # payload can be an empty string if served as a heartbeat
 header = Header('device_id')
 rsp = client.publish_event_sync(header, b'payload')
 print(rsp.text)
 ```
+
+### Publish Event Asynchronously
+
+``` py
+client.publish_event(header, b'payload')
+```
```

### Comparing `w3bstream_client_python-0.4.5/README.md` & `w3bstream_client_python-0.4.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -21,7 +21,13 @@
 client = Client("http_route", "api_key")
 # device_id is the identity for the device
 # payload can be an empty string if served as a heartbeat
 header = Header('device_id')
 rsp = client.publish_event_sync(header, b'payload')
 print(rsp.text)
 ```
+
+### Publish Event Asynchronously
+
+``` py
+client.publish_event(header, b'payload')
+```
```

### Comparing `w3bstream_client_python-0.4.5/src/w3bstream_client_python/client.py` & `w3bstream_client_python-0.4.6/src/w3bstream_client_python/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,93 +13,93 @@
     def __init__(self, device_id: str, event_type: str = 'DEFAULT', timestamp: datetime.datetime = datetime.datetime.utcnow()):
         self.event_type = event_type
         self.device_id = device_id
         self.timestamp = timestamp
 
 
 PUBLISH_INTERVAL = 5
-PUBLISH_BATCH_SIZE = 10
+_PUBLISH_BATCH_SIZE = 1
 
 
 @typechecked
 class Client:
     def __init__(self, url: str, api_key: str, queue_size: int = 0):
         self.url = url
-        # self.project = project
         self.api_key = api_key
         self.queue = queue.Queue(queue_size)
-        # self.thread = threading.Thread(target=self._worker)
-        # self.thread.start()
+        self.thread = threading.Thread(target=self._worker, daemon=True)
+        self.thread.start()
 
     def publish_event_sync(self, header: Header, payload: bytes) -> requests.Response:
         """
         Publishes an event synchronously.
         """
         body = [{
             'device_id': header.device_id,
             'event_type': header.event_type,
             'payload': payload.decode('utf-8'),
             'timestamp':  int(round(header.timestamp.timestamp())),
         }]
         return self._publish_event(body)
 
-    # def publish_event(self, header: Header, payload: bytes) -> bool:
-    #     """
-    #     Publishes an event asynchronously.
-
-    #     No callback is provided because the event is added to a queue and published in batches.
-    #     If encountering errors when publishing, response body will be printed to stderr.
-
-    #     Returns:
-    #         True if the event was successfully added to the queue, False otherwise.
-    #     """
-    #     try:
-    #         self.queue.put_nowait((header, payload))
-    #         return True
-    #     except queue.Full:
-    #         sys.stderr.write(
-    #             "The queue is full when publishing the data to W3bstream")
-    #         return False
-
-    # def _worker(self):
-    #     while True:
-    #         # fetch events
-    #         events = []
-    #         for header, payload in self._fetch_event_batch():
-    #             events.append({
-    #                 'device_id': header.device_id,
-    #                 'event_type': header.event_type,
-    #                 'payload': payload.decode('utf-8'),
-    #                 'timestamp':  int(round(header.timestamp.timestamp())),
-    #             })
-    #         # publish events
-    #         resp = self._publish_event(events)
-    #         if resp.status_code != 200:
-    #             sys.stderr.write(
-    #                 "An error occurred when publishing the data to W3bstream: %s" % resp.text)
-    #         # sleep interval
-    #         time.sleep(PUBLISH_INTERVAL)
-
-    # def _fetch_event_batch(self):
-    #     """
-    #     Fetches a batch of events from the queue.
-
-    #     Fetches up to PUBLISH_BATCH_SIZE events from the queue.
-    #     It will block until at least one event is available.
-    #     """
-    #     count = 0
-    #     while count < PUBLISH_BATCH_SIZE:
-    #         try:
-    #             if count == 0:
-    #                 yield self.queue.get()
-    #             else:
-    #                 yield self.queue.get_nowait()
-    #             count += 1
-    #         except queue.Empty:
-    #             break
+    def publish_event(self, header: Header, payload: bytes) -> bool:
+        """
+        Publishes an event asynchronously.
+
+        No callback is provided because the event is added to a queue and published in batches.
+        If encountering errors when publishing, response body will be printed to stderr.
+
+        Returns:
+            True if the event was successfully added to the queue, False otherwise.
+        """
+        try:
+            self.queue.put_nowait((header, payload))
+            return True
+        except queue.Full:
+            sys.stderr.write(
+                "The queue is full when publishing the data to W3bstream")
+            return False
+
+    def _worker(self):
+        while True:
+            # fetch events
+            events = []
+            for header, payload in self._fetch_event_batch():
+                events.append({
+                    'device_id': header.device_id,
+                    'event_type': header.event_type,
+                    'payload': payload.decode('utf-8'),
+                    'timestamp':  int(round(header.timestamp.timestamp())),
+                })
+            # publish events
+            resp = self._publish_event(events)
+            if resp.status_code >= 400:
+                # TODO: Support retry mechanism when failed to publish
+                sys.stderr.write(
+                    "An error occurred when publishing the data to W3bstream: status_code %d, body: %s" % (resp.status_code, resp.text))
+            # sleep interval
+            time.sleep(PUBLISH_INTERVAL)
+
+    def _fetch_event_batch(self):
+        """
+        Fetches a batch of events from the queue.
+
+        Fetches up to _PUBLISH_BATCH_SIZE events from the queue.
+        It will block until at least one event is available.
+        """
+        count = 0
+        while count < _PUBLISH_BATCH_SIZE:
+            try:
+                if count == 0:
+                    yield self.queue.get()
+                else:
+                    yield self.queue.get_nowait()
+                count += 1
+            except queue.Empty:
+                break
 
     def _publish_event(self, events: list) -> requests.Response:
         meta_data = events[0]
         headers = {
             'Authorization': 'Bearer ' + self.api_key,
             'Content-Type': 'application/octet-stream',
         }
```

