# Comparing `tmp/streamz_pulsar-0.1.0.post1.tar.gz` & `tmp/streamz_pulsar-0.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamz_pulsar-0.1.0.post1.tar", max compression
+gzip compressed data, was "streamz_pulsar-0.1.0.post2.tar", max compression
```

## Comparing `streamz_pulsar-0.1.0.post1.tar` & `streamz_pulsar-0.1.0.post2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1827 2023-06-24 06:29:14.047593 streamz_pulsar-0.1.0.post1/README.md
--rw-r--r--   0        0        0     1041 2023-06-24 06:43:21.676834 streamz_pulsar-0.1.0.post1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-23 14:49:28.393705 streamz_pulsar-0.1.0.post1/streamz_pulsar/__init__.py
--rw-r--r--   0        0        0      393 2023-06-23 14:28:24.077213 streamz_pulsar-0.1.0.post1/streamz_pulsar/base.py
--rw-r--r--   0        0        0     1611 2023-06-24 06:24:04.917299 streamz_pulsar-0.1.0.post1/streamz_pulsar/sinks.py
--rw-r--r--   0        0        0       51 2023-06-24 05:25:46.624145 streamz_pulsar-0.1.0.post1/streamz_pulsar/sources/__init__.py
--rw-r--r--   0        0        0     3149 2023-06-24 06:29:29.518373 streamz_pulsar-0.1.0.post1/streamz_pulsar/sources/from_pulsar.py
--rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 streamz_pulsar-0.1.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1827 2023-07-12 14:06:16.274117 streamz_pulsar-0.1.0.post2/README.md
+-rw-r--r--   0        0        0     1040 2023-07-12 14:16:35.791410 streamz_pulsar-0.1.0.post2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-12 14:06:16.274510 streamz_pulsar-0.1.0.post2/streamz_pulsar/__init__.py
+-rw-r--r--   0        0        0      393 2023-07-12 14:06:16.274565 streamz_pulsar-0.1.0.post2/streamz_pulsar/base.py
+-rw-r--r--   0        0        0     1619 2023-07-12 14:11:53.260772 streamz_pulsar-0.1.0.post2/streamz_pulsar/sinks.py
+-rw-r--r--   0        0        0       51 2023-07-12 14:06:16.274706 streamz_pulsar-0.1.0.post2/streamz_pulsar/sources/__init__.py
+-rw-r--r--   0        0        0     3152 2023-07-12 14:12:39.700559 streamz_pulsar-0.1.0.post2/streamz_pulsar/sources/from_pulsar.py
+-rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 streamz_pulsar-0.1.0.post2/PKG-INFO
```

### Comparing `streamz_pulsar-0.1.0.post1/README.md` & `streamz_pulsar-0.1.0.post2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Pulsar plugin for Streamz
 
 This a plugin for [Streamz](https://github.com/python-streamz/streamz) that adds stream
-nodes for writing and reading data from/to Poetry.
+nodes for writing and reading data from/to Pulsar.
 
 ## 🛠 Installation
 
 Latest stable version is available on PyPI
 
 ```sh
 pip install streamz_pulsar
```

### Comparing `streamz_pulsar-0.1.0.post1/pyproject.toml` & `streamz_pulsar-0.1.0.post2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "streamz_pulsar"
-version = "0.1.0.post1"
+version = "0.1.0.post2"
 description = ""
 authors = [
     "Marek Wadinger <marekwadinger@icloud.com>",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -31,15 +31,14 @@
 
 [tool.poetry.plugins."streamz.sources"]
 from_pulsar = "streamz_pulsar.sources:from_pulsar"
 
 [tool.poetry.plugins."streamz.sinks"]
 to_pulsar = "streamz_pulsar.sinks:to_pulsar"
 
-
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report html --cov-report term-missing --cov-fail-under 0"
 
 [tool.pylint]
 max-line-length = 79
 disable = [
     "W"
```

### Comparing `streamz_pulsar-0.1.0.post1/streamz_pulsar/sinks.py` & `streamz_pulsar-0.1.0.post2/streamz_pulsar/sinks.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,32 +25,31 @@
         Settings to set up the stream, see
         https://pulsar.apache.org/api/python/3.2.x/pulsar.Client.html
         Examples:
         service_url: The Pulsar service url eg: pulsar://my-broker.com:6650/
 
     Examples
     --------
-    >>> import pulsar
     >>> from streamz import Stream
-    >>> s = Stream.from_pulsar(
-    ...     ['my-topic'],
-    ...     subscription_name='my-sub',
-    ...     consumer_params={'service_url': 'pulsar://localhost:6650'}
-    ...     )
-    >>> s.map(lambda x: x.decode())
-    >>> L = s.sink_to_list()
+    >>> source = Stream()
+    >>> producer_ = source.to_pulsar(
+    ...     'my-topic',
+    ...     producer_config={'service_url': 'pulsar://localhost:6650'}
+    ...     )  # doctest: +SKIP
+    >>> for i in range(3):
+    ...     source.emit(('hello-pulsar-%d' % i).encode('utf-8'))
     """
     def __init__(self, upstream, topic, producer_config, **kwargs):
 
         self.topic = topic
         self.client = pulsar.Client(**producer_config)
         self.producer = self.client.create_producer(self.topic)
 
         kwargs["ensure_io_loop"] = True
-        Stream.__init__(self, upstream, **kwargs)
+        super().__init__(upstream, **kwargs)
         self.stopped = False
         self.polltime = 0.2
         self.futures = []
 
     def update(self, x, who=None, metadata=None):
         self.producer.send(x)
```

### Comparing `streamz_pulsar-0.1.0.post1/streamz_pulsar/sources/from_pulsar.py` & `streamz_pulsar-0.1.0.post2/streamz_pulsar/sources/from_pulsar.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,22 +34,23 @@
         group.id, Identity of the consumer. If multiple sources share the same
         group, each message will be passed to only one of them.
     poll_interval: number
         Seconds that elapse between polling Pulsar for new messages
 
     Examples
     --------
+    >>> import pulsar
     >>> from streamz import Stream
-    >>> source = Stream()
-    >>> producer_ = source.to_pulsar(
-    ...     'my-topic',
-    ...     producer_config={'service_url': 'pulsar://localhost:6650'}
-    ...     )  # doctest: +SKIP
-    >>> for i in range(3):
-    ...     source.emit(('hello-pulsar-%d' % i).encode('utf-8'))
+    >>> s = Stream.from_pulsar(
+    ...     ['my-topic'],
+    ...     subscription_name='my-sub',
+    ...     consumer_params={'service_url': 'pulsar://localhost:6650'}
+    ...     )
+    >>> decoder = s.map(lambda x: x.decode())
+    >>> L = decoder.sink_to_list()
     """
     def __init__(
             self,
             topics,
             subscription_name,
             consumer_params,
             poll_interval=0.1,
```

### Comparing `streamz_pulsar-0.1.0.post1/PKG-INFO` & `streamz_pulsar-0.1.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamz-pulsar
-Version: 0.1.0.post1
+Version: 0.1.0.post2
 Summary: 
 Home-page: https://github.com/MarekWadinger/streamz_pulsar
 Keywords: streamz,pulsar
 Author: Marek Wadinger
 Author-email: marekwadinger@icloud.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 Requires-Dist: streamz (>=0.6.4,<0.7.0)
 Project-URL: Repository, https://github.com/MarekWadinger/streamz_pulsar
 Description-Content-Type: text/markdown
 
 # Pulsar plugin for Streamz
 
 This a plugin for [Streamz](https://github.com/python-streamz/streamz) that adds stream
-nodes for writing and reading data from/to Poetry.
+nodes for writing and reading data from/to Pulsar.
 
 ## 🛠 Installation
 
 Latest stable version is available on PyPI
 
 ```sh
 pip install streamz_pulsar
```

