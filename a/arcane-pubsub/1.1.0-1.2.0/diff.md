# Comparing `tmp/arcane-pubsub-1.1.0.tar.gz` & `tmp/arcane_pubsub-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcane-pubsub-1.1.0.tar", max compression
+gzip compressed data, was "arcane_pubsub-1.2.0.tar", max compression
```

## Comparing `arcane-pubsub-1.1.0.tar` & `arcane_pubsub-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      377 2022-03-10 10:28:23.323617 arcane-pubsub-1.1.0/README.md
--rw-r--r--   0        0        0       43 2022-03-10 10:28:23.323617 arcane-pubsub-1.1.0/arcane/pubsub/__init__.py
--rw-r--r--   0        0        0     2514 2022-03-10 10:28:23.323617 arcane-pubsub-1.1.0/arcane/pubsub/client.py
--rw-r--r--   0        0        0     1094 2022-03-10 10:28:23.323617 arcane-pubsub-1.1.0/arcane/pubsub/utils.py
--rw-r--r--   0        0        0      443 2022-03-10 10:28:23.323617 arcane-pubsub-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1096 2022-03-10 10:28:55.047575 arcane-pubsub-1.1.0/setup.py
--rw-r--r--   0        0        0     1025 2022-03-10 10:28:55.047917 arcane-pubsub-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      576 2023-07-12 14:35:46.835047 arcane_pubsub-1.2.0/README.md
+-rw-r--r--   0        0        0       43 2023-07-12 14:35:46.835047 arcane_pubsub-1.2.0/arcane/pubsub/__init__.py
+-rw-r--r--   0        0        0     4355 2023-07-12 14:35:46.835047 arcane_pubsub-1.2.0/arcane/pubsub/client.py
+-rw-r--r--   0        0        0     1094 2023-07-12 14:35:46.835047 arcane_pubsub-1.2.0/arcane/pubsub/utils.py
+-rw-r--r--   0        0        0      460 2023-07-12 14:35:46.835047 arcane_pubsub-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 arcane_pubsub-1.2.0/PKG-INFO
```

### Comparing `arcane-pubsub-1.1.0/arcane/pubsub/utils.py` & `arcane_pubsub-1.2.0/arcane/pubsub/utils.py`

 * *Files identical despite different names*

### Comparing `arcane-pubsub-1.1.0/PKG-INFO` & `arcane_pubsub-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: arcane-pubsub
-Version: 1.1.0
+Version: 1.2.0
 Summary: Override pubsub client
 Author: Arcane
 Author-email: product@arcane.run
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arcane-firebase (>=0.2.0,<0.3.0)
+Requires-Dist: avro (>=1.11.2,<2.0.0)
 Requires-Dist: google-cloud-pubsub (>=2.11.0,<3.0.0)
 Requires-Dist: typing-extensions (>=3.7)
 Description-Content-Type: text/markdown
 
 # Arcane PubSub
 
 This package is base on [google-cloud-pubsub](https://pypi.org/project/google-cloud-pubsub/).
@@ -35,7 +37,18 @@
 from configure import Config
 
 client = pubsub.Client(Config.KEY)
 
 client.push_to_topic('project', 'topic', {"parameter": "value"})
 ```
 
+Publish with a new schema
+
+```python
+result = pubsub_client.publish_with_schema(
+    project='my-project',
+    topic_name='my-topic-with-schema',
+    message=message,
+    await_response=True,
+)
+
+```
```

