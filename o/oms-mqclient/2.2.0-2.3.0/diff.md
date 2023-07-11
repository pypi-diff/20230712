# Comparing `tmp/oms-mqclient-2.2.0.tar.gz` & `tmp/oms-mqclient-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oms-mqclient-2.2.0.tar", last modified: Tue Jul 11 01:28:57 2023, max compression
+gzip compressed data, was "oms-mqclient-2.3.0.tar", last modified: Tue Jul 11 22:08:25 2023, max compression
```

## Comparing `oms-mqclient-2.2.0.tar` & `oms-mqclient-2.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.574231 oms-mqclient-2.2.0/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2674 2023-07-11 01:28:57.574231 oms-mqclient-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1354 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.566231 oms-mqclient-2.2.0/mqclient/
--rw-r--r--   0 root         (0) root         (0)      582 2023-07-11 01:28:55.000000 oms-mqclient-2.2.0/mqclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5972 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_client_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.566231 oms-mqclient-2.2.0/mqclient/broker_clients/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13328 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_clients/apachepulsar.py
--rw-r--r--   0 root         (0) root         (0)    13368 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_clients/nats.py
--rw-r--r--   0 root         (0) root         (0)    15335 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_clients/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1791 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/broker_clients/utils.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/config.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/log_msgs.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/py.typed
--rw-r--r--   0 root         (0) root         (0)    24593 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/queue.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/mqclient/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.566231 oms-mqclient-2.2.0/oms_mqclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2674 2023-07-11 01:28:57.000000 oms-mqclient-2.2.0/oms_mqclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1151 2023-07-11 01:28:57.000000 oms-mqclient-2.2.0/oms_mqclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:28:57.000000 oms-mqclient-2.2.0/oms_mqclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      298 2023-07-11 01:28:57.000000 oms-mqclient-2.2.0/oms_mqclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 01:28:57.000000 oms-mqclient-2.2.0/oms_mqclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2731 2023-07-11 01:28:57.574231 oms-mqclient-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.562231 oms-mqclient-2.2.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.570231 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9038 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
--rw-r--r--   0 root         (0) root         (0)    33482 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/integrate_queue.py
--rw-r--r--   0 root         (0) root         (0)    20234 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/unit_tests.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/abstract_broker_client_tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.570231 oms-mqclient-2.2.0/tests/integrate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/integrate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      962 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/integrate/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/integrate/test_nats.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/integrate/test_pulsar.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/integrate/test_rabbitmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.570231 oms-mqclient-2.2.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.570231 oms-mqclient-2.2.0/tests/unit/pulsar/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/unit/pulsar/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5586 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/unit/pulsar/test_pulsar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:28:57.570231 oms-mqclient-2.2.0/tests/unit/rabbitmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/unit/rabbitmq/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9196 2023-07-11 01:28:54.000000 oms-mqclient-2.2.0/tests/unit/rabbitmq/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.077164 oms-mqclient-2.3.0/mqclient/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5972 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_client_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.077164 oms-mqclient-2.3.0/mqclient/broker_clients/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_clients/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_clients/apachepulsar.py
+-rw-r--r--   0 root         (0) root         (0)    13421 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_clients/nats.py
+-rw-r--r--   0 root         (0) root         (0)    15335 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_clients/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/broker_clients/utils.py
+-rw-r--r--   0 root         (0) root         (0)      375 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/config.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/log_msgs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/py.typed
+-rw-r--r--   0 root         (0) root         (0)    24216 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/mqclient/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.077164 oms-mqclient-2.3.0/oms_mqclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-07-11 22:08:25.000000 oms-mqclient-2.3.0/oms_mqclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-07-11 22:08:25.000000 oms-mqclient-2.3.0/oms_mqclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 22:08:25.000000 oms-mqclient-2.3.0/oms_mqclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      298 2023-07-11 22:08:25.000000 oms-mqclient-2.3.0/oms_mqclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-11 22:08:25.000000 oms-mqclient-2.3.0/oms_mqclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2731 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.073164 oms-mqclient-2.3.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.077164 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9038 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py
+-rw-r--r--   0 root         (0) root         (0)    30730 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/integrate_queue.py
+-rw-r--r--   0 root         (0) root         (0)    20234 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/unit_tests.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/abstract_broker_client_tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/tests/integrate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/integrate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      962 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/integrate/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/integrate/test_nats.py
+-rw-r--r--   0 root         (0) root         (0)      859 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/integrate/test_pulsar.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/integrate/test_rabbitmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/tests/unit/pulsar/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/unit/pulsar/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5586 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/unit/pulsar/test_pulsar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 22:08:25.081164 oms-mqclient-2.3.0/tests/unit/rabbitmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/unit/rabbitmq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9196 2023-07-11 22:08:22.000000 oms-mqclient-2.3.0/tests/unit/rabbitmq/test_rabbitmq.py
```

### Comparing `oms-mqclient-2.2.0/LICENSE` & `oms-mqclient-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/PKG-INFO` & `oms-mqclient-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.2.0/README.md` & `oms-mqclient-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/mqclient/__init__.py` & `oms-mqclient-2.3.0/mqclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `oms-mqclient-2.2.0/mqclient/broker_client_interface.py` & `oms-mqclient-2.3.0/mqclient/broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/mqclient/broker_client_manager.py` & `oms-mqclient-2.3.0/mqclient/broker_client_manager.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/mqclient/broker_clients/apachepulsar.py` & `oms-mqclient-2.3.0/mqclient/broker_clients/apachepulsar.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,16 @@
         """Connect to subscriber."""
         LOGGER.debug(log_msgs.CONNECTING_SUB)
         await super().connect()
 
         self.consumer = self.client.subscribe(
             self.topic,
             self.subscription_name,
-            receiver_queue_size=self.prefetch,
+            # Neither receive with timeout nor partitioned topics can be used if the consumer queue size is zero.
+            receiver_queue_size=max(self.prefetch, 1),
             unacked_messages_timeout_ms=(
                 self.ack_timeout * 1000
                 if self.ack_timeout and self.ack_timeout > 10
                 else None
             ),
             consumer_type=pulsar.ConsumerType.Shared,
             initial_position=pulsar.InitialPosition.Earliest,
```

