# Comparing `tmp/velikafkaclient-1.0.3.tar.gz` & `tmp/velikafkaclient-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velikafkaclient-1.0.3.tar", last modified: Tue Jul 11 15:34:47 2023, max compression
+gzip compressed data, was "velikafkaclient-1.0.4.tar", last modified: Wed Jul 12 05:56:58 2023, max compression
```

## Comparing `velikafkaclient-1.0.3.tar` & `velikafkaclient-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-11 15:34:47.060711 velikafkaclient-1.0.3/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/MANIFEST.in
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3464 2023-07-11 15:34:47.060600 velikafkaclient-1.0.3/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3279 2023-07-11 15:34:28.000000 velikafkaclient-1.0.3/readme.md
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-11 15:34:47.060741 velikafkaclient-1.0.3/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-11 15:34:36.000000 velikafkaclient-1.0.3/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-11 15:34:47.059157 velikafkaclient-1.0.3/velikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2046 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/consumer.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      374 2023-07-11 11:27:00.000000 velikafkaclient-1.0.3/velikafkaclient/decorators.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/eventregistration.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-11 15:34:47.060042 velikafkaclient-1.0.3/velikafkaclient/events/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/events/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      126 2023-07-11 11:27:00.000000 velikafkaclient-1.0.3/velikafkaclient/events/base.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/events/triptracker.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/exceptions.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-11 11:27:00.000000 velikafkaclient-1.0.3/velikafkaclient/producer.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-11 15:34:47.060416 velikafkaclient-1.0.3/velikafkaclient/topics/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/topics/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/topics/topics.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.3/velikafkaclient/topics/triptracker.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-11 15:34:47.059662 velikafkaclient-1.0.3/velikafkaclient.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3464 2023-07-11 15:34:47.000000 velikafkaclient-1.0.3/velikafkaclient.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      577 2023-07-11 15:34:47.000000 velikafkaclient-1.0.3/velikafkaclient.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-11 15:34:47.000000 velikafkaclient-1.0.3/velikafkaclient.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-11 15:34:47.000000 velikafkaclient-1.0.3/velikafkaclient.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-12 05:56:58.618696 velikafkaclient-1.0.4/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-07-05 09:25:18.000000 velikafkaclient-1.0.4/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-12 05:56:58.618581 velikafkaclient-1.0.4/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2193 2023-07-12 05:55:37.000000 velikafkaclient-1.0.4/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-07-12 05:56:58.618724 velikafkaclient-1.0.4/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      398 2023-07-12 05:56:48.000000 velikafkaclient-1.0.4/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-12 05:56:58.616959 velikafkaclient-1.0.4/velikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      116 2023-07-05 09:25:18.000000 velikafkaclient-1.0.4/velikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2145 2023-07-11 16:03:33.000000 velikafkaclient-1.0.4/velikafkaclient/consumer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      374 2023-07-11 11:27:00.000000 velikafkaclient-1.0.4/velikafkaclient/decorators.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     3489 2023-07-05 09:25:18.000000 velikafkaclient-1.0.4/velikafkaclient/eventregistration.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-12 05:56:58.617991 velikafkaclient-1.0.4/velikafkaclient/events/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.4/velikafkaclient/events/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      126 2023-07-11 11:27:00.000000 velikafkaclient-1.0.4/velikafkaclient/events/base.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1923 2023-07-05 09:25:18.000000 velikafkaclient-1.0.4/velikafkaclient/events/triptracker.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      160 2023-07-05 09:25:18.000000 velikafkaclient-1.0.4/velikafkaclient/exceptions.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      392 2023-07-11 16:03:33.000000 velikafkaclient-1.0.4/velikafkaclient/killer.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1260 2023-07-11 11:27:00.000000 velikafkaclient-1.0.4/velikafkaclient/producer.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-12 05:56:58.618414 velikafkaclient-1.0.4/velikafkaclient/topics/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-05 09:25:18.000000 velikafkaclient-1.0.4/velikafkaclient/topics/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      263 2023-07-05 09:25:18.000000 velikafkaclient-1.0.4/velikafkaclient/topics/topics.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1124 2023-07-05 09:25:18.000000 velikafkaclient-1.0.4/velikafkaclient/topics/triptracker.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-07-12 05:56:58.617591 velikafkaclient-1.0.4/velikafkaclient.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     2378 2023-07-12 05:56:58.000000 velikafkaclient-1.0.4/velikafkaclient.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      603 2023-07-12 05:56:58.000000 velikafkaclient-1.0.4/velikafkaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-07-12 05:56:58.000000 velikafkaclient-1.0.4/velikafkaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       16 2023-07-12 05:56:58.000000 velikafkaclient-1.0.4/velikafkaclient.egg-info/top_level.txt
```

### Comparing `velikafkaclient-1.0.3/velikafkaclient/consumer.py` & `velikafkaclient-1.0.4/velikafkaclient/consumer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 
 from aiokafka import AIOKafkaConsumer
 
 from .eventregistration import kafka_topic_events
 from .exceptions import InvalidEventTopicException, InvalidEventStructure
+from .killer import KafkaClientGracefulKiller
 
 
 class AsyncKafkaConsumer:
 
     def __init__(self, bootstrap_servers, group_id=None):
         self.kafka_topic_events = kafka_topic_events
         self.client = None
         self.bootstrap_servers = bootstrap_servers
         self.group_id = group_id
         self.subscriptions = dict()
         self.topics = set()
+        self.killer = KafkaClientGracefulKiller(self)
 
     async def start(self):
         if self.client is not None:
             raise Exception("Consumer already started, stop before starting again <3")
         self.client = AIOKafkaConsumer(
             *list(self.topics),
             bootstrap_servers=self.bootstrap_servers,
@@ -47,8 +49,7 @@
                 data = json.loads(decoded_msg)
                 msg_event = topic_event_model(**data)
                 handler = await self.subscriptions[msg.topic](msg_event)
                 print(handler)
             except Exception as e:
                 # TODO add proper exception handling
                 raise InvalidEventStructure(f"Invalid event structure {str(msg.value)} for topic {msg.topic}")
-
```

### Comparing `velikafkaclient-1.0.3/velikafkaclient/eventregistration.py` & `velikafkaclient-1.0.4/velikafkaclient/eventregistration.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.3/velikafkaclient/events/triptracker.py` & `velikafkaclient-1.0.4/velikafkaclient/events/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.3/velikafkaclient/producer.py` & `velikafkaclient-1.0.4/velikafkaclient/producer.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.3/velikafkaclient/topics/triptracker.py` & `velikafkaclient-1.0.4/velikafkaclient/topics/triptracker.py`

 * *Files identical despite different names*

### Comparing `velikafkaclient-1.0.3/velikafkaclient.egg-info/SOURCES.txt` & `velikafkaclient-1.0.4/velikafkaclient.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 readme.md
 setup.py
 velikafkaclient/__init__.py
 velikafkaclient/consumer.py
 velikafkaclient/decorators.py
 velikafkaclient/eventregistration.py
 velikafkaclient/exceptions.py
+velikafkaclient/killer.py
 velikafkaclient/producer.py
 velikafkaclient.egg-info/PKG-INFO
 velikafkaclient.egg-info/SOURCES.txt
 velikafkaclient.egg-info/dependency_links.txt
 velikafkaclient.egg-info/top_level.txt
 velikafkaclient/events/__init__.py
 velikafkaclient/events/base.py
```

