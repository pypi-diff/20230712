# Comparing `tmp/kade_drive-0.7.0.tar.gz` & `tmp/kade_drive-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kade_drive-0.7.0.tar", max compression
+gzip compressed data, was "kade_drive-0.8.1.tar", max compression
```

## Comparing `kade_drive-0.7.0.tar` & `kade_drive-0.8.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.7.0/LICENSE
--rw-r--r--   0        0        0     2165 2023-07-10 05:18:08.765855 kade_drive-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-07-05 21:17:07.161141 kade_drive-0.7.0/kade_drive/__init__.py
--rw-r--r--   0        0        0     1907 2023-07-11 18:08:36.988438 kade_drive-0.7.0/kade_drive/cli.py
--rw-r--r--   0        0        0     8974 2023-07-11 18:36:40.105435 kade_drive-0.7.0/kade_drive/client.py
--rw-r--r--   0        0        0        1 2023-07-05 21:17:07.161141 kade_drive-0.7.0/kade_drive/core/__init__.py
--rw-r--r--   0        0        0      130 2023-07-06 00:47:02.809455 kade_drive-0.7.0/kade_drive/core/config.py
--rw-r--r--   0        0        0     9561 2023-07-09 15:55:04.310834 kade_drive-0.7.0/kade_drive/core/crawling.py
--rw-r--r--   0        0        0    20831 2023-07-11 19:05:31.237835 kade_drive-0.7.0/kade_drive/core/network.py
--rw-r--r--   0        0        0     3915 2023-07-09 01:01:28.935150 kade_drive-0.7.0/kade_drive/core/node.py
--rw-r--r--   0        0        0     8752 2023-07-11 18:36:40.105435 kade_drive-0.7.0/kade_drive/core/protocol.py
--rw-r--r--   0        0        0     8819 2023-07-11 18:36:40.105435 kade_drive-0.7.0/kade_drive/core/routing.py
--rw-r--r--   0        0        0     9825 2023-07-11 18:37:58.242000 kade_drive-0.7.0/kade_drive/core/storage.py
--rw-r--r--   0        0        0     1319 2023-07-09 17:55:02.693868 kade_drive-0.7.0/kade_drive/core/utils.py
--rw-r--r--   0        0        0     2778 2023-07-11 18:36:40.106435 kade_drive-0.7.0/kade_drive/server.py
--rw-r--r--   0        0        0      769 2023-07-10 04:35:06.243561 kade_drive-0.7.0/kade_drive/test_store_file.py
--rw-r--r--   0        0        0       25 2023-07-05 21:17:07.162141 kade_drive-0.7.0/kade_drive/tests/__init__.py
--rw-r--r--   0        0        0     1731 2023-07-07 20:16:46.224385 kade_drive-0.7.0/kade_drive/tests/conftest.py
--rw-r--r--   0        0        0     3100 2023-07-05 21:17:07.163141 kade_drive-0.7.0/kade_drive/tests/data_to_split.txt
--rw-r--r--   0        0        0     1796 2023-07-07 20:16:46.223385 kade_drive-0.7.0/kade_drive/tests/test_node.py
--rw-r--r--   0        0        0     4642 2023-07-07 20:16:46.181385 kade_drive-0.7.0/kade_drive/tests/test_routing.py
--rw-r--r--   0        0        0        1 2023-07-06 00:26:51.787726 kade_drive-0.7.0/kade_drive/tests/test_server.py
--rw-r--r--   0        0        0      768 2023-07-07 20:16:46.129384 kade_drive-0.7.0/kade_drive/tests/test_splitdata.py
--rw-r--r--   0        0        0     1459 2023-07-06 00:47:02.811454 kade_drive-0.7.0/kade_drive/tests/test_storage.py
--rw-r--r--   0        0        0      727 2023-07-07 20:16:46.129384 kade_drive-0.7.0/kade_drive/tests/test_utils.py
--rw-r--r--   0        0        0      760 2023-07-11 19:31:22.383949 kade_drive-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 kade_drive-0.7.0/setup.py
--rw-r--r--   0        0        0     2739 1970-01-01 00:00:00.000000 kade_drive-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-31 00:41:16.838542 kade_drive-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2579 2023-07-12 15:38:09.079550 kade_drive-0.8.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 21:17:07.161141 kade_drive-0.8.1/kade_drive/__init__.py
+-rw-r--r--   0        0        0     1914 2023-07-12 15:38:09.084550 kade_drive-0.8.1/kade_drive/cli.py
+-rw-r--r--   0        0        0     9108 2023-07-12 15:38:09.084550 kade_drive-0.8.1/kade_drive/client.py
+-rw-r--r--   0        0        0        1 2023-07-05 21:17:07.161141 kade_drive-0.8.1/kade_drive/core/__init__.py
+-rw-r--r--   0        0        0      130 2023-07-06 00:47:02.809455 kade_drive-0.8.1/kade_drive/core/config.py
+-rw-r--r--   0        0        0     9635 2023-07-12 15:38:09.084550 kade_drive-0.8.1/kade_drive/core/crawling.py
+-rw-r--r--   0        0        0    21018 2023-07-12 15:57:39.167589 kade_drive-0.8.1/kade_drive/core/network.py
+-rw-r--r--   0        0        0     3915 2023-07-09 01:01:28.935150 kade_drive-0.8.1/kade_drive/core/node.py
+-rw-r--r--   0        0        0     8749 2023-07-12 15:55:26.352414 kade_drive-0.8.1/kade_drive/core/protocol.py
+-rw-r--r--   0        0        0     8819 2023-07-11 18:36:40.105435 kade_drive-0.8.1/kade_drive/core/routing.py
+-rw-r--r--   0        0        0     9635 2023-07-12 15:55:10.756393 kade_drive-0.8.1/kade_drive/core/storage.py
+-rw-r--r--   0        0        0     1319 2023-07-09 17:55:02.693868 kade_drive-0.8.1/kade_drive/core/utils.py
+-rw-r--r--   0        0        0     2778 2023-07-11 18:36:40.106435 kade_drive-0.8.1/kade_drive/server.py
+-rw-r--r--   0        0        0      769 2023-07-10 04:35:06.243561 kade_drive-0.8.1/kade_drive/test_store_file.py
+-rw-r--r--   0        0        0       25 2023-07-05 21:17:07.162141 kade_drive-0.8.1/kade_drive/tests/__init__.py
+-rw-r--r--   0        0        0     1731 2023-07-07 20:16:46.224385 kade_drive-0.8.1/kade_drive/tests/conftest.py
+-rw-r--r--   0        0        0     3100 2023-07-05 21:17:07.163141 kade_drive-0.8.1/kade_drive/tests/data_to_split.txt
+-rw-r--r--   0        0        0     1796 2023-07-07 20:16:46.223385 kade_drive-0.8.1/kade_drive/tests/test_node.py
+-rw-r--r--   0        0        0     4642 2023-07-07 20:16:46.181385 kade_drive-0.8.1/kade_drive/tests/test_routing.py
+-rw-r--r--   0        0        0        1 2023-07-06 00:26:51.787726 kade_drive-0.8.1/kade_drive/tests/test_server.py
+-rw-r--r--   0        0        0      768 2023-07-07 20:16:46.129384 kade_drive-0.8.1/kade_drive/tests/test_splitdata.py
+-rw-r--r--   0        0        0     1459 2023-07-06 00:47:02.811454 kade_drive-0.8.1/kade_drive/tests/test_storage.py
+-rw-r--r--   0        0        0      727 2023-07-07 20:16:46.129384 kade_drive-0.8.1/kade_drive/tests/test_utils.py
+-rw-r--r--   0        0        0      760 2023-07-12 16:12:52.817058 kade_drive-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3623 1970-01-01 00:00:00.000000 kade_drive-0.8.1/setup.py
+-rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 kade_drive-0.8.1/PKG-INFO
```

### Comparing `kade_drive-0.7.0/LICENSE` & `kade_drive-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/cli.py` & `kade_drive-0.8.1/kade_drive/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         print(
             "Error Connecting to the network, Please check your conectivity and verify that at least one server is online."
         )
         return
 
     print("Wellcome to CLI interface for distributed Filesystem")
     while True:
