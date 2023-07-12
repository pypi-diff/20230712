# Comparing `tmp/nameko_kafka-0.2.0.tar.gz` & `tmp/nameko_kafka-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nameko_kafka-0.2.0.tar", last modified: Sat Jul 25 19:06:25 2020, max compression
+gzip compressed data, was "nameko_kafka-0.2.1.tar", last modified: Wed Jul 12 02:25:54 2023, max compression
```

## Comparing `nameko_kafka-0.2.0.tar` & `nameko_kafka-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 ketan      (501) staff       (20)        0 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/
--rw-r--r--   0 ketan      (501) staff       (20)    11318 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/PKG-INFO
--rw-r--r--   0 ketan      (501) staff       (20)     8047 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/README.md
-drwxr-xr-x   0 ketan      (501) staff       (20)        0 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/nameko_kafka/
--rw-r--r--   0 ketan      (501) staff       (20)      238 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/__init__.py
--rw-r--r--   0 ketan      (501) staff       (20)      127 2020-03-28 04:27:34.000000 nameko_kafka-0.2.0/nameko_kafka/constants.py
-drwxr-xr-x   0 ketan      (501) staff       (20)        0 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/nameko_kafka/consumers/
--rw-r--r--   0 ketan      (501) staff       (20)      169 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/consumers/__init__.py
--rw-r--r--   0 ketan      (501) staff       (20)      518 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/consumers/default.py
--rw-r--r--   0 ketan      (501) staff       (20)     3761 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/consumers/exactly_once.py
--rw-r--r--   0 ketan      (501) staff       (20)     2127 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/consumers/least_once.py
--rw-r--r--   0 ketan      (501) staff       (20)     2123 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/consumers/most_once.py
--rw-r--r--   0 ketan      (501) staff       (20)     1571 2020-03-28 05:49:28.000000 nameko_kafka-0.2.0/nameko_kafka/dependency.py
--rw-r--r--   0 ketan      (501) staff       (20)     3148 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/entrypoint.py
-drwxr-xr-x   0 ketan      (501) staff       (20)        0 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/nameko_kafka/storage/
--rw-r--r--   0 ketan      (501) staff       (20)       32 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/storage/__init__.py
--rw-r--r--   0 ketan      (501) staff       (20)     2040 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/storage/base.py
--rw-r--r--   0 ketan      (501) staff       (20)     2025 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/storage/mongo.py
--rw-r--r--   0 ketan      (501) staff       (20)      262 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/nameko_kafka/version.py
-drwxr-xr-x   0 ketan      (501) staff       (20)        0 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/nameko_kafka.egg-info/
--rw-r--r--   0 ketan      (501) staff       (20)    11318 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/nameko_kafka.egg-info/PKG-INFO
--rw-r--r--   0 ketan      (501) staff       (20)      871 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/nameko_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 ketan      (501) staff       (20)        1 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/nameko_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 ketan      (501) staff       (20)      213 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/nameko_kafka.egg-info/requires.txt
--rw-r--r--   0 ketan      (501) staff       (20)       19 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/nameko_kafka.egg-info/top_level.txt
--rw-r--r--   0 ketan      (501) staff       (20)       38 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/setup.cfg
--rw-r--r--   0 ketan      (501) staff       (20)     2269 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/setup.py
-drwxr-xr-x   0 ketan      (501) staff       (20)        0 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/tests/
-drwxr-xr-x   0 ketan      (501) staff       (20)        0 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/tests/storage/
--rw-r--r--   0 ketan      (501) staff       (20)        0 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/tests/storage/__init__.py
--rw-r--r--   0 ketan      (501) staff       (20)     1681 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/tests/storage/test_base.py
--rw-r--r--   0 ketan      (501) staff       (20)     2051 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/tests/storage/test_mongo.py
-drwxr-xr-x   0 ketan      (501) staff       (20)        0 2020-07-25 19:06:25.000000 nameko_kafka-0.2.0/tests/test_consumers/
--rw-r--r--   0 ketan      (501) staff       (20)        0 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/tests/test_consumers/__init__.py
--rw-r--r--   0 ketan      (501) staff       (20)      705 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/tests/test_consumers/test_default.py
--rw-r--r--   0 ketan      (501) staff       (20)     2140 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/tests/test_consumers/test_exactly_once.py
--rw-r--r--   0 ketan      (501) staff       (20)     1464 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/tests/test_consumers/test_least_once.py
--rw-r--r--   0 ketan      (501) staff       (20)     1483 2020-07-25 19:02:14.000000 nameko_kafka-0.2.0/tests/test_consumers/test_most_once.py
+drwxr-xr-x   0 ketan      (501) staff       (20)        0 2023-07-12 02:25:54.251971 nameko_kafka-0.2.1/
+-rw-r--r--   0 ketan      (501) staff       (20)     1068 2020-03-27 19:31:35.000000 nameko_kafka-0.2.1/LICENSE
+-rw-r--r--   0 ketan      (501) staff       (20)     8957 2023-07-12 02:25:54.251315 nameko_kafka-0.2.1/PKG-INFO
+-rw-r--r--   0 ketan      (501) staff       (20)     8047 2023-07-12 02:21:51.000000 nameko_kafka-0.2.1/README.md
+drwxr-xr-x   0 ketan      (501) staff       (20)        0 2023-07-12 02:25:54.231049 nameko_kafka-0.2.1/nameko_kafka/
+-rw-r--r--   0 ketan      (501) staff       (20)      238 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/nameko_kafka/__init__.py
+-rw-r--r--   0 ketan      (501) staff       (20)      127 2020-03-28 04:27:34.000000 nameko_kafka-0.2.1/nameko_kafka/constants.py
+drwxr-xr-x   0 ketan      (501) staff       (20)        0 2023-07-12 02:25:54.240544 nameko_kafka-0.2.1/nameko_kafka/consumers/
+-rw-r--r--   0 ketan      (501) staff       (20)      169 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/nameko_kafka/consumers/__init__.py
+-rw-r--r--   0 ketan      (501) staff       (20)      518 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/nameko_kafka/consumers/default.py
+-rw-r--r--   0 ketan      (501) staff       (20)     3761 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/nameko_kafka/consumers/exactly_once.py
+-rw-r--r--   0 ketan      (501) staff       (20)     2127 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/nameko_kafka/consumers/least_once.py
+-rw-r--r--   0 ketan      (501) staff       (20)     2123 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/nameko_kafka/consumers/most_once.py
+-rw-r--r--   0 ketan      (501) staff       (20)     1571 2020-03-28 05:49:28.000000 nameko_kafka-0.2.1/nameko_kafka/dependency.py
+-rw-r--r--   0 ketan      (501) staff       (20)     3148 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/nameko_kafka/entrypoint.py
+drwxr-xr-x   0 ketan      (501) staff       (20)        0 2023-07-12 02:25:54.242924 nameko_kafka-0.2.1/nameko_kafka/storage/
+-rw-r--r--   0 ketan      (501) staff       (20)       32 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/nameko_kafka/storage/__init__.py
+-rw-r--r--   0 ketan      (501) staff       (20)     2040 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/nameko_kafka/storage/base.py
+-rw-r--r--   0 ketan      (501) staff       (20)     2025 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/nameko_kafka/storage/mongo.py
+-rw-r--r--   0 ketan      (501) staff       (20)      262 2023-07-12 02:21:51.000000 nameko_kafka-0.2.1/nameko_kafka/version.py
+drwxr-xr-x   0 ketan      (501) staff       (20)        0 2023-07-12 02:25:54.233106 nameko_kafka-0.2.1/nameko_kafka.egg-info/
+-rw-r--r--   0 ketan      (501) staff       (20)     8957 2023-07-12 02:25:54.000000 nameko_kafka-0.2.1/nameko_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 ketan      (501) staff       (20)      944 2023-07-12 02:25:54.000000 nameko_kafka-0.2.1/nameko_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 ketan      (501) staff       (20)        1 2023-07-12 02:25:54.000000 nameko_kafka-0.2.1/nameko_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 ketan      (501) staff       (20)      237 2023-07-12 02:25:54.000000 nameko_kafka-0.2.1/nameko_kafka.egg-info/requires.txt
+-rw-r--r--   0 ketan      (501) staff       (20)       19 2023-07-12 02:25:54.000000 nameko_kafka-0.2.1/nameko_kafka.egg-info/top_level.txt
+-rw-r--r--   0 ketan      (501) staff       (20)       38 2023-07-12 02:25:54.252258 nameko_kafka-0.2.1/setup.cfg
+-rw-r--r--   0 ketan      (501) staff       (20)     2245 2023-07-12 02:21:51.000000 nameko_kafka-0.2.1/setup.py
+drwxr-xr-x   0 ketan      (501) staff       (20)        0 2023-07-12 02:25:54.244964 nameko_kafka-0.2.1/tests/
+drwxr-xr-x   0 ketan      (501) staff       (20)        0 2023-07-12 02:25:54.248920 nameko_kafka-0.2.1/tests/test_consumers/
+-rw-r--r--   0 ketan      (501) staff       (20)        0 2020-07-25 19:02:14.000000 nameko_kafka-0.2.1/tests/test_consumers/__init__.py
+-rw-r--r--   0 ketan      (501) staff       (20)      705 2023-02-09 18:42:35.000000 nameko_kafka-0.2.1/tests/test_consumers/test_default.py
+-rw-r--r--   0 ketan      (501) staff       (20)     2140 2023-02-09 18:42:35.000000 nameko_kafka-0.2.1/tests/test_consumers/test_exactly_once.py
+-rw-r--r--   0 ketan      (501) staff       (20)     1464 2023-02-09 18:42:35.000000 nameko_kafka-0.2.1/tests/test_consumers/test_least_once.py
+-rw-r--r--   0 ketan      (501) staff       (20)     1483 2023-02-09 18:42:35.000000 nameko_kafka-0.2.1/tests/test_consumers/test_most_once.py
+-rw-r--r--   0 ketan      (501) staff       (20)     2989 2023-02-09 18:42:35.000000 nameko_kafka-0.2.1/tests/test_dependency.py
+-rw-r--r--   0 ketan      (501) staff       (20)     4444 2023-07-12 02:21:51.000000 nameko_kafka-0.2.1/tests/test_entrypoint.py
+drwxr-xr-x   0 ketan      (501) staff       (20)        0 2023-07-12 02:25:54.250683 nameko_kafka-0.2.1/tests/test_storage/
+-rw-r--r--   0 ketan      (501) staff       (20)        0 2023-07-12 02:21:51.000000 nameko_kafka-0.2.1/tests/test_storage/__init__.py
+-rw-r--r--   0 ketan      (501) staff       (20)     1681 2023-07-12 02:21:51.000000 nameko_kafka-0.2.1/tests/test_storage/test_base.py
+-rw-r--r--   0 ketan      (501) staff       (20)     2076 2023-07-12 02:21:51.000000 nameko_kafka-0.2.1/tests/test_storage/test_mongo.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nameko_kafka-0.2.0/PKG-INFO` & `nameko_kafka-0.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,312 +1,16 @@
 Metadata-Version: 2.1
 Name: nameko_kafka
