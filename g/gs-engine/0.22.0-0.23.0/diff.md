# Comparing `tmp/gs_engine-0.22.0-py2.py3-none-macosx_12_0_arm64.whl.zip` & `tmp/gs_engine-0.23.0-py2.py3-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11815 bytes, number of entries: 9
--rw-r--r--  2.0 unx      694 b- defN 23-Jun-06 08:10 graphscope_runtime/__init__.py
--rw-rw-r--  2.0 unx      804 b- defN 23-Jun-06 01:44 gs_engine-0.22.0.dist-info/RECORD
--rw-r--r--  2.0 unx      138 b- defN 23-Jun-06 08:40 gs_engine-0.22.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-06 08:40 gs_engine-0.22.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx    21655 b- defN 23-Jun-06 08:40 gs_engine-0.22.0.dist-info/METADATA
--rw-r--r--  2.0 unx     1573 b- defN 23-Jun-06 08:10 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 23-Jun-06 08:10 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-06 08:10 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-06 08:10 graphscope.runtime/conf/log4rs.yml
-9 files, 25989 bytes uncompressed, 10425 bytes compressed:  59.9%
+Zip file size: 11833 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      804 b- defN 23-Jul-04 11:01 gs_engine-0.23.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      140 b- defN 23-Jul-04 10:44 gs_engine-0.23.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-04 10:44 gs_engine-0.23.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx    21671 b- defN 23-Jul-04 10:44 gs_engine-0.23.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      694 b- defN 23-Jul-04 08:42 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx     1573 b- defN 23-Jul-04 08:42 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      398 b- defN 23-Jul-04 08:42 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      503 b- defN 23-Jul-04 08:42 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-04 08:42 graphscope.runtime/conf/log4rs.yml
+9 files, 26006 bytes uncompressed, 10443 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: graphscope_runtime/__init__.py
+Filename: gs_engine-0.23.0.dist-info/RECORD
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/RECORD
+Filename: gs_engine-0.23.0.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/WHEEL
+Filename: gs_engine-0.23.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/top_level.txt
+Filename: gs_engine-0.23.0.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.22.0.dist-info/METADATA
+Filename: graphscope_runtime/__init__.py
 Comment: 
 
 Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
 Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment:
```

## graphscope.runtime/conf/frontend.vineyard.properties

```diff
@@ -10,12 +10,12 @@
 # e.g. 1.2.3.4:1234,1.2.3.5:1234
 pegasus.hosts = PEGASUS_HOSTS
 
 # graph schema path
 graph.schema = GRAPH_SCHEMA
 
 ## Frontend Config
-frontend.service.port = FRONTEND_SERVICE_PORT
+gremlin.server.port = FRONTEND_SERVICE_PORT
 
 # disable the authentication if username or password is not set
 #auth.username = default
-#auth.password = default
+#auth.password = default
```

## Comparing `gs_engine-0.22.0.dist-info/METADATA` & `gs_engine-0.23.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.22.0
+Version: 0.23.0
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -367,15 +367,15 @@
 # make interactive
 # make analytical
 # make learning
 ```
 
 ### Building Docker images
 
-GraphScope ships with a [Dockerfile](k8s/graphscope.Dockerfile) that can build docker images for releasing. The images are built on a `builder` image with all dependencies installed and copied to
+GraphScope ships with a [Dockerfile](k8s/dockerfiles/graphscope-dev.Dockerfile) that can build docker images for releasing. The images are built on a `builder` image with all dependencies installed and copied to
 a `runtime-base` image. To build images with latest version of GraphScope, go to the `k8s/internal` directory under root directory and run this command.
 
 ```bash
 # by default, the built image is tagged as graphscope/graphscope:SHORTSHA
 # cd k8s
 make graphscope
 ```
```

