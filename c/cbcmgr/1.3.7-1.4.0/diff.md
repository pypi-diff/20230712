# Comparing `tmp/cbcmgr-1.3.7.tar.gz` & `tmp/cbcmgr-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcmgr-1.3.7.tar", last modified: Fri Jul  7 23:46:08 2023, max compression
+gzip compressed data, was "cbcmgr-1.4.0.tar", last modified: Wed Jul 12 01:30:29 2023, max compression
```

## Comparing `cbcmgr-1.3.7.tar` & `cbcmgr-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 23:46:08.080478 cbcmgr-1.3.7/
--rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.3.7/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 23:46:08.080349 cbcmgr-1.3.7/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.3.7/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 23:46:08.061800 cbcmgr-1.3.7/cbcmgr/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.3.7/cbcmgr/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)    11122 2023-07-07 23:20:50.000000 cbcmgr-1.3.7/cbcmgr/cb_connect.py
--rw-r--r--   0 michael    (501) staff       (20)    27405 2023-07-07 23:33:22.000000 cbcmgr-1.3.7/cbcmgr/cb_management.py
--rw-r--r--   0 michael    (501) staff       (20)    11287 2023-07-07 23:20:50.000000 cbcmgr-1.3.7/cbcmgr/cb_session.py
--rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.3.7/cbcmgr/config.py
--rw-r--r--   0 michael    (501) staff       (20)     4293 2023-07-07 00:23:23.000000 cbcmgr-1.3.7/cbcmgr/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.3.7/cbcmgr/httpsessionmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.3.7/cbcmgr/retry.py
--rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.3.7/cbcmgr/schema.py
--rw-r--r--   0 michael    (501) staff       (20)      814 2023-07-07 15:20:08.000000 cbcmgr-1.3.7/cbcmgr/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-07 23:46:08.080137 cbcmgr-1.3.7/cbcmgr.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-07 23:46:08.000000 cbcmgr-1.3.7/cbcmgr.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      375 2023-07-07 23:46:08.000000 cbcmgr-1.3.7/cbcmgr.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-07 23:46:08.000000 cbcmgr-1.3.7/cbcmgr.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-07 23:46:08.000000 cbcmgr-1.3.7/cbcmgr.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-07 23:46:08.000000 cbcmgr-1.3.7/cbcmgr.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-07 23:46:08.080521 cbcmgr-1.3.7/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-07 21:00:17.000000 cbcmgr-1.3.7/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 01:30:29.498381 cbcmgr-1.4.0/
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2023-02-14 15:09:46.000000 cbcmgr-1.4.0/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-12 01:30:29.498184 cbcmgr-1.4.0/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      790 2023-02-22 04:43:20.000000 cbcmgr-1.4.0/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 01:30:29.468236 cbcmgr-1.4.0/cbcmgr/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-02-14 15:09:46.000000 cbcmgr-1.4.0/cbcmgr/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)    10719 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_connect.py
+-rw-r--r--   0 michael    (501) staff       (20)    11149 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_connect_lite.py
+-rw-r--r--   0 michael    (501) staff       (20)    27544 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_management.py
+-rw-r--r--   0 michael    (501) staff       (20)     7249 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_operation_s.py
+-rw-r--r--   0 michael    (501) staff       (20)     3719 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_pathmap.py
+-rw-r--r--   0 michael    (501) staff       (20)    13289 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/cb_session.py
+-rw-r--r--   0 michael    (501) staff       (20)     2021 2023-07-07 19:01:23.000000 cbcmgr-1.4.0/cbcmgr/config.py
+-rw-r--r--   0 michael    (501) staff       (20)     4334 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)    11048 2023-06-12 14:40:15.000000 cbcmgr-1.4.0/cbcmgr/httpsessionmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)      938 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/id_format.py
+-rw-r--r--   0 michael    (501) staff       (20)     2373 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/mt_pool.py
+-rw-r--r--   0 michael    (501) staff       (20)     2825 2023-07-07 21:38:37.000000 cbcmgr-1.4.0/cbcmgr/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)     7843 2023-05-02 21:24:28.000000 cbcmgr-1.4.0/cbcmgr/schema.py
+-rw-r--r--   0 michael    (501) staff       (20)     1446 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/cbcmgr/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-12 01:30:29.497832 cbcmgr-1.4.0/cbcmgr.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1589 2023-07-12 01:30:29.000000 cbcmgr-1.4.0/cbcmgr.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      485 2023-07-12 01:30:29.000000 cbcmgr-1.4.0/cbcmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-12 01:30:29.000000 cbcmgr-1.4.0/cbcmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       67 2023-07-12 01:30:29.000000 cbcmgr-1.4.0/cbcmgr.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        7 2023-07-12 01:30:29.000000 cbcmgr-1.4.0/cbcmgr.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-07-12 01:30:29.498463 cbcmgr-1.4.0/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1266 2023-07-12 01:28:33.000000 cbcmgr-1.4.0/setup.py
```

### Comparing `cbcmgr-1.3.7/LICENSE.txt` & `cbcmgr-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.7/PKG-INFO` & `cbcmgr-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.7
+Version: 1.4.0
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.7/README.md` & `cbcmgr-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.7/cbcmgr/cb_connect.py` & `cbcmgr-1.4.0/cbcmgr/cb_connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 ##
 ##
 