-        command = input("cli > ").split(" ")
+        command = input("cli > ").strip().split(" ")
         if command[0] == "exit":
             break
 
         if command[0] == "help":
             print(
                 """Command - args - description\n
 put - %key %value - stores %value in the network asociated with %key
@@ -27,15 +27,15 @@
 help - * - displays this message
 exit - * - close the client
             """
             )
             continue
         args = command[1:] if len(command) >= 1 else []
         func = getattr(ClientSession, command[0], None)
-        if func is None or not callable(func) :
+        if func is None or not callable(func):
             print(
                 f'command {command[0]} not found, use "help" to see supported commands'
             )
             continue
 
         if not response:
             response = client_session.connect(use_broadcast_if_needed=True)
```

### Comparing `kade_drive-0.7.0/kade_drive/client.py` & `kade_drive-0.8.1/kade_drive/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,17 +154,21 @@
                     tuple[str, int]
                 ] = self.connection.root.get_file_chunk_location(chunk_key)
             except EOFError as e:
                 logger.error(
                     f"Connection lost in get when doing get_file_chunk_location, exception: {e}"
                 )
                 return None, None
+            
+            if locations is None:
+                continue
+            
             logger.debug(
                 f"locations for chunk_key {chunk_key} are {locations}")
-            if self.bootstrap_nodes[0] in locations:
+            if not locations is None and len(locations) > 0 and self.bootstrap_nodes[0] in locations:
                 logger.debug("Using primary connection to get chunk")
                 try:
                     data_received.append(
                         self.connection.root.rpc_get_file_chunk_value(
                             chunk_key)
                     )
                 except EOFError as e:
```

### Comparing `kade_drive-0.7.0/kade_drive/core/crawling.py` & `kade_drive-0.8.1/kade_drive/core/crawling.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,16 @@
           2. current nearest list needs to keep track of who has been queried
              already sort by nearest, keep KSIZE
           3. if list is same as last time, next call should be to everyone not
              yet queried
           4. repeat, unless nearest list has all been queried, then ur done
         """
 
-        logger.debug("crawling network with nearest: %s", str(tuple(self.nearest)))
+        logger.debug("crawling network with nearest: %s",
+                     str(tuple(self.nearest)))
         # define the alpha based on the latest crawled nodes
         count = self.alpha
         if self.nearest.get_ids() == self.last_ids_crawled:
             count = len(self.nearest)
         # uodate latest crawled nodes
         self.last_ids_crawled = self.nearest.get_ids()
 
@@ -70,16 +71,17 @@
         for peer in self.nearest.get_uncontacted()[:count]:
             logger.debug("Peer %s %s", type(peer), peer)
             if peer.ip == "192.168.133.1":
                 continue
             try:
                 session = rpyc.connect(host=peer.ip, port=peer.port)
                 conn = session.root
-            except ConnectionError as e:
-                logger.warning(f"Failed to connect to {peer.id} {peer.ip}, e: {e}")
+            except (ConnectionError, OSError) as e:
+                logger.warning(
+                    f"Failed to connect to {peer.id} {peer.ip}, e: {e}")
                 session = None
                 conn = None
 
             logger.debug(
                 f"Connection is {conn is not None} and self.node is {self.node is not None}"
             )
             logger.debug(f"Calling : {rpcmethod}")
@@ -152,15 +154,16 @@
         """
         # create a counter for each value found
 
         value_counts = Counter(values)
         # if more than one value is found for a key raise a warning
         if len(value_counts) != 1:
             logger.debug(
-                "Got multiple values for key %i: %s", self.node.long_id, str(values)
+                "Got multiple values for key %i: %s", self.node.long_id, str(
+                    values)
             )
         # get the most common item in the network
         # this is, if there were more than one value
         # for the key, choose the most replicated one
         value = value_counts.most_common(1)[0][0]
 
         # choose the closest node who doesnt had the value
```

### Comparing `kade_drive-0.7.0/kade_drive/core/network.py` & `kade_drive-0.8.1/kade_drive/core/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from kade_drive.core.routing import RoutingTable
 from kade_drive.core.utils import digest
 from kade_drive.core.storage import PersistentStorage
 from kade_drive.core.node import Node
 from kade_drive.core.crawling import ChunkLocationSpiderCrawl, ValueSpiderCrawl
 from kade_drive.core.crawling import NodeSpiderCrawl
 from kade_drive.core.utils import is_port_in_use
+import datetime
 
 # from models.file import File
 
 # Create a file handler
 # file_handler = logging.FileHandler("log_file.log")
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
 # file_handler.setFormatter(formatter)
@@ -86,16 +87,15 @@
                 print(interface, port)
                 Server.node.ip = interface
                 Server.node.port = port
                 t = ThreadedServer(
                     ServerService,
                     port=port,
                     hostname=interface,
-                    protocol_config={
-                        "allow_public_attrs": True, "allow_pickle": True},
+                    protocol_config={"allow_public_attrs": True, "allow_pickle": True},
                 )
                 t.start()
             except Exception as e:
                 logger.critical(f"Server Listen failed: {e}")
 
     @staticmethod
     def bootstrap(addrs: list[tuple[str, str]]):