-Version: 0.2.0
+Version: 0.2.1
 Summary: Kafka extension for Nameko microservice framework
 Home-page: https://github.com/ketgo/nameko-kafka
 Author: Ketan Goyal
 Author-email: ketangoyal1988@gmail.com
 License: MIT
-Description: # Nameko-Kafka
-        
-        [![Build Status](https://travis-ci.com/ketgo/nameko-kafka.svg?branch=master)](https://travis-ci.com/ketgo/nameko-kafka)
-        [![codecov.io](https://codecov.io/gh/ketgo/nameko-kafka/coverage.svg?branch=master)](https://codecov.io/gh/ketgo/nameko-kafka/coverage.svg?branch=master)
-        [![MIT licensed](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
-        ---
-        
-        Kafka extension for [Nameko](https://www.nameko.io/) microservice framework. 
-        
-        ## Introduction
-        
-        This is a Nameko microservice framework [extension](https://nameko.readthedocs.io/en/stable/key_concepts.html) to support 
-        Kafka entrypoint and dependency. The motivation behind the project is issue [569](https://github.com/nameko/nameko/issues/569). 
-        _Nameko-kafka_ provide a simple implementation of the entrypoint based on the approach by [calumpeterwebb](https://medium.com/@calumpeterwebb/nameko-tutorial-creating-a-kafka-consuming-microservice-c4a7adb804d0).
-        It also includes a dependency provider for publishing Kafka messages from within a Nameko service.
-        
-        ## Installation
-        
-        The package is supports Python >= 3.5
-        ```bash
-        $ pip install nameko-kafka
-        ```
-        
-        ## Usage
-        
-        The extension can be used for both, a service dependency and entrypoint. Example usage for both cases are shown in the
-        following sections.
-        
-        ## Dependency
-        
-        This is basically a [python-kafka](https://github.com/dpkp/kafka-python) producer in the form of Nameko dependency. 
-        Nameko uses dependency injection to instantiate the producer. You just need to declare it in your service class as shown:
-        
-        ```python
-        from nameko.rpc import rpc
-        from nameko_kafka import KafkaProducer
-        
-        
-        class MyService:
-            """
-                My microservice
-            """
-            name = "my-service"
-            # Kafak dependency
-            producer = KafkaProducer(bootstrap_servers='localhost:1234')
-            
-            @rpc
-            def method(self):
-                # Publish message using dependency
-                self.producer.send("kafka-topic", value=b"my-message", key=b"my-key")
-        ```
-        
-        Here `KafkaProducer` accepts all options valid for `python-kafka`'s [KafkaProducer](https://kafka-python.readthedocs.io/en/master/apidoc/KafkaProducer.html).
-        
-        ### Entrypoint
-        
-        You can use the `nameko_kafka.consume` decorator in your services to process Kafka messages:
-        
-        ```python
-        from nameko_kafka import consume
-        
-        
-        class MyService:
-            """
-                My microservice 
-            """
-            name = "my-service"
-        
-            @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234')
-            def method(self, message):
-                # Your message handler
-                handle_message(message) 
-        ```
-        
-        The `consume` decorator accepts all the options valid for `python-kafka`'s [KafkaConsumer](https://kafka-python.readthedocs.io/en/master/apidoc/KafkaConsumer.html). 
-        
-        On top of the default `python-kafka`'s autocommit feature, the entrypoint also comes with support for three different 
-        types of offset commit strategies: _at least once_, _at most once_ and _exactly once_. The three strategies correspond 
-        to the different message delivery semantics achievable in Kafka. Examples for each are shown in the following subsections.
-        
-        #### At Least Once
-        
-        ```python
-        from nameko_kafka import consume, Semantic
-        
-        
-        class MyService:
-            """
-                My microservice 
-            """
-            name = "my-service"
-            
-            # At least once semantic consumer
-            @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234', semantic=Semantic.AT_LEAST_ONCE)
-            def method(self, message):
-                # Your message handler
-                handle_message(message) 
-        ```
-        
-        #### At Most Once
-        
-        ```python
-        from nameko_kafka import consume, Semantic
-        
-        
-        class MyService:
-            """
-                My microservice 
-            """
-            name = "my-service"
-            
-            # At most once semantic consumer
-            @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234', semantic=Semantic.AT_MOST_ONCE)
-            def method(self, message):
-                # Your message handler
-                handle_message(message) 
-        ```
-        
-        #### Exactly Once
-        
-        The exactly once semantic requires a persistent storage to save message offsets. Such a persistent store can be 
-        implemented using the `OffsetStorage` interface provided by Nameko-kafka. There can be various backend implementations 
-        like RDBMS, NoSQL databases, etc. Support for some comes out of the box:
-        
-        ##### MongoDB Storage 
-        
-        ```python
-        from nameko_kafka import consume, Semantic
-        from nameko_kafka.storage import MongoStorage
-        
-        from pymongo import MongoClient
-        
-        
-        class MyService:
-            """
-                My microservice 
-            """
-            name = "my-service"
-            
-            # At most once semantic consumer
-            @consume(
-                "kafka-topic", 
-                group_id="my-group", 
-                bootstrap_servers='localhost:1234', 
-                semantic=Semantic.EXACTLY_ONCE,
-                storage=MongoStorage(
-                    # MongoDB backend client
-                    client=MongoClient('localhost', 27017),
-                    # Database to use for storage
-                    db_name="database-name",
-                    # Collection to use for storage
-                    collection="collection-name"
-                )       
-            )
-            def method(self, message):
-                # Your message handler
-                handle_message(message) 
-        ```
-        
-        Note: If the `db_name` and `collection` arguments are not specified, the default value of `"nameko_kafka_offsets"` and 
-        `"offsets"` will be used by the storage respectively.
-        
-        ##### SQL Storage
-        
-        Part of v0.2.1
-        
-        ##### S3 Storage
-        
-        Part of v0.2.2
-        
-        ##### Azure Block Storage
-        
-        Part of v0.2.3
-        
-        ##### Create Custom Storage
-        
-        You can create your own offset storage by implementing the `OffsetStorage` interface. It exposes the following methods:
-        
-        ```python
-        from nameko_kafka.storage.base import OffsetStorage
-        
-        class MyStorage(OffsetStorage):
-            """
-                My custom offset storage.
-            """
-        
-            def setup(self):
-                """
-                    Method for setup of the storage.
-                """
-        
-            def stop(self):
-                """
-                    Method to teardown the storage.
-                """
-        
-            def read(self, topic, partition):
-                """
-                    Read last stored offset from storage for 
-                    given topic and partition.
-        
-                    :param topic: message topic
-                    :param partition: partition number of the topic
-                    :returns: last committed offset value
-                """
-        
-            def write(self, offsets):
-                """
-                    Write offsets to storage.
-        
-                    :param offsets: mapping between topic-partition
-                        tuples and corresponding latest offset value, 
-                        e.g.
-                        {
-                            ("topic-1", 0): 1,
-                            ("topic-1", 1): 3,
-                            ("topic-2", 1): 10,
-                            ...
-                        }
-                """
-        ```
-        
-        
-        ## Configurations
-        
-        The extension configurations can be set in a nameko [config.yaml]((https://docs.nameko.io/en/stable/cli.html)) file, or 
-        by environment variables.
-        
-        ### Config File
-        
-        ```yaml
-        # Config for entrypoint
-        KAFKA_CONSUMER:
-          bootstrap_servers: 'localhost:1234'
-          retry_backoff_ms: 100
-          ...
-        
-        # Config for dependency
-        KAFKA_PRODUCER:
-          bootstrap_servers: 'localhost:1234'
-          retries: 3
-          ...
-        ```
-        
-        ### Environment Variables
-        
-        ```.env
-        # Config for entrypoint
-        KAFKA_CONSUMER='{"bootstrap_servers": "localhost:1234", "retry_backoff_ms": 100}'
-        
-        # Config for dependency
-        KAFKA_PRODUCER='{"bootstrap_servers": "localhost:1234", "retries": 3}'
-        ```
-        
-        ## Milestones
-        
-        - [x] Kafka Entrypoint
-        - [x] Kafka Dependency
-        - [x] Commit strategies: 
-            - _ALMOST_ONCE_DELIVERY_
-            - _AT_LEAST_ONCE_DELIVERY_ 
-            - _EXACTLY_ONCE_DELIVERY_
-        - [x] Commit storage for _EXACT_ONCE_DELIVERY_ strategy
-        
-        ## Developers
-        
-        For development a kafka broker is required. You can spawn one using the [docker-compose.yml](https://github.com/ketgo/nameko-kafka/blob/master/tests/conftest.py) 
-        file in the `tests` folder:
-        ```bash
-        $ cd tests
-        $ docker-compose up -d 
-        ```
-        
-        To install all package dependencies:
-        ```bash
-        $ pip install -r .[dev]
-        or
-        $ make deps
-        ```
-        
-        Other useful commands:
-        ```bash
-        $ pytest --cov=nameko_kafka tests/			# to get coverage report
-        or
-        $ make coverage
-        
-        $ pylint nameko_kafka       # to check code quality with PyLint
-        or
-        $ make lint
-        ```
-        
-        ## Contributions
-        
-        Issue reports and Pull requests are always welcomed. Thanks!
-        
 Keywords: nameko,kafka,microservice
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
@@ -314,7 +18,303 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mongo
 Provides-Extra: sql
+License-File: LICENSE
+
+# Nameko-Kafka
+
+[![Build Status](https://travis-ci.com/ketgo/nameko-kafka.svg?branch=master)](https://travis-ci.com/ketgo/nameko-kafka)
+[![codecov.io](https://codecov.io/gh/ketgo/nameko-kafka/coverage.svg?branch=master)](https://codecov.io/gh/ketgo/nameko-kafka/coverage.svg?branch=master)
+[![MIT licensed](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
+---
+
+Kafka extension for [Nameko](https://www.nameko.io/) microservice framework. 
+
+## Introduction
+
+This is a Nameko microservice framework [extension](https://nameko.readthedocs.io/en/stable/key_concepts.html) to support 
+Kafka entrypoint and dependency. The motivation behind the project is issue [569](https://github.com/nameko/nameko/issues/569). 
+_Nameko-kafka_ provide a simple implementation of the entrypoint based on the approach by [calumpeterwebb](https://medium.com/@calumpeterwebb/nameko-tutorial-creating-a-kafka-consuming-microservice-c4a7adb804d0).
+It also includes a dependency provider for publishing Kafka messages from within a Nameko service.
+
+## Installation
+
+The package is supports Python >= 3.5
+```bash
+$ pip install nameko-kafka
+```
+
+## Usage
+
+The extension can be used for both, a service dependency and entrypoint. Example usage for both cases are shown in the
+following sections.
+
+## Dependency
+
+This is basically a [python-kafka](https://github.com/dpkp/kafka-python) producer in the form of Nameko dependency. 
+Nameko uses dependency injection to instantiate the producer. You just need to declare it in your service class as shown:
+
+```python
+from nameko.rpc import rpc
+from nameko_kafka import KafkaProducer
+
+
+class MyService:
+    """
+        My microservice
+    """
+    name = "my-service"
+    # Kafak dependency
+    producer = KafkaProducer(bootstrap_servers='localhost:1234')
+    
+    @rpc
+    def method(self):
+        # Publish message using dependency
+        self.producer.send("kafka-topic", value=b"my-message", key=b"my-key")
+```
+
+Here `KafkaProducer` accepts all options valid for `python-kafka`'s [KafkaProducer](https://kafka-python.readthedocs.io/en/master/apidoc/KafkaProducer.html).
+
+### Entrypoint
+
+You can use the `nameko_kafka.consume` decorator in your services to process Kafka messages:
+
+```python
+from nameko_kafka import consume
+
+
+class MyService:
+    """
+        My microservice 
+    """
+    name = "my-service"
+
+    @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234')
+    def method(self, message):
+        # Your message handler
+        handle_message(message) 
+```
+
+The `consume` decorator accepts all the options valid for `python-kafka`'s [KafkaConsumer](https://kafka-python.readthedocs.io/en/master/apidoc/KafkaConsumer.html). 
+
+On top of the default `python-kafka`'s autocommit feature, the entrypoint also comes with support for three different 
+types of offset commit strategies: _at least once_, _at most once_ and _exactly once_. The three strategies correspond 
+to the different message delivery semantics achievable in Kafka. Examples for each are shown in the following subsections.
+
+#### At Least Once
+
+```python
+from nameko_kafka import consume, Semantic
+
+
+class MyService:
+    """
+        My microservice 
+    """
+    name = "my-service"
+    
+    # At least once semantic consumer
+    @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234', semantic=Semantic.AT_LEAST_ONCE)
+    def method(self, message):
+        # Your message handler
+        handle_message(message) 
+```
+
+#### At Most Once
+
+```python
+from nameko_kafka import consume, Semantic
+
+
+class MyService:
+    """
+        My microservice 
+    """
+    name = "my-service"
+    
+    # At most once semantic consumer
+    @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234', semantic=Semantic.AT_MOST_ONCE)
+    def method(self, message):
+        # Your message handler
+        handle_message(message) 
+```
+
+#### Exactly Once
+
+The exactly once semantic requires a persistent storage to save message offsets. Such a persistent store can be 
+implemented using the `OffsetStorage` interface provided by Nameko-kafka. There can be various backend implementations 
+like RDBMS, NoSQL databases, etc. Support for some comes out of the box:
+
+##### MongoDB Storage 
+
+```python
+from nameko_kafka import consume, Semantic
+from nameko_kafka.storage import MongoStorage
+
+from pymongo import MongoClient
+
+
+class MyService:
+    """
+        My microservice 
+    """
+    name = "my-service"
+    
+    # At most once semantic consumer
+    @consume(
+        "kafka-topic", 
+        group_id="my-group", 
+        bootstrap_servers='localhost:1234', 
+        semantic=Semantic.EXACTLY_ONCE,
+        storage=MongoStorage(
+            # MongoDB backend client
+            client=MongoClient('localhost', 27017),
+            # Database to use for storage
+            db_name="database-name",
+            # Collection to use for storage
+            collection="collection-name"
+        )       
+    )
+    def method(self, message):
+        # Your message handler
+        handle_message(message) 
+```
+
+Note: If the `db_name` and `collection` arguments are not specified, the default value of `"nameko_kafka_offsets"` and 
+`"offsets"` will be used by the storage respectively.
+
+##### SQL Storage
+
+Part of v0.3.0
+
+##### S3 Storage
+
+Part of v0.4.0
+
+##### Azure Block Storage
+
+Part of v0.5.0
+
+##### Create Custom Storage
+
+You can create your own offset storage by implementing the `OffsetStorage` interface. It exposes the following methods:
+
+```python
+from nameko_kafka.storage.base import OffsetStorage
+
+class MyStorage(OffsetStorage):
+    """
+        My custom offset storage.
+    """
+
+    def setup(self):
+        """
+            Method for setup of the storage.
+        """
+
+    def stop(self):
+        """
+            Method to teardown the storage.
+        """
+
+    def read(self, topic, partition):
+        """
+            Read last stored offset from storage for 
+            given topic and partition.
+
+            :param topic: message topic
+            :param partition: partition number of the topic
+            :returns: last committed offset value
+        """
+
+    def write(self, offsets):
+        """
+            Write offsets to storage.
+
+            :param offsets: mapping between topic-partition
+                tuples and corresponding latest offset value, 
+                e.g.
+                {
+                    ("topic-1", 0): 1,
+                    ("topic-1", 1): 3,
+                    ("topic-2", 1): 10,
+                    ...
+                }
+        """
+```
+
+
+## Configurations
+
+The extension configurations can be set in a nameko [config.yaml]((https://docs.nameko.io/en/stable/cli.html)) file, or 
+by environment variables.
+
+### Config File
+
+```yaml
+# Config for entrypoint
+KAFKA_CONSUMER:
+  bootstrap_servers: 'localhost:1234'
+  retry_backoff_ms: 100
+  ...
+
+# Config for dependency
+KAFKA_PRODUCER:
+  bootstrap_servers: 'localhost:1234'
+  retries: 3
+  ...
+```
+
+### Environment Variables
+
+```.env
+# Config for entrypoint
+KAFKA_CONSUMER='{"bootstrap_servers": "localhost:1234", "retry_backoff_ms": 100}'
+
+# Config for dependency
+KAFKA_PRODUCER='{"bootstrap_servers": "localhost:1234", "retries": 3}'
+```
+
+## Milestones
+
+- [x] Kafka Entrypoint
+- [x] Kafka Dependency
+- [x] Commit strategies: 
+    - _ALMOST_ONCE_DELIVERY_
+    - _AT_LEAST_ONCE_DELIVERY_ 
+    - _EXACTLY_ONCE_DELIVERY_
+- [x] Commit storage for _EXACT_ONCE_DELIVERY_ strategy
+
+## Developers
+
+For development a kafka broker is required. You can spawn one using the [docker-compose.yml](https://github.com/ketgo/nameko-kafka/blob/master/tests/conftest.py) 
+file in the `tests` folder:
+```bash
+$ cd tests
+$ docker-compose up -d 
+```
+
+To install all package dependencies:
+```bash
+$ pip install -r .[dev]
+or
+$ make deps
+```
+
+Other useful commands:
+```bash
+$ pytest --cov=nameko_kafka tests/			# to get coverage report
+or
+$ make coverage
+
+$ pylint nameko_kafka       # to check code quality with PyLint
+or
+$ make lint
+```
+
+## Contributions
+
+Issue reports and Pull requests are always welcomed. Thanks!
```

### Comparing `nameko_kafka-0.2.0/README.md` & `nameko_kafka-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -158,23 +158,23 @@
 ```
 
 Note: If the `db_name` and `collection` arguments are not specified, the default value of `"nameko_kafka_offsets"` and 
 `"offsets"` will be used by the storage respectively.
 
 ##### SQL Storage
 
-Part of v0.2.1
+Part of v0.3.0
 
 ##### S3 Storage
 
-Part of v0.2.2
+Part of v0.4.0
 
 ##### Azure Block Storage
 
-Part of v0.2.3
+Part of v0.5.0
 
 ##### Create Custom Storage
 
 You can create your own offset storage by implementing the `OffsetStorage` interface. It exposes the following methods:
 
 ```python
 from nameko_kafka.storage.base import OffsetStorage
```

### Comparing `nameko_kafka-0.2.0/nameko_kafka/consumers/default.py` & `nameko_kafka-0.2.1/nameko_kafka/consumers/default.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/nameko_kafka/consumers/exactly_once.py` & `nameko_kafka-0.2.1/nameko_kafka/consumers/exactly_once.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/nameko_kafka/consumers/least_once.py` & `nameko_kafka-0.2.1/nameko_kafka/consumers/least_once.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/nameko_kafka/consumers/most_once.py` & `nameko_kafka-0.2.1/nameko_kafka/consumers/most_once.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/nameko_kafka/dependency.py` & `nameko_kafka-0.2.1/nameko_kafka/dependency.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/nameko_kafka/entrypoint.py` & `nameko_kafka-0.2.1/nameko_kafka/entrypoint.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/nameko_kafka/storage/base.py` & `nameko_kafka-0.2.1/nameko_kafka/storage/base.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/nameko_kafka/storage/mongo.py` & `nameko_kafka-0.2.1/nameko_kafka/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/nameko_kafka.egg-info/PKG-INFO` & `nameko_kafka-0.2.1/nameko_kafka.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,312 +1,16 @@
 Metadata-Version: 2.1
 Name: nameko-kafka
-Version: 0.2.0
+Version: 0.2.1
 Summary: Kafka extension for Nameko microservice framework
 Home-page: https://github.com/ketgo/nameko-kafka
 Author: Ketan Goyal
 Author-email: ketangoyal1988@gmail.com
 License: MIT
-Description: # Nameko-Kafka
-        
-        [![Build Status](https://travis-ci.com/ketgo/nameko-kafka.svg?branch=master)](https://travis-ci.com/ketgo/nameko-kafka)
-        [![codecov.io](https://codecov.io/gh/ketgo/nameko-kafka/coverage.svg?branch=master)](https://codecov.io/gh/ketgo/nameko-kafka/coverage.svg?branch=master)
-        [![MIT licensed](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
-        ---
-        
-        Kafka extension for [Nameko](https://www.nameko.io/) microservice framework. 
-        
-        ## Introduction
-        
-        This is a Nameko microservice framework [extension](https://nameko.readthedocs.io/en/stable/key_concepts.html) to support 
-        Kafka entrypoint and dependency. The motivation behind the project is issue [569](https://github.com/nameko/nameko/issues/569). 
-        _Nameko-kafka_ provide a simple implementation of the entrypoint based on the approach by [calumpeterwebb](https://medium.com/@calumpeterwebb/nameko-tutorial-creating-a-kafka-consuming-microservice-c4a7adb804d0).
-        It also includes a dependency provider for publishing Kafka messages from within a Nameko service.
-        
-        ## Installation
-        
-        The package is supports Python >= 3.5
-        ```bash
-        $ pip install nameko-kafka
-        ```
-        
-        ## Usage
-        
-        The extension can be used for both, a service dependency and entrypoint. Example usage for both cases are shown in the
-        following sections.
-        
-        ## Dependency
-        
-        This is basically a [python-kafka](https://github.com/dpkp/kafka-python) producer in the form of Nameko dependency. 
-        Nameko uses dependency injection to instantiate the producer. You just need to declare it in your service class as shown:
-        
-        ```python
-        from nameko.rpc import rpc
-        from nameko_kafka import KafkaProducer
-        
-        
-        class MyService:
-            """
-                My microservice
-            """
-            name = "my-service"
-            # Kafak dependency
-            producer = KafkaProducer(bootstrap_servers='localhost:1234')
-            
-            @rpc
-            def method(self):
-                # Publish message using dependency
-                self.producer.send("kafka-topic", value=b"my-message", key=b"my-key")
-        ```
-        
-        Here `KafkaProducer` accepts all options valid for `python-kafka`'s [KafkaProducer](https://kafka-python.readthedocs.io/en/master/apidoc/KafkaProducer.html).
-        
-        ### Entrypoint
-        
-        You can use the `nameko_kafka.consume` decorator in your services to process Kafka messages:
-        
-        ```python
-        from nameko_kafka import consume
-        
-        
-        class MyService:
-            """
-                My microservice 
-            """
-            name = "my-service"
-        
-            @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234')
-            def method(self, message):
-                # Your message handler
-                handle_message(message) 
-        ```
-        
-        The `consume` decorator accepts all the options valid for `python-kafka`'s [KafkaConsumer](https://kafka-python.readthedocs.io/en/master/apidoc/KafkaConsumer.html). 
-        
-        On top of the default `python-kafka`'s autocommit feature, the entrypoint also comes with support for three different 
-        types of offset commit strategies: _at least once_, _at most once_ and _exactly once_. The three strategies correspond 
-        to the different message delivery semantics achievable in Kafka. Examples for each are shown in the following subsections.
-        
-        #### At Least Once
-        
-        ```python
-        from nameko_kafka import consume, Semantic
-        
-        
-        class MyService:
-            """
-                My microservice 
-            """
-            name = "my-service"
-            
-            # At least once semantic consumer
-            @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234', semantic=Semantic.AT_LEAST_ONCE)
-            def method(self, message):
-                # Your message handler
-                handle_message(message) 
-        ```
-        
-        #### At Most Once
-        
-        ```python
-        from nameko_kafka import consume, Semantic
-        
-        
-        class MyService:
-            """
-                My microservice 
-            """
-            name = "my-service"
-            
-            # At most once semantic consumer
-            @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234', semantic=Semantic.AT_MOST_ONCE)
-            def method(self, message):
-                # Your message handler
-                handle_message(message) 
-        ```
-        
-        #### Exactly Once
-        
-        The exactly once semantic requires a persistent storage to save message offsets. Such a persistent store can be 
-        implemented using the `OffsetStorage` interface provided by Nameko-kafka. There can be various backend implementations 
-        like RDBMS, NoSQL databases, etc. Support for some comes out of the box:
-        
-        ##### MongoDB Storage 
-        
-        ```python
-        from nameko_kafka import consume, Semantic
-        from nameko_kafka.storage import MongoStorage
-        
-        from pymongo import MongoClient
-        
-        
-        class MyService:
-            """
-                My microservice 
-            """
-            name = "my-service"
-            
-            # At most once semantic consumer
-            @consume(
-                "kafka-topic", 
-                group_id="my-group", 
-                bootstrap_servers='localhost:1234', 
-                semantic=Semantic.EXACTLY_ONCE,
-                storage=MongoStorage(
-                    # MongoDB backend client
-                    client=MongoClient('localhost', 27017),
-                    # Database to use for storage
-                    db_name="database-name",
-                    # Collection to use for storage
-                    collection="collection-name"
-                )       
-            )
-            def method(self, message):
-                # Your message handler
-                handle_message(message) 
-        ```
-        
-        Note: If the `db_name` and `collection` arguments are not specified, the default value of `"nameko_kafka_offsets"` and 
-        `"offsets"` will be used by the storage respectively.
-        
-        ##### SQL Storage
-        
-        Part of v0.2.1
-        
-        ##### S3 Storage
-        
-        Part of v0.2.2
-        
-        ##### Azure Block Storage
-        
-        Part of v0.2.3
-        
-        ##### Create Custom Storage
-        
-        You can create your own offset storage by implementing the `OffsetStorage` interface. It exposes the following methods:
-        
-        ```python
-        from nameko_kafka.storage.base import OffsetStorage
-        
-        class MyStorage(OffsetStorage):
-            """
-                My custom offset storage.
-            """
-        
-            def setup(self):
-                """
-                    Method for setup of the storage.
-                """
-        
-            def stop(self):
-                """
-                    Method to teardown the storage.
-                """
-        
-            def read(self, topic, partition):
-                """
-                    Read last stored offset from storage for 
-                    given topic and partition.
-        
-                    :param topic: message topic
-                    :param partition: partition number of the topic
-                    :returns: last committed offset value
-                """
-        
-            def write(self, offsets):
-                """
-                    Write offsets to storage.
-        
-                    :param offsets: mapping between topic-partition
-                        tuples and corresponding latest offset value, 
-                        e.g.
-                        {
-                            ("topic-1", 0): 1,
-                            ("topic-1", 1): 3,
-                            ("topic-2", 1): 10,
-                            ...
-                        }
-                """
-        ```
-        
-        
-        ## Configurations
-        
-        The extension configurations can be set in a nameko [config.yaml]((https://docs.nameko.io/en/stable/cli.html)) file, or 
-        by environment variables.
-        
-        ### Config File
-        
-        ```yaml
-        # Config for entrypoint
-        KAFKA_CONSUMER:
-          bootstrap_servers: 'localhost:1234'
-          retry_backoff_ms: 100
-          ...
-        
-        # Config for dependency
-        KAFKA_PRODUCER:
-          bootstrap_servers: 'localhost:1234'
-          retries: 3
-          ...
-        ```
-        
-        ### Environment Variables
-        
-        ```.env
-        # Config for entrypoint
-        KAFKA_CONSUMER='{"bootstrap_servers": "localhost:1234", "retry_backoff_ms": 100}'
-        
-        # Config for dependency
-        KAFKA_PRODUCER='{"bootstrap_servers": "localhost:1234", "retries": 3}'
-        ```
-        
-        ## Milestones
-        
-        - [x] Kafka Entrypoint
-        - [x] Kafka Dependency
-        - [x] Commit strategies: 
-            - _ALMOST_ONCE_DELIVERY_
-            - _AT_LEAST_ONCE_DELIVERY_ 
-            - _EXACTLY_ONCE_DELIVERY_
-        - [x] Commit storage for _EXACT_ONCE_DELIVERY_ strategy
-        
-        ## Developers
-        
-        For development a kafka broker is required. You can spawn one using the [docker-compose.yml](https://github.com/ketgo/nameko-kafka/blob/master/tests/conftest.py) 
-        file in the `tests` folder:
-        ```bash
-        $ cd tests
-        $ docker-compose up -d 
-        ```
-        
-        To install all package dependencies:
-        ```bash
-        $ pip install -r .[dev]
-        or
-        $ make deps
-        ```
-        
-        Other useful commands:
-        ```bash
-        $ pytest --cov=nameko_kafka tests/			# to get coverage report
-        or
-        $ make coverage
-        
-        $ pylint nameko_kafka       # to check code quality with PyLint
-        or
-        $ make lint
-        ```
-        
-        ## Contributions
-        
-        Issue reports and Pull requests are always welcomed. Thanks!
-        
 Keywords: nameko,kafka,microservice
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
@@ -314,7 +18,303 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: mongo
 Provides-Extra: sql
+License-File: LICENSE
+
+# Nameko-Kafka
+
+[![Build Status](https://travis-ci.com/ketgo/nameko-kafka.svg?branch=master)](https://travis-ci.com/ketgo/nameko-kafka)
+[![codecov.io](https://codecov.io/gh/ketgo/nameko-kafka/coverage.svg?branch=master)](https://codecov.io/gh/ketgo/nameko-kafka/coverage.svg?branch=master)
+[![MIT licensed](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
+---
+
+Kafka extension for [Nameko](https://www.nameko.io/) microservice framework. 
+
+## Introduction
+
+This is a Nameko microservice framework [extension](https://nameko.readthedocs.io/en/stable/key_concepts.html) to support 
+Kafka entrypoint and dependency. The motivation behind the project is issue [569](https://github.com/nameko/nameko/issues/569). 
+_Nameko-kafka_ provide a simple implementation of the entrypoint based on the approach by [calumpeterwebb](https://medium.com/@calumpeterwebb/nameko-tutorial-creating-a-kafka-consuming-microservice-c4a7adb804d0).
+It also includes a dependency provider for publishing Kafka messages from within a Nameko service.
+
+## Installation
+
+The package is supports Python >= 3.5
+```bash
+$ pip install nameko-kafka
+```
+
+## Usage
+
+The extension can be used for both, a service dependency and entrypoint. Example usage for both cases are shown in the
+following sections.
+
+## Dependency
+
+This is basically a [python-kafka](https://github.com/dpkp/kafka-python) producer in the form of Nameko dependency. 
+Nameko uses dependency injection to instantiate the producer. You just need to declare it in your service class as shown:
+
+```python
+from nameko.rpc import rpc
+from nameko_kafka import KafkaProducer
+
+
+class MyService:
+    """
+        My microservice
+    """
+    name = "my-service"
+    # Kafak dependency
+    producer = KafkaProducer(bootstrap_servers='localhost:1234')
+    
+    @rpc
+    def method(self):
+        # Publish message using dependency
+        self.producer.send("kafka-topic", value=b"my-message", key=b"my-key")
+```
+
+Here `KafkaProducer` accepts all options valid for `python-kafka`'s [KafkaProducer](https://kafka-python.readthedocs.io/en/master/apidoc/KafkaProducer.html).
+
+### Entrypoint
+
+You can use the `nameko_kafka.consume` decorator in your services to process Kafka messages:
+
+```python
+from nameko_kafka import consume
+
+
+class MyService:
+    """
+        My microservice 
+    """
+    name = "my-service"
+
+    @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234')
+    def method(self, message):
+        # Your message handler
+        handle_message(message) 
+```
+
+The `consume` decorator accepts all the options valid for `python-kafka`'s [KafkaConsumer](https://kafka-python.readthedocs.io/en/master/apidoc/KafkaConsumer.html). 
+
+On top of the default `python-kafka`'s autocommit feature, the entrypoint also comes with support for three different 
+types of offset commit strategies: _at least once_, _at most once_ and _exactly once_. The three strategies correspond 
+to the different message delivery semantics achievable in Kafka. Examples for each are shown in the following subsections.
+
+#### At Least Once
+
+```python
+from nameko_kafka import consume, Semantic
+
+
+class MyService:
+    """
+        My microservice 
+    """
+    name = "my-service"
+    
+    # At least once semantic consumer
+    @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234', semantic=Semantic.AT_LEAST_ONCE)
+    def method(self, message):
+        # Your message handler
+        handle_message(message) 
+```
+
+#### At Most Once
+
+```python
+from nameko_kafka import consume, Semantic
+
+
+class MyService:
+    """
+        My microservice 
+    """
+    name = "my-service"
+    
+    # At most once semantic consumer
+    @consume("kafka-topic", group_id="my-group", bootstrap_servers='localhost:1234', semantic=Semantic.AT_MOST_ONCE)
+    def method(self, message):
+        # Your message handler
+        handle_message(message) 
+```
+
+#### Exactly Once
+
+The exactly once semantic requires a persistent storage to save message offsets. Such a persistent store can be 
+implemented using the `OffsetStorage` interface provided by Nameko-kafka. There can be various backend implementations 
+like RDBMS, NoSQL databases, etc. Support for some comes out of the box:
+
+##### MongoDB Storage 
+
+```python
+from nameko_kafka import consume, Semantic
+from nameko_kafka.storage import MongoStorage
+
+from pymongo import MongoClient
+
+
+class MyService:
+    """
+        My microservice 
+    """
+    name = "my-service"
+    
+    # At most once semantic consumer
+    @consume(
+        "kafka-topic", 
+        group_id="my-group", 
+        bootstrap_servers='localhost:1234', 
+        semantic=Semantic.EXACTLY_ONCE,
+        storage=MongoStorage(
+            # MongoDB backend client
+            client=MongoClient('localhost', 27017),
+            # Database to use for storage
+            db_name="database-name",
+            # Collection to use for storage
+            collection="collection-name"
+        )       
+    )
+    def method(self, message):
+        # Your message handler
+        handle_message(message) 
+```
+
+Note: If the `db_name` and `collection` arguments are not specified, the default value of `"nameko_kafka_offsets"` and 
+`"offsets"` will be used by the storage respectively.
+
+##### SQL Storage
+
+Part of v0.3.0
+
+##### S3 Storage
+
+Part of v0.4.0
+
+##### Azure Block Storage
+
+Part of v0.5.0
+
+##### Create Custom Storage
+
+You can create your own offset storage by implementing the `OffsetStorage` interface. It exposes the following methods:
+
+```python
+from nameko_kafka.storage.base import OffsetStorage
+
+class MyStorage(OffsetStorage):
+    """
+        My custom offset storage.
+    """
+
+    def setup(self):
+        """
+            Method for setup of the storage.
+        """
+
+    def stop(self):
+        """
+            Method to teardown the storage.
+        """
+
+    def read(self, topic, partition):
+        """
+            Read last stored offset from storage for 
+            given topic and partition.
+
+            :param topic: message topic
+            :param partition: partition number of the topic
+            :returns: last committed offset value
+        """
+
+    def write(self, offsets):
+        """
+            Write offsets to storage.
+
+            :param offsets: mapping between topic-partition
+                tuples and corresponding latest offset value, 
+                e.g.
+                {
+                    ("topic-1", 0): 1,
+                    ("topic-1", 1): 3,
+                    ("topic-2", 1): 10,
+                    ...
+                }
+        """
+```
+
+
+## Configurations
+
+The extension configurations can be set in a nameko [config.yaml]((https://docs.nameko.io/en/stable/cli.html)) file, or 
+by environment variables.
+
+### Config File
+
+```yaml
+# Config for entrypoint
+KAFKA_CONSUMER:
+  bootstrap_servers: 'localhost:1234'
+  retry_backoff_ms: 100
+  ...
+
+# Config for dependency
+KAFKA_PRODUCER:
+  bootstrap_servers: 'localhost:1234'
+  retries: 3
+  ...
+```
+
+### Environment Variables
+
+```.env
+# Config for entrypoint
+KAFKA_CONSUMER='{"bootstrap_servers": "localhost:1234", "retry_backoff_ms": 100}'
+
+# Config for dependency
+KAFKA_PRODUCER='{"bootstrap_servers": "localhost:1234", "retries": 3}'
+```
+
+## Milestones
+
+- [x] Kafka Entrypoint
+- [x] Kafka Dependency
+- [x] Commit strategies: 
+    - _ALMOST_ONCE_DELIVERY_
+    - _AT_LEAST_ONCE_DELIVERY_ 
+    - _EXACTLY_ONCE_DELIVERY_
+- [x] Commit storage for _EXACT_ONCE_DELIVERY_ strategy
+
+## Developers
+
+For development a kafka broker is required. You can spawn one using the [docker-compose.yml](https://github.com/ketgo/nameko-kafka/blob/master/tests/conftest.py) 
+file in the `tests` folder:
+```bash
+$ cd tests
+$ docker-compose up -d 
+```
+
+To install all package dependencies:
+```bash
+$ pip install -r .[dev]
+or
+$ make deps
+```
+
+Other useful commands:
+```bash
+$ pytest --cov=nameko_kafka tests/			# to get coverage report
+or
+$ make coverage
+
+$ pylint nameko_kafka       # to check code quality with PyLint
+or
+$ make lint
+```
+
+## Contributions
+
+Issue reports and Pull requests are always welcomed. Thanks!
```

### Comparing `nameko_kafka-0.2.0/nameko_kafka.egg-info/SOURCES.txt` & `nameko_kafka-0.2.1/nameko_kafka.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 nameko_kafka/__init__.py
 nameko_kafka/constants.py
 nameko_kafka/dependency.py
 nameko_kafka/entrypoint.py
 nameko_kafka/version.py
@@ -14,15 +15,17 @@
 nameko_kafka/consumers/default.py
 nameko_kafka/consumers/exactly_once.py
 nameko_kafka/consumers/least_once.py
 nameko_kafka/consumers/most_once.py
 nameko_kafka/storage/__init__.py
 nameko_kafka/storage/base.py
 nameko_kafka/storage/mongo.py
-tests/storage/__init__.py
-tests/storage/test_base.py
-tests/storage/test_mongo.py
+tests/test_dependency.py
+tests/test_entrypoint.py
 tests/test_consumers/__init__.py
 tests/test_consumers/test_default.py
 tests/test_consumers/test_exactly_once.py
 tests/test_consumers/test_least_once.py
-tests/test_consumers/test_most_once.py
+tests/test_consumers/test_most_once.py
+tests/test_storage/__init__.py
+tests/test_storage/test_base.py
+tests/test_storage/test_mongo.py
```

### Comparing `nameko_kafka-0.2.0/setup.py` & `nameko_kafka-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 extra_requires_sql = [
     'SQLAlchemy~=1.3'
 ]
 extra_requires_utils = [
     'pytest~=5.0',
     'pytest-cov~=2.0',
     'pytest-mock~=3.0',
+    'pytest-eventlet~=1.0.0',
     'pylint~=2.0',
     'bandit~=1.6',
     'PyMySQL~=0.9',
     'psycopg2cffi~=2.7'
 ]
 extra_requires_dev = extra_requires_utils + \
                      extra_requires_mongo + \
@@ -41,17 +42,16 @@
         url='https://github.com/ketgo/nameko-kafka',
         long_description=long_description,
         long_description_content_type='text/markdown',
         py_modules=['nameko_kafka'],
         package_dir={'nameko_kafka': 'nameko_kafka'},
         python_requires='>=3.4',
         install_requires=[
-            'nameko',
-            'kafka-python',
-            'wrapt==1.11'  # Fixed version: needed by kafka-python
+            'nameko~=2.14',
+            'kafka-python~=2.0.2',
         ],
         extras_require={
             'dev': extra_requires_dev,
             'mongo': extra_requires_mongo,
             'sql': extra_requires_sql,
         },
         packages=find_packages(exclude=('tests',)),
```

### Comparing `nameko_kafka-0.2.0/tests/storage/test_base.py` & `nameko_kafka-0.2.1/tests/test_storage/test_base.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/tests/storage/test_mongo.py` & `nameko_kafka-0.2.1/tests/test_storage/test_mongo.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 import pytest
 from pymongo import MongoClient
 
 from nameko_kafka.storage.mongo import MongoStorage, DEFAULT_DB_NAME, DEFAULT_COLLECTION_NAME
 
-DEFAULT_MONGODB_HOST = "127.0.0.1:27017"
+DEFAULT_MONGODB_HOST = "mongodb://mongo:password@127.0.0.1:27017"
 DB_NAME = 'nameko_kafka_test'
 COLLECTION = 'offsets_test'
 
 
 def create_client() -> MongoClient:
     host = os.getenv("MONGODB_HOST", DEFAULT_MONGODB_HOST)
     return MongoClient(host)
```

### Comparing `nameko_kafka-0.2.0/tests/test_consumers/test_default.py` & `nameko_kafka-0.2.1/tests/test_consumers/test_default.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/tests/test_consumers/test_exactly_once.py` & `nameko_kafka-0.2.1/tests/test_consumers/test_exactly_once.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/tests/test_consumers/test_least_once.py` & `nameko_kafka-0.2.1/tests/test_consumers/test_least_once.py`

 * *Files identical despite different names*

### Comparing `nameko_kafka-0.2.0/tests/test_consumers/test_most_once.py` & `nameko_kafka-0.2.1/tests/test_consumers/test_most_once.py`

 * *Files identical despite different names*