+from __future__ import annotations
 from .exceptions import (CollectionNameNotFound, IndexExistsError, QueryArgumentsError, QueryEmptyException, ClusterNotConnected, BucketNotConnected,
                          ScopeNotConnected, CollectionSubdocUpsertError, BucketWaitException, BucketStatsError, CollectionCountException, CollectionCountError)
 from .retry import retry, retry_inline
 from .cb_session import CBSession
 from .httpsessionmgr import APISession
 from datetime import timedelta
 from typing import Union, Dict, Any, List
 import logging
 import concurrent.futures
 from couchbase.cluster import Cluster
 import couchbase.subdocument as SD
 from couchbase.exceptions import (CouchbaseException, QueryIndexNotFoundException, DocumentNotFoundException, DocumentExistsException, QueryIndexAlreadyExistsException,
                                   PathNotFoundException)
-from couchbase.options import (QueryOptions, LockMode, ClusterOptions, TLSVerifyMode, WaitUntilReadyOptions)
+from couchbase.options import (QueryOptions, WaitUntilReadyOptions)
 from couchbase.management.options import GetAllQueryIndexOptions
 from couchbase.management.queries import CreatePrimaryQueryIndexOptions, DropPrimaryQueryIndexOptions
 from couchbase.diagnostics import ServiceType
 
 logger = logging.getLogger('cbutil.connect')
 logger.addHandler(logging.NullHandler())
 JSONType = Union[str, int, float, bool, None, Dict[str, Any], List[Any]]
 
 
 class CBConnect(CBSession):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.is_reachable()
-        self.check_cluster()
-        self.cluster_options = ClusterOptions(self.auth,
-                                              timeout_options=self.timeouts,
-                                              tls_verify=TLSVerifyMode.NO_VERIFY,
-                                              lockmode=LockMode.WAIT)
-        if self.use_external_network:
-            self.cluster_options.update(network="external")
-        else:
-            self.cluster_options.update(network="default")
 
-    def connect(self, bucket: str = None, scope: str = "_default", collection: str = "_default"):
+    def connect(self, bucket: str = None, scope: str = "_default", collection: str = "_default") -> CBConnect:
         logger.debug(f"connect: connect string {self.cb_connect_string}")
         self._cluster = Cluster.connect(self.cb_connect_string, self.cluster_options)
         self._cluster.wait_until_ready(timedelta(seconds=4), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue, ServiceType.Management]))
         if bucket:
             self.bucket(bucket)
             self.scope(scope)
             self.collection(collection)
         return self
 
+    def connect_cluster(self) -> CBConnect:
+        self._cluster = self.session()
+        return self
+
     def bucket(self, name: str):
         logger.debug(f"bucket: connecting bucket {name}")
         if self._cluster:
             self._bucket = retry_inline(self._cluster.bucket, name)
             self._bucket_name = name
         else:
             raise ClusterNotConnected("no cluster connected")