@@ -103,36 +103,33 @@
         Bootstrap the server by connecting to other known nodes in the network.
 
         Args:
             addrs: A `list` of (ip, port) `tuple` pairs.  Note that only IP
                    addresses are acceptable - hostnames will cause an error.
         """
 
-        logger.debug(
-            f"Attempting to bootstrap node with {len(addrs)} initial contacts")
+        logger.debug(f"Attempting to bootstrap node with {len(addrs)} initial contacts")
         cos = list(map(Server.bootstrap_node, addrs))
         nodes = [node for node in cos if node is not None]
-        spider = NodeSpiderCrawl(
-            Server.node, nodes, Server.ksize, Server.alpha)
+        spider = NodeSpiderCrawl(Server.node, nodes, Server.ksize, Server.alpha)
         res = spider.find()
         logger.debug("results of spider find: %s", res)
 
         return res
 
     @staticmethod
     def bootstrap_node(addr: tuple[str, str]):
         response = None
         with ServerSession(addr[0], addr[1]) as conn:
             if conn:
                 response = conn.rpc_ping(
                     (Server.node.ip, Server.node.port), Server.node.id
                 )
                 node = Node(response, addr[0], addr[1]) if response else None
-                response = FileSystemProtocol.process_response(
-                    conn, response, node)
+                response = FileSystemProtocol.process_response(conn, response, node)
 
                 return node
 
     @staticmethod
     def split_data(data: bytes, chunk_size: int):
         """Split data into chunks of less than chunk_size, it must be less than 16mb"""
         if not isinstance(data, bytes):
@@ -146,15 +143,15 @@
         count = 0
         last_position = 0
         while not (fixed_chunks == count):
             if count == 0:
                 chunks.append(data[0:chunk_size])
                 last_position = chunk_size
             else:
-                chunks.append(data[last_position: last_position + chunk_size])
+                chunks.append(data[last_position : last_position + chunk_size])
                 last_position = last_position + chunk_size
             count += 1
         return chunks
 
     @staticmethod
     def _handle_empty_neighbors(dkey, metadata, value, exclude_current):
         logger.debug("There are no known neighbors to set key %s", dkey.hex())
@@ -179,22 +176,26 @@
 
         node = Node(dkey)
         assert node is not None
         nearest = FileSystemProtocol.router.find_neighbors(node)
         logger.info(f"nearest in set_digest is {nearest}")
 
         if not nearest or len(nearest) == 0:
-            return Server._handle_empty_neighbors(dkey, metadata, value, exclude_current)
+            return Server._handle_empty_neighbors(
+                dkey, metadata, value, exclude_current
+            )
         spider = NodeSpiderCrawl(node, nearest, Server.ksize, Server.alpha)
         nodes = spider.find()
         logger.debug("setting '%s' on %s", dkey, list(map(str, nodes)))
 
         if not nodes or len(nodes) == 0:
-            return Server._handle_empty_neighbors(dkey, metadata, value, exclude_current)
-        
+            return Server._handle_empty_neighbors(
+                dkey, metadata, value, exclude_current
+            )
+
         # if this node is close too, then store here as well
         biggest = max([n.distance_to(node) for n in nodes])
         if Server.node.distance_to(node) < biggest and not exclude_current:
             if metadata:
                 Server.storage.set_metadata(dkey, value, False)
             else:
                 Server.storage.set_value(dkey, value, False)
@@ -205,15 +206,24 @@
             with ServerSession(address[0], address[1]) as conn:
                 response = FileSystemProtocol.call_check_if_new_value_exists(
                     conn, n, dkey
                 )
                 contains, date = None, None
                 if response is not None:
                     contains, date = response
-                if local_last_write is None or date is None or date < local_last_write:
+                # patch to make sure no invalid data is compared
+                valid_data = True
+                if not type(date) == type(datetime.datetime.now()):
+                    valid_data = False
+
+                if (
+                    local_last_write is None
+                    or date is None
+                    or (valid_data and date < local_last_write)
+                ):
                     result = FileSystemProtocol.call_store(
                         conn, n, dkey, value, metadata
                     )
                     if result:
                         any_result = True
 
                 if contains:
@@ -223,26 +233,24 @@
         return any_result
 
     @staticmethod
     def find_replicas():
         nearest = FileSystemProtocol.router.find_neighbors(
             Server.node, Server.alpha, exclude=Server.node
         )
-        spider = NodeSpiderCrawl(Server.node, nearest,
-                                 Server.ksize, Server.alpha)
+        spider = NodeSpiderCrawl(Server.node, nearest, Server.ksize, Server.alpha)
 
         nodes = spider.find()
 
         keys_to_find = Server.storage.keys()
         keys_dict = {}
         for n in nodes:
             with ServerSession(n.ip, n.port) as conn:
                 for k, is_metadata in keys_to_find:
-                    contains = FileSystemProtocol.call_contains(
-                        conn, n, k, is_metadata)
+                    contains = FileSystemProtocol.call_contains(conn, n, k, is_metadata)
                     if contains:
                         if (k, is_metadata) not in keys_dict:
                             keys_dict[(k, is_metadata)] = 0
                         keys_dict[(k, is_metadata)] += 1
 
         return_list = []
         for k in keys_dict:
@@ -260,30 +268,28 @@
 
                 results = []
                 for node_id in FileSystemProtocol.get_refresh_ids():
                     node = Node(node_id)
                     nearest = FileSystemProtocol.router.find_neighbors(
                         node, Server.alpha
                     )
-                    spider = NodeSpiderCrawl(
-                        node, nearest, Server.ksize, Server.alpha)
+                    spider = NodeSpiderCrawl(node, nearest, Server.ksize, Server.alpha)
 
                     results.append(spider.find())
 
                 # Republishing keys to mantain the network updated
 
                 logger.debug("Republishing old keys")
                 for (
                     key,
                     value,
                     is_metadata,
                     last_write,
                 ) in Server.storage.iter_older_than(5):
-                    Server.set_digest(key, value, is_metadata,
-                                      exclude_current=True)
+                    Server.set_digest(key, value, is_metadata, exclude_current=True)
                     Server.storage.update_republish(key)
                 keys_to_replicate = Server.find_replicas()
 
                 # Republishing keys that have less replicas than the replication factor
 
                 if len(keys_to_replicate):
                     for key, is_metadata in keys_to_replicate:
@@ -330,15 +336,18 @@
 
         node = Node(key)
         nearest = FileSystemProtocol.router.find_neighbors(node)
         if not nearest:
             logger.debug(f"There are no known neighbors to get key {key}")
             if Server.storage.contains(key):
                 logger.debug("Getting key from this same node")
-                return pickle.loads(Server.storage.get(key, True))
+                data = Server.storage.get(key, True)
+                if data is None:
+                    return None
+                return pickle.loads(data)
             return None
         spider = ValueSpiderCrawl(node, nearest, Server.ksize, Server.alpha)
         data = spider.find()
         if data is None:
             logger.debug("NONE DATA")
             return None
         logger.debug(f"DATA {data}")
@@ -376,16 +385,15 @@
                 logger.debug(
                     f"Found in this server, {Server.node.ip}, port, {Server.node.port}"
                 )
                 return [(Server.node.ip, Server.node.port)]
             return None
 
         logger.debug("Initiating ChunkLocationSpiderCrawl")
-        spider = ChunkLocationSpiderCrawl(
-            node, nearest, Server.ksize, Server.alpha)
+        spider = ChunkLocationSpiderCrawl(node, nearest, Server.ksize, Server.alpha)
         results = spider.find()
         logger.debug(f"results of ChunkLocationSpider {results}")
         return results
 
     @rpyc.exposed
     def rpc_find_chunk_location(
         self, sender: tuple[str, str], nodeid: bytes, key: bytes
@@ -436,16 +444,15 @@
             FileSystemProtocol.wellcome_if_new(conn, source)
 
         logger.debug(
             f"got a store request from %s, storing '%s'='%s' {sender}, {key}, {value}"
         )
         # store values and report success
         if metadata:
-            FileSystemProtocol.storage.set_metadata(
-                key, value, republish_data=False)
+            FileSystemProtocol.storage.set_metadata(key, value, republish_data=False)
         else:
             FileSystemProtocol.storage.set_value(key, value, metadata=False)
         return True
 
     @rpyc.exposed
     def rpc_find_value(
         self, sender: tuple[str, str], nodeid: bytes, key: bytes, metadata=True
@@ -454,16 +461,15 @@
         # if a new node is sending the request, give all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
             logger.info(f"wellcome_If_new in find_value {address}")
             FileSystemProtocol.wellcome_if_new(conn, source)
         # get value from storage
         if not FileSystemProtocol.storage.contains(key, metadata):
-            logger.debug(
-                f"Value with key {key} not found, calling rpc_find_node")
+            logger.debug(f"Value with key {key} not found, calling rpc_find_node")
             logger.debug(f"type of key is {type(key)}")
 
             return self.rpc_find_node(sender, nodeid, key)
 
         value = FileSystemProtocol.storage.get(key, None, metadata)
         logger.debug(f"returning value {value}")
         return {"value": value}
@@ -475,45 +481,42 @@
         Args:
             sender : sender node
             nodeid (bytes): node to be probed
 
         Returns:
             bytes: node id if alive, None if not
         """
