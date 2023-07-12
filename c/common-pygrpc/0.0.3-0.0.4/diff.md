# Comparing `tmp/common_pygrpc-0.0.3-py3-none-any.whl.zip` & `tmp/common_pygrpc-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 18033 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     5476 b- defN 23-Jul-11 01:41 common_pb2.py
--rw-rw-rw-  2.0 fat     2360 b- defN 23-Jul-11 01:41 common_pb2_grpc.py
--rw-rw-rw-  2.0 fat     8014 b- defN 23-Jul-11 01:38 grpclib.py
--rw-rw-rw-  2.0 fat    34507 b- defN 23-Jul-11 01:41 common_pygrpc-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      771 b- defN 23-Jul-11 01:41 common_pygrpc-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 01:41 common_pygrpc-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       35 b- defN 23-Jul-11 01:41 common_pygrpc-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      628 b- defN 23-Jul-11 01:41 common_pygrpc-0.0.3.dist-info/RECORD
-8 files, 51883 bytes uncompressed, 16943 bytes compressed:  67.3%
+Zip file size: 18154 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     5476 b- defN 23-Jul-12 01:25 common_pb2.py
+-rw-rw-rw-  2.0 fat     2360 b- defN 23-Jul-12 01:25 common_pb2_grpc.py
+-rw-rw-rw-  2.0 fat     8659 b- defN 23-Jul-12 01:24 grpclib.py
+-rw-rw-rw-  2.0 fat    34507 b- defN 23-Jul-12 01:25 common_pygrpc-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      771 b- defN 23-Jul-12 01:25 common_pygrpc-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 01:25 common_pygrpc-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       35 b- defN 23-Jul-12 01:25 common_pygrpc-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      628 b- defN 23-Jul-12 01:25 common_pygrpc-0.0.4.dist-info/RECORD
+8 files, 52528 bytes uncompressed, 17064 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: common_pb2_grpc.py
 Comment: 
 
 Filename: grpclib.py
 Comment: 
 
-Filename: common_pygrpc-0.0.3.dist-info/LICENSE
+Filename: common_pygrpc-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: common_pygrpc-0.0.3.dist-info/METADATA
+Filename: common_pygrpc-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: common_pygrpc-0.0.3.dist-info/WHEEL
+Filename: common_pygrpc-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: common_pygrpc-0.0.3.dist-info/top_level.txt
+Filename: common_pygrpc-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: common_pygrpc-0.0.3.dist-info/RECORD
+Filename: common_pygrpc-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## grpclib.py

```diff
@@ -57,14 +57,31 @@
 class Server:
 
     def __init__(self, server, host, port):
         self.server = server
         self.host = host
         self.port = port
         self.addr = host + ':' + str(port)
+        self._channel = None
+
+    def copy(self):
+        return type(self)(self.server, self.host, self.port)
+
+    @property
+    def channel(self):
+        if self._channel is None:
+            self._channel = grpc.insecure_channel(self.addr)
+        return self._channel
+
+    def __enter__(self):
+        stub = common_pb2_grpc.CommonServiceStub(self.channel)
+        return stub
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.channel.close()
 
 
 class CommonService(common_pb2_grpc.CommonServiceServicer):
 
     @classmethod
     def clazz_handler(cls, clazz):
         return clazz
@@ -114,25 +131,32 @@
         """
         get server stub
         :param server:
         :return:
         """
         return self.stubs.get(server)
 
+    def get_server(self, server):
+        return self.server_address.get(server)
+
     def load(self, servers):
         """
         load grpc server list
         :param servers: Server
         :return:
         """
         for server in servers:
-            self.stubs[server.server] = server.addr
+            channel = grpc.insecure_channel(server.addr)
+            stub = common_pb2_grpc.CommonServiceStub(channel)
+            self.stubs[server.server] = stub
+            self.stubs[server.server] = server
 
     def __init__(self):
         self.stubs = {}
+        self.server_address = {}
 
 
 class GrpcServer:
     def __init__(self, host='0.0.0.0', port=6565, max_workers=10):
         self.address = host + ':' + str(port)
         self.max_workers = max_workers
         self.service = CommonService()
@@ -180,24 +204,24 @@
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             sig = inspect.signature(func)
             bind = sig.bind(*args, **kwargs).arguments
             if sig.parameters.get("cls"):
                 cls = bind.get("cls")
                 bind.pop("cls")
-            rpc_client_addr = grpc_client.connect(server)
-            with grpc.insecure_channel(rpc_client_addr) as channel:
-                response_json = GrpcHelper.call_rpc_result(
-                    rpc_client=common_pb2_grpc.CommonServiceStub(channel),
-                    clazz=func.__module__,
-                    method=func.__qualname__,
-                    args=(),
-                    kwargs={k: v for k, v in bind.items()},
-                )
-                return response_json
+                bind.pop("cls")
+            rpc_client = grpc_client.connect(server)
+            response_json = GrpcHelper.call_rpc_result(
+                rpc_client,
+                clazz=func.__module__,
+                method=func.__qualname__,
+                args=(),
+                kwargs={k: v for k, v in bind.items()},
+            )
+            return response_json
 
         return wrapper
 
     return decorator
 
 
 class GrpcHelper:
```

## Comparing `common_pygrpc-0.0.3.dist-info/LICENSE` & `common_pygrpc-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `common_pygrpc-0.0.3.dist-info/METADATA` & `common_pygrpc-0.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-pygrpc
-Version: 0.0.3
+Version: 0.0.4
 Summary: common python grpc service
 Home-page: https://github.com/reggiepy/common_pygrpc
 Author: reggiepy
 Author-email: reggiepy@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