### Comparing `oms-mqclient-2.2.0/mqclient/broker_clients/nats.py` & `oms-mqclient-2.3.0/mqclient/broker_clients/nats.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,16 +198,16 @@
         if not timeout_millis:
             timeout_millis = DEFAULT_TIMEOUT_MILLIS
 
         try:
             nats_msgs: List[nats.aio.msg.Msg] = await utils.auto_retry_call(
                 func=functools.partial(
                     self._subscription.fetch,
-                    num_messages,
-                    int(math.ceil(timeout_millis / 1000)),
+                    batch=num_messages,
+                    timeout=int(math.ceil(timeout_millis / 1000)),
                 ),
                 retries=retries,
                 retry_delay=retry_delay,
                 close=self.close,
                 connect=self.connect,
                 logger=LOGGER,
                 nonretriable_conditions=lambda e: isinstance(
@@ -337,15 +337,15 @@
         if not self._subscription:
             raise RuntimeError("subscriber is not connected")
 
         msg = None
         try:
             gen = self._gen_messages(
                 timeout * 1000,
-                self.prefetch,
+                self.prefetch + 1,  # prefetch + 1 = # of msgs pulled
                 retries,
                 retry_delay,
             )
             while True:
                 # get message
                 LOGGER.debug(log_msgs.MSGGEN_GET_NEW_MESSAGE)
                 msg = await _anext(gen, None)
```

### Comparing `oms-mqclient-2.2.0/mqclient/broker_clients/rabbitmq.py` & `oms-mqclient-2.3.0/mqclient/broker_clients/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/mqclient/broker_clients/utils.py` & `oms-mqclient-2.3.0/mqclient/broker_clients/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/mqclient/log_msgs.py` & `oms-mqclient-2.3.0/mqclient/log_msgs.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/mqclient/queue.py` & `oms-mqclient-2.3.0/mqclient/queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 )
 
 from . import broker_client_manager
 from . import telemetry as wtt
 from .broker_client_interface import AckException, Message, NackException, Pub, Sub
 from .config import (
     DEFAULT_EXCEPT_ERRORS,
+    DEFAULT_PREFETCH,
     DEFAULT_RETRIES,
     DEFAULT_RETRY_DELAY,
     DEFAULT_TIMEOUT,
 )
 
 LOGGER = logging.getLogger("mqclient")
 
@@ -63,26 +64,30 @@
     """
 
     def __init__(
         self,
         broker_client: str,
         address: str = "localhost",
         name: str = "",
-        prefetch: int = 1,
+        prefetch: int = DEFAULT_PREFETCH,
         timeout: int = DEFAULT_TIMEOUT,
         ack_timeout: Optional[int] = None,
         retry_delay: int = DEFAULT_RETRY_DELAY,  # seconds
         retries: int = DEFAULT_RETRIES,  # ex: 2 means 1 initial try and 2 retries
         except_errors: bool = DEFAULT_EXCEPT_ERRORS,
         auth_token: str = "",
     ) -> None:
         self._broker_client = broker_client_manager.get_broker_client(broker_client)
         self._address = address
         self._name = name if name else Queue.make_name()
+
+        if prefetch < 0:
+            raise ValueError("prefetch must be non-negative")
         self._prefetch = prefetch
+
         self._auth_token = auth_token
 
         if ack_timeout is not None and ack_timeout <= 0:
             raise ValueError("timeout must be positive")
         self._ack_timeout = ack_timeout
 
         # properties
@@ -292,15 +297,14 @@
             "self._name",
             "self._prefetch",
             "self.timeout",
         ]
     )
     async def open_sub_manual_acking(
         self,
-        ack_pending_limit: Optional[int] = None,
     ) -> AsyncGenerator["ManualQueueSubResource", None]:
         """Open a resource to receive messages from the queue as an iterator.
 
         This returns a context-manager with an iterator function `iter_messages()`.
         The iterator stops when no messages are received for `timeout` seconds.
         Multiple calls to `open_sub()` is okay, but reusing the returned
         instance is not.
@@ -310,20 +314,15 @@
         *Unlike `open_sub()`*, the caller is responsible for:
             - All acking and/or nacking
             - Any error handling
 
         **NOTE: unless you need to parallelize your message processing,
         use `open_sub()`**
 
-        Args:
-            ack_pending_limit (int, optional):
-                how many messages are expected to be pending before being
-                acked. If not given, the `self.prefetch` is used. If you
-                surpass this limit, the iterator will raise a
-                `TooManyMessagesPendingAckException`.
+        NOTE: prefetching is disabled for this method
 
         Examples:
             async with queue.open_sub_manual_acking() as sub:
                 async for msg in sub.iter_messages():
                     print(msg.data)
                     sub.ack(msg)
                     # if you choose not to nack on an error,
@@ -354,27 +353,34 @@
 
                 for msg in pending:
                     await sub.ack(msg)
 
         Returns:
             ManualQueueSubResource -- context manager w/ iterator function
         """
-        sub = await self._create_sub_queue(prefetch_override=ack_pending_limit)
+        sub = await self._create_sub_queue(
+            # if prefetch=N (N>0), pika requires N acks/nacks before it gets more messages
+            #   We could implement logic that checks if this condition is met
+            #   but that would go against the intention of the "manual" usage,
+            #   e.g. a long running client with long running, parallel tasks
+            #   that finish at different times shouldn't have to wait for all
+            #   tasks to finish before getting more messages.
+            prefetch_override=0,
+        )
 
         try:
             yield ManualQueueSubResource(
                 functools.partial(
                     sub.get_message,
                     self.timeout * 1000,
                     retries=self.retries,
                     retry_delay=self.retry_delay,
                 ),
                 functools.partial(self._safe_ack, sub),
                 functools.partial(self._safe_nack, sub),
-                ack_pending_limit=sub.prefetch,
             )
         finally:
             await sub.close()
 
     @contextlib.asynccontextmanager  # needs to wrap @wtt stuff to span children correctly
     @wtt.spanned(
         these=[
@@ -455,18 +461,14 @@
         )
 
 
 class EmptyQueueException(Exception):
     """Raised when the queue is empty."""
 
 
-class TooManyMessagesPendingAckException(Exception):
-    """Raised when the ack-pending limit has been surpassed."""
-
-
 class QueuePubResource:
     """A manager class around `Pub.send_message()`."""
 
     def __init__(self, pub: Pub, retries: int, retry_delay: int):
         self.pub = pub
         self.retries = retries
         self.retry_delay = retry_delay
@@ -487,58 +489,46 @@
     """A manager class around `Sub.get_message()`."""
 
     def __init__(
         self,
         get_message_function: Callable[[], Awaitable[Optional[Message]]],
         ack_function: Callable[[Message], Awaitable[None]],
         nack_function: Callable[[Message], Awaitable[None]],
-        ack_pending_limit: int,
     ) -> None:
         self._get_message = get_message_function
         self._ack_function = ack_function
         self._nack_function = nack_function
-        self._ack_pending = 0
-        self._ack_pending_limit = ack_pending_limit
 
     async def iter_messages(self) -> AsyncIterator[Message]:
         """Yield a message."""
 
         @wtt.spanned(
             kind=wtt.SpanKind.CONSUMER,
             carrier="msg.headers",
             carrier_relation=wtt.CarrierRelation.LINK,
         )
         def add_span_link(msg: Message) -> Message:
             return msg
 
         while True:
-            if self._ack_pending >= self._ack_pending_limit:
-                raise TooManyMessagesPendingAckException(
-                    f"{self._ack_pending} messages are pending ack/nack "
-                    f"(out of {self._ack_pending_limit} allowed)"
-                )
-
             raw_msg = await self._get_message()
             if not raw_msg:  # no message -> close and exit
                 return
 
             msg = add_span_link(raw_msg)  # got a message -> link and proceed
             LOGGER.info(f"Received Message: {_message_size_message(msg)}")
-            self._ack_pending += 1
             yield msg
 
     async def ack(self, msg: Message) -> None:
         """Acknowledge the message."""
         await self._ack_function(msg)
-        self._ack_pending -= 1
 
     async def nack(self, msg: Message) -> None:
         """Acknowledge the message."""
         await self._nack_function(msg)
-        self._ack_pending -= 1
 
 
 class QueueSubResource:
     """An async context-manager generator, wraps `Sub.message_generator()`."""
 
     RUNTIME_ERROR_CONTEXT_STRING = (
         "'QueueSubResource' object's runtime "
```

### Comparing `oms-mqclient-2.2.0/mqclient/telemetry.py` & `oms-mqclient-2.3.0/mqclient/telemetry.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/oms_mqclient.egg-info/PKG-INFO` & `oms-mqclient-2.3.0/oms_mqclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oms-mqclient
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Message Queue Client API Supporting Apache Pulsar, Google's PubSub (GCP), RabbitMQ, and NATS.io
 Home-page: https://github.com/Observation-Management-Service/MQClient
 Download-URL: https://pypi.org/project/oms-mqclient/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/Observation-Management-Service/MQClient/issues
```

### Comparing `oms-mqclient-2.2.0/oms_mqclient.egg-info/SOURCES.txt` & `oms-mqclient-2.3.0/oms_mqclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/setup.cfg` & `oms-mqclient-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py` & `oms-mqclient-2.3.0/tests/abstract_broker_client_tests/integrate_broker_client_interface.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/tests/abstract_broker_client_tests/integrate_queue.py` & `oms-mqclient-2.3.0/tests/abstract_broker_client_tests/integrate_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import asyncio
 import logging
 from multiprocessing.dummy import Pool as ThreadPool
 from typing import Any, List
 
 import asyncstdlib as asl
 import pytest
-from mqclient.queue import Queue, TooManyMessagesPendingAckException
+from mqclient.queue import Queue
 
 from .utils import (
     DATA_LIST,
     _log_recv,
     _log_recv_multiple,
     _log_send,
     all_were_received,
@@ -827,15 +827,15 @@
                 _log_send(d)
 
         class TestException(Exception):  # pylint: disable=C0115
             pass
 
         sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
         sub.timeout = 1
-        async with sub.open_sub_manual_acking(ack_pending_limit=len(DATA_LIST)) as gen:
+        async with sub.open_sub_manual_acking() as gen:
             pending = []
             async for i, msg in asl.enumerate(gen.iter_messages()):
                 try:
                     # DO WORK!
                     print(f"{i}: `{msg.data}`")
                     if i % 3 == 0:  # nack every 1/3
                         raise TestException()
@@ -849,73 +849,7 @@
                     await gen.nack(msg)
 
             for msg in pending:  # messages with index not %2 nor %3, (1,5,7,...)
                 await gen.ack(msg)
 
         print(all_recvd)
         assert all_were_received(all_recvd)
-
-    @pytest.mark.asyncio
-    async def test_250__delayed_acking__fail(
-        self, queue_name: str, auth_token: str
-    ) -> None:
-        """Test open_sub_manual_acking() w/ delayed acking AND surpass
-        `ack_pending_limit`."""
-        all_recvd: List[Any] = []
-
-        async with Queue(
-            self.broker_client, name=queue_name, auth_token=auth_token
-        ).open_pub() as p:
-            for d in DATA_LIST:
-                await p.send(d)
-                _log_send(d)
-
-        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
-        sub.timeout = 1
-        ack_pending_limit = len(DATA_LIST) // 2
-        async with sub.open_sub_manual_acking(ack_pending_limit) as gen:
-            messages = []
-            with pytest.raises(TooManyMessagesPendingAckException):
-                async for i, msg in asl.enumerate(gen.iter_messages()):
-                    print(f"{i}: `{msg.data}`")
-                    all_recvd.append(_log_recv(msg.data))
-                    messages.append(msg)
-                    # assert msg.data == DATA_LIST[i]  # we don't guarantee order
-                    assert gen._ack_pending == i + 1
-
-        print(all_recvd)
-        assert not all_were_received(all_recvd)
-
-    @pytest.mark.asyncio
-    async def test_251__no_nacking__fail(
-        self, queue_name: str, auth_token: str
-    ) -> None:
-        """Test open_sub_manual_acking() w/ delayed acking AND surpass
-        `ack_pending_limit`."""
-        all_recvd: List[Any] = []
-
-        async with Queue(
-            self.broker_client, name=queue_name, auth_token=auth_token
-        ).open_pub() as p:
-            for d in DATA_LIST:
-                await p.send(d)
-                _log_send(d)
-
-        sub = Queue(self.broker_client, name=queue_name, auth_token=auth_token)
-        sub.timeout = 1
-        ack_pending_limit = len(DATA_LIST) // 2
-        async with sub.open_sub_manual_acking(ack_pending_limit) as gen:
-            messages = []
-            with pytest.raises(TooManyMessagesPendingAckException):
-                async for i, msg in asl.enumerate(gen.iter_messages()):
-                    print(f"{i}: `{msg.data}`")
-                    all_recvd.append(_log_recv(msg.data))
-                    messages.append(msg)
-                    # assert msg.data == DATA_LIST[i]  # we don't guarantee order
-                    if i % 2 == 0:
-                        pass  # eventually enough "passes" causes a TooManyMessagesPendingAckException
-                    else:
-                        await gen.ack(msg)
-                    assert gen._ack_pending == (i // 2) + 1
-
-        print(all_recvd)
-        assert not all_were_received(all_recvd)
```

### Comparing `oms-mqclient-2.2.0/tests/abstract_broker_client_tests/unit_tests.py` & `oms-mqclient-2.3.0/tests/abstract_broker_client_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/tests/abstract_broker_client_tests/utils.py` & `oms-mqclient-2.3.0/tests/abstract_broker_client_tests/utils.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/tests/integrate/conftest.py` & `oms-mqclient-2.3.0/tests/integrate/conftest.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/tests/integrate/test_nats.py` & `oms-mqclient-2.3.0/tests/integrate/test_nats.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/tests/integrate/test_pulsar.py` & `oms-mqclient-2.3.0/tests/integrate/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/tests/integrate/test_rabbitmq.py` & `oms-mqclient-2.3.0/tests/integrate/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/tests/unit/pulsar/test_pulsar.py` & `oms-mqclient-2.3.0/tests/unit/pulsar/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `oms-mqclient-2.2.0/tests/unit/rabbitmq/test_rabbitmq.py` & `oms-mqclient-2.3.0/tests/unit/rabbitmq/test_rabbitmq.py`

 * *Files identical despite different names*