-        logger.debug(
-            f"rpc ping called from {nodeid}, {sender[0]}, {sender[1]}")
+        logger.debug(f"rpc ping called from {nodeid}, {sender[0]}, {sender[1]}")
         source = Node(nodeid, sender[0], sender[1])
         # if a new node is sending the request, give all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
             logger.info(f"wellcome_If_new in ping {address}")
             FileSystemProtocol.wellcome_if_new(conn, source)
         logger.debug("return ping")
         return FileSystemProtocol.source_node.id
 
     @rpyc.exposed
     def rpc_find_node(self, sender, nodeid: bytes, key: bytes):
-        logger.debug(
-            f"finding neighbors of {int(nodeid.hex(), 16)} in local table")
+        logger.debug(f"finding neighbors of {int(nodeid.hex(), 16)} in local table")
 
         source = Node(nodeid, sender[0], sender[1])
 
         logger.debug(f"node id {nodeid}")
         # if a new node is sending the request, give all data it should contain
         address = (source.ip, source.port)
         with ServerSession(address[0], address[1]) as conn:
             logger.info(f"wellcome_If_new in find_node {address}")
             FileSystemProtocol.wellcome_if_new(conn, source)
         # create a fictional node to perform the search
         logger.debug(f"fictional key {key}")
         logger.debug(f"SEnder [0] Sender [1] {source.ip}, {source.port}")
         node = Node(key)
         # ask for the neighbors of the node
-        neighbors = FileSystemProtocol.router.find_neighbors(
-            node, exclude=source)
+        neighbors = FileSystemProtocol.router.find_neighbors(node, exclude=source)
         logger.debug(f"neighbors of find_node: { neighbors}")
         return list(map(tuple, neighbors))
 
     @rpyc.exposed
     def rpc_contains(self, sender, nodeid: bytes, key: bytes, is_metadata=True):
         source = Node(nodeid, sender[0], sender[1])
         # if a new node is sending the request, givemsg all data it should contain