```

### Comparing `cbcmgr-1.3.7/cbcmgr/cb_management.py` & `cbcmgr-1.4.0/cbcmgr/cb_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ##
 ##
 
+from __future__ import annotations
 from .exceptions import (IndexNotReady, IndexNotFoundError, CollectionNameNotFound, IndexStatError, ClusterHealthCheckError, PathMapUpsertError, CollectionUpsertError,
                          ScopeCreateException, BucketCreateException, CollectionCreateException)
 from .retry import retry, retry_inline
 from .cb_connect import CBConnect
 from .util import r_getattr, omit_path, copy_path
 from .config import UpsertMapConfig, MapUpsertType
 from datetime import timedelta
@@ -62,14 +63,18 @@
 
 
 class CBManager(CBConnect):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+    def connect_cluster(self) -> CBManager:
+        self._cluster = self.session()
+        return self
+
     def create_bucket(self, name, quota: int = 256, replicas: int = 0):
         if not name:
             raise BucketCreateException(f"bucket name can not be null")
         self._cluster.wait_until_ready(timedelta(seconds=5), WaitUntilReadyOptions(service_types=[ServiceType.KeyValue]))
         logger.debug(f"create_bucket: create bucket {name}")
         try:
             bm = self._cluster.buckets()
```

### Comparing `cbcmgr-1.3.7/cbcmgr/cb_session.py` & `cbcmgr-1.4.0/cbcmgr/cb_session.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,36 +5,59 @@
 from .retry import retry
 from .httpsessionmgr import APISession
 from .config import KeyStyle
 import logging
 import socket
 import dns.resolver
 import uuid
+import hashlib
 from typing import Union
+from enum import Enum
 from datetime import timedelta
 from couchbase.auth import PasswordAuthenticator
-from couchbase.options import ClusterTimeoutOptions, ClusterOptions, LockMode
+from couchbase.options import ClusterTimeoutOptions, LockMode, ClusterOptions, TLSVerifyMode
 from couchbase.cluster import Cluster
+from acouchbase.cluster import AsyncCluster
+from couchbase.bucket import Bucket
+from acouchbase.bucket import AsyncBucket
+from couchbase.scope import Scope
+from acouchbase.scope import AsyncScope
+from couchbase.collection import Collection
+from acouchbase.collection import AsyncCollection
 from couchbase.diagnostics import ServiceType, PingState
+from couchbase.management.buckets import CreateBucketSettings, BucketType, StorageBackend
+from couchbase.management.collections import CollectionSpec
+from couchbase.management.options import CreateQueryIndexOptions, CreatePrimaryQueryIndexOptions
+from couchbase.exceptions import (BucketNotFoundException, ScopeNotFoundException, CollectionNotFoundException, BucketAlreadyExistsException, ScopeAlreadyExistsException,
+                                  CollectionAlreadyExistsException, QueryIndexAlreadyExistsException)
 
 logger = logging.getLogger('cbutil.session')
 logger.addHandler(logging.NullHandler())
 
 
+class BucketMode(Enum):
+    DEFAULT = 0
+    CACHE = 1
+    CAPACITY = 2
+
+
 class CBSession(object):
 
-    def __init__(self, hostname: str, username: str, password: str, ssl=False, external=False):
+    def __init__(self, hostname: str, username: str, password: str, ssl=False, external=False, kv_timeout: int = 5, query_timeout: int = 60):
         self.cluster_node_count = None
         self._cluster = None
         self._bucket = None
         self._scope = None
         self._collection = None
         self._bucket_name = None
         self._scope_name = "_default"
         self._collection_name = "_default"
+        self.kv_timeout = kv_timeout
+        self.query_timeout = query_timeout
+        self.hostname = hostname
         self.username = username
         self.password = password
         self.ssl = ssl
         self.rally_host_name = hostname
         self.rally_cluster_node = self.rally_host_name
         self.rally_dns_domain = False
         self.use_external_network = external
