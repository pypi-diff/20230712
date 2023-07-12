# Comparing `tmp/zimran-events-0.2.6.tar.gz` & `tmp/zimran-events-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.2.6.tar", last modified: Tue May 30 05:02:41 2023, max compression
+gzip compressed data, was "zimran-events-0.3.0.tar", last modified: Wed Jul 12 12:39:04 2023, max compression
```

## Comparing `zimran-events-0.2.6.tar` & `zimran-events-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.695969 zimran-events-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.687969 zimran-events-0.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.691969 zimran-events-0.2.6/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.691969 zimran-events-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 05:02:32.000000 zimran-events-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-30 05:02:41.695969 zimran-events-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-30 05:02:32.000000 zimran-events-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-30 05:02:32.000000 zimran-events-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-30 05:02:32.000000 zimran-events-0.2.6/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 05:02:41.695969 zimran-events-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.691969 zimran-events-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-30 05:02:32.000000 zimran-events-0.2.6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.687969 zimran-events-0.2.6/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.691969 zimran-events-0.2.6/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.695969 zimran-events-0.2.6/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-30 05:02:41.000000 zimran-events-0.2.6/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-30 05:02:41.000000 zimran-events-0.2.6/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:02:41.000000 zimran-events-0.2.6/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-30 05:02:41.000000 zimran-events-0.2.6/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 05:02:41.000000 zimran-events-0.2.6/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-12 12:38:56.000000 zimran-events-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-12 12:38:56.000000 zimran-events-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-12 12:39:04.041852 zimran-events-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-12 12:38:56.000000 zimran-events-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-12 12:38:56.000000 zimran-events-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-12 12:38:56.000000 zimran-events-0.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:39:04.041852 zimran-events-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-12 12:38:56.000000 zimran-events-0.3.0/tests/test_legacy_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-12 12:38:56.000000 zimran-events-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-12 12:38:56.000000 zimran-events-0.3.0/zimran/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:39:04.041852 zimran-events-0.3.0/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-12 12:39:04.000000 zimran-events-0.3.0/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-12 12:39:04.000000 zimran-events-0.3.0/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:39:04.000000 zimran-events-0.3.0/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-12 12:39:04.000000 zimran-events-0.3.0/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-12 12:39:04.000000 zimran-events-0.3.0/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.2.6/.github/scripts/release.py` & `zimran-events-0.3.0/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.6/.gitignore` & `zimran-events-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.6/.pre-commit-config.yaml` & `zimran-events-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.6/LICENSE` & `zimran-events-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.6/PKG-INFO` & `zimran-events-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.6
+Version: 0.3.0
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,15 +36,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-## zimran-contrib
+## zimran-events
 
 The `zimran-py-events` module provides AMQP interface
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?color=green&style=plastic)](https://opensource.org/licenses/MIT)
 ![code size](<https://img.shields.io/github/languages/code-size/zimran-tech/zimran-py-events?style=plastic>)
 
 ## Installation
@@ -69,21 +69,21 @@
 ```
 
 **Consumer**
 
 ```python
 
 from zimran.events import Consumer
-from zimran.events.schemas import ExchangeScheme
+from zimran.events.dto import Exchange
 
 consumer = Consumer(service_name='my-service', broker_url='')
 consumer.add_event_handler(
             name='routing-key',
             handler=handler_func,
-            exchange=ExchangeScheme(
+            exchange=Exchange(
                 name='exchange-name',
                 type='exchange-type',
                 durable=True,
             )
            )
 
 # or
```

### Comparing `zimran-events-0.2.6/README.md` & `zimran-events-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## zimran-contrib
+## zimran-events
 
 The `zimran-py-events` module provides AMQP interface
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?color=green&style=plastic)](https://opensource.org/licenses/MIT)
 ![code size](<https://img.shields.io/github/languages/code-size/zimran-tech/zimran-py-events?style=plastic>)
 
 ## Installation
@@ -27,21 +27,21 @@
 ```
 
 **Consumer**
 
 ```python
 
 from zimran.events import Consumer
-from zimran.events.schemas import ExchangeScheme
+from zimran.events.dto import Exchange
 
 consumer = Consumer(service_name='my-service', broker_url='')
 consumer.add_event_handler(
             name='routing-key',
             handler=handler_func,
-            exchange=ExchangeScheme(
+            exchange=Exchange(
                 name='exchange-name',
                 type='exchange-type',
                 durable=True,
             )
            )
 
 # or
```

### Comparing `zimran-events-0.2.6/pyproject.toml` & `zimran-events-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.2.6"
+version = "0.3.0"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 
-dependencies = ["pika>=1.3.1", "aio-pika>=9.0.5", "aioretry>=5.0.2"]
+dependencies = ["pika==1.3.2", "aio-pika==9.1.4", "aioretry==5.0.2"]
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `zimran-events-0.2.6/tests/test_utils.py` & `zimran-events-0.3.0/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 
 from aiormq.exceptions import AMQPConnectionError
 
 from zimran.events import utils
+from zimran.events.dto import ChannelProperties, Exchange
 from zimran.events.exceptions import ChannelPropertiesTypeError, ExchangeTypeError
-from zimran.events.schemas import ChannelPropertiesScheme, ExchangeScheme
 
 
 @pytest.mark.parametrize(
     'case, expected',
     [
         ['payments.orders.oneclick.*.created', 'payments.orders.oneclick.created_q'],
         ['payments.orders.oneclick.#.', 'payments.orders.oneclick_q'],
@@ -17,22 +17,22 @@
 def test_queue_name_cleaner(case, expected):
     got = utils.cleanup_and_normalize_queue_name(case)
 
     assert expected == got
 
 
 def test_validate_exchange():
-    utils.validate_exchange(ExchangeScheme(name='exchange'))
+    utils.validate_exchange(Exchange(name='exchange'))
 
     with pytest.raises(ExchangeTypeError):
         utils.validate_exchange({'name': 'exchange'})
 
 
 def test_validate_channel_props():
-    utils.validate_channel_properties(ChannelPropertiesScheme())
+    utils.validate_channel_properties(ChannelProperties())
 
     with pytest.raises(ChannelPropertiesTypeError):
         utils.validate_channel_properties({})
 
 
 def test_retry_policy():
     class Info:
```

### Comparing `zimran-events-0.2.6/zimran/events/consumer.py` & `zimran-events-0.3.0/zimran/events/consumer.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 except ImportError:
     import logging
 
     logger = logging.getLogger(__name__)
 
 
 from zimran.events.connection import AsyncConnection, Connection
-from zimran.events.constants import DEAD_LETTER_EXCHANGE_NAME
+from zimran.events.constants import DEFAULT_DEAD_LETTER_EXCHANGE_NAME
 from zimran.events.schemas import ExchangeScheme
 from zimran.events.utils import cleanup_and_normalize_queue_name, retry_policy, validate_exchange
 
 
 class ConsumerMixin:
     def handle_event(self, name: str, *, exchange: ExchangeScheme | None = None):
         if exchange is not None:
@@ -56,22 +56,25 @@
         self._event_handlers = {}
 
     def run(self):
         try:
             channel = self.channel
             channel.basic_qos(prefetch_count=self._prefetch_count)
 
+            self._declare_unroutable_queue(channel)
+            self._declare_default_dead_letter_exchange(channel)
+
             consumer_amount = 0
             for event_name, data in self._event_handlers.items():
                 queue_name = cleanup_and_normalize_queue_name(f'{self._service_name}.{event_name}')
                 channel.queue_declare(
                     queue_name,
                     durable=True,
                     arguments={
-                        'x-dead-letter-exchange': DEAD_LETTER_EXCHANGE_NAME,
+                        'x-dead-letter-exchange': DEFAULT_DEAD_LETTER_EXCHANGE_NAME,
                     },
                 )
 
                 if exchange := data['exchange']:
                     channel.exchange_declare(
                         exchange=exchange.name,
                         exchange_type=exchange.type,
@@ -108,23 +111,30 @@
         self._event_handlers = {}
 
     @retry(retry_policy)
     async def run(self):
         try:
             channel = await self.channel
             await channel.set_qos(prefetch_count=self._prefetch_count)
+            await self._declare_unroutable_queue(channel)
+
+            await asyncio.gather(
+                self._declare_unroutable_queue(channel),
+                self._declare_default_dead_letter_exchange(channel),
+                return_exceptions=True,
+            )
 
             consumer_amount = 0
             for event_name, data in self._event_handlers.items():
                 queue_name = cleanup_and_normalize_queue_name(f'{self._service_name}.{event_name}')
                 queue = await channel.declare_queue(
                     queue_name,
                     durable=True,
                     arguments={
-                        'x-dead-letter-exchange': DEAD_LETTER_EXCHANGE_NAME,
+                        'x-dead-letter-exchange': DEFAULT_DEAD_LETTER_EXCHANGE_NAME,
                     },
                 )
                 if _exchange := data['exchange']:
                     exchange = await channel.declare_exchange(**_exchange.as_dict(exclude_none=True))
                     await queue.bind(exchange=exchange, routing_key=event_name)
 
                 await queue.consume(data['handler'])
```

### Comparing `zimran-events-0.2.6/zimran/events/producer.py` & `zimran-events-0.3.0/zimran/events/producer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import json
 
 import aio_pika
 import pika
 from aioretry import retry
 
 
@@ -39,14 +40,16 @@
         body = json.dumps(payload, default=str)
         if exchange is None:
             self.channel.basic_publish(exchange='', routing_key=routing_key, body=body, properties=basic_properties)
             logger.info(f'Message published to basic exchange | routing_key: {routing_key}')
             return
 
         validate_exchange(exchange)
+        self._declare_unroutable_queue(channel=self.channel)
+        self._declare_default_dead_letter_exchange(channel=self.channel)
 
         self.channel.exchange_declare(
             exchange=exchange.name,
             exchange_type=exchange.type,
             **exchange.as_dict(exclude=['name', 'type', 'timeout'], exclude_none=True),
         )
 
@@ -82,15 +85,20 @@
         channel = await self.channel
         if exchange is None:
             await channel.default_exchange.publish(message=message, routing_key=routing_key)
             logger.info(f'Message published to basic exchange | routing_key: {routing_key}')
             return
 
         validate_exchange(exchange)
+        declared_exchange, *_ = await asyncio.gather(
+            channel.declare_exchange(**exchange.as_dict(exclude_none=True)),
+            self._declare_unroutable_queue(channel=channel),
+            self._declare_default_dead_letter_exchange(channel=channel),
+            return_exceptions=True,
+        )
 
-        declared_exchange = await channel.declare_exchange(**exchange.as_dict(exclude_none=True))
         await declared_exchange.publish(message=message, routing_key=routing_key)
         logger.info(f'Message published to {exchange.name} exchange | routing_key: {routing_key}')
 
     @staticmethod
     def _get_message(properties: ChannelPropertiesScheme, payload: dict):
         return aio_pika.Message(body=json.dumps(payload, default=str).encode(), **properties.as_dict(exclude_none=True))
```

### Comparing `zimran-events-0.2.6/zimran/events/schemas.py` & `zimran-events-0.3.0/zimran/events/dto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 import datetime
 import uuid
 from dataclasses import asdict, dataclass
 
 
-class SchemeBase:
+class Base:
     def as_dict(self, exclude: list | None = None, exclude_none: bool = False) -> dict:
         excluded_keys = exclude if isinstance(exclude, (list, tuple)) else []
         data = {key: val for key, val in asdict(self).items() if key not in excluded_keys}
 
         if exclude_none:
             data = {key: val for key, val in data.items() if val is not None}
 
         return data
 
 
 @dataclass(kw_only=True)
-class ExchangeScheme(SchemeBase):
+class Exchange(Base):
     name: str
     durable: bool = True
     type: str = 'direct'  # noqa: A003
     internal: bool = False
-    durable: bool = True
     passive: bool = False
     auto_delete: bool = False
     arguments: dict | None = None
     timeout: float | int | None = None
 
     def __post_init__(self):
         if self.arguments is None:
             self.arguments = {}
 
 
 @dataclass(kw_only=True)
-class ChannelPropertiesScheme(SchemeBase):
+class ChannelProperties(Base):
     correlation_id: str | None = None
     content_type: str = 'application/json'
     delivery_mode: int = 2  # Persistent
     headers: dict | None = None
     priority: int | None = None
     reply_to: str | None = None
     expiration: datetime.datetime | None = None
```

### Comparing `zimran-events-0.2.6/zimran/events/utils.py` & `zimran-events-0.3.0/zimran/events/utils.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.6/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.3.0/zimran_events.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.6
+Version: 0.3.0
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,15 +36,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-## zimran-contrib
+## zimran-events
 
 The `zimran-py-events` module provides AMQP interface
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?color=green&style=plastic)](https://opensource.org/licenses/MIT)
 ![code size](<https://img.shields.io/github/languages/code-size/zimran-tech/zimran-py-events?style=plastic>)
 
 ## Installation
@@ -69,21 +69,21 @@
 ```
 
 **Consumer**
 
 ```python
 
 from zimran.events import Consumer
-from zimran.events.schemas import ExchangeScheme
+from zimran.events.dto import Exchange
 
 consumer = Consumer(service_name='my-service', broker_url='')
 consumer.add_event_handler(
             name='routing-key',
             handler=handler_func,
-            exchange=ExchangeScheme(
+            exchange=Exchange(
                 name='exchange-name',
                 type='exchange-type',
                 durable=True,
             )
            )
 
 # or
```

### Comparing `zimran-events-0.2.6/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.3.0/zimran_events.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 LICENSE
 README.md
 pyproject.toml
 pytest.ini
 .github/scripts/release.py
 .github/workflows/publish.yml
 .github/workflows/release.yml
+tests/test_legacy_scheme.py
 tests/test_utils.py
 zimran/events/__init__.py
 zimran/events/connection.py
 zimran/events/constants.py
 zimran/events/consumer.py
+zimran/events/dto.py
 zimran/events/exceptions.py
 zimran/events/producer.py
 zimran/events/schemas.py
 zimran/events/utils.py
 zimran_events.egg-info/PKG-INFO
 zimran_events.egg-info/SOURCES.txt
 zimran_events.egg-info/dependency_links.txt
```

