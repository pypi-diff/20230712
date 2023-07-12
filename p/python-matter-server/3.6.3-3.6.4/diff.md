# Comparing `tmp/python-matter-server-3.6.3.tar.gz` & `tmp/python-matter-server-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.6.3.tar", last modified: Thu Jun 29 08:56:13 2023, max compression
+gzip compressed data, was "python-matter-server-3.6.4.tar", last modified: Wed Jul 12 18:46:49 2023, max compression
```

## Comparing `python-matter-server-3.6.3.tar` & `python-matter-server-3.6.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    36859 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-29 08:55:47.000000 python-matter-server-3.6.3/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-29 08:56:00.000000 python-matter-server-3.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-06-29 08:56:12.000000 python-matter-server-3.6.3/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-29 08:56:13.000000 python-matter-server-3.6.3/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:56:12.000000 python-matter-server-3.6.3/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 08:56:13.000000 python-matter-server-3.6.3/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:56:11.000000 python-matter-server-3.6.3/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 08:56:13.000000 python-matter-server-3.6.3/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 08:56:13.000000 python-matter-server-3.6.3/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 08:56:13.442350 python-matter-server-3.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.969142 python-matter-server-3.6.4/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.969142 python-matter-server-3.6.4/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19354 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.969142 python-matter-server-3.6.4/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.969142 python-matter-server-3.6.4/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.969142 python-matter-server-3.6.4/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37306 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-12 18:46:34.000000 python-matter-server-3.6.4/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-12 18:46:38.000000 python-matter-server-3.6.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:46:47.000000 python-matter-server-3.6.4/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-12 18:46:49.000000 python-matter-server-3.6.4/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 18:46:49.973142 python-matter-server-3.6.4/setup.cfg
```

### Comparing `python-matter-server-3.6.3/LICENSE` & `python-matter-server-3.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/PKG-INFO` & `python-matter-server-3.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.6.3
+Version: 3.6.4
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.6.3/README.md` & `python-matter-server-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/client/client.py` & `python-matter-server-3.6.4/matter_server/client/client.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/client/connection.py` & `python-matter-server-3.6.4/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/client/exceptions.py` & `python-matter-server-3.6.4/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/client/models/device_types.py` & `python-matter-server-3.6.4/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/client/models/node.py` & `python-matter-server-3.6.4/matter_server/client/models/node.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/common/errors.py` & `python-matter-server-3.6.4/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/common/helpers/api.py` & `python-matter-server-3.6.4/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/common/helpers/json.py` & `python-matter-server-3.6.4/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/common/helpers/util.py` & `python-matter-server-3.6.4/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/common/models.py` & `python-matter-server-3.6.4/matter_server/common/models.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/server/__main__.py` & `python-matter-server-3.6.4/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/server/client_handler.py` & `python-matter-server-3.6.4/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/server/const.py` & `python-matter-server-3.6.4/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/server/device_controller.py` & `python-matter-server-3.6.4/matter_server/server/device_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 _T = TypeVar("_T")
 
 DATA_KEY_NODES = "nodes"
 DATA_KEY_LAST_NODE_ID = "last_node_id"
 
 LOGGER = logging.getLogger(__name__)
 INTERVIEW_TASK_LIMIT = 5