@@ -45,34 +68,57 @@
         self.all_hosts = []
         self.node_cycle = None
         self.cluster_info = None
         self.sw_version = None
         self.memory_quota = None
         self.cluster_services = []
         self.auth = PasswordAuthenticator(self.username, self.password)
-        self.timeouts = ClusterTimeoutOptions(query_timeout=timedelta(seconds=60),
-                                              kv_timeout=timedelta(seconds=5),
-                                              bootstrap_timeout=timedelta(seconds=5),
-                                              resolve_timeout=timedelta(seconds=5),
-                                              connect_timeout=timedelta(seconds=5),
-                                              management_timeout=timedelta(seconds=5))
+        self.timeouts = ClusterTimeoutOptions(query_timeout=timedelta(seconds=query_timeout),
+                                              kv_timeout=timedelta(seconds=kv_timeout),
+                                              bootstrap_timeout=timedelta(seconds=kv_timeout),
+                                              resolve_timeout=timedelta(seconds=kv_timeout),
+                                              connect_timeout=timedelta(seconds=kv_timeout),
+                                              management_timeout=timedelta(seconds=kv_timeout))
 
         if self.ssl:
             self.prefix = "https://"
             self.cb_prefix = "couchbases://"
             self.srv_prefix = "_couchbases._tcp."
             self.admin_port = "18091"
             self.node_port = "19102"
         else:
             self.prefix = "http://"
             self.cb_prefix = "couchbase://"
             self.srv_prefix = "_couchbase._tcp."
             self.admin_port = "8091"
             self.node_port = "9102"
 
+        self.is_reachable()
+        self.check_cluster()
+
+        self.cluster_options = ClusterOptions(self.auth,
+                                              timeout_options=self.timeouts,
+                                              tls_verify=TLSVerifyMode.NO_VERIFY,
+                                              lockmode=LockMode.WAIT)
+
+        if self.use_external_network:
+            self.cluster_options.update(network="external")
+        else:
+            self.cluster_options.update(network="default")
+
+    @retry()
+    def session(self) -> Cluster:
+        return Cluster.connect(self.cb_connect_string, self.cluster_options)
+
+    @retry()
+    async def session_a(self) -> AsyncCluster:
+        cluster = await AsyncCluster.connect(self.cb_connect_string, self.cluster_options)
+        await cluster.on_connect()
+        return cluster
+
     def construct_key(self, key):
         if type(key) == int or str(key).isdigit():
             if self._collection.name != "_default":
                 return self._collection.name + ':' + str(key)
             else:
                 return self._bucket.name + ':' + str(key)
         else:
```

### Comparing `cbcmgr-1.3.7/cbcmgr/config.py` & `cbcmgr-1.4.0/cbcmgr/config.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.7/cbcmgr/exceptions.py` & `cbcmgr-1.4.0/cbcmgr/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,7 +316,11 @@
 
 class KeyFormatError(CBException):
     pass
 
 
 class PathMapUpsertError(CBException):
     pass
+
+
+class TaskError(CBException):
+    pass
```

### Comparing `cbcmgr-1.3.7/cbcmgr/httpsessionmgr.py` & `cbcmgr-1.4.0/cbcmgr/httpsessionmgr.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.7/cbcmgr/retry.py` & `cbcmgr-1.4.0/cbcmgr/retry.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.7/cbcmgr/schema.py` & `cbcmgr-1.4.0/cbcmgr/schema.py`

 * *Files identical despite different names*

### Comparing `cbcmgr-1.3.7/cbcmgr.egg-info/PKG-INFO` & `cbcmgr-1.4.0/cbcmgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcmgr
-Version: 1.3.7
+Version: 1.4.0
 Summary: Couchbase connection manager
 Home-page: https://github.com/mminichino/cb-util
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: MIT License
 Keywords: couchbase,nosql,pycouchbase,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cbcmgr-1.3.7/setup.py` & `cbcmgr-1.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cbcmgr',
-    version='1.3.7',
+    version='1.4.0',
     packages=['cbcmgr'],
     url='https://github.com/mminichino/cb-util',
     license='MIT License',
     author='Michael Minichino',
     python_requires='>=3.9',
     install_requires=[
         'attrs',
```