```

### Comparing `kade_drive-0.7.0/kade_drive/core/node.py` & `kade_drive-0.8.1/kade_drive/core/node.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/core/protocol.py` & `kade_drive-0.8.1/kade_drive/core/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
         """
         # if the node is in the table, do nothing
         if not FileSystemProtocol.router.is_new_node(node):
             return
 
         # TODO uncomment this
         if (node.ip, node.port) == (FileSystemProtocol.source_node.ip, FileSystemProtocol.source_node.port):
-            logger.critical("called wellcome if new in self")
+            logger.debug("called wellcome if new in self")
             return
         # add node to table
 
         logger.debug("Adding new node to contacts")
         FileSystemProtocol.router.add_contact(node)
 
         logger.info(f"never seen {node} before, adding to router")
```

### Comparing `kade_drive-0.7.0/kade_drive/core/routing.py` & `kade_drive-0.8.1/kade_drive/core/routing.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/core/storage.py` & `kade_drive-0.8.1/kade_drive/core/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,25 +60,23 @@
         os.makedirs(self.timestamp_path, exist_ok=True)
 
     def update_timestamp(self, filename: str, republish_data=False, is_write=False):
         self.ensure_dir_paths()
         data = {}
         if os.path.exists(os.path.join(self.timestamp_path, str(filename))):
             with open(os.path.join(self.timestamp_path, str(filename)), "rb") as f:
-                #  BUGGGG
                 data = pickle.load(f)
 
         data["date"] = datetime.now()
         data["republish"] = republish_data
 
         if is_write:
-            data['last_write'] = datetime.now()
+            data["last_write"] = datetime.now()
 
-        logger.debug(
-            f"mira ruta {os.path.join(self.timestamp_path, str(filename))}")
+        logger.debug(f"mira ruta {os.path.join(self.timestamp_path, str(filename))}")
         with open(os.path.join(self.timestamp_path, str(filename)), "wb") as f:
             pickle.dump(data, f)
 
     def update_republish(self, key: bytes):
         str_key = str(base64.urlsafe_b64encode(key))
         with open(os.path.join(self.timestamp_path, str_key), "rb") as f:
             data = pickle.load(f)
@@ -102,44 +100,43 @@
                             data = pickle.load(f)
 
                         if (datetime.now() - data["date"]).seconds > self.ttl:
                             logger.info(
                                 f"Removing file {file}, beacuse it has not been accessed in {self.ttl/60} minutes"
                             )
                             if Path(os.path.join(self.values_path, str(file))).exists():
-                                os.remove(os.path.join(
-                                    self.values_path, str(file)))
+                                os.remove(os.path.join(self.values_path, str(file)))
                             if Path(
                                 os.path.join(self.metadata_path, str(file))
                             ).exists():
-                                os.remove(os.path.join(
-                                    self.metadata_path, str(file)))
+                                os.remove(os.path.join(self.metadata_path, str(file)))
                             if Path(os.path.join(self.keys_path, str(file))).exists():
-                                os.remove(os.path.join(
-                                    self.keys_path, str(file)))
+                                os.remove(os.path.join(self.keys_path, str(file)))
 
-                            os.remove(os.path.join(
-                                self.timestamp_path, str(file)))
+                            os.remove(os.path.join(self.timestamp_path, str(file)))
             sleep(self.ttl)
 
     def get_value(self, str_key: str, update_timestamp=True, metadata=True):
         self.ensure_dir_paths()
         if metadata:
             path = os.path.join(self.metadata_path, str_key)
         else:
             path = os.path.join(self.values_path, str_key)
-        with open(path, "rb") as f:
-            result = f.read()
+
+        result = None
+        if os.path.exists(path):
+            with open(path, "rb") as f:
+                result = f.read()
 
         if result is not None:
             if update_timestamp:
                 self.update_timestamp(str_key, republish_data=True)
         if not result:
-            logger.error(f"tried to get non existing data with key {str_key}")
-            print("Tried to get data that is not in db")
+            logger.warning(f"tried to get non existing data with key {str_key}")
+
         return result
 
     def set_value(self, key: bytes, value, metadata=True, republish_data=False):
         str_key = str(base64.urlsafe_b64encode(key))
         self.ensure_dir_paths()
         self.update_timestamp(str_key, republish_data, is_write=True)
         if metadata:
@@ -203,15 +200,15 @@
         path = Path(os.path.join(self.timestamp_path, str_key))
         if not path.exists():
             return False, None
 
         with open(os.path.join(self.timestamp_path, str_key), "rb") as f:
             data = pickle.load(f)
 
-        return True, data['last_write']
+        return True, data["last_write"]
 
     def __getitem__(self, key: bytes):
         self.cull()
         str_key = str(base64.urlsafe_b64encode(key))
         result = self.get_value(str_key)
         if result is None:
             raise KeyError()
@@ -231,15 +228,15 @@
                         "republish"
                     ]:
                         key, is_metadata = self.get_key_in_bytes(str(file))
                         value = self.get_value(
                             str(file), update_timestamp=False, metadata=is_metadata
                         )
                         assert value is not None
-                        yield key, value, is_metadata, data['last_write']
+                        yield key, value, is_metadata, data["last_write"]
 
     def keys(self):
         ikeys_files = os.listdir(os.path.join(self.keys_path))
         ikeys = []
         imetadata = []
         for key_name in ikeys_files:
             k, m = self.get_key_in_bytes(key_name)
@@ -259,10 +256,9 @@
             ikeys.append(k)
             imetadata.append(m)
 
         logger.debug("ikeys: %s", ikeys)
         ivalues: list[bytes] = []
 
         for i, ik in enumerate(ikeys):
-            ivalues.append(
-                self.get(ik, update_timestamp=False, metadata=imetadata[i]))
+            ivalues.append(self.get(ik, update_timestamp=False, metadata=imetadata[i]))
         return zip(ikeys, ivalues, imetadata)
```

### Comparing `kade_drive-0.7.0/kade_drive/core/utils.py` & `kade_drive-0.8.1/kade_drive/core/utils.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/server.py` & `kade_drive-0.8.1/kade_drive/server.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/test_store_file.py` & `kade_drive-0.8.1/kade_drive/test_store_file.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/tests/conftest.py` & `kade_drive-0.8.1/kade_drive/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/tests/data_to_split.txt` & `kade_drive-0.8.1/kade_drive/tests/data_to_split.txt`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/tests/test_node.py` & `kade_drive-0.8.1/kade_drive/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/tests/test_routing.py` & `kade_drive-0.8.1/kade_drive/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/tests/test_splitdata.py` & `kade_drive-0.8.1/kade_drive/tests/test_splitdata.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/tests/test_storage.py` & `kade_drive-0.8.1/kade_drive/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/kade_drive/tests/test_utils.py` & `kade_drive-0.8.1/kade_drive/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `kade_drive-0.7.0/pyproject.toml` & `kade_drive-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kade_drive"
-version = "0.7.0"
+version = "0.8.1"
 description = "distributed file system based on kademlia dht"
 authors = ["DanielUH2019 <danielcardenascabrera2016@gmail.com>", "JavierOramas <javiale2000@gmail.com>", "Lia001218 <liazerqueraf@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "kade_drive"}]
 
 [tool.poetry.dependencies]
```

### Comparing `kade_drive-0.7.0/setup.py` & `kade_drive-0.8.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 entry_points = \
 {'console_scripts': ['cli = kade_drive.cli:start_cli',
                      'server = kade_drive.server:start',
                      'test_store = kade_drive.test_store_file:test_store_df']}
 
 setup_kwargs = {
     'name': 'kade-drive',
-    'version': '0.7.0',
+    'version': '0.8.1',
     'description': 'distributed file system based on kademlia dht',
-    'long_description': '![Python Version](https://img.shields.io/badge/Python-3.10-blue)\n![Code Style](https://img.shields.io/badge/Code%20Style-Black-black)\n![Poetry Version](https://img.shields.io/badge/Poetry-1.3.1-blue)\n![Docker Support](https://img.shields.io/badge/Docker-Supported-brightgreen?logo=docker)\n![Docker Build Status](https://img.shields.io/docker/build/geekslabtech/kade-drive)\n![Visits](https://badges.pufler.dev/visits/geeksLabTech/kade-drive)\n![Contributors](https://img.shields.io/github/contributors/geeksLabTech/kade-drive)\n![Release Version](https://img.shields.io/github/v/release/geeksLabTech/kade-drive)\n![Documentation](https://img.shields.io/badge/docs-available-brightgreen)\n![Package Version](https://img.shields.io/pypi/v/kade-drive)\n![Downloads](https://img.shields.io/pypi/dm/kade-drive)\n![Release Date](https://img.shields.io/github/release-date/geeksLabTech/kade-drive)\n![Code Size](https://img.shields.io/github/languages/code-size/geeksLabTech/kade-drive)\n\nDistributed file system based on <https://github.com/bmuller/kademlia> for the final project of distributed systems\n\n## Documentation\n\n<https://geekslabtech.github.io/kade-drive/>\n\n## Basic Usage\n\n- Clone the repo and run `poetry install`\n- Run `poetry run server` in one pc or several pc in a local network\n- Run `poetry run cli` in any pc of the network and start playing with the system\n\n### Usage with docker\n\n- Build the image with `make docker`\n- Run `make shell` to start the Docker container with an interactive Bash shell\n- Now you can run `poetry run server` to start a server or `poetry run cli`\n\n## Installation\n\n```console\npip install kade-drive\n```\n\n## Server\n\n```Python\nfrom kade_drive.server import start_server\n\nstart_server()\n```\n\n## Client\n\n### Note: Make sure that there exist at least a server in the local network\n\n```Python\nfrom kade_drive.cli import ClientSession\n\nclient = ClientSession()\nclient.connect()\nresponse, _ = client.put(4, 5)\n# If true, it means that the value was setted correctly, false otherwise\nassert response is True\nvalue, _ = client.get(4)\nassert value == 5\n```\n\n### Tests\n\nTo run tests make shure that there is at least one server in the network.\n',
+    'long_description': '![Python Version](https://img.shields.io/badge/Python-3.10-blue)\n![Code Style](https://img.shields.io/badge/Code%20Style-Black-black)\n![Poetry Version](https://img.shields.io/badge/Poetry-1.3.1-blue)\n![Docker Support](https://img.shields.io/badge/Docker-Supported-brightgreen?logo=docker)\n[![Docker Pulls](https://badgen.net/docker/pulls/joramas/kade-drive?icon=docker&label=pulls)](https://hub.docker.com/r/joramas/kade-drive/)\n[![Docker Stars](https://badgen.net/docker/stars/joramas/kade-drive?icon=docker&label=stars)](https://hub.docker.com/r/joramas/kade-drive/)\n[![Docker Image Size](https://badgen.net/docker/size/joramas/kade-drive?icon=docker&label=image%20size)](https://hub.docker.com/r/joramas/kade-drive/)\n![Visits](https://badges.pufler.dev/visits/geeksLabTech/kade-drive)\n![Contributors](https://img.shields.io/github/contributors/geeksLabTech/kade-drive)\n![Release Version](https://img.shields.io/github/v/release/geeksLabTech/kade-drive)\n![Documentation](https://img.shields.io/badge/docs-available-brightgreen)\n![Package Version](https://img.shields.io/pypi/v/kade-drive)\n![Downloads](https://img.shields.io/pypi/dm/kade-drive)\n![Release Date](https://img.shields.io/github/release-date/geeksLabTech/kade-drive)\n![Code Size](https://img.shields.io/github/languages/code-size/geeksLabTech/kade-drive)\n\nDistributed file system based on <https://github.com/bmuller/kademlia> for the final project of distributed systems\n\n## Documentation\n\n<https://geekslabtech.github.io/kade-drive/>\n\n## Basic Usage\n\n- Clone the repo and run `poetry install`\n- Run `poetry run server` in one pc or several pc in a local network\n- Run `poetry run cli` in any pc of the network and start playing with the system\n\n### Usage with docker\n\n- Build the image with `make docker` or pull it from docker.hub `docker pull joramas/kade-drive:latest`\n- Run `make shell` to start the Docker container with an interactive Bash shell\n- Now you can run `poetry run server` to start a server or `poetry run cli`\n\n## Installation\n\n```console\npip install kade-drive\n```\n\n## Server\n\n```Python\nfrom kade_drive.server import start_server\n\nstart_server()\n```\n\n## Client\n\n### Note: Make sure that there exist at least a server in the local network\n\n```Python\nfrom kade_drive.cli import ClientSession\n\nclient = ClientSession()\nclient.connect()\nresponse, _ = client.put(4, 5)\n# If true, it means that the value was setted correctly, false otherwise\nassert response is True\nvalue, _ = client.get(4)\nassert value == 5\n```\n\n### Tests\n\nTo run tests make shure that there is at least one server in the network.\n',
     'author': 'DanielUH2019',
     'author_email': 'danielcardenascabrera2016@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `kade_drive-0.7.0/PKG-INFO` & `kade_drive-0.8.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kade-drive
-Version: 0.7.0
+Version: 0.8.1
 Summary: distributed file system based on kademlia dht
 License: MIT
 Author: DanielUH2019
 Author-email: danielcardenascabrera2016@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,17 @@
 Requires-Dist: typer (==0.9.0)
 Description-Content-Type: text/markdown
 
 ![Python Version](https://img.shields.io/badge/Python-3.10-blue)
 ![Code Style](https://img.shields.io/badge/Code%20Style-Black-black)
 ![Poetry Version](https://img.shields.io/badge/Poetry-1.3.1-blue)
 ![Docker Support](https://img.shields.io/badge/Docker-Supported-brightgreen?logo=docker)
-![Docker Build Status](https://img.shields.io/docker/build/geekslabtech/kade-drive)
+[![Docker Pulls](https://badgen.net/docker/pulls/joramas/kade-drive?icon=docker&label=pulls)](https://hub.docker.com/r/joramas/kade-drive/)
+[![Docker Stars](https://badgen.net/docker/stars/joramas/kade-drive?icon=docker&label=stars)](https://hub.docker.com/r/joramas/kade-drive/)
+[![Docker Image Size](https://badgen.net/docker/size/joramas/kade-drive?icon=docker&label=image%20size)](https://hub.docker.com/r/joramas/kade-drive/)
 ![Visits](https://badges.pufler.dev/visits/geeksLabTech/kade-drive)
 ![Contributors](https://img.shields.io/github/contributors/geeksLabTech/kade-drive)
 ![Release Version](https://img.shields.io/github/v/release/geeksLabTech/kade-drive)
 ![Documentation](https://img.shields.io/badge/docs-available-brightgreen)
 ![Package Version](https://img.shields.io/pypi/v/kade-drive)
 ![Downloads](https://img.shields.io/pypi/dm/kade-drive)
 ![Release Date](https://img.shields.io/github/release-date/geeksLabTech/kade-drive)
@@ -39,15 +41,15 @@
 
 - Clone the repo and run `poetry install`
 - Run `poetry run server` in one pc or several pc in a local network
 - Run `poetry run cli` in any pc of the network and start playing with the system
 
 ### Usage with docker
 
-- Build the image with `make docker`
+- Build the image with `make docker` or pull it from docker.hub `docker pull joramas/kade-drive:latest`
 - Run `make shell` to start the Docker container with an interactive Bash shell
 - Now you can run `poetry run server` to start a server or `poetry run cli`
 
 ## Installation
 
 ```console
 pip install kade-drive
```