+MAX_POLL_INTERVAL = 600
 
 # a list of attributes we should always watch on all nodes
 DEFAULT_SUBSCRIBE_ATTRIBUTES: set[tuple[int | str, int | str, int | str]] = {
     ("*", 0x001D, 0x00000000),  # all endpoints, descriptor cluster, deviceTypeList
     ("*", 0x001D, 0x00000003),  # all endpoints, descriptor cluster, partsList
     (0, 0x0028, "*"),  # endpoint 0, BasicInformation cluster, all attributes
     ("*", 0x0039, "*"),  # BridgedDeviceBasicInformation
@@ -80,14 +81,15 @@
         self._nodes: dict[int, MatterNodeData | None] = {}
         self.wifi_credentials_set: bool = False
         self.thread_credentials_set: bool = False
         self.compressed_fabric_id: int | None = None
         self._interview_limit: asyncio.Semaphore = asyncio.Semaphore(
             INTERVIEW_TASK_LIMIT
         )
+        self._resolve_lock: asyncio.Lock = asyncio.Lock()
         self._node_lock: dict[int, asyncio.Lock] = {}
 
     async def initialize(self) -> None:
         """Async initialize of controller."""
         # (re)fetch all PAA certificates once at startup
         # NOTE: this must be done before initializing the controller
         await fetch_certificates()
@@ -579,17 +581,17 @@
                 # the current subscription already matches, no need to re-setup
                 node_logger.debug("Re-using existing subscription.")
                 return
             async with node_lock:
                 node_logger.debug("Unsubscribing from existing subscription.")
                 await self._call_sdk(prev_sub.Shutdown)
 
-        node_logger.debug("Setting up attributes and events subscription.")
         self._attr_subscriptions[node_id] = attr_subscriptions
         async with node_lock:
+            node_logger.debug("Setting up attributes and events subscription.")
             sub: Attribute.SubscriptionTransaction = await self.chip_controller.Read(
                 nodeid=node_id,
                 # In order to prevent network congestion due to wildcard subscriptions on all nodes,
                 # we keep a list of attributes we are explicitly interested in.
                 attributes=attr_subscriptions,
                 # simply subscribe to all (urgent and non urgent) device events
                 events=[("*", 1), ("*", 0)],
@@ -693,14 +695,26 @@
                 terminationError,
                 nextResubscribeIntervalMsec,
             )
             # mark node as unavailable and signal consumers
             if node.available:
                 node.available = False
                 self.server.signal_event(EventType.NODE_UPDATED, node)
+            if nextResubscribeIntervalMsec / 1000 > MAX_POLL_INTERVAL:
+                # workaround to handle devices that are unplugged
+                # from power for a longer period of time
+                # cancel subscription and add this node to our node polling job
+                # TODO: fix this once OerationalNodeDiscovery is available:
+                # https://github.com/project-chip/connectedhomeip/pull/26718
+                sub.Shutdown()
+                self._subscriptions.pop(node_id)
+                assert self.server.loop
+                self.server.loop.create_task(
+                    self._check_interview_and_subscription(node_id, MAX_POLL_INTERVAL)
+                )
 
         def resubscription_succeeded(
             transaction: Attribute.SubscriptionTransaction,
         ) -> None:
             # pylint: disable=unused-argument, invalid-name
             node_logger.info("Re-Subscription succeeded")
             # mark node as available and signal consumers
@@ -740,28 +754,29 @@
             await self.server.loop.run_in_executor(
                 None,
                 partial(func, *args, **kwargs),
             ),
         )
 
     async def _check_interview_and_subscription(
-        self, node_id: int, reschedule_interval: int = 300
+        self, node_id: int, reschedule_interval: int = 30
     ) -> None:
         """Handle interview (if needed) and subscription for known node."""
 
         def reschedule() -> None:
             """(Re)Schedule interview and/or initial subscription for a node."""
             assert self.server.loop is not None
             self.server.loop.call_later(
                 reschedule_interval,
                 asyncio.create_task,
                 self._check_interview_and_subscription(
                     node_id,
-                    # increase interval at each attempt with maximum of 1 hour
-                    min(reschedule_interval + 300, 3600),
+                    # increase interval at each attempt with maximum of
+                    # MAX_POLL_INTERVAL seconds (= 10 minutes)
+                    min(reschedule_interval + 10, MAX_POLL_INTERVAL),
                 ),
             )
 
         # (re)interview node (only) if needed
         node_data = self._nodes.get(node_id)
         if (
             node_data is None
@@ -789,14 +804,16 @@
             await self._subscribe_node(node_id)
         except NodeNotResolving:
             LOGGER.warning(
                 "Unable to subscribe to Node %s as it is unavailable, "
                 "will retry later in the background.",
                 node_id,
             )
+            # TODO: fix this once OperationalNodeDiscovery is available:
+            # https://github.com/project-chip/connectedhomeip/pull/26718
             reschedule()
 
     @staticmethod
     def _parse_attributes_from_read_result(
         read_result: dict[int, dict[Type, dict[Type, Any]]]
     ) -> dict[str, Any]:
         """Parse attributes from ReadResult."""
@@ -833,45 +850,31 @@
                             attribute_path,
                             err,
                         )
                         continue
                     result[attribute_path] = attr_value
         return result
 
-    async def _resolve_node(
-        self, node_id: int, retries: int = 3, allow_pase: bool = False
-    ) -> None:
+    async def _resolve_node(self, node_id: int, retries: int = 3) -> None:
         """Resolve a Node on the network."""
         node_lock = self._get_node_lock(node_id)
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
         try:
-            if allow_pase:
-                # last attempt allows PASE connection (last resort)
-                LOGGER.debug(
-                    "Attempting to resolve node %s (with PASE connection)", node_id
+            async with node_lock, self._resolve_lock:
+                LOGGER.debug("Attempting to resolve node %s...", node_id)
+                await self._call_sdk(
+                    self.chip_controller.ResolveNode,
+                    nodeid=node_id,
                 )
-                async with node_lock:
-                    await self._call_sdk(
-                        self.chip_controller.GetConnectedDeviceSync,
-                        nodeid=node_id,
-                        allowPASE=True,
-                        timeoutMs=30000,
-                    )
-                return
-            LOGGER.debug("Resolving node %s", node_id)
-            await self._call_sdk(self.chip_controller.ResolveNode, nodeid=node_id)
         except (ChipStackError, TimeoutError) as err:
-            if not retries:
+            if retries <= 1:
                 # when we're out of retries, raise NodeNotResolving
                 raise NodeNotResolving(f"Unable to resolve Node {node_id}") from err
-            async with node_lock:
-                await self._resolve_node(
-                    node_id=node_id, retries=retries - 1, allow_pase=retries - 1 == 0
-                )
+            await self._resolve_node(node_id=node_id, retries=retries - 1)
             await asyncio.sleep(2)
 
     def _handle_endpoints_removed(self, node_id: int, endpoints: Iterable[int]) -> None:
         """Handle callback for when bridge endpoint(s) get deleted."""
         node = cast(MatterNodeData, self._nodes[node_id])
         for endpoint_id in endpoints:
             node.attributes = {
```

### Comparing `python-matter-server-3.6.3/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.6.4/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/server/server.py` & `python-matter-server-3.6.4/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/server/stack.py` & `python-matter-server-3.6.4/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/server/storage.py` & `python-matter-server-3.6.4/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/matter_server/server/vendor_info.py` & `python-matter-server-3.6.4/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.6.3/pyproject.toml` & `python-matter-server-3.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools~=62.3",
     "wheel~=0.37.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.6.3"
+version = "3.6.4"
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "The Home Assistant Authors", email = "hello@home-assistant.io" },
 ]
 classifiers = [
```

### Comparing `python-matter-server-3.6.3/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-3.6.4/python_matter_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.6.3
+Version: 3.6.4
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.6.3/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.6.4/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

