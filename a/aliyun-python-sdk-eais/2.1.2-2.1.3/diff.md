# Comparing `tmp/aliyun-python-sdk-eais-2.1.2.tar.gz` & `tmp/aliyun-python-sdk-eais-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-eais-2.1.2.tar", last modified: Tue Jan 10 06:12:50 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-eais-2.1.3.tar", last modified: Wed Jul 12 03:09:07 2023, max compression
```

## Comparing `aliyun-python-sdk-eais-2.1.2.tar` & `aliyun-python-sdk-eais-2.1.3.tar`

### file list

```diff
@@ -1,33 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:12:50.000000 aliyun-python-sdk-eais-2.1.2/
--rw-r--r--   0 root         (0) root         (0)      575 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2023-01-10 06:12:50.000000 aliyun-python-sdk-eais-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:12:50.000000 aliyun-python-sdk-eais-2.1.2/aliyun_python_sdk_eais.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyun_python_sdk_eais.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1131 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyun_python_sdk_eais.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyun_python_sdk_eais.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyun_python_sdk_eais.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyun_python_sdk_eais.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:12:50.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:12:50.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:12:50.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/
--rw-r--r--   0 root         (0) root         (0)     1789 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/AttachEaiRequest.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/ChangeResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     4830 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/CreateEaiAllRequest.py
--rw-r--r--   0 root         (0) root         (0)     2624 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/CreateEaiEciRequest.py
--rw-r--r--   0 root         (0) root         (0)     2624 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/CreateEaiEcsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/CreateEaiJupyterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/CreateEaiRequest.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/DeleteEaiAllRequest.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/DeleteEaiRequest.py
--rw-r--r--   0 root         (0) root         (0)     2742 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/DescribeEaisRequest.py
--rw-r--r--   0 root         (0) root         (0)     1275 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1562 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/DetachEaiRequest.py
--rw-r--r--   0 root         (0) root         (0)     2200 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/GetInstanceMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-01-10 06:12:50.000000 aliyun-python-sdk-eais-2.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2023-01-10 06:12:49.000000 aliyun-python-sdk-eais-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyun_python_sdk_eais.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyun_python_sdk_eais.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyun_python_sdk_eais.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyun_python_sdk_eais.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyun_python_sdk_eais.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyun_python_sdk_eais.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/AttachEaiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/AttachEaisEiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/ChangeResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4830 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaiAllRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaiEciRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaiEcsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaiJupyterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaisEiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DeleteEaiAllRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DeleteEaiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DeleteEaisEiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2742 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DescribeEaisRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DetachEaiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DetachEaisEiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/GetInstanceMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/StartEaisEiRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/StopEaisEiRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-07-12 03:09:07.000000 aliyun-python-sdk-eais-2.1.3/setup.py
```

### Comparing `aliyun-python-sdk-eais-2.1.2/LICENSE` & `aliyun-python-sdk-eais-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/PKG-INFO` & `aliyun-python-sdk-eais-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eais
-Version: 2.1.2
+Version: 2.1.3
 Summary: The eais module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eais
```

### Comparing `aliyun-python-sdk-eais-2.1.2/README.rst` & `aliyun-python-sdk-eais-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyun_python_sdk_eais.egg-info/PKG-INFO` & `aliyun-python-sdk-eais-2.1.3/aliyun_python_sdk_eais.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-eais
-Version: 2.1.2
+Version: 2.1.3
 Summary: The eais module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-eais
```

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/endpoint.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/AttachEaiRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/AttachEaiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/ChangeResourceGroupRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/ChangeResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/CreateEaiAllRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaiAllRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/CreateEaiEciRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaiEciRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/CreateEaiEcsRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaiEcsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/CreateEaiJupyterRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaiJupyterRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,7 +58,12 @@
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_EnvironmentVar(self): # Array
 		return self.get_query_params().get('EnvironmentVar')
 
 	def set_EnvironmentVar(self, EnvironmentVar):  # Array
 		self.add_query_param("EnvironmentVar", json.dumps(EnvironmentVar))
+	def get_EaisName(self): # String
+		return self.get_query_params().get('EaisName')
+
+	def set_EaisName(self, EaisName):  # String
+		self.add_query_param('EaisName', EaisName)
```

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/CreateEaiRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/CreateEaiRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Image(self): # String
+		return self.get_query_params().get('Image')
+
+	def set_Image(self, Image):  # String
+		self.add_query_param('Image', Image)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
 	def get_SecurityGroupId(self): # String
 		return self.get_query_params().get('SecurityGroupId')
```

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/DeleteEaiAllRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DeleteEaiAllRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/DeleteEaiRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DeleteEaiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/DescribeEaisRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DescribeEaisRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/DescribeRegionsRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/DetachEaiRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/DetachEaiRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/aliyunsdkeais/request/v20190624/GetInstanceMetricsRequest.py` & `aliyun-python-sdk-eais-2.1.3/aliyunsdkeais/request/v20190624/GetInstanceMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-eais-2.1.2/setup.py` & `aliyun-python-sdk-eais-2.1.3/setup.py`

 * *Files identical despite different names*

