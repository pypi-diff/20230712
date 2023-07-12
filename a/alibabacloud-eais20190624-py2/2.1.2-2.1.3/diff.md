# Comparing `tmp/alibabacloud_eais20190624_py2-2.1.2.tar.gz` & `tmp/alibabacloud_eais20190624_py2-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eais20190624_py2-2.1.2.tar", last modified: Tue Jan 10 06:15:23 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eais20190624_py2-2.1.3.tar", last modified: Wed Jul 12 03:14:37 2023, max compression
```

## Comparing `alibabacloud_eais20190624_py2-2.1.2.tar` & `alibabacloud_eais20190624_py2-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/
--rw-r--r--   0 root         (0) root         (0)      638 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25353 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624/client.py
--rw-r--r--   0 root         (0) root         (0)    85242 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2023-01-10 06:15:23.000000 alibabacloud_eais20190624_py2-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:14:37.000000 alibabacloud_eais20190624_py2-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-12 03:14:36.000000 alibabacloud_eais20190624_py2-2.1.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-12 03:14:36.000000 alibabacloud_eais20190624_py2-2.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-12 03:14:36.000000 alibabacloud_eais20190624_py2-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-07-12 03:14:37.000000 alibabacloud_eais20190624_py2-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-07-12 03:14:36.000000 alibabacloud_eais20190624_py2-2.1.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-12 03:14:36.000000 alibabacloud_eais20190624_py2-2.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:14:37.000000 alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 03:14:36.000000 alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33049 2023-07-12 03:14:36.000000 alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624/client.py
+-rw-r--r--   0 root         (0) root         (0)   106457 2023-07-12 03:14:36.000000 alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:14:37.000000 alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-07-12 03:14:37.000000 alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-07-12 03:14:37.000000 alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 03:14:37.000000 alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-12 03:14:37.000000 alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-12 03:14:37.000000 alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 03:14:37.000000 alibabacloud_eais20190624_py2-2.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-07-12 03:14:36.000000 alibabacloud_eais20190624_py2-2.1.3/setup.py
```

### Comparing `alibabacloud_eais20190624_py2-2.1.2/ChangeLog.md` & `alibabacloud_eais20190624_py2-2.1.3/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-01-10 Version: 2.1.2
+- Support ResourceGroup.
+
 2022-12-13 Version: 2.1.1
 - Add OpenAPI GetInstanceMetrics.
 
 2022-11-23 Version: 2.1.0
 - Add OpenAPI GetInstanceMetrics.
 - OpenAPI DescribeEais Add return parameter StartTime.
```

### Comparing `alibabacloud_eais20190624_py2-2.1.2/LICENSE` & `alibabacloud_eais20190624_py2-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eais20190624_py2-2.1.2/PKG-INFO` & `alibabacloud_eais20190624_py2-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eais20190624_py2
-Version: 2.1.2
+Version: 2.1.3
 Summary: Alibaba Cloud eais (20190624) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eais20190624_py2-2.1.2/README-CN.md` & `alibabacloud_eais20190624_py2-2.1.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eais20190624_py2-2.1.2/README.md` & `alibabacloud_eais20190624_py2-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624/client.py` & `alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -111,14 +111,48 @@
             self.call_api(params, req, runtime)
         )
 
     def attach_eai(self, request):
         runtime = util_models.RuntimeOptions()
         return self.attach_eai_with_options(request, runtime)
 
+    def attach_eais_ei_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.client_instance_id):
+            query['ClientInstanceId'] = request.client_instance_id
+        if not UtilClient.is_unset(request.ei_instance_id):
+            query['EiInstanceId'] = request.ei_instance_id
+        if not UtilClient.is_unset(request.ei_instance_type):
+            query['EiInstanceType'] = request.ei_instance_type
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AttachEaisEi',
+            version='2019-06-24',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            eais_20190624_models.AttachEaisEiResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def attach_eais_ei(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.attach_eais_ei_with_options(request, runtime)
+
     def change_resource_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.resource_id):
             query['ResourceId'] = request.resource_id
@@ -148,14 +182,16 @@
         return self.change_resource_group_with_options(request, runtime)
 
     def create_eai_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.image):
+            query['Image'] = request.image
         if not UtilClient.is_unset(request.instance_name):
             query['InstanceName'] = request.instance_name
         if not UtilClient.is_unset(request.instance_type):
             query['InstanceType'] = request.instance_type
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -362,14 +398,16 @@
         request = eais_20190624_models.CreateEaiJupyterShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.environment_var):
             request.environment_var_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.environment_var, 'EnvironmentVar', 'json')
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.eais_name):
+            query['EaisName'] = request.eais_name
         if not UtilClient.is_unset(request.eais_type):
             query['EaisType'] = request.eais_type
         if not UtilClient.is_unset(request.environment_var_shrink):
             query['EnvironmentVar'] = request.environment_var_shrink
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -397,14 +435,54 @@
             self.call_api(params, req, runtime)
         )
 
     def create_eai_jupyter(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_eai_jupyter_with_options(request, runtime)
 
+    def create_eais_ei_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.instance_name):
+            query['InstanceName'] = request.instance_name
+        if not UtilClient.is_unset(request.instance_type):
+            query['InstanceType'] = request.instance_type
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.security_group_id):
+            query['SecurityGroupId'] = request.security_group_id
+        if not UtilClient.is_unset(request.v_switch_id):
+            query['VSwitchId'] = request.v_switch_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateEaisEi',
+            version='2019-06-24',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            eais_20190624_models.CreateEaisEiResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def create_eais_ei(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_eais_ei_with_options(request, runtime)
+
     def delete_eai_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.elastic_accelerated_instance_id):
             query['ElasticAcceleratedInstanceId'] = request.elastic_accelerated_instance_id
         if not UtilClient.is_unset(request.force):
             query['Force'] = request.force
@@ -461,14 +539,46 @@
             self.call_api(params, req, runtime)
         )
 
     def delete_eai_all(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_eai_all_with_options(request, runtime)
 
+    def delete_eais_ei_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.ei_instance_id):
+            query['EiInstanceId'] = request.ei_instance_id
+        if not UtilClient.is_unset(request.force):
+            query['Force'] = request.force
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteEaisEi',
+            version='2019-06-24',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            eais_20190624_models.DeleteEaisEiResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def delete_eais_ei(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_eais_ei_with_options(request, runtime)
+
     def describe_eais_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.elastic_accelerated_instance_ids):
             query['ElasticAcceleratedInstanceIds'] = request.elastic_accelerated_instance_ids
         if not UtilClient.is_unset(request.instance_name):
             query['InstanceName'] = request.instance_name
@@ -555,23 +665,55 @@
             self.call_api(params, req, runtime)
         )
 
     def detach_eai(self, request):
         runtime = util_models.RuntimeOptions()
         return self.detach_eai_with_options(request, runtime)
 
+    def detach_eais_ei_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.ei_instance_id):
+            query['EiInstanceId'] = request.ei_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DetachEaisEi',
+            version='2019-06-24',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            eais_20190624_models.DetachEaisEiResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def detach_eais_ei(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.detach_eais_ei_with_options(request, runtime)
+
     def get_instance_metrics_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.metric_type):
             query['MetricType'] = request.metric_type
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.start_time):
             query['StartTime'] = request.start_time
         if not UtilClient.is_unset(request.time_step):
             query['TimeStep'] = request.time_step
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -590,7 +732,67 @@
             eais_20190624_models.GetInstanceMetricsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def get_instance_metrics(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_instance_metrics_with_options(request, runtime)
+
+    def start_eais_ei_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.ei_instance_id):
+            query['EiInstanceId'] = request.ei_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='StartEaisEi',
+            version='2019-06-24',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            eais_20190624_models.StartEaisEiResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def start_eais_ei(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.start_eais_ei_with_options(request, runtime)
+
+    def stop_eais_ei_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.ei_instance_id):
+            query['EiInstanceId'] = request.ei_instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='StopEaisEi',
+            version='2019-06-24',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            eais_20190624_models.StopEaisEiResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def stop_eais_ei(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.stop_eais_ei_with_options(request, runtime)
```

### Comparing `alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624/models.py` & `alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -254,5075 +254,6401 @@
 00000fd0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
 00000fe0: 4174 7461 6368 4561 6952 6573 706f 6e73  AttachEaiRespons
 00000ff0: 6542 6f64 7928 290a 2020 2020 2020 2020  eBody().        
 00001000: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
 00001010: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
 00001020: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
 00001030: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00001040: 6c66 0a0a 0a63 6c61 7373 2043 6861 6e67  lf...class Chang
-00001050: 6552 6573 6f75 7263 6547 726f 7570 5265  eResourceGroupRe
-00001060: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-00001070: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00001080: 5f28 7365 6c66 2c20 7265 736f 7572 6365  _(self, resource
-00001090: 5f67 726f 7570 5f69 643d 4e6f 6e65 2c20  _group_id=None, 
-000010a0: 7265 736f 7572 6365 5f69 643d 4e6f 6e65  resource_id=None
-000010b0: 2c20 7265 736f 7572 6365 5f72 6567 696f  , resource_regio
-000010c0: 6e5f 6964 3d4e 6f6e 6529 3a0a 2020 2020  n_id=None):.    
-000010d0: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
-000010e0: 655f 6772 6f75 705f 6964 203d 2072 6573  e_group_id = res
-000010f0: 6f75 7263 655f 6772 6f75 705f 6964 2020  ource_group_id  
-00001100: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00001110: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
-00001120: 655f 6964 203d 2072 6573 6f75 7263 655f  e_id = resource_
-00001130: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-00001140: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00001150: 6f75 7263 655f 7265 6769 6f6e 5f69 6420  ource_region_id 
-00001160: 3d20 7265 736f 7572 6365 5f72 6567 696f  = resource_regio
-00001170: 6e5f 6964 2020 2320 7479 7065 3a20 7374  n_id  # type: st
-00001180: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
-00001190: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000011a0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-000011b0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-000011c0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-000011d0: 7065 7228 4368 616e 6765 5265 736f 7572  per(ChangeResour
-000011e0: 6365 4772 6f75 7052 6571 7565 7374 2c20  ceGroupRequest, 
-000011f0: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
-00001200: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00001210: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00001220: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00001230: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00001240: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00001250: 2020 2020 2069 6620 7365 6c66 2e72 6573       if self.res
-00001260: 6f75 7263 655f 6772 6f75 705f 6964 2069  ource_group_id i
-00001270: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00001280: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00001290: 5265 736f 7572 6365 4772 6f75 7049 6427  ResourceGroupId'
-000012a0: 5d20 3d20 7365 6c66 2e72 6573 6f75 7263  ] = self.resourc
-000012b0: 655f 6772 6f75 705f 6964 0a20 2020 2020  e_group_id.     
-000012c0: 2020 2069 6620 7365 6c66 2e72 6573 6f75     if self.resou
-000012d0: 7263 655f 6964 2069 7320 6e6f 7420 4e6f  rce_id is not No
-000012e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000012f0: 7265 7375 6c74 5b27 5265 736f 7572 6365  result['Resource
-00001300: 4964 275d 203d 2073 656c 662e 7265 736f  Id'] = self.reso
-00001310: 7572 6365 5f69 640a 2020 2020 2020 2020  urce_id.        
-00001320: 6966 2073 656c 662e 7265 736f 7572 6365  if self.resource
-00001330: 5f72 6567 696f 6e5f 6964 2069 7320 6e6f  _region_id is no
-00001340: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00001350: 2020 2020 7265 7375 6c74 5b27 5265 736f      result['Reso
-00001360: 7572 6365 5265 6769 6f6e 4964 275d 203d  urceRegionId'] =
-00001370: 2073 656c 662e 7265 736f 7572 6365 5f72   self.resource_r
-00001380: 6567 696f 6e5f 6964 0a20 2020 2020 2020  egion_id.       
-00001390: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000013a0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000013b0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-000013c0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-000013d0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000013e0: 6966 206d 2e67 6574 2827 5265 736f 7572  if m.get('Resour
-000013f0: 6365 4772 6f75 7049 6427 2920 6973 206e  ceGroupId') is n
-00001400: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00001410: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
-00001420: 6365 5f67 726f 7570 5f69 6420 3d20 6d2e  ce_group_id = m.
-00001430: 6765 7428 2752 6573 6f75 7263 6547 726f  get('ResourceGro
-00001440: 7570 4964 2729 0a20 2020 2020 2020 2069  upId').        i
-00001450: 6620 6d2e 6765 7428 2752 6573 6f75 7263  f m.get('Resourc
-00001460: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
-00001470: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00001480: 656c 662e 7265 736f 7572 6365 5f69 6420  elf.resource_id 
-00001490: 3d20 6d2e 6765 7428 2752 6573 6f75 7263  = m.get('Resourc
-000014a0: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
-000014b0: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
-000014c0: 5265 6769 6f6e 4964 2729 2069 7320 6e6f  RegionId') is no
-000014d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000014e0: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
-000014f0: 655f 7265 6769 6f6e 5f69 6420 3d20 6d2e  e_region_id = m.
-00001500: 6765 7428 2752 6573 6f75 7263 6552 6567  get('ResourceReg
-00001510: 696f 6e49 6427 290a 2020 2020 2020 2020  ionId').        
-00001520: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00001530: 6173 7320 4368 616e 6765 5265 736f 7572  ass ChangeResour
-00001540: 6365 4772 6f75 7052 6573 706f 6e73 6542  ceGroupResponseB
-00001550: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
-00001560: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00001570: 7365 6c66 2c20 7265 7175 6573 745f 6964  self, request_id
-00001580: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00001590: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-000015a0: 3d20 7265 7175 6573 745f 6964 2020 2320  = request_id  # 
-000015b0: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
-000015c0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000015d0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-000015e0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-000015f0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00001600: 6d61 7020 3d20 7375 7065 7228 4368 616e  map = super(Chan
-00001610: 6765 5265 736f 7572 6365 4772 6f75 7052  geResourceGroupR
-00001620: 6573 706f 6e73 6542 6f64 792c 2073 656c  esponseBody, sel
-00001630: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-00001640: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00001650: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00001660: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00001670: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00001680: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00001690: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-000016a0: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-000016b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000016c0: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
-000016d0: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
-000016e0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-000016f0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00001700: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00001710: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-00001720: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00001730: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00001740: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-00001750: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00001760: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00001770: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
-00001780: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
-00001790: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000017a0: 6c66 0a0a 0a63 6c61 7373 2043 6861 6e67  lf...class Chang
-000017b0: 6552 6573 6f75 7263 6547 726f 7570 5265  eResourceGroupRe
-000017c0: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-000017d0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000017e0: 5f5f 2873 656c 662c 2068 6561 6465 7273  __(self, headers
-000017f0: 3d4e 6f6e 652c 2073 7461 7475 735f 636f  =None, status_co
-00001800: 6465 3d4e 6f6e 652c 2062 6f64 793d 4e6f  de=None, body=No
-00001810: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
-00001820: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-00001830: 6572 7320 2023 2074 7970 653a 2064 6963  ers  # type: dic
-00001840: 745b 7374 722c 2073 7472 5d0a 2020 2020  t[str, str].    
-00001850: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-00001860: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
-00001870: 6465 2020 2320 7479 7065 3a20 696e 740a  de  # type: int.
-00001880: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00001890: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
-000018a0: 3a20 4368 616e 6765 5265 736f 7572 6365  : ChangeResource
-000018b0: 4772 6f75 7052 6573 706f 6e73 6542 6f64  GroupResponseBod
-000018c0: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-000018d0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-000018e0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-000018f0: 5f72 6571 7569 7265 6428 7365 6c66 2e68  _required(self.h
-00001900: 6561 6465 7273 2c20 2768 6561 6465 7273  eaders, 'headers
-00001910: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00001920: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-00001930: 6428 7365 6c66 2e73 7461 7475 735f 636f  d(self.status_co
-00001940: 6465 2c20 2773 7461 7475 735f 636f 6465  de, 'status_code
-00001950: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00001960: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-00001970: 6428 7365 6c66 2e62 6f64 792c 2027 626f  d(self.body, 'bo
-00001980: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
-00001990: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-000019a0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-000019b0: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-000019c0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-000019d0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-000019e0: 3d20 7375 7065 7228 4368 616e 6765 5265  = super(ChangeRe
-000019f0: 736f 7572 6365 4772 6f75 7052 6573 706f  sourceGroupRespo
-00001a00: 6e73 652c 2073 656c 6629 2e74 6f5f 6d61  nse, self).to_ma
-00001a10: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00001a20: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00001a30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001a40: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00001a50: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00001a60: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00001a70: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-00001a80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00001a90: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-00001aa0: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-00001ab0: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-00001ac0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00001ad0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00001ae0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00001af0: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-00001b00: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00001b10: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00001b20: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-00001b30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00001b40: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-00001b50: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-00001b60: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00001b70: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00001b80: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00001b90: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-00001ba0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00001bb0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00001bc0: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-00001bd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00001be0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00001bf0: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-00001c00: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-00001c10: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-00001c20: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-00001c30: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00001c40: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00001c50: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-00001c60: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-00001c70: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-00001c80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00001c90: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-00001ca0: 656c 203d 2043 6861 6e67 6552 6573 6f75  el = ChangeResou
-00001cb0: 7263 6547 726f 7570 5265 7370 6f6e 7365  rceGroupResponse
-00001cc0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
-00001cd0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-00001ce0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-00001cf0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-00001d00: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001d10: 660a 0a0a 636c 6173 7320 4372 6561 7465  f...class Create
-00001d20: 4561 6952 6571 7565 7374 2854 6561 4d6f  EaiRequest(TeaMo
-00001d30: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00001d40: 696e 6974 5f5f 2873 656c 662c 2063 6c69  init__(self, cli
-00001d50: 656e 745f 746f 6b65 6e3d 4e6f 6e65 2c20  ent_token=None, 
-00001d60: 696e 7374 616e 6365 5f6e 616d 653d 4e6f  instance_name=No
-00001d70: 6e65 2c20 696e 7374 616e 6365 5f74 7970  ne, instance_typ
-00001d80: 653d 4e6f 6e65 2c20 7265 6769 6f6e 5f69  e=None, region_i
-00001d90: 643d 4e6f 6e65 2c0a 2020 2020 2020 2020  d=None,.        
-00001da0: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
-00001db0: 655f 6772 6f75 705f 6964 3d4e 6f6e 652c  e_group_id=None,
-00001dc0: 2073 6563 7572 6974 795f 6772 6f75 705f   security_group_
-00001dd0: 6964 3d4e 6f6e 652c 2076 5f73 7769 7463  id=None, v_switc
-00001de0: 685f 6964 3d4e 6f6e 6529 3a0a 2020 2020  h_id=None):.    
-00001df0: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
-00001e00: 746f 6b65 6e20 3d20 636c 6965 6e74 5f74  token = client_t
-00001e10: 6f6b 656e 2020 2320 7479 7065 3a20 7374  oken  # type: st
-00001e20: 720a 2020 2020 2020 2020 7365 6c66 2e69  r.        self.i
-00001e30: 6e73 7461 6e63 655f 6e61 6d65 203d 2069  nstance_name = i
-00001e40: 6e73 7461 6e63 655f 6e61 6d65 2020 2320  nstance_name  # 
-00001e50: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-00001e60: 2020 7365 6c66 2e69 6e73 7461 6e63 655f    self.instance_
-00001e70: 7479 7065 203d 2069 6e73 7461 6e63 655f  type = instance_
-00001e80: 7479 7065 2020 2320 7479 7065 3a20 7374  type  # type: st
-00001e90: 720a 2020 2020 2020 2020 7365 6c66 2e72  r.        self.r
-00001ea0: 6567 696f 6e5f 6964 203d 2072 6567 696f  egion_id = regio
-00001eb0: 6e5f 6964 2020 2320 7479 7065 3a20 7374  n_id  # type: st
-00001ec0: 720a 2020 2020 2020 2020 7365 6c66 2e72  r.        self.r
-00001ed0: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-00001ee0: 203d 2072 6573 6f75 7263 655f 6772 6f75   = resource_grou
-00001ef0: 705f 6964 2020 2320 7479 7065 3a20 7374  p_id  # type: st
-00001f00: 720a 2020 2020 2020 2020 7365 6c66 2e73  r.        self.s
-00001f10: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
-00001f20: 203d 2073 6563 7572 6974 795f 6772 6f75   = security_grou
-00001f30: 705f 6964 2020 2320 7479 7065 3a20 7374  p_id  # type: st
-00001f40: 720a 2020 2020 2020 2020 7365 6c66 2e76  r.        self.v
-00001f50: 5f73 7769 7463 685f 6964 203d 2076 5f73  _switch_id = v_s
-00001f60: 7769 7463 685f 6964 2020 2320 7479 7065  witch_id  # type
-00001f70: 3a20 7374 720a 0a20 2020 2064 6566 2076  : str..    def v
-00001f80: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-00001f90: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00001fa0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-00001fb0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-00001fc0: 3d20 7375 7065 7228 4372 6561 7465 4561  = super(CreateEa
-00001fd0: 6952 6571 7565 7374 2c20 7365 6c66 292e  iRequest, self).
-00001fe0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00001ff0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00002000: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00002010: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00002020: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00002030: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00002040: 6620 7365 6c66 2e63 6c69 656e 745f 746f  f self.client_to
-00002050: 6b65 6e20 6973 206e 6f74 204e 6f6e 653a  ken is not None:
-00002060: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00002070: 756c 745b 2743 6c69 656e 7454 6f6b 656e  ult['ClientToken
-00002080: 275d 203d 2073 656c 662e 636c 6965 6e74  '] = self.client
-00002090: 5f74 6f6b 656e 0a20 2020 2020 2020 2069  _token.        i
-000020a0: 6620 7365 6c66 2e69 6e73 7461 6e63 655f  f self.instance_
-000020b0: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-000020c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000020d0: 7375 6c74 5b27 496e 7374 616e 6365 4e61  sult['InstanceNa
-000020e0: 6d65 275d 203d 2073 656c 662e 696e 7374  me'] = self.inst
-000020f0: 616e 6365 5f6e 616d 650a 2020 2020 2020  ance_name.      
-00002100: 2020 6966 2073 656c 662e 696e 7374 616e    if self.instan
-00002110: 6365 5f74 7970 6520 6973 206e 6f74 204e  ce_type is not N
-00002120: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002130: 2072 6573 756c 745b 2749 6e73 7461 6e63   result['Instanc
-00002140: 6554 7970 6527 5d20 3d20 7365 6c66 2e69  eType'] = self.i
-00002150: 6e73 7461 6e63 655f 7479 7065 0a20 2020  nstance_type.   
-00002160: 2020 2020 2069 6620 7365 6c66 2e72 6567       if self.reg
-00002170: 696f 6e5f 6964 2069 7320 6e6f 7420 4e6f  ion_id is not No
-00002180: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002190: 7265 7375 6c74 5b27 5265 6769 6f6e 4964  result['RegionId
-000021a0: 275d 203d 2073 656c 662e 7265 6769 6f6e  '] = self.region
-000021b0: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-000021c0: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
-000021d0: 7570 5f69 6420 6973 206e 6f74 204e 6f6e  up_id is not Non
-000021e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000021f0: 6573 756c 745b 2752 6573 6f75 7263 6547  esult['ResourceG
-00002200: 726f 7570 4964 275d 203d 2073 656c 662e  roupId'] = self.
-00002210: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-00002220: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00002230: 662e 7365 6375 7269 7479 5f67 726f 7570  f.security_group
-00002240: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00002250: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00002260: 756c 745b 2753 6563 7572 6974 7947 726f  ult['SecurityGro
-00002270: 7570 4964 275d 203d 2073 656c 662e 7365  upId'] = self.se
-00002280: 6375 7269 7479 5f67 726f 7570 5f69 640a  curity_group_id.
-00002290: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000022a0: 765f 7377 6974 6368 5f69 6420 6973 206e  v_switch_id is n
-000022b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000022c0: 2020 2020 2072 6573 756c 745b 2756 5377       result['VSw
-000022d0: 6974 6368 4964 275d 203d 2073 656c 662e  itchId'] = self.
-000022e0: 765f 7377 6974 6368 5f69 640a 2020 2020  v_switch_id.    
-000022f0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00002300: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00002310: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-00002320: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00002330: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00002340: 2020 2069 6620 6d2e 6765 7428 2743 6c69     if m.get('Cli
-00002350: 656e 7454 6f6b 656e 2729 2069 7320 6e6f  entToken') is no
-00002360: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002370: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
-00002380: 746f 6b65 6e20 3d20 6d2e 6765 7428 2743  token = m.get('C
-00002390: 6c69 656e 7454 6f6b 656e 2729 0a20 2020  lientToken').   
-000023a0: 2020 2020 2069 6620 6d2e 6765 7428 2749       if m.get('I
-000023b0: 6e73 7461 6e63 654e 616d 6527 2920 6973  nstanceName') is
-000023c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000023d0: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
-000023e0: 616e 6365 5f6e 616d 6520 3d20 6d2e 6765  ance_name = m.ge
-000023f0: 7428 2749 6e73 7461 6e63 654e 616d 6527  t('InstanceName'
-00002400: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00002410: 6574 2827 496e 7374 616e 6365 5479 7065  et('InstanceType
-00002420: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00002430: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002440: 2e69 6e73 7461 6e63 655f 7479 7065 203d  .instance_type =
-00002450: 206d 2e67 6574 2827 496e 7374 616e 6365   m.get('Instance
-00002460: 5479 7065 2729 0a20 2020 2020 2020 2069  Type').        i
-00002470: 6620 6d2e 6765 7428 2752 6567 696f 6e49  f m.get('RegionI
-00002480: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00002490: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000024a0: 662e 7265 6769 6f6e 5f69 6420 3d20 6d2e  f.region_id = m.
-000024b0: 6765 7428 2752 6567 696f 6e49 6427 290a  get('RegionId').
-000024c0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000024d0: 2827 5265 736f 7572 6365 4772 6f75 7049  ('ResourceGroupI
-000024e0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-000024f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002500: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
-00002510: 5f69 6420 3d20 6d2e 6765 7428 2752 6573  _id = m.get('Res
-00002520: 6f75 7263 6547 726f 7570 4964 2729 0a20  ourceGroupId'). 
-00002530: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00002540: 2753 6563 7572 6974 7947 726f 7570 4964  'SecurityGroupId
-00002550: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00002560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002570: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
-00002580: 6964 203d 206d 2e67 6574 2827 5365 6375  id = m.get('Secu
-00002590: 7269 7479 4772 6f75 7049 6427 290a 2020  rityGroupId').  
-000025a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000025b0: 5653 7769 7463 6849 6427 2920 6973 206e  VSwitchId') is n
-000025c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000025d0: 2020 2020 2073 656c 662e 765f 7377 6974       self.v_swit
-000025e0: 6368 5f69 6420 3d20 6d2e 6765 7428 2756  ch_id = m.get('V
-000025f0: 5377 6974 6368 4964 2729 0a20 2020 2020  SwitchId').     
-00002600: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00002610: 0a63 6c61 7373 2043 7265 6174 6545 6169  .class CreateEai
-00002620: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
-00002630: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00002640: 5f5f 696e 6974 5f5f 2873 656c 662c 2065  __init__(self, e
-00002650: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
-00002660: 6564 5f69 6e73 7461 6e63 655f 6964 3d4e  ed_instance_id=N
-00002670: 6f6e 652c 2072 6571 7565 7374 5f69 643d  one, request_id=
-00002680: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-00002690: 656c 662e 656c 6173 7469 635f 6163 6365  elf.elastic_acce
-000026a0: 6c65 7261 7465 645f 696e 7374 616e 6365  lerated_instance
-000026b0: 5f69 6420 3d20 656c 6173 7469 635f 6163  _id = elastic_ac
-000026c0: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
-000026d0: 6365 5f69 6420 2023 2074 7970 653a 2073  ce_id  # type: s
-000026e0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-000026f0: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
-00002700: 7565 7374 5f69 6420 2023 2074 7970 653a  uest_id  # type:
-00002710: 2073 7472 0a0a 2020 2020 6465 6620 7661   str..    def va
-00002720: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-00002730: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00002740: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-00002750: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-00002760: 2073 7570 6572 2843 7265 6174 6545 6169   super(CreateEai
-00002770: 5265 7370 6f6e 7365 426f 6479 2c20 7365  ResponseBody, se
-00002780: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
-00002790: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-000027a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000027b0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-000027c0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-000027d0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-000027e0: 2020 2069 6620 7365 6c66 2e65 6c61 7374     if self.elast
-000027f0: 6963 5f61 6363 656c 6572 6174 6564 5f69  ic_accelerated_i
-00002800: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
-00002810: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002820: 2020 2020 7265 7375 6c74 5b27 456c 6173      result['Elas
-00002830: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
-00002840: 7374 616e 6365 4964 275d 203d 2073 656c  stanceId'] = sel
-00002850: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-00002860: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-00002870: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00002880: 662e 7265 7175 6573 745f 6964 2069 7320  f.request_id is 
-00002890: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000028a0: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-000028b0: 7175 6573 7449 6427 5d20 3d20 7365 6c66  questId'] = self
-000028c0: 2e72 6571 7565 7374 5f69 640a 2020 2020  .request_id.    
-000028d0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-000028e0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-000028f0: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-00002900: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00002910: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00002920: 2020 2069 6620 6d2e 6765 7428 2745 6c61     if m.get('Ela
-00002930: 7374 6963 4163 6365 6c65 7261 7465 6449  sticAcceleratedI
-00002940: 6e73 7461 6e63 6549 6427 2920 6973 206e  nstanceId') is n
-00002950: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00002960: 2020 2020 2073 656c 662e 656c 6173 7469       self.elasti
-00002970: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
-00002980: 7374 616e 6365 5f69 6420 3d20 6d2e 6765  stance_id = m.ge
-00002990: 7428 2745 6c61 7374 6963 4163 6365 6c65  t('ElasticAccele
-000029a0: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
-000029b0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000029c0: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
-000029d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000029e0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-000029f0: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
-00002a00: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
-00002a10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00002a20: 660a 0a0a 636c 6173 7320 4372 6561 7465  f...class Create
-00002a30: 4561 6952 6573 706f 6e73 6528 5465 614d  EaiResponse(TeaM
-00002a40: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-00002a50: 5f69 6e69 745f 5f28 7365 6c66 2c20 6865  _init__(self, he
-00002a60: 6164 6572 733d 4e6f 6e65 2c20 7374 6174  aders=None, stat
-00002a70: 7573 5f63 6f64 653d 4e6f 6e65 2c20 626f  us_code=None, bo
-00002a80: 6479 3d4e 6f6e 6529 3a0a 2020 2020 2020  dy=None):.      
-00002a90: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-00002aa0: 2068 6561 6465 7273 2020 2320 7479 7065   headers  # type
-00002ab0: 3a20 6469 6374 5b73 7472 2c20 7374 725d  : dict[str, str]
-00002ac0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-00002ad0: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
-00002ae0: 7573 5f63 6f64 6520 2023 2074 7970 653a  us_code  # type:
-00002af0: 2069 6e74 0a20 2020 2020 2020 2073 656c   int.        sel
-00002b00: 662e 626f 6479 203d 2062 6f64 7920 2023  f.body = body  #
-00002b10: 2074 7970 653a 2043 7265 6174 6545 6169   type: CreateEai
-00002b20: 5265 7370 6f6e 7365 426f 6479 0a0a 2020  ResponseBody..  
-00002b30: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00002b40: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-00002b50: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-00002b60: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
-00002b70: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
-00002b80: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-00002b90: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-00002ba0: 662e 7374 6174 7573 5f63 6f64 652c 2027  f.status_code, '
-00002bb0: 7374 6174 7573 5f63 6f64 6527 290a 2020  status_code').  
-00002bc0: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-00002bd0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-00002be0: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
-00002bf0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00002c00: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-00002c10: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-00002c20: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-00002c30: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00002c40: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00002c50: 6572 2843 7265 6174 6545 6169 5265 7370  er(CreateEaiResp
-00002c60: 6f6e 7365 2c20 7365 6c66 292e 746f 5f6d  onse, self).to_m
-00002c70: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00002c80: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00002c90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00002ca0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00002cb0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00002cc0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00002cd0: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-00002ce0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002cf0: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-00002d00: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-00002d10: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-00002d20: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00002d30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00002d40: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00002d50: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-00002d60: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00002d70: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00002d80: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-00002d90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002da0: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-00002db0: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-00002dc0: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-00002dd0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00002de0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00002df0: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-00002e00: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00002e10: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00002e20: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-00002e30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00002e40: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00002e50: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-00002e60: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-00002e70: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-00002e80: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-00002e90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002ea0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00002eb0: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-00002ec0: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-00002ed0: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-00002ee0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00002ef0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-00002f00: 6465 6c20 3d20 4372 6561 7465 4561 6952  del = CreateEaiR
-00002f10: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
-00002f20: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00002f30: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
-00002f40: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
-00002f50: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
-00002f60: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-00002f70: 2043 7265 6174 6545 6169 416c 6c52 6571   CreateEaiAllReq
-00002f80: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
-00002f90: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00002fa0: 2873 656c 662c 2063 6c69 656e 745f 696d  (self, client_im
-00002fb0: 6167 655f 6964 3d4e 6f6e 652c 2063 6c69  age_id=None, cli
-00002fc0: 656e 745f 696e 7374 616e 6365 5f6e 616d  ent_instance_nam
-00002fd0: 653d 4e6f 6e65 2c20 636c 6965 6e74 5f69  e=None, client_i
-00002fe0: 6e73 7461 6e63 655f 7479 7065 3d4e 6f6e  nstance_type=Non
-00002ff0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00003000: 2020 2020 636c 6965 6e74 5f69 6e74 6572      client_inter
-00003010: 6e65 745f 6d61 785f 6261 6e64 7769 6474  net_max_bandwidt
-00003020: 685f 696e 3d4e 6f6e 652c 2063 6c69 656e  h_in=None, clien
-00003030: 745f 696e 7465 726e 6574 5f6d 6178 5f62  t_internet_max_b
-00003040: 616e 6477 6964 7468 5f6f 7574 3d4e 6f6e  andwidth_out=Non
-00003050: 652c 2063 6c69 656e 745f 7061 7373 776f  e, client_passwo
-00003060: 7264 3d4e 6f6e 652c 0a20 2020 2020 2020  rd=None,.       
-00003070: 2020 2020 2020 2020 2020 636c 6965 6e74            client
-00003080: 5f73 6563 7572 6974 795f 6772 6f75 705f  _security_group_
-00003090: 6964 3d4e 6f6e 652c 2063 6c69 656e 745f  id=None, client_
-000030a0: 7379 7374 656d 5f64 6973 6b5f 6361 7465  system_disk_cate
-000030b0: 676f 7279 3d4e 6f6e 652c 2063 6c69 656e  gory=None, clien
-000030c0: 745f 7379 7374 656d 5f64 6973 6b5f 7369  t_system_disk_si
-000030d0: 7a65 3d4e 6f6e 652c 2063 6c69 656e 745f  ze=None, client_
-000030e0: 746f 6b65 6e3d 4e6f 6e65 2c0a 2020 2020  token=None,.    
-000030f0: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
-00003100: 656e 745f 7673 7769 7463 685f 6964 3d4e  ent_vswitch_id=N
-00003110: 6f6e 652c 2063 6c69 656e 745f 7a6f 6e65  one, client_zone
-00003120: 5f69 643d 4e6f 6e65 2c20 6561 695f 696e  _id=None, eai_in
-00003130: 7374 616e 6365 5f74 7970 653d 4e6f 6e65  stance_type=None
-00003140: 2c20 696e 7374 616e 6365 5f6e 616d 653d  , instance_name=
-00003150: 4e6f 6e65 2c20 7265 6769 6f6e 5f69 643d  None, region_id=
-00003160: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00003170: 2020 2020 2020 2072 6573 6f75 7263 655f         resource_
-00003180: 6772 6f75 705f 6964 3d4e 6f6e 6529 3a0a  group_id=None):.
-00003190: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-000031a0: 656e 745f 696d 6167 655f 6964 203d 2063  ent_image_id = c
-000031b0: 6c69 656e 745f 696d 6167 655f 6964 2020  lient_image_id  
-000031c0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-000031d0: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
-000031e0: 696e 7374 616e 6365 5f6e 616d 6520 3d20  instance_name = 
-000031f0: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
-00003200: 6e61 6d65 2020 2320 7479 7065 3a20 7374  name  # type: st
-00003210: 720a 2020 2020 2020 2020 7365 6c66 2e63  r.        self.c
-00003220: 6c69 656e 745f 696e 7374 616e 6365 5f74  lient_instance_t
-00003230: 7970 6520 3d20 636c 6965 6e74 5f69 6e73  ype = client_ins
-00003240: 7461 6e63 655f 7479 7065 2020 2320 7479  tance_type  # ty
-00003250: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-00003260: 7365 6c66 2e63 6c69 656e 745f 696e 7465  self.client_inte
-00003270: 726e 6574 5f6d 6178 5f62 616e 6477 6964  rnet_max_bandwid
-00003280: 7468 5f69 6e20 3d20 636c 6965 6e74 5f69  th_in = client_i
-00003290: 6e74 6572 6e65 745f 6d61 785f 6261 6e64  nternet_max_band
-000032a0: 7769 6474 685f 696e 2020 2320 7479 7065  width_in  # type
-000032b0: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
-000032c0: 6c66 2e63 6c69 656e 745f 696e 7465 726e  lf.client_intern
-000032d0: 6574 5f6d 6178 5f62 616e 6477 6964 7468  et_max_bandwidth
-000032e0: 5f6f 7574 203d 2063 6c69 656e 745f 696e  _out = client_in
-000032f0: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
-00003300: 6964 7468 5f6f 7574 2020 2320 7479 7065  idth_out  # type
-00003310: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
-00003320: 6c66 2e63 6c69 656e 745f 7061 7373 776f  lf.client_passwo
-00003330: 7264 203d 2063 6c69 656e 745f 7061 7373  rd = client_pass
-00003340: 776f 7264 2020 2320 7479 7065 3a20 7374  word  # type: st
-00003350: 720a 2020 2020 2020 2020 7365 6c66 2e63  r.        self.c
-00003360: 6c69 656e 745f 7365 6375 7269 7479 5f67  lient_security_g
-00003370: 726f 7570 5f69 6420 3d20 636c 6965 6e74  roup_id = client
-00003380: 5f73 6563 7572 6974 795f 6772 6f75 705f  _security_group_
-00003390: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-000033a0: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-000033b0: 656e 745f 7379 7374 656d 5f64 6973 6b5f  ent_system_disk_
-000033c0: 6361 7465 676f 7279 203d 2063 6c69 656e  category = clien
-000033d0: 745f 7379 7374 656d 5f64 6973 6b5f 6361  t_system_disk_ca
-000033e0: 7465 676f 7279 2020 2320 7479 7065 3a20  tegory  # type: 
-000033f0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-00003400: 2e63 6c69 656e 745f 7379 7374 656d 5f64  .client_system_d
-00003410: 6973 6b5f 7369 7a65 203d 2063 6c69 656e  isk_size = clien
-00003420: 745f 7379 7374 656d 5f64 6973 6b5f 7369  t_system_disk_si
-00003430: 7a65 2020 2320 7479 7065 3a20 696e 740a  ze  # type: int.
-00003440: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-00003450: 656e 745f 746f 6b65 6e20 3d20 636c 6965  ent_token = clie
-00003460: 6e74 5f74 6f6b 656e 2020 2320 7479 7065  nt_token  # type
-00003470: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-00003480: 6c66 2e63 6c69 656e 745f 7673 7769 7463  lf.client_vswitc
-00003490: 685f 6964 203d 2063 6c69 656e 745f 7673  h_id = client_vs
-000034a0: 7769 7463 685f 6964 2020 2320 7479 7065  witch_id  # type
-000034b0: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-000034c0: 6c66 2e63 6c69 656e 745f 7a6f 6e65 5f69  lf.client_zone_i
-000034d0: 6420 3d20 636c 6965 6e74 5f7a 6f6e 655f  d = client_zone_
-000034e0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-000034f0: 2020 2020 2020 2020 7365 6c66 2e65 6169          self.eai
-00003500: 5f69 6e73 7461 6e63 655f 7479 7065 203d  _instance_type =
-00003510: 2065 6169 5f69 6e73 7461 6e63 655f 7479   eai_instance_ty
-00003520: 7065 2020 2320 7479 7065 3a20 7374 720a  pe  # type: str.
-00003530: 2020 2020 2020 2020 7365 6c66 2e69 6e73          self.ins
-00003540: 7461 6e63 655f 6e61 6d65 203d 2069 6e73  tance_name = ins
-00003550: 7461 6e63 655f 6e61 6d65 2020 2320 7479  tance_name  # ty
-00003560: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-00003570: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
-00003580: 2072 6567 696f 6e5f 6964 2020 2320 7479   region_id  # ty
-00003590: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-000035a0: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
-000035b0: 6f75 705f 6964 203d 2072 6573 6f75 7263  oup_id = resourc
-000035c0: 655f 6772 6f75 705f 6964 2020 2320 7479  e_group_id  # ty
-000035d0: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
-000035e0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-000035f0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00003600: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00003610: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00003620: 7020 3d20 7375 7065 7228 4372 6561 7465  p = super(Create
-00003630: 4561 6941 6c6c 5265 7175 6573 742c 2073  EaiAllRequest, s
-00003640: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
-00003650: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-00003660: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00003670: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-00003680: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-00003690: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-000036a0: 2020 2020 6966 2073 656c 662e 636c 6965      if self.clie
-000036b0: 6e74 5f69 6d61 6765 5f69 6420 6973 206e  nt_image_id is n
-000036c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000036d0: 2020 2020 2072 6573 756c 745b 2743 6c69       result['Cli
-000036e0: 656e 7449 6d61 6765 4964 275d 203d 2073  entImageId'] = s
-000036f0: 656c 662e 636c 6965 6e74 5f69 6d61 6765  elf.client_image
-00003700: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-00003710: 656c 662e 636c 6965 6e74 5f69 6e73 7461  elf.client_insta
-00003720: 6e63 655f 6e61 6d65 2069 7320 6e6f 7420  nce_name is not 
-00003730: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003740: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-00003750: 496e 7374 616e 6365 4e61 6d65 275d 203d  InstanceName'] =
-00003760: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
-00003770: 7461 6e63 655f 6e61 6d65 0a20 2020 2020  tance_name.     
-00003780: 2020 2069 6620 7365 6c66 2e63 6c69 656e     if self.clien
-00003790: 745f 696e 7374 616e 6365 5f74 7970 6520  t_instance_type 
-000037a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000037b0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000037c0: 2743 6c69 656e 7449 6e73 7461 6e63 6554  'ClientInstanceT
-000037d0: 7970 6527 5d20 3d20 7365 6c66 2e63 6c69  ype'] = self.cli
-000037e0: 656e 745f 696e 7374 616e 6365 5f74 7970  ent_instance_typ
-000037f0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00003800: 662e 636c 6965 6e74 5f69 6e74 6572 6e65  f.client_interne
-00003810: 745f 6d61 785f 6261 6e64 7769 6474 685f  t_max_bandwidth_
-00003820: 696e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  in is not None:.
-00003830: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00003840: 6c74 5b27 436c 6965 6e74 496e 7465 726e  lt['ClientIntern
-00003850: 6574 4d61 7842 616e 6477 6964 7468 496e  etMaxBandwidthIn
-00003860: 275d 203d 2073 656c 662e 636c 6965 6e74  '] = self.client
-00003870: 5f69 6e74 6572 6e65 745f 6d61 785f 6261  _internet_max_ba
-00003880: 6e64 7769 6474 685f 696e 0a20 2020 2020  ndwidth_in.     
-00003890: 2020 2069 6620 7365 6c66 2e63 6c69 656e     if self.clien
-000038a0: 745f 696e 7465 726e 6574 5f6d 6178 5f62  t_internet_max_b
-000038b0: 616e 6477 6964 7468 5f6f 7574 2069 7320  andwidth_out is 
-000038c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000038d0: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
-000038e0: 6965 6e74 496e 7465 726e 6574 4d61 7842  ientInternetMaxB
-000038f0: 616e 6477 6964 7468 4f75 7427 5d20 3d20  andwidthOut'] = 
-00003900: 7365 6c66 2e63 6c69 656e 745f 696e 7465  self.client_inte
-00003910: 726e 6574 5f6d 6178 5f62 616e 6477 6964  rnet_max_bandwid
-00003920: 7468 5f6f 7574 0a20 2020 2020 2020 2069  th_out.        i
-00003930: 6620 7365 6c66 2e63 6c69 656e 745f 7061  f self.client_pa
-00003940: 7373 776f 7264 2069 7320 6e6f 7420 4e6f  ssword is not No
-00003950: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00003960: 7265 7375 6c74 5b27 436c 6965 6e74 5061  result['ClientPa
-00003970: 7373 776f 7264 275d 203d 2073 656c 662e  ssword'] = self.
-00003980: 636c 6965 6e74 5f70 6173 7377 6f72 640a  client_password.
-00003990: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000039a0: 636c 6965 6e74 5f73 6563 7572 6974 795f  client_security_
-000039b0: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
-000039c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000039d0: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-000039e0: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
-000039f0: 5d20 3d20 7365 6c66 2e63 6c69 656e 745f  ] = self.client_
-00003a00: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
-00003a10: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00003a20: 662e 636c 6965 6e74 5f73 7973 7465 6d5f  f.client_system_
-00003a30: 6469 736b 5f63 6174 6567 6f72 7920 6973  disk_category is
-00003a40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00003a50: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
-00003a60: 6c69 656e 7453 7973 7465 6d44 6973 6b43  lientSystemDiskC
-00003a70: 6174 6567 6f72 7927 5d20 3d20 7365 6c66  ategory'] = self
-00003a80: 2e63 6c69 656e 745f 7379 7374 656d 5f64  .client_system_d
-00003a90: 6973 6b5f 6361 7465 676f 7279 0a20 2020  isk_category.   
-00003aa0: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
-00003ab0: 656e 745f 7379 7374 656d 5f64 6973 6b5f  ent_system_disk_
-00003ac0: 7369 7a65 2069 7320 6e6f 7420 4e6f 6e65  size is not None
-00003ad0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00003ae0: 7375 6c74 5b27 436c 6965 6e74 5379 7374  sult['ClientSyst
-00003af0: 656d 4469 736b 5369 7a65 275d 203d 2073  emDiskSize'] = s
-00003b00: 656c 662e 636c 6965 6e74 5f73 7973 7465  elf.client_syste
-00003b10: 6d5f 6469 736b 5f73 697a 650a 2020 2020  m_disk_size.    
-00003b20: 2020 2020 6966 2073 656c 662e 636c 6965      if self.clie
-00003b30: 6e74 5f74 6f6b 656e 2069 7320 6e6f 7420  nt_token is not 
-00003b40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003b50: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-00003b60: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e63  Token'] = self.c
-00003b70: 6c69 656e 745f 746f 6b65 6e0a 2020 2020  lient_token.    
-00003b80: 2020 2020 6966 2073 656c 662e 636c 6965      if self.clie
-00003b90: 6e74 5f76 7377 6974 6368 5f69 6420 6973  nt_vswitch_id is
-00003ba0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00003bb0: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
-00003bc0: 6c69 656e 7456 5377 6974 6368 4964 275d  lientVSwitchId']
-00003bd0: 203d 2073 656c 662e 636c 6965 6e74 5f76   = self.client_v
-00003be0: 7377 6974 6368 5f69 640a 2020 2020 2020  switch_id.      
-00003bf0: 2020 6966 2073 656c 662e 636c 6965 6e74    if self.client
-00003c00: 5f7a 6f6e 655f 6964 2069 7320 6e6f 7420  _zone_id is not 
-00003c10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003c20: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-00003c30: 5a6f 6e65 4964 275d 203d 2073 656c 662e  ZoneId'] = self.
-00003c40: 636c 6965 6e74 5f7a 6f6e 655f 6964 0a20  client_zone_id. 
-00003c50: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-00003c60: 6169 5f69 6e73 7461 6e63 655f 7479 7065  ai_instance_type
-00003c70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00003c80: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00003c90: 5b27 4561 6949 6e73 7461 6e63 6554 7970  ['EaiInstanceTyp
-00003ca0: 6527 5d20 3d20 7365 6c66 2e65 6169 5f69  e'] = self.eai_i
-00003cb0: 6e73 7461 6e63 655f 7479 7065 0a20 2020  nstance_type.   
-00003cc0: 2020 2020 2069 6620 7365 6c66 2e69 6e73       if self.ins
-00003cd0: 7461 6e63 655f 6e61 6d65 2069 7320 6e6f  tance_name is no
-00003ce0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00003cf0: 2020 2020 7265 7375 6c74 5b27 496e 7374      result['Inst
-00003d00: 616e 6365 4e61 6d65 275d 203d 2073 656c  anceName'] = sel
-00003d10: 662e 696e 7374 616e 6365 5f6e 616d 650a  f.instance_name.
-00003d20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003d30: 7265 6769 6f6e 5f69 6420 6973 206e 6f74  region_id is not
-00003d40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00003d50: 2020 2072 6573 756c 745b 2752 6567 696f     result['Regio
-00003d60: 6e49 6427 5d20 3d20 7365 6c66 2e72 6567  nId'] = self.reg
-00003d70: 696f 6e5f 6964 0a20 2020 2020 2020 2069  ion_id.        i
-00003d80: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
-00003d90: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
-00003da0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003db0: 2020 7265 7375 6c74 5b27 5265 736f 7572    result['Resour
-00003dc0: 6365 4772 6f75 7049 6427 5d20 3d20 7365  ceGroupId'] = se
-00003dd0: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
-00003de0: 705f 6964 0a20 2020 2020 2020 2072 6574  p_id.        ret
-00003df0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00003e00: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00003e10: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-00003e20: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-00003e30: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-00003e40: 2e67 6574 2827 436c 6965 6e74 496d 6167  .get('ClientImag
-00003e50: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
-00003e60: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00003e70: 656c 662e 636c 6965 6e74 5f69 6d61 6765  elf.client_image
-00003e80: 5f69 6420 3d20 6d2e 6765 7428 2743 6c69  _id = m.get('Cli
-00003e90: 656e 7449 6d61 6765 4964 2729 0a20 2020  entImageId').   
-00003ea0: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
-00003eb0: 6c69 656e 7449 6e73 7461 6e63 654e 616d  lientInstanceNam
-00003ec0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00003ed0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003ee0: 662e 636c 6965 6e74 5f69 6e73 7461 6e63  f.client_instanc
-00003ef0: 655f 6e61 6d65 203d 206d 2e67 6574 2827  e_name = m.get('
-00003f00: 436c 6965 6e74 496e 7374 616e 6365 4e61  ClientInstanceNa
-00003f10: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
-00003f20: 6d2e 6765 7428 2743 6c69 656e 7449 6e73  m.get('ClientIns
-00003f30: 7461 6e63 6554 7970 6527 2920 6973 206e  tanceType') is n
-00003f40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00003f50: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-00003f60: 5f69 6e73 7461 6e63 655f 7479 7065 203d  _instance_type =
-00003f70: 206d 2e67 6574 2827 436c 6965 6e74 496e   m.get('ClientIn
-00003f80: 7374 616e 6365 5479 7065 2729 0a20 2020  stanceType').   
-00003f90: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
-00003fa0: 6c69 656e 7449 6e74 6572 6e65 744d 6178  lientInternetMax
-00003fb0: 4261 6e64 7769 6474 6849 6e27 2920 6973  BandwidthIn') is
-00003fc0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00003fd0: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
-00003fe0: 6e74 5f69 6e74 6572 6e65 745f 6d61 785f  nt_internet_max_
-00003ff0: 6261 6e64 7769 6474 685f 696e 203d 206d  bandwidth_in = m
-00004000: 2e67 6574 2827 436c 6965 6e74 496e 7465  .get('ClientInte
-00004010: 726e 6574 4d61 7842 616e 6477 6964 7468  rnetMaxBandwidth
-00004020: 496e 2729 0a20 2020 2020 2020 2069 6620  In').        if 
-00004030: 6d2e 6765 7428 2743 6c69 656e 7449 6e74  m.get('ClientInt
-00004040: 6572 6e65 744d 6178 4261 6e64 7769 6474  ernetMaxBandwidt
-00004050: 684f 7574 2729 2069 7320 6e6f 7420 4e6f  hOut') is not No
-00004060: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00004070: 7365 6c66 2e63 6c69 656e 745f 696e 7465  self.client_inte
-00004080: 726e 6574 5f6d 6178 5f62 616e 6477 6964  rnet_max_bandwid
-00004090: 7468 5f6f 7574 203d 206d 2e67 6574 2827  th_out = m.get('
-000040a0: 436c 6965 6e74 496e 7465 726e 6574 4d61  ClientInternetMa
-000040b0: 7842 616e 6477 6964 7468 4f75 7427 290a  xBandwidthOut').
-000040c0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000040d0: 2827 436c 6965 6e74 5061 7373 776f 7264  ('ClientPassword
-000040e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000040f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004100: 2e63 6c69 656e 745f 7061 7373 776f 7264  .client_password
-00004110: 203d 206d 2e67 6574 2827 436c 6965 6e74   = m.get('Client
-00004120: 5061 7373 776f 7264 2729 0a20 2020 2020  Password').     
-00004130: 2020 2069 6620 6d2e 6765 7428 2743 6c69     if m.get('Cli
-00004140: 656e 7453 6563 7572 6974 7947 726f 7570  entSecurityGroup
-00004150: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00004160: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00004170: 6c66 2e63 6c69 656e 745f 7365 6375 7269  lf.client_securi
-00004180: 7479 5f67 726f 7570 5f69 6420 3d20 6d2e  ty_group_id = m.
-00004190: 6765 7428 2743 6c69 656e 7453 6563 7572  get('ClientSecur
-000041a0: 6974 7947 726f 7570 4964 2729 0a20 2020  ityGroupId').   
-000041b0: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
-000041c0: 6c69 656e 7453 7973 7465 6d44 6973 6b43  lientSystemDiskC
-000041d0: 6174 6567 6f72 7927 2920 6973 206e 6f74  ategory') is not
-000041e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000041f0: 2020 2073 656c 662e 636c 6965 6e74 5f73     self.client_s
-00004200: 7973 7465 6d5f 6469 736b 5f63 6174 6567  ystem_disk_categ
-00004210: 6f72 7920 3d20 6d2e 6765 7428 2743 6c69  ory = m.get('Cli
-00004220: 656e 7453 7973 7465 6d44 6973 6b43 6174  entSystemDiskCat
-00004230: 6567 6f72 7927 290a 2020 2020 2020 2020  egory').        
-00004240: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
-00004250: 5379 7374 656d 4469 736b 5369 7a65 2729  SystemDiskSize')
-00004260: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00004270: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00004280: 6c69 656e 745f 7379 7374 656d 5f64 6973  lient_system_dis
-00004290: 6b5f 7369 7a65 203d 206d 2e67 6574 2827  k_size = m.get('
-000042a0: 436c 6965 6e74 5379 7374 656d 4469 736b  ClientSystemDisk
-000042b0: 5369 7a65 2729 0a20 2020 2020 2020 2069  Size').        i
-000042c0: 6620 6d2e 6765 7428 2743 6c69 656e 7454  f m.get('ClientT
-000042d0: 6f6b 656e 2729 2069 7320 6e6f 7420 4e6f  oken') is not No
-000042e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000042f0: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
-00004300: 6e20 3d20 6d2e 6765 7428 2743 6c69 656e  n = m.get('Clien
-00004310: 7454 6f6b 656e 2729 0a20 2020 2020 2020  tToken').       
-00004320: 2069 6620 6d2e 6765 7428 2743 6c69 656e   if m.get('Clien
-00004330: 7456 5377 6974 6368 4964 2729 2069 7320  tVSwitchId') is 
-00004340: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00004350: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-00004360: 745f 7673 7769 7463 685f 6964 203d 206d  t_vswitch_id = m
-00004370: 2e67 6574 2827 436c 6965 6e74 5653 7769  .get('ClientVSwi
-00004380: 7463 6849 6427 290a 2020 2020 2020 2020  tchId').        
-00004390: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
-000043a0: 5a6f 6e65 4964 2729 2069 7320 6e6f 7420  ZoneId') is not 
-000043b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000043c0: 2020 7365 6c66 2e63 6c69 656e 745f 7a6f    self.client_zo
-000043d0: 6e65 5f69 6420 3d20 6d2e 6765 7428 2743  ne_id = m.get('C
-000043e0: 6c69 656e 745a 6f6e 6549 6427 290a 2020  lientZoneId').  
-000043f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00004400: 4561 6949 6e73 7461 6e63 6554 7970 6527  EaiInstanceType'
-00004410: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00004420: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004430: 6561 695f 696e 7374 616e 6365 5f74 7970  eai_instance_typ
-00004440: 6520 3d20 6d2e 6765 7428 2745 6169 496e  e = m.get('EaiIn
-00004450: 7374 616e 6365 5479 7065 2729 0a20 2020  stanceType').   
-00004460: 2020 2020 2069 6620 6d2e 6765 7428 2749       if m.get('I
-00004470: 6e73 7461 6e63 654e 616d 6527 2920 6973  nstanceName') is
-00004480: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00004490: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
-000044a0: 616e 6365 5f6e 616d 6520 3d20 6d2e 6765  ance_name = m.ge
-000044b0: 7428 2749 6e73 7461 6e63 654e 616d 6527  t('InstanceName'
-000044c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000044d0: 6574 2827 5265 6769 6f6e 4964 2729 2069  et('RegionId') i
-000044e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000044f0: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
-00004500: 696f 6e5f 6964 203d 206d 2e67 6574 2827  ion_id = m.get('
-00004510: 5265 6769 6f6e 4964 2729 0a20 2020 2020  RegionId').     
-00004520: 2020 2069 6620 6d2e 6765 7428 2752 6573     if m.get('Res
-00004530: 6f75 7263 6547 726f 7570 4964 2729 2069  ourceGroupId') i
-00004540: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00004550: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-00004560: 6f75 7263 655f 6772 6f75 705f 6964 203d  ource_group_id =
-00004570: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
-00004580: 4772 6f75 7049 6427 290a 2020 2020 2020  GroupId').      
-00004590: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-000045a0: 636c 6173 7320 4372 6561 7465 4561 6941  class CreateEaiA
-000045b0: 6c6c 5265 7370 6f6e 7365 426f 6479 2854  llResponseBody(T
-000045c0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-000045d0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-000045e0: 2063 6c69 656e 745f 696e 7374 616e 6365   client_instance
-000045f0: 5f69 643d 4e6f 6e65 2c20 656c 6173 7469  _id=None, elasti
-00004600: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
-00004610: 7374 616e 6365 5f69 643d 4e6f 6e65 2c20  stance_id=None, 
-00004620: 7265 7175 6573 745f 6964 3d4e 6f6e 6529  request_id=None)
-00004630: 3a0a 2020 2020 2020 2020 7365 6c66 2e63  :.        self.c
-00004640: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
-00004650: 6420 3d20 636c 6965 6e74 5f69 6e73 7461  d = client_insta
-00004660: 6e63 655f 6964 2020 2320 7479 7065 3a20  nce_id  # type: 
-00004670: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-00004680: 2e65 6c61 7374 6963 5f61 6363 656c 6572  .elastic_acceler
-00004690: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
-000046a0: 203d 2065 6c61 7374 6963 5f61 6363 656c   = elastic_accel
-000046b0: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
-000046c0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-000046d0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
-000046e0: 7565 7374 5f69 6420 3d20 7265 7175 6573  uest_id = reques
-000046f0: 745f 6964 2020 2320 7479 7065 3a20 7374  t_id  # type: st
-00004700: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
-00004710: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00004720: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00004730: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00004740: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-00004750: 7065 7228 4372 6561 7465 4561 6941 6c6c  per(CreateEaiAll
-00004760: 5265 7370 6f6e 7365 426f 6479 2c20 7365  ResponseBody, se
-00004770: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
-00004780: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00004790: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000047a0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-000047b0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-000047c0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-000047d0: 2020 2069 6620 7365 6c66 2e63 6c69 656e     if self.clien
-000047e0: 745f 696e 7374 616e 6365 5f69 6420 6973  t_instance_id is
-000047f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00004800: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
-00004810: 6c69 656e 7449 6e73 7461 6e63 6549 6427  lientInstanceId'
-00004820: 5d20 3d20 7365 6c66 2e63 6c69 656e 745f  ] = self.client_
-00004830: 696e 7374 616e 6365 5f69 640a 2020 2020  instance_id.    
-00004840: 2020 2020 6966 2073 656c 662e 656c 6173      if self.elas
-00004850: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
-00004860: 696e 7374 616e 6365 5f69 6420 6973 206e  instance_id is n
-00004870: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00004880: 2020 2020 2072 6573 756c 745b 2745 6c61       result['Ela
-00004890: 7374 6963 4163 6365 6c65 7261 7465 6449  sticAcceleratedI
-000048a0: 6e73 7461 6e63 6549 6427 5d20 3d20 7365  nstanceId'] = se
-000048b0: 6c66 2e65 6c61 7374 6963 5f61 6363 656c  lf.elastic_accel
-000048c0: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
-000048d0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-000048e0: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
-000048f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00004900: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-00004910: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
-00004920: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
-00004930: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00004940: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-00004950: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
-00004960: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00004970: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-00004980: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
-00004990: 6965 6e74 496e 7374 616e 6365 4964 2729  ientInstanceId')
-000049a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000049b0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000049c0: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
-000049d0: 6420 3d20 6d2e 6765 7428 2743 6c69 656e  d = m.get('Clien
-000049e0: 7449 6e73 7461 6e63 6549 6427 290a 2020  tInstanceId').  
-000049f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00004a00: 456c 6173 7469 6341 6363 656c 6572 6174  ElasticAccelerat
-00004a10: 6564 496e 7374 616e 6365 4964 2729 2069  edInstanceId') i
-00004a20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00004a30: 2020 2020 2020 2020 7365 6c66 2e65 6c61          self.ela
-00004a40: 7374 6963 5f61 6363 656c 6572 6174 6564  stic_accelerated
-00004a50: 5f69 6e73 7461 6e63 655f 6964 203d 206d  _instance_id = m
-00004a60: 2e67 6574 2827 456c 6173 7469 6341 6363  .get('ElasticAcc
-00004a70: 656c 6572 6174 6564 496e 7374 616e 6365  eleratedInstance
-00004a80: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-00004a90: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-00004aa0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00004ab0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004ac0: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
-00004ad0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-00004ae0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004af0: 7365 6c66 0a0a 0a63 6c61 7373 2043 7265  self...class Cre
-00004b00: 6174 6545 6169 416c 6c52 6573 706f 6e73  ateEaiAllRespons
-00004b10: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
-00004b20: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00004b30: 6c66 2c20 6865 6164 6572 733d 4e6f 6e65  lf, headers=None
-00004b40: 2c20 7374 6174 7573 5f63 6f64 653d 4e6f  , status_code=No
-00004b50: 6e65 2c20 626f 6479 3d4e 6f6e 6529 3a0a  ne, body=None):.
-00004b60: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00004b70: 6465 7273 203d 2068 6561 6465 7273 2020  ders = headers  
-00004b80: 2320 7479 7065 3a20 6469 6374 5b73 7472  # type: dict[str
-00004b90: 2c20 7374 725d 0a20 2020 2020 2020 2073  , str].        s
-00004ba0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00004bb0: 3d20 7374 6174 7573 5f63 6f64 6520 2023  = status_code  #
-00004bc0: 2074 7970 653a 2069 6e74 0a20 2020 2020   type: int.     
-00004bd0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-00004be0: 6f64 7920 2023 2074 7970 653a 2043 7265  ody  # type: Cre
-00004bf0: 6174 6545 6169 416c 6c52 6573 706f 6e73  ateEaiAllRespons
-00004c00: 6542 6f64 790a 0a20 2020 2064 6566 2076  eBody..    def v
-00004c10: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-00004c20: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-00004c30: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-00004c40: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
-00004c50: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
-00004c60: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-00004c70: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
-00004c80: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
-00004c90: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
-00004ca0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-00004cb0: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
-00004cc0: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
-00004cd0: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-00004ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004cf0: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-00004d00: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00004d10: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00004d20: 6d61 7020 3d20 7375 7065 7228 4372 6561  map = super(Crea
-00004d30: 7465 4561 6941 6c6c 5265 7370 6f6e 7365  teEaiAllResponse
-00004d40: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
-00004d50: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00004d60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00004d70: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00004d80: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00004d90: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00004da0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-00004db0: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
-00004dc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00004dd0: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
-00004de0: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
-00004df0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00004e00: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
-00004e10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00004e20: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
-00004e30: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
-00004e40: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
-00004e50: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-00004e60: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-00004e70: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00004e80: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-00004e90: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
-00004ea0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00004eb0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00004ec0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
-00004ed0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00004ee0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00004ef0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00004f00: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-00004f10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00004f20: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-00004f30: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-00004f40: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-00004f50: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00004f60: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00004f70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004f80: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
-00004f90: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00004fa0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00004fb0: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
-00004fc0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00004fd0: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-00004fe0: 3d20 4372 6561 7465 4561 6941 6c6c 5265  = CreateEaiAllRe
-00004ff0: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
-00005000: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-00005010: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-00005020: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-00005030: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-00005040: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00005050: 4372 6561 7465 4561 6945 6369 5265 7175  CreateEaiEciRequ
-00005060: 6573 7445 6369 436f 6e74 6169 6e65 7228  estEciContainer(
-00005070: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00005080: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00005090: 2c20 6172 673d 4e6f 6e65 2c20 636f 6d6d  , arg=None, comm
-000050a0: 616e 643d 4e6f 6e65 2c20 696d 6167 653d  and=None, image=
-000050b0: 4e6f 6e65 2c20 6e61 6d65 3d4e 6f6e 652c  None, name=None,
-000050c0: 2076 6f6c 756d 6573 3d4e 6f6e 6529 3a0a   volumes=None):.
-000050d0: 2020 2020 2020 2020 7365 6c66 2e61 7267          self.arg
-000050e0: 203d 2061 7267 2020 2320 7479 7065 3a20   = arg  # type: 
-000050f0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-00005100: 2e63 6f6d 6d61 6e64 203d 2063 6f6d 6d61  .command = comma
-00005110: 6e64 2020 2320 7479 7065 3a20 7374 720a  nd  # type: str.
-00005120: 2020 2020 2020 2020 7365 6c66 2e69 6d61          self.ima
-00005130: 6765 203d 2069 6d61 6765 2020 2320 7479  ge = image  # ty
-00005140: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-00005150: 7365 6c66 2e6e 616d 6520 3d20 6e61 6d65  self.name = name
-00005160: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-00005170: 2020 2020 2020 7365 6c66 2e76 6f6c 756d        self.volum
-00005180: 6573 203d 2076 6f6c 756d 6573 2020 2320  es = volumes  # 
-00005190: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
-000051a0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000051b0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-000051c0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-000051d0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-000051e0: 6d61 7020 3d20 7375 7065 7228 4372 6561  map = super(Crea
-000051f0: 7465 4561 6945 6369 5265 7175 6573 7445  teEaiEciRequestE
-00005200: 6369 436f 6e74 6169 6e65 722c 2073 656c  ciContainer, sel
-00005210: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-00005220: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00005230: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00005240: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00005250: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00005260: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00005270: 2020 6966 2073 656c 662e 6172 6720 6973    if self.arg is
-00005280: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00005290: 2020 2020 2020 2072 6573 756c 745b 2741         result['A
-000052a0: 7267 275d 203d 2073 656c 662e 6172 670a  rg'] = self.arg.
-000052b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000052c0: 636f 6d6d 616e 6420 6973 206e 6f74 204e  command is not N
-000052d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000052e0: 2072 6573 756c 745b 2743 6f6d 6d61 6e64   result['Command
-000052f0: 275d 203d 2073 656c 662e 636f 6d6d 616e  '] = self.comman
-00005300: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00005310: 662e 696d 6167 6520 6973 206e 6f74 204e  f.image is not N
-00005320: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00005330: 2072 6573 756c 745b 2749 6d61 6765 275d   result['Image']
-00005340: 203d 2073 656c 662e 696d 6167 650a 2020   = self.image.  
-00005350: 2020 2020 2020 6966 2073 656c 662e 6e61        if self.na
-00005360: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
-00005370: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00005380: 6c74 5b27 4e61 6d65 275d 203d 2073 656c  lt['Name'] = sel
-00005390: 662e 6e61 6d65 0a20 2020 2020 2020 2069  f.name.        i
-000053a0: 6620 7365 6c66 2e76 6f6c 756d 6573 2069  f self.volumes i
-000053b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000053c0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000053d0: 566f 6c75 6d65 7327 5d20 3d20 7365 6c66  Volumes'] = self
-000053e0: 2e76 6f6c 756d 6573 0a20 2020 2020 2020  .volumes.       
-000053f0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00005400: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-00005410: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-00005420: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00005430: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00005440: 6966 206d 2e67 6574 2827 4172 6727 2920  if m.get('Arg') 
-00005450: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00005460: 2020 2020 2020 2020 2073 656c 662e 6172           self.ar
-00005470: 6720 3d20 6d2e 6765 7428 2741 7267 2729  g = m.get('Arg')
-00005480: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00005490: 7428 2743 6f6d 6d61 6e64 2729 2069 7320  t('Command') is 
-000054a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000054b0: 2020 2020 2020 7365 6c66 2e63 6f6d 6d61        self.comma
-000054c0: 6e64 203d 206d 2e67 6574 2827 436f 6d6d  nd = m.get('Comm
-000054d0: 616e 6427 290a 2020 2020 2020 2020 6966  and').        if
-000054e0: 206d 2e67 6574 2827 496d 6167 6527 2920   m.get('Image') 
-000054f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00005500: 2020 2020 2020 2020 2073 656c 662e 696d           self.im
-00005510: 6167 6520 3d20 6d2e 6765 7428 2749 6d61  age = m.get('Ima
-00005520: 6765 2729 0a20 2020 2020 2020 2069 6620  ge').        if 
-00005530: 6d2e 6765 7428 274e 616d 6527 2920 6973  m.get('Name') is
-00005540: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00005550: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
-00005560: 203d 206d 2e67 6574 2827 4e61 6d65 2729   = m.get('Name')
-00005570: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00005580: 7428 2756 6f6c 756d 6573 2729 2069 7320  t('Volumes') is 
-00005590: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000055a0: 2020 2020 2020 7365 6c66 2e76 6f6c 756d        self.volum
-000055b0: 6573 203d 206d 2e67 6574 2827 566f 6c75  es = m.get('Volu
-000055c0: 6d65 7327 290a 2020 2020 2020 2020 7265  mes').        re
-000055d0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-000055e0: 7320 4372 6561 7465 4561 6945 6369 5265  s CreateEaiEciRe
-000055f0: 7175 6573 7445 6369 2854 6561 4d6f 6465  questEci(TeaMode
-00005600: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00005610: 6974 5f5f 2873 656c 662c 2063 6f6e 7461  it__(self, conta
-00005620: 696e 6572 3d4e 6f6e 652c 2065 6970 5f69  iner=None, eip_i
-00005630: 643d 4e6f 6e65 2c20 6e61 6d65 3d4e 6f6e  d=None, name=Non
-00005640: 652c 2074 7970 653d 4e6f 6e65 2c20 766f  e, type=None, vo
-00005650: 6c75 6d65 3d4e 6f6e 6529 3a0a 2020 2020  lume=None):.    
-00005660: 2020 2020 7365 6c66 2e63 6f6e 7461 696e      self.contain
-00005670: 6572 203d 2063 6f6e 7461 696e 6572 2020  er = container  
-00005680: 2320 7479 7065 3a20 4372 6561 7465 4561  # type: CreateEa
-00005690: 6945 6369 5265 7175 6573 7445 6369 436f  iEciRequestEciCo
-000056a0: 6e74 6169 6e65 720a 2020 2020 2020 2020  ntainer.        
-000056b0: 7365 6c66 2e65 6970 5f69 6420 3d20 6569  self.eip_id = ei
-000056c0: 705f 6964 2020 2320 7479 7065 3a20 7374  p_id  # type: st
-000056d0: 720a 2020 2020 2020 2020 7365 6c66 2e6e  r.        self.n
-000056e0: 616d 6520 3d20 6e61 6d65 2020 2320 7479  ame = name  # ty
-000056f0: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-00005700: 7365 6c66 2e74 7970 6520 3d20 7479 7065  self.type = type
-00005710: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-00005720: 2020 2020 2020 7365 6c66 2e76 6f6c 756d        self.volum
-00005730: 6520 3d20 766f 6c75 6d65 2020 2320 7479  e = volume  # ty
-00005740: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
-00005750: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-00005760: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00005770: 2e63 6f6e 7461 696e 6572 3a0a 2020 2020  .container:.    
-00005780: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00005790: 7461 696e 6572 2e76 616c 6964 6174 6528  tainer.validate(
-000057a0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-000057b0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000057c0: 205f 6d61 7020 3d20 7375 7065 7228 4372   _map = super(Cr
-000057d0: 6561 7465 4561 6945 6369 5265 7175 6573  eateEaiEciReques
-000057e0: 7445 6369 2c20 7365 6c66 292e 746f 5f6d  tEci, self).to_m
-000057f0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00005800: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00005810: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00005820: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00005830: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00005840: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00005850: 6c66 2e63 6f6e 7461 696e 6572 2069 7320  lf.container is 
-00005860: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00005870: 2020 2020 2020 7265 7375 6c74 5b27 436f        result['Co
-00005880: 6e74 6169 6e65 7227 5d20 3d20 7365 6c66  ntainer'] = self
-00005890: 2e63 6f6e 7461 696e 6572 2e74 6f5f 6d61  .container.to_ma
-000058a0: 7028 290a 2020 2020 2020 2020 6966 2073  p().        if s
-000058b0: 656c 662e 6569 705f 6964 2069 7320 6e6f  elf.eip_id is no
-000058c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000058d0: 2020 2020 7265 7375 6c74 5b27 4569 7049      result['EipI
-000058e0: 6427 5d20 3d20 7365 6c66 2e65 6970 5f69  d'] = self.eip_i
-000058f0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00005900: 662e 6e61 6d65 2069 7320 6e6f 7420 4e6f  f.name is not No
-00005910: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00005920: 7265 7375 6c74 5b27 4e61 6d65 275d 203d  result['Name'] =
-00005930: 2073 656c 662e 6e61 6d65 0a20 2020 2020   self.name.     
-00005940: 2020 2069 6620 7365 6c66 2e74 7970 6520     if self.type 
-00005950: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00005960: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00005970: 2754 7970 6527 5d20 3d20 7365 6c66 2e74  'Type'] = self.t
-00005980: 7970 650a 2020 2020 2020 2020 6966 2073  ype.        if s
-00005990: 656c 662e 766f 6c75 6d65 2069 7320 6e6f  elf.volume is no
-000059a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000059b0: 2020 2020 7265 7375 6c74 5b27 566f 6c75      result['Volu
-000059c0: 6d65 275d 203d 2073 656c 662e 766f 6c75  me'] = self.volu
-000059d0: 6d65 0a20 2020 2020 2020 2072 6574 7572  me.        retur
-000059e0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000059f0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00005a00: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-00005a10: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00005a20: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00005a30: 6574 2827 436f 6e74 6169 6e65 7227 2920  et('Container') 
-00005a40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00005a50: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-00005a60: 6465 6c20 3d20 4372 6561 7465 4561 6945  del = CreateEaiE
-00005a70: 6369 5265 7175 6573 7445 6369 436f 6e74  ciRequestEciCont
-00005a80: 6169 6e65 7228 290a 2020 2020 2020 2020  ainer().        
-00005a90: 2020 2020 7365 6c66 2e63 6f6e 7461 696e      self.contain
-00005aa0: 6572 203d 2074 656d 705f 6d6f 6465 6c2e  er = temp_model.
-00005ab0: 6672 6f6d 5f6d 6170 286d 5b27 436f 6e74  from_map(m['Cont
-00005ac0: 6169 6e65 7227 5d29 0a20 2020 2020 2020  ainer']).       
-00005ad0: 2069 6620 6d2e 6765 7428 2745 6970 4964   if m.get('EipId
-00005ae0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00005af0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005b00: 2e65 6970 5f69 6420 3d20 6d2e 6765 7428  .eip_id = m.get(
-00005b10: 2745 6970 4964 2729 0a20 2020 2020 2020  'EipId').       
-00005b20: 2069 6620 6d2e 6765 7428 274e 616d 6527   if m.get('Name'
-00005b30: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00005b40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005b50: 6e61 6d65 203d 206d 2e67 6574 2827 4e61  name = m.get('Na
-00005b60: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
-00005b70: 6d2e 6765 7428 2754 7970 6527 2920 6973  m.get('Type') is
-00005b80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00005b90: 2020 2020 2020 2073 656c 662e 7479 7065         self.type
-00005ba0: 203d 206d 2e67 6574 2827 5479 7065 2729   = m.get('Type')
-00005bb0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00005bc0: 7428 2756 6f6c 756d 6527 2920 6973 206e  t('Volume') is n
-00005bd0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00005be0: 2020 2020 2073 656c 662e 766f 6c75 6d65       self.volume
-00005bf0: 203d 206d 2e67 6574 2827 566f 6c75 6d65   = m.get('Volume
-00005c00: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00005c10: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2043  n self...class C
-00005c20: 7265 6174 6545 6169 4563 6952 6571 7565  reateEaiEciReque
-00005c30: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
-00005c40: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00005c50: 656c 662c 2063 6c69 656e 745f 746f 6b65  elf, client_toke
-00005c60: 6e3d 4e6f 6e65 2c20 6561 6973 5f6e 616d  n=None, eais_nam
-00005c70: 653d 4e6f 6e65 2c20 6561 6973 5f74 7970  e=None, eais_typ
-00005c80: 653d 4e6f 6e65 2c20 6563 693d 4e6f 6e65  e=None, eci=None
-00005c90: 2c20 7265 6769 6f6e 5f69 643d 4e6f 6e65  , region_id=None
-00005ca0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005cb0: 2020 2072 6573 6f75 7263 655f 6772 6f75     resource_grou
-00005cc0: 705f 6964 3d4e 6f6e 652c 2073 6563 7572  p_id=None, secur
-00005cd0: 6974 795f 6772 6f75 705f 6964 3d4e 6f6e  ity_group_id=Non
-00005ce0: 652c 2076 5f73 7769 7463 685f 6964 3d4e  e, v_switch_id=N
-00005cf0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-00005d00: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
-00005d10: 3d20 636c 6965 6e74 5f74 6f6b 656e 2020  = client_token  
-00005d20: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00005d30: 2020 2020 7365 6c66 2e65 6169 735f 6e61      self.eais_na
-00005d40: 6d65 203d 2065 6169 735f 6e61 6d65 2020  me = eais_name  
-00005d50: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00005d60: 2020 2020 7365 6c66 2e65 6169 735f 7479      self.eais_ty
-00005d70: 7065 203d 2065 6169 735f 7479 7065 2020  pe = eais_type  
-00005d80: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00005d90: 2020 2020 7365 6c66 2e65 6369 203d 2065      self.eci = e
-00005da0: 6369 2020 2320 7479 7065 3a20 4372 6561  ci  # type: Crea
-00005db0: 7465 4561 6945 6369 5265 7175 6573 7445  teEaiEciRequestE
-00005dc0: 6369 0a20 2020 2020 2020 2073 656c 662e  ci.        self.
-00005dd0: 7265 6769 6f6e 5f69 6420 3d20 7265 6769  region_id = regi
-00005de0: 6f6e 5f69 6420 2023 2074 7970 653a 2073  on_id  # type: s
-00005df0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-00005e00: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-00005e10: 6420 3d20 7265 736f 7572 6365 5f67 726f  d = resource_gro
-00005e20: 7570 5f69 6420 2023 2074 7970 653a 2073  up_id  # type: s
-00005e30: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-00005e40: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
-00005e50: 6420 3d20 7365 6375 7269 7479 5f67 726f  d = security_gro
-00005e60: 7570 5f69 6420 2023 2074 7970 653a 2073  up_id  # type: s
-00005e70: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-00005e80: 765f 7377 6974 6368 5f69 6420 3d20 765f  v_switch_id = v_
-00005e90: 7377 6974 6368 5f69 6420 2023 2074 7970  switch_id  # typ
-00005ea0: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
-00005eb0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-00005ec0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00005ed0: 6563 693a 0a20 2020 2020 2020 2020 2020  eci:.           
-00005ee0: 2073 656c 662e 6563 692e 7661 6c69 6461   self.eci.valida
-00005ef0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-00005f00: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00005f10: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00005f20: 2843 7265 6174 6545 6169 4563 6952 6571  (CreateEaiEciReq
-00005f30: 7565 7374 2c20 7365 6c66 292e 746f 5f6d  uest, self).to_m
-00005f40: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00005f50: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00005f60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00005f70: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00005f80: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00005f90: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00005fa0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
-00005fb0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00005fc0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00005fd0: 2743 6c69 656e 7454 6f6b 656e 275d 203d  'ClientToken'] =
-00005fe0: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
-00005ff0: 656e 0a20 2020 2020 2020 2069 6620 7365  en.        if se
-00006000: 6c66 2e65 6169 735f 6e61 6d65 2069 7320  lf.eais_name is 
-00006010: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00006020: 2020 2020 2020 7265 7375 6c74 5b27 4561        result['Ea
-00006030: 6973 4e61 6d65 275d 203d 2073 656c 662e  isName'] = self.
-00006040: 6561 6973 5f6e 616d 650a 2020 2020 2020  eais_name.      
-00006050: 2020 6966 2073 656c 662e 6561 6973 5f74    if self.eais_t
-00006060: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
-00006070: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00006080: 756c 745b 2745 6169 7354 7970 6527 5d20  ult['EaisType'] 
-00006090: 3d20 7365 6c66 2e65 6169 735f 7479 7065  = self.eais_type
-000060a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000060b0: 2e65 6369 2069 7320 6e6f 7420 4e6f 6e65  .eci is not None
-000060c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000060d0: 7375 6c74 5b27 4563 6927 5d20 3d20 7365  sult['Eci'] = se
-000060e0: 6c66 2e65 6369 2e74 6f5f 6d61 7028 290a  lf.eci.to_map().
-000060f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00006100: 7265 6769 6f6e 5f69 6420 6973 206e 6f74  region_id is not
-00006110: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006120: 2020 2072 6573 756c 745b 2752 6567 696f     result['Regio
-00006130: 6e49 6427 5d20 3d20 7365 6c66 2e72 6567  nId'] = self.reg
-00006140: 696f 6e5f 6964 0a20 2020 2020 2020 2069  ion_id.        i
-00006150: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
-00006160: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
-00006170: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006180: 2020 7265 7375 6c74 5b27 5265 736f 7572    result['Resour
-00006190: 6365 4772 6f75 7049 6427 5d20 3d20 7365  ceGroupId'] = se
-000061a0: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
-000061b0: 705f 6964 0a20 2020 2020 2020 2069 6620  p_id.        if 
-000061c0: 7365 6c66 2e73 6563 7572 6974 795f 6772  self.security_gr
-000061d0: 6f75 705f 6964 2069 7320 6e6f 7420 4e6f  oup_id is not No
-000061e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000061f0: 7265 7375 6c74 5b27 5365 6375 7269 7479  result['Security
-00006200: 4772 6f75 7049 6427 5d20 3d20 7365 6c66  GroupId'] = self
-00006210: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
-00006220: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-00006230: 6c66 2e76 5f73 7769 7463 685f 6964 2069  lf.v_switch_id i
-00006240: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00006250: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00006260: 5653 7769 7463 6849 6427 5d20 3d20 7365  VSwitchId'] = se
-00006270: 6c66 2e76 5f73 7769 7463 685f 6964 0a20  lf.v_switch_id. 
-00006280: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00006290: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-000062a0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-000062b0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000062c0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000062d0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000062e0: 436c 6965 6e74 546f 6b65 6e27 2920 6973  ClientToken') is
-000062f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00006300: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
-00006310: 6e74 5f74 6f6b 656e 203d 206d 2e67 6574  nt_token = m.get
-00006320: 2827 436c 6965 6e74 546f 6b65 6e27 290a  ('ClientToken').
-00006330: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00006340: 2827 4561 6973 4e61 6d65 2729 2069 7320  ('EaisName') is 
-00006350: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00006360: 2020 2020 2020 7365 6c66 2e65 6169 735f        self.eais_
-00006370: 6e61 6d65 203d 206d 2e67 6574 2827 4561  name = m.get('Ea
-00006380: 6973 4e61 6d65 2729 0a20 2020 2020 2020  isName').       
-00006390: 2069 6620 6d2e 6765 7428 2745 6169 7354   if m.get('EaisT
-000063a0: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
-000063b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000063c0: 656c 662e 6561 6973 5f74 7970 6520 3d20  elf.eais_type = 
-000063d0: 6d2e 6765 7428 2745 6169 7354 7970 6527  m.get('EaisType'
-000063e0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000063f0: 6574 2827 4563 6927 2920 6973 206e 6f74  et('Eci') is not
-00006400: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006410: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-00006420: 4372 6561 7465 4561 6945 6369 5265 7175  CreateEaiEciRequ
-00006430: 6573 7445 6369 2829 0a20 2020 2020 2020  estEci().       
-00006440: 2020 2020 2073 656c 662e 6563 6920 3d20       self.eci = 
-00006450: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-00006460: 6d61 7028 6d5b 2745 6369 275d 290a 2020  map(m['Eci']).  
-00006470: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00006480: 5265 6769 6f6e 4964 2729 2069 7320 6e6f  RegionId') is no
-00006490: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000064a0: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
-000064b0: 6964 203d 206d 2e67 6574 2827 5265 6769  id = m.get('Regi
-000064c0: 6f6e 4964 2729 0a20 2020 2020 2020 2069  onId').        i
-000064d0: 6620 6d2e 6765 7428 2752 6573 6f75 7263  f m.get('Resourc
-000064e0: 6547 726f 7570 4964 2729 2069 7320 6e6f  eGroupId') is no
-000064f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00006500: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
-00006510: 655f 6772 6f75 705f 6964 203d 206d 2e67  e_group_id = m.g
-00006520: 6574 2827 5265 736f 7572 6365 4772 6f75  et('ResourceGrou
-00006530: 7049 6427 290a 2020 2020 2020 2020 6966  pId').        if
-00006540: 206d 2e67 6574 2827 5365 6375 7269 7479   m.get('Security
-00006550: 4772 6f75 7049 6427 2920 6973 206e 6f74  GroupId') is not
+00001040: 6c66 0a0a 0a63 6c61 7373 2041 7474 6163  lf...class Attac
+00001050: 6845 6169 7345 6952 6571 7565 7374 2854  hEaisEiRequest(T
+00001060: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00001070: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00001080: 2063 6c69 656e 745f 696e 7374 616e 6365   client_instance
+00001090: 5f69 643d 4e6f 6e65 2c20 6569 5f69 6e73  _id=None, ei_ins
+000010a0: 7461 6e63 655f 6964 3d4e 6f6e 652c 2065  tance_id=None, e
+000010b0: 695f 696e 7374 616e 6365 5f74 7970 653d  i_instance_type=
+000010c0: 4e6f 6e65 2c20 7265 6769 6f6e 5f69 643d  None, region_id=
+000010d0: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
+000010e0: 656c 662e 636c 6965 6e74 5f69 6e73 7461  elf.client_insta
+000010f0: 6e63 655f 6964 203d 2063 6c69 656e 745f  nce_id = client_
+00001100: 696e 7374 616e 6365 5f69 6420 2023 2074  instance_id  # t
+00001110: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00001120: 2073 656c 662e 6569 5f69 6e73 7461 6e63   self.ei_instanc
+00001130: 655f 6964 203d 2065 695f 696e 7374 616e  e_id = ei_instan
+00001140: 6365 5f69 6420 2023 2074 7970 653a 2073  ce_id  # type: s
+00001150: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+00001160: 6569 5f69 6e73 7461 6e63 655f 7479 7065  ei_instance_type
+00001170: 203d 2065 695f 696e 7374 616e 6365 5f74   = ei_instance_t
+00001180: 7970 6520 2023 2074 7970 653a 2073 7472  ype  # type: str
+00001190: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+000011a0: 6769 6f6e 5f69 6420 3d20 7265 6769 6f6e  gion_id = region
+000011b0: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
+000011c0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+000011d0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+000011e0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+000011f0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+00001200: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+00001210: 6572 2841 7474 6163 6845 6169 7345 6952  er(AttachEaisEiR
+00001220: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
+00001230: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00001240: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00001250: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00001260: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00001270: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00001280: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00001290: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
+000012a0: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
+000012b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000012c0: 2072 6573 756c 745b 2743 6c69 656e 7449   result['ClientI
+000012d0: 6e73 7461 6e63 6549 6427 5d20 3d20 7365  nstanceId'] = se
+000012e0: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
+000012f0: 6365 5f69 640a 2020 2020 2020 2020 6966  ce_id.        if
+00001300: 2073 656c 662e 6569 5f69 6e73 7461 6e63   self.ei_instanc
+00001310: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+00001320: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00001330: 7375 6c74 5b27 4569 496e 7374 616e 6365  sult['EiInstance
+00001340: 4964 275d 203d 2073 656c 662e 6569 5f69  Id'] = self.ei_i
+00001350: 6e73 7461 6e63 655f 6964 0a20 2020 2020  nstance_id.     
+00001360: 2020 2069 6620 7365 6c66 2e65 695f 696e     if self.ei_in
+00001370: 7374 616e 6365 5f74 7970 6520 6973 206e  stance_type is n
+00001380: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00001390: 2020 2020 2072 6573 756c 745b 2745 6949       result['EiI
+000013a0: 6e73 7461 6e63 6554 7970 6527 5d20 3d20  nstanceType'] = 
+000013b0: 7365 6c66 2e65 695f 696e 7374 616e 6365  self.ei_instance
+000013c0: 5f74 7970 650a 2020 2020 2020 2020 6966  _type.        if
+000013d0: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+000013e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000013f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00001400: 2752 6567 696f 6e49 6427 5d20 3d20 7365  'RegionId'] = se
+00001410: 6c66 2e72 6567 696f 6e5f 6964 0a20 2020  lf.region_id.   
+00001420: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00001430: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00001440: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+00001450: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00001460: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00001470: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
+00001480: 6965 6e74 496e 7374 616e 6365 4964 2729  ientInstanceId')
+00001490: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000014a0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000014b0: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
+000014c0: 6420 3d20 6d2e 6765 7428 2743 6c69 656e  d = m.get('Clien
+000014d0: 7449 6e73 7461 6e63 6549 6427 290a 2020  tInstanceId').  
+000014e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000014f0: 4569 496e 7374 616e 6365 4964 2729 2069  EiInstanceId') i
+00001500: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00001510: 2020 2020 2020 2020 7365 6c66 2e65 695f          self.ei_
+00001520: 696e 7374 616e 6365 5f69 6420 3d20 6d2e  instance_id = m.
+00001530: 6765 7428 2745 6949 6e73 7461 6e63 6549  get('EiInstanceI
+00001540: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+00001550: 2e67 6574 2827 4569 496e 7374 616e 6365  .get('EiInstance
+00001560: 5479 7065 2729 2069 7320 6e6f 7420 4e6f  Type') is not No
+00001570: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00001580: 7365 6c66 2e65 695f 696e 7374 616e 6365  self.ei_instance
+00001590: 5f74 7970 6520 3d20 6d2e 6765 7428 2745  _type = m.get('E
+000015a0: 6949 6e73 7461 6e63 6554 7970 6527 290a  iInstanceType').
+000015b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000015c0: 2827 5265 6769 6f6e 4964 2729 2069 7320  ('RegionId') is 
+000015d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000015e0: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
+000015f0: 6e5f 6964 203d 206d 2e67 6574 2827 5265  n_id = m.get('Re
+00001600: 6769 6f6e 4964 2729 0a20 2020 2020 2020  gionId').       
+00001610: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00001620: 6c61 7373 2041 7474 6163 6845 6169 7345  lass AttachEaisE
+00001630: 6952 6573 706f 6e73 6542 6f64 7928 5465  iResponseBody(Te
+00001640: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00001650: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00001660: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
+00001670: 6964 3d4e 6f6e 652c 2065 695f 696e 7374  id=None, ei_inst
+00001680: 616e 6365 5f69 643d 4e6f 6e65 2c20 7265  ance_id=None, re
+00001690: 7175 6573 745f 6964 3d4e 6f6e 6529 3a0a  quest_id=None):.
+000016a0: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
+000016b0: 656e 745f 696e 7374 616e 6365 5f69 6420  ent_instance_id 
+000016c0: 3d20 636c 6965 6e74 5f69 6e73 7461 6e63  = client_instanc
+000016d0: 655f 6964 2020 2320 7479 7065 3a20 7374  e_id  # type: st
+000016e0: 720a 2020 2020 2020 2020 7365 6c66 2e65  r.        self.e
+000016f0: 695f 696e 7374 616e 6365 5f69 6420 3d20  i_instance_id = 
+00001700: 6569 5f69 6e73 7461 6e63 655f 6964 2020  ei_instance_id  
+00001710: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+00001720: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+00001730: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
+00001740: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
+00001750: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+00001760: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00001770: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+00001780: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00001790: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+000017a0: 4174 7461 6368 4561 6973 4569 5265 7370  AttachEaisEiResp
+000017b0: 6f6e 7365 426f 6479 2c20 7365 6c66 292e  onseBody, self).
+000017c0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000017d0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+000017e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000017f0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00001800: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00001810: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00001820: 6620 7365 6c66 2e63 6c69 656e 745f 696e  f self.client_in
+00001830: 7374 616e 6365 5f69 6420 6973 206e 6f74  stance_id is not
+00001840: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00001850: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
+00001860: 7449 6e73 7461 6e63 6549 6427 5d20 3d20  tInstanceId'] = 
+00001870: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
+00001880: 616e 6365 5f69 640a 2020 2020 2020 2020  ance_id.        
+00001890: 6966 2073 656c 662e 6569 5f69 6e73 7461  if self.ei_insta
+000018a0: 6e63 655f 6964 2069 7320 6e6f 7420 4e6f  nce_id is not No
+000018b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000018c0: 7265 7375 6c74 5b27 4569 496e 7374 616e  result['EiInstan
+000018d0: 6365 4964 275d 203d 2073 656c 662e 6569  ceId'] = self.ei
+000018e0: 5f69 6e73 7461 6e63 655f 6964 0a20 2020  _instance_id.   
+000018f0: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
+00001900: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
+00001910: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00001920: 2072 6573 756c 745b 2752 6571 7565 7374   result['Request
+00001930: 4964 275d 203d 2073 656c 662e 7265 7175  Id'] = self.requ
+00001940: 6573 745f 6964 0a20 2020 2020 2020 2072  est_id.        r
+00001950: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00001960: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00001970: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
+00001980: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00001990: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000019a0: 206d 2e67 6574 2827 436c 6965 6e74 496e   m.get('ClientIn
+000019b0: 7374 616e 6365 4964 2729 2069 7320 6e6f  stanceId') is no
+000019c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000019d0: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
+000019e0: 696e 7374 616e 6365 5f69 6420 3d20 6d2e  instance_id = m.
+000019f0: 6765 7428 2743 6c69 656e 7449 6e73 7461  get('ClientInsta
+00001a00: 6e63 6549 6427 290a 2020 2020 2020 2020  nceId').        
+00001a10: 6966 206d 2e67 6574 2827 4569 496e 7374  if m.get('EiInst
+00001a20: 616e 6365 4964 2729 2069 7320 6e6f 7420  anceId') is not 
+00001a30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00001a40: 2020 7365 6c66 2e65 695f 696e 7374 616e    self.ei_instan
+00001a50: 6365 5f69 6420 3d20 6d2e 6765 7428 2745  ce_id = m.get('E
+00001a60: 6949 6e73 7461 6e63 6549 6427 290a 2020  iInstanceId').  
+00001a70: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00001a80: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
+00001a90: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00001aa0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+00001ab0: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
+00001ac0: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
+00001ad0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00001ae0: 636c 6173 7320 4174 7461 6368 4561 6973  class AttachEais
+00001af0: 4569 5265 7370 6f6e 7365 2854 6561 4d6f  EiResponse(TeaMo
+00001b00: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00001b10: 696e 6974 5f5f 2873 656c 662c 2068 6561  init__(self, hea
+00001b20: 6465 7273 3d4e 6f6e 652c 2073 7461 7475  ders=None, statu
+00001b30: 735f 636f 6465 3d4e 6f6e 652c 2062 6f64  s_code=None, bod
+00001b40: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
+00001b50: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00001b60: 6865 6164 6572 7320 2023 2074 7970 653a  headers  # type:
+00001b70: 2064 6963 745b 7374 722c 2073 7472 5d0a   dict[str, str].
+00001b80: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00001b90: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+00001ba0: 735f 636f 6465 2020 2320 7479 7065 3a20  s_code  # type: 
+00001bb0: 696e 740a 2020 2020 2020 2020 7365 6c66  int.        self
+00001bc0: 2e62 6f64 7920 3d20 626f 6479 2020 2320  .body = body  # 
+00001bd0: 7479 7065 3a20 4174 7461 6368 4561 6973  type: AttachEais
+00001be0: 4569 5265 7370 6f6e 7365 426f 6479 0a0a  EiResponseBody..
+00001bf0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00001c00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00001c10: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+00001c20: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
+00001c30: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
+00001c40: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00001c50: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+00001c60: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
+00001c70: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
+00001c80: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00001c90: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+00001ca0: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
+00001cb0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00001cc0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+00001cd0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+00001ce0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+00001cf0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00001d00: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00001d10: 7570 6572 2841 7474 6163 6845 6169 7345  uper(AttachEaisE
+00001d20: 6952 6573 706f 6e73 652c 2073 656c 6629  iResponse, self)
+00001d30: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00001d40: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00001d50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00001d60: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00001d70: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00001d80: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00001d90: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+00001da0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00001db0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00001dc0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+00001dd0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+00001de0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00001df0: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00001e00: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00001e10: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00001e20: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00001e30: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00001e40: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00001e50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00001e60: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+00001e70: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+00001e80: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00001e90: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00001ea0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00001eb0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+00001ec0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00001ed0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00001ee0: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+00001ef0: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00001f00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001f10: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+00001f20: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+00001f30: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+00001f40: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+00001f50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00001f60: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00001f70: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+00001f80: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+00001f90: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+00001fa0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+00001fb0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00001fc0: 6d70 5f6d 6f64 656c 203d 2041 7474 6163  mp_model = Attac
+00001fd0: 6845 6169 7345 6952 6573 706f 6e73 6542  hEaisEiResponseB
+00001fe0: 6f64 7928 290a 2020 2020 2020 2020 2020  ody().          
+00001ff0: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
+00002000: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
+00002010: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
+00002020: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00002030: 0a0a 0a63 6c61 7373 2043 6861 6e67 6552  ...class ChangeR
+00002040: 6573 6f75 7263 6547 726f 7570 5265 7175  esourceGroupRequ
+00002050: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+00002060: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00002070: 7365 6c66 2c20 7265 736f 7572 6365 5f67  self, resource_g
+00002080: 726f 7570 5f69 643d 4e6f 6e65 2c20 7265  roup_id=None, re
+00002090: 736f 7572 6365 5f69 643d 4e6f 6e65 2c20  source_id=None, 
+000020a0: 7265 736f 7572 6365 5f72 6567 696f 6e5f  resource_region_
+000020b0: 6964 3d4e 6f6e 6529 3a0a 2020 2020 2020  id=None):.      
+000020c0: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+000020d0: 6772 6f75 705f 6964 203d 2072 6573 6f75  group_id = resou
+000020e0: 7263 655f 6772 6f75 705f 6964 2020 2320  rce_group_id  # 
+000020f0: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
+00002100: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+00002110: 6964 203d 2072 6573 6f75 7263 655f 6964  id = resource_id
+00002120: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+00002130: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
+00002140: 7263 655f 7265 6769 6f6e 5f69 6420 3d20  rce_region_id = 
+00002150: 7265 736f 7572 6365 5f72 6567 696f 6e5f  resource_region_
+00002160: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+00002170: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00002180: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00002190: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+000021a0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+000021b0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+000021c0: 7228 4368 616e 6765 5265 736f 7572 6365  r(ChangeResource
+000021d0: 4772 6f75 7052 6571 7565 7374 2c20 7365  GroupRequest, se
+000021e0: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+000021f0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00002200: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00002210: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00002220: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00002230: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00002240: 2020 2069 6620 7365 6c66 2e72 6573 6f75     if self.resou
+00002250: 7263 655f 6772 6f75 705f 6964 2069 7320  rce_group_id is 
+00002260: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00002270: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
+00002280: 736f 7572 6365 4772 6f75 7049 6427 5d20  sourceGroupId'] 
+00002290: 3d20 7365 6c66 2e72 6573 6f75 7263 655f  = self.resource_
+000022a0: 6772 6f75 705f 6964 0a20 2020 2020 2020  group_id.       
+000022b0: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
+000022c0: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+000022d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000022e0: 7375 6c74 5b27 5265 736f 7572 6365 4964  sult['ResourceId
+000022f0: 275d 203d 2073 656c 662e 7265 736f 7572  '] = self.resour
+00002300: 6365 5f69 640a 2020 2020 2020 2020 6966  ce_id.        if
+00002310: 2073 656c 662e 7265 736f 7572 6365 5f72   self.resource_r
+00002320: 6567 696f 6e5f 6964 2069 7320 6e6f 7420  egion_id is not 
+00002330: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00002340: 2020 7265 7375 6c74 5b27 5265 736f 7572    result['Resour
+00002350: 6365 5265 6769 6f6e 4964 275d 203d 2073  ceRegionId'] = s
+00002360: 656c 662e 7265 736f 7572 6365 5f72 6567  elf.resource_reg
+00002370: 696f 6e5f 6964 0a20 2020 2020 2020 2072  ion_id.        r
+00002380: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00002390: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+000023a0: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
+000023b0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000023c0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000023d0: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+000023e0: 4772 6f75 7049 6427 2920 6973 206e 6f74  GroupId') is not
+000023f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00002400: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
+00002410: 5f67 726f 7570 5f69 6420 3d20 6d2e 6765  _group_id = m.ge
+00002420: 7428 2752 6573 6f75 7263 6547 726f 7570  t('ResourceGroup
+00002430: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+00002440: 6d2e 6765 7428 2752 6573 6f75 7263 6549  m.get('ResourceI
+00002450: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00002460: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002470: 662e 7265 736f 7572 6365 5f69 6420 3d20  f.resource_id = 
+00002480: 6d2e 6765 7428 2752 6573 6f75 7263 6549  m.get('ResourceI
+00002490: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+000024a0: 2e67 6574 2827 5265 736f 7572 6365 5265  .get('ResourceRe
+000024b0: 6769 6f6e 4964 2729 2069 7320 6e6f 7420  gionId') is not 
+000024c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000024d0: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+000024e0: 7265 6769 6f6e 5f69 6420 3d20 6d2e 6765  region_id = m.ge
+000024f0: 7428 2752 6573 6f75 7263 6552 6567 696f  t('ResourceRegio
+00002500: 6e49 6427 290a 2020 2020 2020 2020 7265  nId').        re
+00002510: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00002520: 7320 4368 616e 6765 5265 736f 7572 6365  s ChangeResource
+00002530: 4772 6f75 7052 6573 706f 6e73 6542 6f64  GroupResponseBod
+00002540: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+00002550: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00002560: 6c66 2c20 7265 7175 6573 745f 6964 3d4e  lf, request_id=N
+00002570: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+00002580: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+00002590: 7265 7175 6573 745f 6964 2020 2320 7479  request_id  # ty
+000025a0: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
+000025b0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+000025c0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000025d0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+000025e0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+000025f0: 7020 3d20 7375 7065 7228 4368 616e 6765  p = super(Change
+00002600: 5265 736f 7572 6365 4772 6f75 7052 6573  ResourceGroupRes
+00002610: 706f 6e73 6542 6f64 792c 2073 656c 6629  ponseBody, self)
+00002620: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00002630: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00002640: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00002650: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00002660: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00002670: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00002680: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+00002690: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000026a0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000026b0: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
+000026c0: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
+000026d0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+000026e0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+000026f0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00002700: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+00002710: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00002720: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00002730: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
+00002740: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00002750: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+00002760: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
+00002770: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
+00002780: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00002790: 0a0a 0a63 6c61 7373 2043 6861 6e67 6552  ...class ChangeR
+000027a0: 6573 6f75 7263 6547 726f 7570 5265 7370  esourceGroupResp
+000027b0: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+000027c0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000027d0: 2873 656c 662c 2068 6561 6465 7273 3d4e  (self, headers=N
+000027e0: 6f6e 652c 2073 7461 7475 735f 636f 6465  one, status_code
+000027f0: 3d4e 6f6e 652c 2062 6f64 793d 4e6f 6e65  =None, body=None
+00002800: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00002810: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+00002820: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
+00002830: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
+00002840: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+00002850: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
+00002860: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
+00002870: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00002880: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
+00002890: 4368 616e 6765 5265 736f 7572 6365 4772  ChangeResourceGr
+000028a0: 6f75 7052 6573 706f 6e73 6542 6f64 790a  oupResponseBody.
+000028b0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000028c0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000028d0: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+000028e0: 6571 7569 7265 6428 7365 6c66 2e68 6561  equired(self.hea
+000028f0: 6465 7273 2c20 2768 6561 6465 7273 2729  ders, 'headers')
+00002900: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00002910: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+00002920: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00002930: 2c20 2773 7461 7475 735f 636f 6465 2729  , 'status_code')
+00002940: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00002950: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+00002960: 7365 6c66 2e62 6f64 792c 2027 626f 6479  self.body, 'body
+00002970: 2729 0a20 2020 2020 2020 2069 6620 7365  ').        if se
+00002980: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+00002990: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+000029a0: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+000029b0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+000029c0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+000029d0: 7375 7065 7228 4368 616e 6765 5265 736f  super(ChangeReso
+000029e0: 7572 6365 4772 6f75 7052 6573 706f 6e73  urceGroupRespons
+000029f0: 652c 2073 656c 6629 2e74 6f5f 6d61 7028  e, self).to_map(
+00002a00: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00002a10: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00002a20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00002a30: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00002a40: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00002a50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00002a60: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+00002a70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00002a80: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
+00002a90: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
+00002aa0: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00002ab0: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
+00002ac0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00002ad0: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+00002ae0: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
+00002af0: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
+00002b00: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00002b10: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+00002b20: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00002b30: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
+00002b40: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
+00002b50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002b60: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00002b70: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00002b80: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00002b90: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00002ba0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00002bb0: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+00002bc0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00002bd0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00002be0: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+00002bf0: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+00002c00: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00002c10: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00002c20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002c30: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00002c40: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00002c50: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00002c60: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+00002c70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00002c80: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00002c90: 203d 2043 6861 6e67 6552 6573 6f75 7263   = ChangeResourc
+00002ca0: 6547 726f 7570 5265 7370 6f6e 7365 426f  eGroupResponseBo
+00002cb0: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+00002cc0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+00002cd0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00002ce0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+00002cf0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00002d00: 0a0a 636c 6173 7320 4372 6561 7465 4561  ..class CreateEa
+00002d10: 6952 6571 7565 7374 2854 6561 4d6f 6465  iRequest(TeaMode
+00002d20: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00002d30: 6974 5f5f 2873 656c 662c 2063 6c69 656e  it__(self, clien
+00002d40: 745f 746f 6b65 6e3d 4e6f 6e65 2c20 696d  t_token=None, im
+00002d50: 6167 653d 4e6f 6e65 2c20 696e 7374 616e  age=None, instan
+00002d60: 6365 5f6e 616d 653d 4e6f 6e65 2c20 696e  ce_name=None, in
+00002d70: 7374 616e 6365 5f74 7970 653d 4e6f 6e65  stance_type=None
+00002d80: 2c20 7265 6769 6f6e 5f69 643d 4e6f 6e65  , region_id=None
+00002d90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002da0: 2020 2072 6573 6f75 7263 655f 6772 6f75     resource_grou
+00002db0: 705f 6964 3d4e 6f6e 652c 2073 6563 7572  p_id=None, secur
+00002dc0: 6974 795f 6772 6f75 705f 6964 3d4e 6f6e  ity_group_id=Non
+00002dd0: 652c 2076 5f73 7769 7463 685f 6964 3d4e  e, v_switch_id=N
+00002de0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+00002df0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
+00002e00: 3d20 636c 6965 6e74 5f74 6f6b 656e 2020  = client_token  
+00002e10: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+00002e20: 2020 2020 7365 6c66 2e69 6d61 6765 203d      self.image =
+00002e30: 2069 6d61 6765 2020 2320 7479 7065 3a20   image  # type: 
+00002e40: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+00002e50: 2e69 6e73 7461 6e63 655f 6e61 6d65 203d  .instance_name =
+00002e60: 2069 6e73 7461 6e63 655f 6e61 6d65 2020   instance_name  
+00002e70: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+00002e80: 2020 2020 7365 6c66 2e69 6e73 7461 6e63      self.instanc
+00002e90: 655f 7479 7065 203d 2069 6e73 7461 6e63  e_type = instanc
+00002ea0: 655f 7479 7065 2020 2320 7479 7065 3a20  e_type  # type: 
+00002eb0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+00002ec0: 2e72 6567 696f 6e5f 6964 203d 2072 6567  .region_id = reg
+00002ed0: 696f 6e5f 6964 2020 2320 7479 7065 3a20  ion_id  # type: 
+00002ee0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+00002ef0: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
+00002f00: 6964 203d 2072 6573 6f75 7263 655f 6772  id = resource_gr
+00002f10: 6f75 705f 6964 2020 2320 7479 7065 3a20  oup_id  # type: 
+00002f20: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+00002f30: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
+00002f40: 6964 203d 2073 6563 7572 6974 795f 6772  id = security_gr
+00002f50: 6f75 705f 6964 2020 2320 7479 7065 3a20  oup_id  # type: 
+00002f60: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+00002f70: 2e76 5f73 7769 7463 685f 6964 203d 2076  .v_switch_id = v
+00002f80: 5f73 7769 7463 685f 6964 2020 2320 7479  _switch_id  # ty
+00002f90: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
+00002fa0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00002fb0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00002fc0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00002fd0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00002fe0: 7020 3d20 7375 7065 7228 4372 6561 7465  p = super(Create
+00002ff0: 4561 6952 6571 7565 7374 2c20 7365 6c66  EaiRequest, self
+00003000: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00003010: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00003020: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00003030: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00003040: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00003050: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00003060: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
+00003070: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
+00003080: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00003090: 6573 756c 745b 2743 6c69 656e 7454 6f6b  esult['ClientTok
+000030a0: 656e 275d 203d 2073 656c 662e 636c 6965  en'] = self.clie
+000030b0: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
+000030c0: 2069 6620 7365 6c66 2e69 6d61 6765 2069   if self.image i
+000030d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000030e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000030f0: 496d 6167 6527 5d20 3d20 7365 6c66 2e69  Image'] = self.i
+00003100: 6d61 6765 0a20 2020 2020 2020 2069 6620  mage.        if 
+00003110: 7365 6c66 2e69 6e73 7461 6e63 655f 6e61  self.instance_na
+00003120: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+00003130: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00003140: 6c74 5b27 496e 7374 616e 6365 4e61 6d65  lt['InstanceName
+00003150: 275d 203d 2073 656c 662e 696e 7374 616e  '] = self.instan
+00003160: 6365 5f6e 616d 650a 2020 2020 2020 2020  ce_name.        
+00003170: 6966 2073 656c 662e 696e 7374 616e 6365  if self.instance
+00003180: 5f74 7970 6520 6973 206e 6f74 204e 6f6e  _type is not Non
+00003190: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000031a0: 6573 756c 745b 2749 6e73 7461 6e63 6554  esult['InstanceT
+000031b0: 7970 6527 5d20 3d20 7365 6c66 2e69 6e73  ype'] = self.ins
+000031c0: 7461 6e63 655f 7479 7065 0a20 2020 2020  tance_type.     
+000031d0: 2020 2069 6620 7365 6c66 2e72 6567 696f     if self.regio
+000031e0: 6e5f 6964 2069 7320 6e6f 7420 4e6f 6e65  n_id is not None
+000031f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00003200: 7375 6c74 5b27 5265 6769 6f6e 4964 275d  sult['RegionId']
+00003210: 203d 2073 656c 662e 7265 6769 6f6e 5f69   = self.region_i
+00003220: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+00003230: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
+00003240: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00003250: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00003260: 756c 745b 2752 6573 6f75 7263 6547 726f  ult['ResourceGro
+00003270: 7570 4964 275d 203d 2073 656c 662e 7265  upId'] = self.re
+00003280: 736f 7572 6365 5f67 726f 7570 5f69 640a  source_group_id.
+00003290: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000032a0: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
+000032b0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+000032c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000032d0: 745b 2753 6563 7572 6974 7947 726f 7570  t['SecurityGroup
+000032e0: 4964 275d 203d 2073 656c 662e 7365 6375  Id'] = self.secu
+000032f0: 7269 7479 5f67 726f 7570 5f69 640a 2020  rity_group_id.  
+00003300: 2020 2020 2020 6966 2073 656c 662e 765f        if self.v_
+00003310: 7377 6974 6368 5f69 6420 6973 206e 6f74  switch_id is not
+00003320: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00003330: 2020 2072 6573 756c 745b 2756 5377 6974     result['VSwit
+00003340: 6368 4964 275d 203d 2073 656c 662e 765f  chId'] = self.v_
+00003350: 7377 6974 6368 5f69 640a 2020 2020 2020  switch_id.      
+00003360: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00003370: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00003380: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+00003390: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+000033a0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+000033b0: 2069 6620 6d2e 6765 7428 2743 6c69 656e   if m.get('Clien
+000033c0: 7454 6f6b 656e 2729 2069 7320 6e6f 7420  tToken') is not 
+000033d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000033e0: 2020 7365 6c66 2e63 6c69 656e 745f 746f    self.client_to
+000033f0: 6b65 6e20 3d20 6d2e 6765 7428 2743 6c69  ken = m.get('Cli
+00003400: 656e 7454 6f6b 656e 2729 0a20 2020 2020  entToken').     
+00003410: 2020 2069 6620 6d2e 6765 7428 2749 6d61     if m.get('Ima
+00003420: 6765 2729 2069 7320 6e6f 7420 4e6f 6e65  ge') is not None
+00003430: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00003440: 6c66 2e69 6d61 6765 203d 206d 2e67 6574  lf.image = m.get
+00003450: 2827 496d 6167 6527 290a 2020 2020 2020  ('Image').      
+00003460: 2020 6966 206d 2e67 6574 2827 496e 7374    if m.get('Inst
+00003470: 616e 6365 4e61 6d65 2729 2069 7320 6e6f  anceName') is no
+00003480: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00003490: 2020 2020 7365 6c66 2e69 6e73 7461 6e63      self.instanc
+000034a0: 655f 6e61 6d65 203d 206d 2e67 6574 2827  e_name = m.get('
+000034b0: 496e 7374 616e 6365 4e61 6d65 2729 0a20  InstanceName'). 
+000034c0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000034d0: 2749 6e73 7461 6e63 6554 7970 6527 2920  'InstanceType') 
+000034e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000034f0: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
+00003500: 7374 616e 6365 5f74 7970 6520 3d20 6d2e  stance_type = m.
+00003510: 6765 7428 2749 6e73 7461 6e63 6554 7970  get('InstanceTyp
+00003520: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00003530: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
+00003540: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00003550: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00003560: 6567 696f 6e5f 6964 203d 206d 2e67 6574  egion_id = m.get
+00003570: 2827 5265 6769 6f6e 4964 2729 0a20 2020  ('RegionId').   
+00003580: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+00003590: 6573 6f75 7263 6547 726f 7570 4964 2729  esourceGroupId')
+000035a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000035b0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000035c0: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
+000035d0: 203d 206d 2e67 6574 2827 5265 736f 7572   = m.get('Resour
+000035e0: 6365 4772 6f75 7049 6427 290a 2020 2020  ceGroupId').    
+000035f0: 2020 2020 6966 206d 2e67 6574 2827 5365      if m.get('Se
+00003600: 6375 7269 7479 4772 6f75 7049 6427 2920  curityGroupId') 
+00003610: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00003620: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00003630: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
+00003640: 3d20 6d2e 6765 7428 2753 6563 7572 6974  = m.get('Securit
+00003650: 7947 726f 7570 4964 2729 0a20 2020 2020  yGroupId').     
+00003660: 2020 2069 6620 6d2e 6765 7428 2756 5377     if m.get('VSw
+00003670: 6974 6368 4964 2729 2069 7320 6e6f 7420  itchId') is not 
+00003680: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00003690: 2020 7365 6c66 2e76 5f73 7769 7463 685f    self.v_switch_
+000036a0: 6964 203d 206d 2e67 6574 2827 5653 7769  id = m.get('VSwi
+000036b0: 7463 6849 6427 290a 2020 2020 2020 2020  tchId').        
+000036c0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+000036d0: 6173 7320 4372 6561 7465 4561 6952 6573  ass CreateEaiRes
+000036e0: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+000036f0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00003700: 6e69 745f 5f28 7365 6c66 2c20 656c 6173  nit__(self, elas
+00003710: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
+00003720: 696e 7374 616e 6365 5f69 643d 4e6f 6e65  instance_id=None
+00003730: 2c20 7265 7175 6573 745f 6964 3d4e 6f6e  , request_id=Non
+00003740: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00003750: 2e65 6c61 7374 6963 5f61 6363 656c 6572  .elastic_acceler
+00003760: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
+00003770: 203d 2065 6c61 7374 6963 5f61 6363 656c   = elastic_accel
+00003780: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
+00003790: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+000037a0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+000037b0: 7565 7374 5f69 6420 3d20 7265 7175 6573  uest_id = reques
+000037c0: 745f 6964 2020 2320 7479 7065 3a20 7374  t_id  # type: st
+000037d0: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
+000037e0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+000037f0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00003800: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00003810: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00003820: 7065 7228 4372 6561 7465 4561 6952 6573  per(CreateEaiRes
+00003830: 706f 6e73 6542 6f64 792c 2073 656c 6629  ponseBody, self)
+00003840: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00003850: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00003860: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00003870: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00003880: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00003890: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000038a0: 6966 2073 656c 662e 656c 6173 7469 635f  if self.elastic_
+000038b0: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
+000038c0: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
+000038d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000038e0: 2072 6573 756c 745b 2745 6c61 7374 6963   result['Elastic
+000038f0: 4163 6365 6c65 7261 7465 6449 6e73 7461  AcceleratedInsta
+00003900: 6e63 6549 6427 5d20 3d20 7365 6c66 2e65  nceId'] = self.e
+00003910: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+00003920: 6564 5f69 6e73 7461 6e63 655f 6964 0a20  ed_instance_id. 
+00003930: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00003940: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
+00003950: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00003960: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
+00003970: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
+00003980: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+00003990: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000039a0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000039b0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+000039c0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000039d0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000039e0: 6966 206d 2e67 6574 2827 456c 6173 7469  if m.get('Elasti
+000039f0: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
+00003a00: 616e 6365 4964 2729 2069 7320 6e6f 7420  anceId') is not 
+00003a10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00003a20: 2020 7365 6c66 2e65 6c61 7374 6963 5f61    self.elastic_a
+00003a30: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
+00003a40: 6e63 655f 6964 203d 206d 2e67 6574 2827  nce_id = m.get('
+00003a50: 456c 6173 7469 6341 6363 656c 6572 6174  ElasticAccelerat
+00003a60: 6564 496e 7374 616e 6365 4964 2729 0a20  edInstanceId'). 
+00003a70: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00003a80: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
+00003a90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00003aa0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+00003ab0: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
+00003ac0: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
+00003ad0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00003ae0: 0a63 6c61 7373 2043 7265 6174 6545 6169  .class CreateEai
+00003af0: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
+00003b00: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00003b10: 6974 5f5f 2873 656c 662c 2068 6561 6465  it__(self, heade
+00003b20: 7273 3d4e 6f6e 652c 2073 7461 7475 735f  rs=None, status_
+00003b30: 636f 6465 3d4e 6f6e 652c 2062 6f64 793d  code=None, body=
+00003b40: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
+00003b50: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
+00003b60: 6164 6572 7320 2023 2074 7970 653a 2064  aders  # type: d
+00003b70: 6963 745b 7374 722c 2073 7472 5d0a 2020  ict[str, str].  
+00003b80: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00003b90: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
+00003ba0: 636f 6465 2020 2320 7479 7065 3a20 696e  code  # type: in
+00003bb0: 740a 2020 2020 2020 2020 7365 6c66 2e62  t.        self.b
+00003bc0: 6f64 7920 3d20 626f 6479 2020 2320 7479  ody = body  # ty
+00003bd0: 7065 3a20 4372 6561 7465 4561 6952 6573  pe: CreateEaiRes
+00003be0: 706f 6e73 6542 6f64 790a 0a20 2020 2064  ponseBody..    d
+00003bf0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00003c00: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00003c10: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+00003c20: 6428 7365 6c66 2e68 6561 6465 7273 2c20  d(self.headers, 
+00003c30: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+00003c40: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+00003c50: 5f72 6571 7569 7265 6428 7365 6c66 2e73  _required(self.s
+00003c60: 7461 7475 735f 636f 6465 2c20 2773 7461  tatus_code, 'sta
+00003c70: 7475 735f 636f 6465 2729 0a20 2020 2020  tus_code').     
+00003c80: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+00003c90: 5f72 6571 7569 7265 6428 7365 6c66 2e62  _required(self.b
+00003ca0: 6f64 792c 2027 626f 6479 2729 0a20 2020  ody, 'body').   
+00003cb0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00003cc0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00003cd0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00003ce0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00003cf0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00003d00: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00003d10: 4372 6561 7465 4561 6952 6573 706f 6e73  CreateEaiRespons
+00003d20: 652c 2073 656c 6629 2e74 6f5f 6d61 7028  e, self).to_map(
+00003d30: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00003d40: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00003d50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00003d60: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00003d70: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00003d80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003d90: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+00003da0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00003db0: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
+00003dc0: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
+00003dd0: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00003de0: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
+00003df0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00003e00: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+00003e10: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
+00003e20: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
+00003e30: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00003e40: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+00003e50: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00003e60: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
+00003e70: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
+00003e80: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003e90: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00003ea0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00003eb0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00003ec0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00003ed0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00003ee0: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+00003ef0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00003f00: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00003f10: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+00003f20: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+00003f30: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00003f40: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00003f50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003f60: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00003f70: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00003f80: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00003f90: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+00003fa0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00003fb0: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00003fc0: 203d 2043 7265 6174 6545 6169 5265 7370   = CreateEaiResp
+00003fd0: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+00003fe0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00003ff0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+00004000: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00004010: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00004020: 2073 656c 660a 0a0a 636c 6173 7320 4372   self...class Cr
+00004030: 6561 7465 4561 6941 6c6c 5265 7175 6573  eateEaiAllReques
+00004040: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+00004050: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00004060: 6c66 2c20 636c 6965 6e74 5f69 6d61 6765  lf, client_image
+00004070: 5f69 643d 4e6f 6e65 2c20 636c 6965 6e74  _id=None, client
+00004080: 5f69 6e73 7461 6e63 655f 6e61 6d65 3d4e  _instance_name=N
+00004090: 6f6e 652c 2063 6c69 656e 745f 696e 7374  one, client_inst
+000040a0: 616e 6365 5f74 7970 653d 4e6f 6e65 2c0a  ance_type=None,.
+000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040c0: 2063 6c69 656e 745f 696e 7465 726e 6574   client_internet
+000040d0: 5f6d 6178 5f62 616e 6477 6964 7468 5f69  _max_bandwidth_i
+000040e0: 6e3d 4e6f 6e65 2c20 636c 6965 6e74 5f69  n=None, client_i
+000040f0: 6e74 6572 6e65 745f 6d61 785f 6261 6e64  nternet_max_band
+00004100: 7769 6474 685f 6f75 743d 4e6f 6e65 2c20  width_out=None, 
+00004110: 636c 6965 6e74 5f70 6173 7377 6f72 643d  client_password=
+00004120: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00004130: 2020 2020 2020 2063 6c69 656e 745f 7365         client_se
+00004140: 6375 7269 7479 5f67 726f 7570 5f69 643d  curity_group_id=
+00004150: 4e6f 6e65 2c20 636c 6965 6e74 5f73 7973  None, client_sys
+00004160: 7465 6d5f 6469 736b 5f63 6174 6567 6f72  tem_disk_categor
+00004170: 793d 4e6f 6e65 2c20 636c 6965 6e74 5f73  y=None, client_s
+00004180: 7973 7465 6d5f 6469 736b 5f73 697a 653d  ystem_disk_size=
+00004190: 4e6f 6e65 2c20 636c 6965 6e74 5f74 6f6b  None, client_tok
+000041a0: 656e 3d4e 6f6e 652c 0a20 2020 2020 2020  en=None,.       
+000041b0: 2020 2020 2020 2020 2020 636c 6965 6e74            client
+000041c0: 5f76 7377 6974 6368 5f69 643d 4e6f 6e65  _vswitch_id=None
+000041d0: 2c20 636c 6965 6e74 5f7a 6f6e 655f 6964  , client_zone_id
+000041e0: 3d4e 6f6e 652c 2065 6169 5f69 6e73 7461  =None, eai_insta
+000041f0: 6e63 655f 7479 7065 3d4e 6f6e 652c 2069  nce_type=None, i
+00004200: 6e73 7461 6e63 655f 6e61 6d65 3d4e 6f6e  nstance_name=Non
+00004210: 652c 2072 6567 696f 6e5f 6964 3d4e 6f6e  e, region_id=Non
+00004220: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00004230: 2020 2020 7265 736f 7572 6365 5f67 726f      resource_gro
+00004240: 7570 5f69 643d 4e6f 6e65 293a 0a20 2020  up_id=None):.   
+00004250: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
+00004260: 5f69 6d61 6765 5f69 6420 3d20 636c 6965  _image_id = clie
+00004270: 6e74 5f69 6d61 6765 5f69 6420 2023 2074  nt_image_id  # t
+00004280: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00004290: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
+000042a0: 7461 6e63 655f 6e61 6d65 203d 2063 6c69  tance_name = cli
+000042b0: 656e 745f 696e 7374 616e 6365 5f6e 616d  ent_instance_nam
+000042c0: 6520 2023 2074 7970 653a 2073 7472 0a20  e  # type: str. 
+000042d0: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+000042e0: 6e74 5f69 6e73 7461 6e63 655f 7479 7065  nt_instance_type
+000042f0: 203d 2063 6c69 656e 745f 696e 7374 616e   = client_instan
+00004300: 6365 5f74 7970 6520 2023 2074 7970 653a  ce_type  # type:
+00004310: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00004320: 662e 636c 6965 6e74 5f69 6e74 6572 6e65  f.client_interne
+00004330: 745f 6d61 785f 6261 6e64 7769 6474 685f  t_max_bandwidth_
+00004340: 696e 203d 2063 6c69 656e 745f 696e 7465  in = client_inte
+00004350: 726e 6574 5f6d 6178 5f62 616e 6477 6964  rnet_max_bandwid
+00004360: 7468 5f69 6e20 2023 2074 7970 653a 2069  th_in  # type: i
+00004370: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
+00004380: 636c 6965 6e74 5f69 6e74 6572 6e65 745f  client_internet_
+00004390: 6d61 785f 6261 6e64 7769 6474 685f 6f75  max_bandwidth_ou
+000043a0: 7420 3d20 636c 6965 6e74 5f69 6e74 6572  t = client_inter
+000043b0: 6e65 745f 6d61 785f 6261 6e64 7769 6474  net_max_bandwidt
+000043c0: 685f 6f75 7420 2023 2074 7970 653a 2069  h_out  # type: i
+000043d0: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
+000043e0: 636c 6965 6e74 5f70 6173 7377 6f72 6420  client_password 
+000043f0: 3d20 636c 6965 6e74 5f70 6173 7377 6f72  = client_passwor
+00004400: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
+00004410: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00004420: 6e74 5f73 6563 7572 6974 795f 6772 6f75  nt_security_grou
+00004430: 705f 6964 203d 2063 6c69 656e 745f 7365  p_id = client_se
+00004440: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
+00004450: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00004460: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
+00004470: 5f73 7973 7465 6d5f 6469 736b 5f63 6174  _system_disk_cat
+00004480: 6567 6f72 7920 3d20 636c 6965 6e74 5f73  egory = client_s
+00004490: 7973 7465 6d5f 6469 736b 5f63 6174 6567  ystem_disk_categ
+000044a0: 6f72 7920 2023 2074 7970 653a 2073 7472  ory  # type: str
+000044b0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+000044c0: 6965 6e74 5f73 7973 7465 6d5f 6469 736b  ient_system_disk
+000044d0: 5f73 697a 6520 3d20 636c 6965 6e74 5f73  _size = client_s
+000044e0: 7973 7465 6d5f 6469 736b 5f73 697a 6520  ystem_disk_size 
+000044f0: 2023 2074 7970 653a 2069 6e74 0a20 2020   # type: int.   
+00004500: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
+00004510: 5f74 6f6b 656e 203d 2063 6c69 656e 745f  _token = client_
+00004520: 746f 6b65 6e20 2023 2074 7970 653a 2073  token  # type: s
+00004530: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+00004540: 636c 6965 6e74 5f76 7377 6974 6368 5f69  client_vswitch_i
+00004550: 6420 3d20 636c 6965 6e74 5f76 7377 6974  d = client_vswit
+00004560: 6368 5f69 6420 2023 2074 7970 653a 2073  ch_id  # type: s
+00004570: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+00004580: 636c 6965 6e74 5f7a 6f6e 655f 6964 203d  client_zone_id =
+00004590: 2063 6c69 656e 745f 7a6f 6e65 5f69 6420   client_zone_id 
+000045a0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+000045b0: 2020 2020 2073 656c 662e 6561 695f 696e       self.eai_in
+000045c0: 7374 616e 6365 5f74 7970 6520 3d20 6561  stance_type = ea
+000045d0: 695f 696e 7374 616e 6365 5f74 7970 6520  i_instance_type 
+000045e0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+000045f0: 2020 2020 2073 656c 662e 696e 7374 616e       self.instan
+00004600: 6365 5f6e 616d 6520 3d20 696e 7374 616e  ce_name = instan
+00004610: 6365 5f6e 616d 6520 2023 2074 7970 653a  ce_name  # type:
+00004620: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00004630: 662e 7265 6769 6f6e 5f69 6420 3d20 7265  f.region_id = re
+00004640: 6769 6f6e 5f69 6420 2023 2074 7970 653a  gion_id  # type:
+00004650: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00004660: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
+00004670: 5f69 6420 3d20 7265 736f 7572 6365 5f67  _id = resource_g
+00004680: 726f 7570 5f69 6420 2023 2074 7970 653a  roup_id  # type:
+00004690: 2073 7472 0a0a 2020 2020 6465 6620 7661   str..    def va
+000046a0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+000046b0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+000046c0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+000046d0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+000046e0: 2073 7570 6572 2843 7265 6174 6545 6169   super(CreateEai
+000046f0: 416c 6c52 6571 7565 7374 2c20 7365 6c66  AllRequest, self
+00004700: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00004710: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00004720: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00004730: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00004740: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00004750: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00004760: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
+00004770: 696d 6167 655f 6964 2069 7320 6e6f 7420  image_id is not 
+00004780: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00004790: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
+000047a0: 496d 6167 6549 6427 5d20 3d20 7365 6c66  ImageId'] = self
+000047b0: 2e63 6c69 656e 745f 696d 6167 655f 6964  .client_image_id
+000047c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000047d0: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
+000047e0: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
+000047f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00004800: 6573 756c 745b 2743 6c69 656e 7449 6e73  esult['ClientIns
+00004810: 7461 6e63 654e 616d 6527 5d20 3d20 7365  tanceName'] = se
+00004820: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
+00004830: 6365 5f6e 616d 650a 2020 2020 2020 2020  ce_name.        
+00004840: 6966 2073 656c 662e 636c 6965 6e74 5f69  if self.client_i
+00004850: 6e73 7461 6e63 655f 7479 7065 2069 7320  nstance_type is 
+00004860: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00004870: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
+00004880: 6965 6e74 496e 7374 616e 6365 5479 7065  ientInstanceType
+00004890: 275d 203d 2073 656c 662e 636c 6965 6e74  '] = self.client
+000048a0: 5f69 6e73 7461 6e63 655f 7479 7065 0a20  _instance_type. 
+000048b0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000048c0: 6c69 656e 745f 696e 7465 726e 6574 5f6d  lient_internet_m
+000048d0: 6178 5f62 616e 6477 6964 7468 5f69 6e20  ax_bandwidth_in 
+000048e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000048f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00004900: 2743 6c69 656e 7449 6e74 6572 6e65 744d  'ClientInternetM
+00004910: 6178 4261 6e64 7769 6474 6849 6e27 5d20  axBandwidthIn'] 
+00004920: 3d20 7365 6c66 2e63 6c69 656e 745f 696e  = self.client_in
+00004930: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
+00004940: 6964 7468 5f69 6e0a 2020 2020 2020 2020  idth_in.        
+00004950: 6966 2073 656c 662e 636c 6965 6e74 5f69  if self.client_i
+00004960: 6e74 6572 6e65 745f 6d61 785f 6261 6e64  nternet_max_band
+00004970: 7769 6474 685f 6f75 7420 6973 206e 6f74  width_out is not
+00004980: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00004990: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
+000049a0: 7449 6e74 6572 6e65 744d 6178 4261 6e64  tInternetMaxBand
+000049b0: 7769 6474 684f 7574 275d 203d 2073 656c  widthOut'] = sel
+000049c0: 662e 636c 6965 6e74 5f69 6e74 6572 6e65  f.client_interne
+000049d0: 745f 6d61 785f 6261 6e64 7769 6474 685f  t_max_bandwidth_
+000049e0: 6f75 740a 2020 2020 2020 2020 6966 2073  out.        if s
+000049f0: 656c 662e 636c 6965 6e74 5f70 6173 7377  elf.client_passw
+00004a00: 6f72 6420 6973 206e 6f74 204e 6f6e 653a  ord is not None:
+00004a10: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00004a20: 756c 745b 2743 6c69 656e 7450 6173 7377  ult['ClientPassw
+00004a30: 6f72 6427 5d20 3d20 7365 6c66 2e63 6c69  ord'] = self.cli
+00004a40: 656e 745f 7061 7373 776f 7264 0a20 2020  ent_password.   
+00004a50: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
+00004a60: 656e 745f 7365 6375 7269 7479 5f67 726f  ent_security_gro
+00004a70: 7570 5f69 6420 6973 206e 6f74 204e 6f6e  up_id is not Non
+00004a80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00004a90: 6573 756c 745b 2743 6c69 656e 7453 6563  esult['ClientSec
+00004aa0: 7572 6974 7947 726f 7570 4964 275d 203d  urityGroupId'] =
+00004ab0: 2073 656c 662e 636c 6965 6e74 5f73 6563   self.client_sec
+00004ac0: 7572 6974 795f 6772 6f75 705f 6964 0a20  urity_group_id. 
+00004ad0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00004ae0: 6c69 656e 745f 7379 7374 656d 5f64 6973  lient_system_dis
+00004af0: 6b5f 6361 7465 676f 7279 2069 7320 6e6f  k_category is no
+00004b00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00004b10: 2020 2020 7265 7375 6c74 5b27 436c 6965      result['Clie
+00004b20: 6e74 5379 7374 656d 4469 736b 4361 7465  ntSystemDiskCate
+00004b30: 676f 7279 275d 203d 2073 656c 662e 636c  gory'] = self.cl
+00004b40: 6965 6e74 5f73 7973 7465 6d5f 6469 736b  ient_system_disk
+00004b50: 5f63 6174 6567 6f72 790a 2020 2020 2020  _category.      
+00004b60: 2020 6966 2073 656c 662e 636c 6965 6e74    if self.client
+00004b70: 5f73 7973 7465 6d5f 6469 736b 5f73 697a  _system_disk_siz
+00004b80: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00004b90: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00004ba0: 745b 2743 6c69 656e 7453 7973 7465 6d44  t['ClientSystemD
+00004bb0: 6973 6b53 697a 6527 5d20 3d20 7365 6c66  iskSize'] = self
+00004bc0: 2e63 6c69 656e 745f 7379 7374 656d 5f64  .client_system_d
+00004bd0: 6973 6b5f 7369 7a65 0a20 2020 2020 2020  isk_size.       
+00004be0: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
+00004bf0: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
+00004c00: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00004c10: 6573 756c 745b 2743 6c69 656e 7454 6f6b  esult['ClientTok
+00004c20: 656e 275d 203d 2073 656c 662e 636c 6965  en'] = self.clie
+00004c30: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
+00004c40: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
+00004c50: 7673 7769 7463 685f 6964 2069 7320 6e6f  vswitch_id is no
+00004c60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00004c70: 2020 2020 7265 7375 6c74 5b27 436c 6965      result['Clie
+00004c80: 6e74 5653 7769 7463 6849 6427 5d20 3d20  ntVSwitchId'] = 
+00004c90: 7365 6c66 2e63 6c69 656e 745f 7673 7769  self.client_vswi
+00004ca0: 7463 685f 6964 0a20 2020 2020 2020 2069  tch_id.        i
+00004cb0: 6620 7365 6c66 2e63 6c69 656e 745f 7a6f  f self.client_zo
+00004cc0: 6e65 5f69 6420 6973 206e 6f74 204e 6f6e  ne_id is not Non
+00004cd0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00004ce0: 6573 756c 745b 2743 6c69 656e 745a 6f6e  esult['ClientZon
+00004cf0: 6549 6427 5d20 3d20 7365 6c66 2e63 6c69  eId'] = self.cli
+00004d00: 656e 745f 7a6f 6e65 5f69 640a 2020 2020  ent_zone_id.    
+00004d10: 2020 2020 6966 2073 656c 662e 6561 695f      if self.eai_
+00004d20: 696e 7374 616e 6365 5f74 7970 6520 6973  instance_type is
+00004d30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00004d40: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
+00004d50: 6169 496e 7374 616e 6365 5479 7065 275d  aiInstanceType']
+00004d60: 203d 2073 656c 662e 6561 695f 696e 7374   = self.eai_inst
+00004d70: 616e 6365 5f74 7970 650a 2020 2020 2020  ance_type.      
+00004d80: 2020 6966 2073 656c 662e 696e 7374 616e    if self.instan
+00004d90: 6365 5f6e 616d 6520 6973 206e 6f74 204e  ce_name is not N
+00004da0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00004db0: 2072 6573 756c 745b 2749 6e73 7461 6e63   result['Instanc
+00004dc0: 654e 616d 6527 5d20 3d20 7365 6c66 2e69  eName'] = self.i
+00004dd0: 6e73 7461 6e63 655f 6e61 6d65 0a20 2020  nstance_name.   
+00004de0: 2020 2020 2069 6620 7365 6c66 2e72 6567       if self.reg
+00004df0: 696f 6e5f 6964 2069 7320 6e6f 7420 4e6f  ion_id is not No
+00004e00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00004e10: 7265 7375 6c74 5b27 5265 6769 6f6e 4964  result['RegionId
+00004e20: 275d 203d 2073 656c 662e 7265 6769 6f6e  '] = self.region
+00004e30: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00004e40: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
+00004e50: 7570 5f69 6420 6973 206e 6f74 204e 6f6e  up_id is not Non
+00004e60: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00004e70: 6573 756c 745b 2752 6573 6f75 7263 6547  esult['ResourceG
+00004e80: 726f 7570 4964 275d 203d 2073 656c 662e  roupId'] = self.
+00004e90: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
+00004ea0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+00004eb0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00004ec0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00004ed0: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+00004ee0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00004ef0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00004f00: 7428 2743 6c69 656e 7449 6d61 6765 4964  t('ClientImageId
+00004f10: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00004f20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004f30: 2e63 6c69 656e 745f 696d 6167 655f 6964  .client_image_id
+00004f40: 203d 206d 2e67 6574 2827 436c 6965 6e74   = m.get('Client
+00004f50: 496d 6167 6549 6427 290a 2020 2020 2020  ImageId').      
+00004f60: 2020 6966 206d 2e67 6574 2827 436c 6965    if m.get('Clie
+00004f70: 6e74 496e 7374 616e 6365 4e61 6d65 2729  ntInstanceName')
+00004f80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00004f90: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00004fa0: 6c69 656e 745f 696e 7374 616e 6365 5f6e  lient_instance_n
+00004fb0: 616d 6520 3d20 6d2e 6765 7428 2743 6c69  ame = m.get('Cli
+00004fc0: 656e 7449 6e73 7461 6e63 654e 616d 6527  entInstanceName'
+00004fd0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00004fe0: 6574 2827 436c 6965 6e74 496e 7374 616e  et('ClientInstan
+00004ff0: 6365 5479 7065 2729 2069 7320 6e6f 7420  ceType') is not 
+00005000: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00005010: 2020 7365 6c66 2e63 6c69 656e 745f 696e    self.client_in
+00005020: 7374 616e 6365 5f74 7970 6520 3d20 6d2e  stance_type = m.
+00005030: 6765 7428 2743 6c69 656e 7449 6e73 7461  get('ClientInsta
+00005040: 6e63 6554 7970 6527 290a 2020 2020 2020  nceType').      
+00005050: 2020 6966 206d 2e67 6574 2827 436c 6965    if m.get('Clie
+00005060: 6e74 496e 7465 726e 6574 4d61 7842 616e  ntInternetMaxBan
+00005070: 6477 6964 7468 496e 2729 2069 7320 6e6f  dwidthIn') is no
+00005080: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00005090: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
+000050a0: 696e 7465 726e 6574 5f6d 6178 5f62 616e  internet_max_ban
+000050b0: 6477 6964 7468 5f69 6e20 3d20 6d2e 6765  dwidth_in = m.ge
+000050c0: 7428 2743 6c69 656e 7449 6e74 6572 6e65  t('ClientInterne
+000050d0: 744d 6178 4261 6e64 7769 6474 6849 6e27  tMaxBandwidthIn'
+000050e0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000050f0: 6574 2827 436c 6965 6e74 496e 7465 726e  et('ClientIntern
+00005100: 6574 4d61 7842 616e 6477 6964 7468 4f75  etMaxBandwidthOu
+00005110: 7427 2920 6973 206e 6f74 204e 6f6e 653a  t') is not None:
+00005120: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005130: 662e 636c 6965 6e74 5f69 6e74 6572 6e65  f.client_interne
+00005140: 745f 6d61 785f 6261 6e64 7769 6474 685f  t_max_bandwidth_
+00005150: 6f75 7420 3d20 6d2e 6765 7428 2743 6c69  out = m.get('Cli
+00005160: 656e 7449 6e74 6572 6e65 744d 6178 4261  entInternetMaxBa
+00005170: 6e64 7769 6474 684f 7574 2729 0a20 2020  ndwidthOut').   
+00005180: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
+00005190: 6c69 656e 7450 6173 7377 6f72 6427 2920  lientPassword') 
+000051a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000051b0: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
+000051c0: 6965 6e74 5f70 6173 7377 6f72 6420 3d20  ient_password = 
+000051d0: 6d2e 6765 7428 2743 6c69 656e 7450 6173  m.get('ClientPas
+000051e0: 7377 6f72 6427 290a 2020 2020 2020 2020  sword').        
+000051f0: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
+00005200: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
+00005210: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00005220: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005230: 636c 6965 6e74 5f73 6563 7572 6974 795f  client_security_
+00005240: 6772 6f75 705f 6964 203d 206d 2e67 6574  group_id = m.get
+00005250: 2827 436c 6965 6e74 5365 6375 7269 7479  ('ClientSecurity
+00005260: 4772 6f75 7049 6427 290a 2020 2020 2020  GroupId').      
+00005270: 2020 6966 206d 2e67 6574 2827 436c 6965    if m.get('Clie
+00005280: 6e74 5379 7374 656d 4469 736b 4361 7465  ntSystemDiskCate
+00005290: 676f 7279 2729 2069 7320 6e6f 7420 4e6f  gory') is not No
+000052a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000052b0: 7365 6c66 2e63 6c69 656e 745f 7379 7374  self.client_syst
+000052c0: 656d 5f64 6973 6b5f 6361 7465 676f 7279  em_disk_category
+000052d0: 203d 206d 2e67 6574 2827 436c 6965 6e74   = m.get('Client
+000052e0: 5379 7374 656d 4469 736b 4361 7465 676f  SystemDiskCatego
+000052f0: 7279 2729 0a20 2020 2020 2020 2069 6620  ry').        if 
+00005300: 6d2e 6765 7428 2743 6c69 656e 7453 7973  m.get('ClientSys
+00005310: 7465 6d44 6973 6b53 697a 6527 2920 6973  temDiskSize') is
+00005320: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00005330: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00005340: 6e74 5f73 7973 7465 6d5f 6469 736b 5f73  nt_system_disk_s
+00005350: 697a 6520 3d20 6d2e 6765 7428 2743 6c69  ize = m.get('Cli
+00005360: 656e 7453 7973 7465 6d44 6973 6b53 697a  entSystemDiskSiz
+00005370: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00005380: 2e67 6574 2827 436c 6965 6e74 546f 6b65  .get('ClientToke
+00005390: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
+000053a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000053b0: 662e 636c 6965 6e74 5f74 6f6b 656e 203d  f.client_token =
+000053c0: 206d 2e67 6574 2827 436c 6965 6e74 546f   m.get('ClientTo
+000053d0: 6b65 6e27 290a 2020 2020 2020 2020 6966  ken').        if
+000053e0: 206d 2e67 6574 2827 436c 6965 6e74 5653   m.get('ClientVS
+000053f0: 7769 7463 6849 6427 2920 6973 206e 6f74  witchId') is not
+00005400: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005410: 2020 2073 656c 662e 636c 6965 6e74 5f76     self.client_v
+00005420: 7377 6974 6368 5f69 6420 3d20 6d2e 6765  switch_id = m.ge
+00005430: 7428 2743 6c69 656e 7456 5377 6974 6368  t('ClientVSwitch
+00005440: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+00005450: 6d2e 6765 7428 2743 6c69 656e 745a 6f6e  m.get('ClientZon
+00005460: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+00005470: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00005480: 656c 662e 636c 6965 6e74 5f7a 6f6e 655f  elf.client_zone_
+00005490: 6964 203d 206d 2e67 6574 2827 436c 6965  id = m.get('Clie
+000054a0: 6e74 5a6f 6e65 4964 2729 0a20 2020 2020  ntZoneId').     
+000054b0: 2020 2069 6620 6d2e 6765 7428 2745 6169     if m.get('Eai
+000054c0: 496e 7374 616e 6365 5479 7065 2729 2069  InstanceType') i
+000054d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000054e0: 2020 2020 2020 2020 7365 6c66 2e65 6169          self.eai
+000054f0: 5f69 6e73 7461 6e63 655f 7479 7065 203d  _instance_type =
+00005500: 206d 2e67 6574 2827 4561 6949 6e73 7461   m.get('EaiInsta
+00005510: 6e63 6554 7970 6527 290a 2020 2020 2020  nceType').      
+00005520: 2020 6966 206d 2e67 6574 2827 496e 7374    if m.get('Inst
+00005530: 616e 6365 4e61 6d65 2729 2069 7320 6e6f  anceName') is no
+00005540: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00005550: 2020 2020 7365 6c66 2e69 6e73 7461 6e63      self.instanc
+00005560: 655f 6e61 6d65 203d 206d 2e67 6574 2827  e_name = m.get('
+00005570: 496e 7374 616e 6365 4e61 6d65 2729 0a20  InstanceName'). 
+00005580: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00005590: 2752 6567 696f 6e49 6427 2920 6973 206e  'RegionId') is n
+000055a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000055b0: 2020 2020 2073 656c 662e 7265 6769 6f6e       self.region
+000055c0: 5f69 6420 3d20 6d2e 6765 7428 2752 6567  _id = m.get('Reg
+000055d0: 696f 6e49 6427 290a 2020 2020 2020 2020  ionId').        
+000055e0: 6966 206d 2e67 6574 2827 5265 736f 7572  if m.get('Resour
+000055f0: 6365 4772 6f75 7049 6427 2920 6973 206e  ceGroupId') is n
+00005600: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00005610: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+00005620: 6365 5f67 726f 7570 5f69 6420 3d20 6d2e  ce_group_id = m.
+00005630: 6765 7428 2752 6573 6f75 7263 6547 726f  get('ResourceGro
+00005640: 7570 4964 2729 0a20 2020 2020 2020 2072  upId').        r
+00005650: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00005660: 7373 2043 7265 6174 6545 6169 416c 6c52  ss CreateEaiAllR
+00005670: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
+00005680: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00005690: 5f69 6e69 745f 5f28 7365 6c66 2c20 636c  _init__(self, cl
+000056a0: 6965 6e74 5f69 6e73 7461 6e63 655f 6964  ient_instance_id
+000056b0: 3d4e 6f6e 652c 2065 6c61 7374 6963 5f61  =None, elastic_a
+000056c0: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
+000056d0: 6e63 655f 6964 3d4e 6f6e 652c 2072 6571  nce_id=None, req
+000056e0: 7565 7374 5f69 643d 4e6f 6e65 293a 0a20  uest_id=None):. 
+000056f0: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00005700: 6e74 5f69 6e73 7461 6e63 655f 6964 203d  nt_instance_id =
+00005710: 2063 6c69 656e 745f 696e 7374 616e 6365   client_instance
+00005720: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
+00005730: 0a20 2020 2020 2020 2073 656c 662e 656c  .        self.el
+00005740: 6173 7469 635f 6163 6365 6c65 7261 7465  astic_accelerate
+00005750: 645f 696e 7374 616e 6365 5f69 6420 3d20  d_instance_id = 
+00005760: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
+00005770: 7465 645f 696e 7374 616e 6365 5f69 6420  ted_instance_id 
+00005780: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00005790: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+000057a0: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
+000057b0: 6420 2023 2074 7970 653a 2073 7472 0a0a  d  # type: str..
+000057c0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000057d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000057e0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+000057f0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00005800: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00005810: 2843 7265 6174 6545 6169 416c 6c52 6573  (CreateEaiAllRes
+00005820: 706f 6e73 6542 6f64 792c 2073 656c 6629  ponseBody, self)
+00005830: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00005840: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00005850: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005860: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00005870: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00005880: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00005890: 6966 2073 656c 662e 636c 6965 6e74 5f69  if self.client_i
+000058a0: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
+000058b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000058c0: 2020 2020 7265 7375 6c74 5b27 436c 6965      result['Clie
+000058d0: 6e74 496e 7374 616e 6365 4964 275d 203d  ntInstanceId'] =
+000058e0: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
+000058f0: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+00005900: 2069 6620 7365 6c66 2e65 6c61 7374 6963   if self.elastic
+00005910: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+00005920: 7461 6e63 655f 6964 2069 7320 6e6f 7420  tance_id is not 
+00005930: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00005940: 2020 7265 7375 6c74 5b27 456c 6173 7469    result['Elasti
+00005950: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
+00005960: 616e 6365 4964 275d 203d 2073 656c 662e  anceId'] = self.
+00005970: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
+00005980: 7465 645f 696e 7374 616e 6365 5f69 640a  ted_instance_id.
+00005990: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000059a0: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
+000059b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000059c0: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
+000059d0: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
+000059e0: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
+000059f0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00005a00: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00005a10: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+00005a20: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00005a30: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00005a40: 2069 6620 6d2e 6765 7428 2743 6c69 656e   if m.get('Clien
+00005a50: 7449 6e73 7461 6e63 6549 6427 2920 6973  tInstanceId') is
+00005a60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00005a70: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00005a80: 6e74 5f69 6e73 7461 6e63 655f 6964 203d  nt_instance_id =
+00005a90: 206d 2e67 6574 2827 436c 6965 6e74 496e   m.get('ClientIn
+00005aa0: 7374 616e 6365 4964 2729 0a20 2020 2020  stanceId').     
+00005ab0: 2020 2069 6620 6d2e 6765 7428 2745 6c61     if m.get('Ela
+00005ac0: 7374 6963 4163 6365 6c65 7261 7465 6449  sticAcceleratedI
+00005ad0: 6e73 7461 6e63 6549 6427 2920 6973 206e  nstanceId') is n
+00005ae0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00005af0: 2020 2020 2073 656c 662e 656c 6173 7469       self.elasti
+00005b00: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
+00005b10: 7374 616e 6365 5f69 6420 3d20 6d2e 6765  stance_id = m.ge
+00005b20: 7428 2745 6c61 7374 6963 4163 6365 6c65  t('ElasticAccele
+00005b30: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
+00005b40: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00005b50: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
+00005b60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00005b70: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00005b80: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
+00005b90: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
+00005ba0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00005bb0: 660a 0a0a 636c 6173 7320 4372 6561 7465  f...class Create
+00005bc0: 4561 6941 6c6c 5265 7370 6f6e 7365 2854  EaiAllResponse(T
+00005bd0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00005be0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00005bf0: 2068 6561 6465 7273 3d4e 6f6e 652c 2073   headers=None, s
+00005c00: 7461 7475 735f 636f 6465 3d4e 6f6e 652c  tatus_code=None,
+00005c10: 2062 6f64 793d 4e6f 6e65 293a 0a20 2020   body=None):.   
+00005c20: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00005c30: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
+00005c40: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
+00005c50: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
+00005c60: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+00005c70: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
+00005c80: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
+00005c90: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+00005ca0: 2020 2320 7479 7065 3a20 4372 6561 7465    # type: Create
+00005cb0: 4561 6941 6c6c 5265 7370 6f6e 7365 426f  EaiAllResponseBo
+00005cc0: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
+00005cd0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00005ce0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+00005cf0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+00005d00: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
+00005d10: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
+00005d20: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+00005d30: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
+00005d40: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
+00005d50: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
+00005d60: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+00005d70: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
+00005d80: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
+00005d90: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+00005da0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00005db0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+00005dc0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00005dd0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00005de0: 203d 2073 7570 6572 2843 7265 6174 6545   = super(CreateE
+00005df0: 6169 416c 6c52 6573 706f 6e73 652c 2073  aiAllResponse, s
+00005e00: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
+00005e10: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00005e20: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00005e30: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00005e40: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00005e50: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00005e60: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
+00005e70: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
+00005e80: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00005e90: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
+00005ea0: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
+00005eb0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+00005ec0: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
+00005ed0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005ee0: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
+00005ef0: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
+00005f00: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+00005f10: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
+00005f20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00005f30: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00005f40: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
+00005f50: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
+00005f60: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00005f70: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00005f80: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+00005f90: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00005fa0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00005fb0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+00005fc0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+00005fd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00005fe0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00005ff0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00006000: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00006010: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+00006020: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00006030: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00006040: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+00006050: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+00006060: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00006070: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+00006080: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00006090: 2020 7465 6d70 5f6d 6f64 656c 203d 2043    temp_model = C
+000060a0: 7265 6174 6545 6169 416c 6c52 6573 706f  reateEaiAllRespo
+000060b0: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
+000060c0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+000060d0: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+000060e0: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+000060f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00006100: 7365 6c66 0a0a 0a63 6c61 7373 2043 7265  self...class Cre
+00006110: 6174 6545 6169 4563 6952 6571 7565 7374  ateEaiEciRequest
+00006120: 4563 6943 6f6e 7461 696e 6572 2854 6561  EciContainer(Tea
+00006130: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+00006140: 5f5f 696e 6974 5f5f 2873 656c 662c 2061  __init__(self, a
+00006150: 7267 3d4e 6f6e 652c 2063 6f6d 6d61 6e64  rg=None, command
+00006160: 3d4e 6f6e 652c 2069 6d61 6765 3d4e 6f6e  =None, image=Non
+00006170: 652c 206e 616d 653d 4e6f 6e65 2c20 766f  e, name=None, vo
+00006180: 6c75 6d65 733d 4e6f 6e65 293a 0a20 2020  lumes=None):.   
+00006190: 2020 2020 2073 656c 662e 6172 6720 3d20       self.arg = 
+000061a0: 6172 6720 2023 2074 7970 653a 2073 7472  arg  # type: str
+000061b0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+000061c0: 6d6d 616e 6420 3d20 636f 6d6d 616e 6420  mmand = command 
+000061d0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+000061e0: 2020 2020 2073 656c 662e 696d 6167 6520       self.image 
+000061f0: 3d20 696d 6167 6520 2023 2074 7970 653a  = image  # type:
+00006200: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00006210: 662e 6e61 6d65 203d 206e 616d 6520 2023  f.name = name  #
+00006220: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
+00006230: 2020 2073 656c 662e 766f 6c75 6d65 7320     self.volumes 
+00006240: 3d20 766f 6c75 6d65 7320 2023 2074 7970  = volumes  # typ
+00006250: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
+00006260: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00006270: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00006280: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00006290: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000062a0: 203d 2073 7570 6572 2843 7265 6174 6545   = super(CreateE
+000062b0: 6169 4563 6952 6571 7565 7374 4563 6943  aiEciRequestEciC
+000062c0: 6f6e 7461 696e 6572 2c20 7365 6c66 292e  ontainer, self).
+000062d0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000062e0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+000062f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00006300: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00006310: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00006320: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00006330: 6620 7365 6c66 2e61 7267 2069 7320 6e6f  f self.arg is no
+00006340: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00006350: 2020 2020 7265 7375 6c74 5b27 4172 6727      result['Arg'
+00006360: 5d20 3d20 7365 6c66 2e61 7267 0a20 2020  ] = self.arg.   
+00006370: 2020 2020 2069 6620 7365 6c66 2e63 6f6d       if self.com
+00006380: 6d61 6e64 2069 7320 6e6f 7420 4e6f 6e65  mand is not None
+00006390: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000063a0: 7375 6c74 5b27 436f 6d6d 616e 6427 5d20  sult['Command'] 
+000063b0: 3d20 7365 6c66 2e63 6f6d 6d61 6e64 0a20  = self.command. 
+000063c0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+000063d0: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+000063e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000063f0: 7375 6c74 5b27 496d 6167 6527 5d20 3d20  sult['Image'] = 
+00006400: 7365 6c66 2e69 6d61 6765 0a20 2020 2020  self.image.     
+00006410: 2020 2069 6620 7365 6c66 2e6e 616d 6520     if self.name 
+00006420: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00006430: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00006440: 274e 616d 6527 5d20 3d20 7365 6c66 2e6e  'Name'] = self.n
+00006450: 616d 650a 2020 2020 2020 2020 6966 2073  ame.        if s
+00006460: 656c 662e 766f 6c75 6d65 7320 6973 206e  elf.volumes is n
+00006470: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00006480: 2020 2020 2072 6573 756c 745b 2756 6f6c       result['Vol
+00006490: 756d 6573 275d 203d 2073 656c 662e 766f  umes'] = self.vo
+000064a0: 6c75 6d65 730a 2020 2020 2020 2020 7265  lumes.        re
+000064b0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000064c0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000064d0: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+000064e0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+000064f0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00006500: 6d2e 6765 7428 2741 7267 2729 2069 7320  m.get('Arg') is 
+00006510: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00006520: 2020 2020 2020 7365 6c66 2e61 7267 203d        self.arg =
+00006530: 206d 2e67 6574 2827 4172 6727 290a 2020   m.get('Arg').  
+00006540: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00006550: 436f 6d6d 616e 6427 2920 6973 206e 6f74  Command') is not
 00006560: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006570: 2020 2073 656c 662e 7365 6375 7269 7479     self.security
-00006580: 5f67 726f 7570 5f69 6420 3d20 6d2e 6765  _group_id = m.ge
-00006590: 7428 2753 6563 7572 6974 7947 726f 7570  t('SecurityGroup
-000065a0: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-000065b0: 6d2e 6765 7428 2756 5377 6974 6368 4964  m.get('VSwitchId
-000065c0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000065d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000065e0: 2e76 5f73 7769 7463 685f 6964 203d 206d  .v_switch_id = m
-000065f0: 2e67 6574 2827 5653 7769 7463 6849 6427  .get('VSwitchId'
-00006600: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00006610: 2073 656c 660a 0a0a 636c 6173 7320 4372   self...class Cr
-00006620: 6561 7465 4561 6945 6369 5368 7269 6e6b  eateEaiEciShrink
-00006630: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
-00006640: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00006650: 745f 5f28 7365 6c66 2c20 636c 6965 6e74  t__(self, client
-00006660: 5f74 6f6b 656e 3d4e 6f6e 652c 2065 6169  _token=None, eai
-00006670: 735f 6e61 6d65 3d4e 6f6e 652c 2065 6169  s_name=None, eai
-00006680: 735f 7479 7065 3d4e 6f6e 652c 2065 6369  s_type=None, eci
-00006690: 5f73 6872 696e 6b3d 4e6f 6e65 2c20 7265  _shrink=None, re
-000066a0: 6769 6f6e 5f69 643d 4e6f 6e65 2c0a 2020  gion_id=None,.  
-000066b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000066c0: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-000066d0: 3d4e 6f6e 652c 2073 6563 7572 6974 795f  =None, security_
-000066e0: 6772 6f75 705f 6964 3d4e 6f6e 652c 2076  group_id=None, v
-000066f0: 5f73 7769 7463 685f 6964 3d4e 6f6e 6529  _switch_id=None)
-00006700: 3a0a 2020 2020 2020 2020 7365 6c66 2e63  :.        self.c
-00006710: 6c69 656e 745f 746f 6b65 6e20 3d20 636c  lient_token = cl
-00006720: 6965 6e74 5f74 6f6b 656e 2020 2320 7479  ient_token  # ty
-00006730: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-00006740: 7365 6c66 2e65 6169 735f 6e61 6d65 203d  self.eais_name =
-00006750: 2065 6169 735f 6e61 6d65 2020 2320 7479   eais_name  # ty
-00006760: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-00006770: 7365 6c66 2e65 6169 735f 7479 7065 203d  self.eais_type =
-00006780: 2065 6169 735f 7479 7065 2020 2320 7479   eais_type  # ty
-00006790: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-000067a0: 7365 6c66 2e65 6369 5f73 6872 696e 6b20  self.eci_shrink 
-000067b0: 3d20 6563 695f 7368 7269 6e6b 2020 2320  = eci_shrink  # 
-000067c0: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-000067d0: 2020 7365 6c66 2e72 6567 696f 6e5f 6964    self.region_id
-000067e0: 203d 2072 6567 696f 6e5f 6964 2020 2320   = region_id  # 
-000067f0: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-00006800: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
-00006810: 6772 6f75 705f 6964 203d 2072 6573 6f75  group_id = resou
-00006820: 7263 655f 6772 6f75 705f 6964 2020 2320  rce_group_id  # 
-00006830: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-00006840: 2020 7365 6c66 2e73 6563 7572 6974 795f    self.security_
-00006850: 6772 6f75 705f 6964 203d 2073 6563 7572  group_id = secur
-00006860: 6974 795f 6772 6f75 705f 6964 2020 2320  ity_group_id  # 
-00006870: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-00006880: 2020 7365 6c66 2e76 5f73 7769 7463 685f    self.v_switch_
-00006890: 6964 203d 2076 5f73 7769 7463 685f 6964  id = v_switch_id
-000068a0: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
-000068b0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-000068c0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-000068d0: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-000068e0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-000068f0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00006900: 4372 6561 7465 4561 6945 6369 5368 7269  CreateEaiEciShri
-00006910: 6e6b 5265 7175 6573 742c 2073 656c 6629  nkRequest, self)
-00006920: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00006930: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-00006940: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006950: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-00006960: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00006970: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00006980: 6966 2073 656c 662e 636c 6965 6e74 5f74  if self.client_t
-00006990: 6f6b 656e 2069 7320 6e6f 7420 4e6f 6e65  oken is not None
-000069a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000069b0: 7375 6c74 5b27 436c 6965 6e74 546f 6b65  sult['ClientToke
-000069c0: 6e27 5d20 3d20 7365 6c66 2e63 6c69 656e  n'] = self.clien
-000069d0: 745f 746f 6b65 6e0a 2020 2020 2020 2020  t_token.        
-000069e0: 6966 2073 656c 662e 6561 6973 5f6e 616d  if self.eais_nam
-000069f0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00006a00: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00006a10: 745b 2745 6169 734e 616d 6527 5d20 3d20  t['EaisName'] = 
-00006a20: 7365 6c66 2e65 6169 735f 6e61 6d65 0a20  self.eais_name. 
-00006a30: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-00006a40: 6169 735f 7479 7065 2069 7320 6e6f 7420  ais_type is not 
-00006a50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006a60: 2020 7265 7375 6c74 5b27 4561 6973 5479    result['EaisTy
-00006a70: 7065 275d 203d 2073 656c 662e 6561 6973  pe'] = self.eais
-00006a80: 5f74 7970 650a 2020 2020 2020 2020 6966  _type.        if
-00006a90: 2073 656c 662e 6563 695f 7368 7269 6e6b   self.eci_shrink
-00006aa0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00006ab0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00006ac0: 5b27 4563 6927 5d20 3d20 7365 6c66 2e65  ['Eci'] = self.e
-00006ad0: 6369 5f73 6872 696e 6b0a 2020 2020 2020  ci_shrink.      
-00006ae0: 2020 6966 2073 656c 662e 7265 6769 6f6e    if self.region
-00006af0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00006b00: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00006b10: 756c 745b 2752 6567 696f 6e49 6427 5d20  ult['RegionId'] 
-00006b20: 3d20 7365 6c66 2e72 6567 696f 6e5f 6964  = self.region_id
-00006b30: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00006b40: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
-00006b50: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00006b60: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00006b70: 6c74 5b27 5265 736f 7572 6365 4772 6f75  lt['ResourceGrou
-00006b80: 7049 6427 5d20 3d20 7365 6c66 2e72 6573  pId'] = self.res
-00006b90: 6f75 7263 655f 6772 6f75 705f 6964 0a20  ource_group_id. 
-00006ba0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00006bb0: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
-00006bc0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00006bd0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00006be0: 5b27 5365 6375 7269 7479 4772 6f75 7049  ['SecurityGroupI
-00006bf0: 6427 5d20 3d20 7365 6c66 2e73 6563 7572  d'] = self.secur
-00006c00: 6974 795f 6772 6f75 705f 6964 0a20 2020  ity_group_id.   
-00006c10: 2020 2020 2069 6620 7365 6c66 2e76 5f73       if self.v_s
-00006c20: 7769 7463 685f 6964 2069 7320 6e6f 7420  witch_id is not 
-00006c30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006c40: 2020 7265 7375 6c74 5b27 5653 7769 7463    result['VSwitc
-00006c50: 6849 6427 5d20 3d20 7365 6c66 2e76 5f73  hId'] = self.v_s
-00006c60: 7769 7463 685f 6964 0a20 2020 2020 2020  witch_id.       
-00006c70: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00006c80: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-00006c90: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-00006ca0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00006cb0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00006cc0: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
-00006cd0: 546f 6b65 6e27 2920 6973 206e 6f74 204e  Token') is not N
-00006ce0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00006cf0: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
-00006d00: 656e 203d 206d 2e67 6574 2827 436c 6965  en = m.get('Clie
-00006d10: 6e74 546f 6b65 6e27 290a 2020 2020 2020  ntToken').      
-00006d20: 2020 6966 206d 2e67 6574 2827 4561 6973    if m.get('Eais
-00006d30: 4e61 6d65 2729 2069 7320 6e6f 7420 4e6f  Name') is not No
-00006d40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00006d50: 7365 6c66 2e65 6169 735f 6e61 6d65 203d  self.eais_name =
-00006d60: 206d 2e67 6574 2827 4561 6973 4e61 6d65   m.get('EaisName
-00006d70: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00006d80: 6765 7428 2745 6169 7354 7970 6527 2920  get('EaisType') 
-00006d90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00006da0: 2020 2020 2020 2020 2073 656c 662e 6561           self.ea
-00006db0: 6973 5f74 7970 6520 3d20 6d2e 6765 7428  is_type = m.get(
-00006dc0: 2745 6169 7354 7970 6527 290a 2020 2020  'EaisType').    
-00006dd0: 2020 2020 6966 206d 2e67 6574 2827 4563      if m.get('Ec
-00006de0: 6927 2920 6973 206e 6f74 204e 6f6e 653a  i') is not None:
-00006df0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006e00: 662e 6563 695f 7368 7269 6e6b 203d 206d  f.eci_shrink = m
-00006e10: 2e67 6574 2827 4563 6927 290a 2020 2020  .get('Eci').    
-00006e20: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-00006e30: 6769 6f6e 4964 2729 2069 7320 6e6f 7420  gionId') is not 
-00006e40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006e50: 2020 7365 6c66 2e72 6567 696f 6e5f 6964    self.region_id
-00006e60: 203d 206d 2e67 6574 2827 5265 6769 6f6e   = m.get('Region
-00006e70: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-00006e80: 6d2e 6765 7428 2752 6573 6f75 7263 6547  m.get('ResourceG
-00006e90: 726f 7570 4964 2729 2069 7320 6e6f 7420  roupId') is not 
-00006ea0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006eb0: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
-00006ec0: 6772 6f75 705f 6964 203d 206d 2e67 6574  group_id = m.get
-00006ed0: 2827 5265 736f 7572 6365 4772 6f75 7049  ('ResourceGroupI
-00006ee0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00006ef0: 2e67 6574 2827 5365 6375 7269 7479 4772  .get('SecurityGr
-00006f00: 6f75 7049 6427 2920 6973 206e 6f74 204e  oupId') is not N
-00006f10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00006f20: 2073 656c 662e 7365 6375 7269 7479 5f67   self.security_g
-00006f30: 726f 7570 5f69 6420 3d20 6d2e 6765 7428  roup_id = m.get(
-00006f40: 2753 6563 7572 6974 7947 726f 7570 4964  'SecurityGroupId
-00006f50: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00006f60: 6765 7428 2756 5377 6974 6368 4964 2729  get('VSwitchId')
-00006f70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00006f80: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-00006f90: 5f73 7769 7463 685f 6964 203d 206d 2e67  _switch_id = m.g
-00006fa0: 6574 2827 5653 7769 7463 6849 6427 290a  et('VSwitchId').
-00006fb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00006fc0: 656c 660a 0a0a 636c 6173 7320 4372 6561  elf...class Crea
-00006fd0: 7465 4561 6945 6369 5265 7370 6f6e 7365  teEaiEciResponse
-00006fe0: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
-00006ff0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00007000: 2873 656c 662c 2063 6c69 656e 745f 696e  (self, client_in
-00007010: 7374 616e 6365 5f69 643d 4e6f 6e65 2c20  stance_id=None, 
-00007020: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
-00007030: 7465 645f 696e 7374 616e 6365 5f69 643d  ted_instance_id=
-00007040: 4e6f 6e65 2c20 7265 7175 6573 745f 6964  None, request_id
-00007050: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00007060: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
-00007070: 616e 6365 5f69 6420 3d20 636c 6965 6e74  ance_id = client
-00007080: 5f69 6e73 7461 6e63 655f 6964 2020 2320  _instance_id  # 
-00007090: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-000070a0: 2020 7365 6c66 2e65 6c61 7374 6963 5f61    self.elastic_a
-000070b0: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
-000070c0: 6e63 655f 6964 203d 2065 6c61 7374 6963  nce_id = elastic
-000070d0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
-000070e0: 7461 6e63 655f 6964 2020 2320 7479 7065  tance_id  # type
-000070f0: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-00007100: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-00007110: 7265 7175 6573 745f 6964 2020 2320 7479  request_id  # ty
-00007120: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
-00007130: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-00007140: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00007150: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00007160: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00007170: 7020 3d20 7375 7065 7228 4372 6561 7465  p = super(Create
-00007180: 4561 6945 6369 5265 7370 6f6e 7365 426f  EaiEciResponseBo
-00007190: 6479 2c20 7365 6c66 292e 746f 5f6d 6170  dy, self).to_map
-000071a0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-000071b0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-000071c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000071d0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-000071e0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-000071f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00007200: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
-00007210: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00007220: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00007230: 756c 745b 2743 6c69 656e 7449 6e73 7461  ult['ClientInsta
-00007240: 6e63 6549 6427 5d20 3d20 7365 6c66 2e63  nceId'] = self.c
-00007250: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
-00007260: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00007270: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-00007280: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-00007290: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000072a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000072b0: 745b 2745 6c61 7374 6963 4163 6365 6c65  t['ElasticAccele
-000072c0: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
-000072d0: 5d20 3d20 7365 6c66 2e65 6c61 7374 6963  ] = self.elastic
-000072e0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
-000072f0: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
-00007300: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
-00007310: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00007320: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00007330: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
-00007340: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
-00007350: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-00007360: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00007370: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00007380: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-00007390: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-000073a0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000073b0: 6574 2827 436c 6965 6e74 496e 7374 616e  et('ClientInstan
-000073c0: 6365 4964 2729 2069 7320 6e6f 7420 4e6f  ceId') is not No
-000073d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000073e0: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
-000073f0: 616e 6365 5f69 6420 3d20 6d2e 6765 7428  ance_id = m.get(
-00007400: 2743 6c69 656e 7449 6e73 7461 6e63 6549  'ClientInstanceI
-00007410: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00007420: 2e67 6574 2827 456c 6173 7469 6341 6363  .get('ElasticAcc
-00007430: 656c 6572 6174 6564 496e 7374 616e 6365  eleratedInstance
-00007440: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00007450: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00007460: 6c66 2e65 6c61 7374 6963 5f61 6363 656c  lf.elastic_accel
-00007470: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
-00007480: 6964 203d 206d 2e67 6574 2827 456c 6173  id = m.get('Elas
-00007490: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
-000074a0: 7374 616e 6365 4964 2729 0a20 2020 2020  stanceId').     
-000074b0: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
-000074c0: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
-000074d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000074e0: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
-000074f0: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
-00007500: 7374 4964 2729 0a20 2020 2020 2020 2072  stId').        r
-00007510: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-00007520: 7373 2043 7265 6174 6545 6169 4563 6952  ss CreateEaiEciR
-00007530: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-00007540: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00007550: 745f 5f28 7365 6c66 2c20 6865 6164 6572  t__(self, header
-00007560: 733d 4e6f 6e65 2c20 7374 6174 7573 5f63  s=None, status_c
-00007570: 6f64 653d 4e6f 6e65 2c20 626f 6479 3d4e  ode=None, body=N
-00007580: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-00007590: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
-000075a0: 6465 7273 2020 2320 7479 7065 3a20 6469  ders  # type: di
-000075b0: 6374 5b73 7472 2c20 7374 725d 0a20 2020  ct[str, str].   
-000075c0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-000075d0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-000075e0: 6f64 6520 2023 2074 7970 653a 2069 6e74  ode  # type: int
-000075f0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-00007600: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
-00007610: 653a 2043 7265 6174 6545 6169 4563 6952  e: CreateEaiEciR
-00007620: 6573 706f 6e73 6542 6f64 790a 0a20 2020  esponseBody..   
-00007630: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00007640: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00007650: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00007660: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
-00007670: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
-00007680: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00007690: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-000076a0: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
-000076b0: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
-000076c0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-000076d0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-000076e0: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
-000076f0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00007700: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-00007710: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-00007720: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-00007730: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00007740: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00007750: 7228 4372 6561 7465 4561 6945 6369 5265  r(CreateEaiEciRe
-00007760: 7370 6f6e 7365 2c20 7365 6c66 292e 746f  sponse, self).to
-00007770: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-00007780: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-00007790: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000077a0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-000077b0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-000077c0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000077d0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-000077e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000077f0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-00007800: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-00007810: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-00007820: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
-00007830: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
-00007840: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00007850: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
-00007860: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
-00007870: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
-00007880: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-00007890: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000078a0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-000078b0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-000078c0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-000078d0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-000078e0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-000078f0: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
-00007900: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-00007910: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00007920: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-00007930: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00007940: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-00007950: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
-00007960: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-00007970: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
-00007980: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
-00007990: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000079a0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-000079b0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
-000079c0: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
-000079d0: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-000079e0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000079f0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-00007a00: 6d6f 6465 6c20 3d20 4372 6561 7465 4561  model = CreateEa
-00007a10: 6945 6369 5265 7370 6f6e 7365 426f 6479  iEciResponseBody
-00007a20: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00007a30: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-00007a40: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-00007a50: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-00007a60: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00007a70: 636c 6173 7320 4372 6561 7465 4561 6945  class CreateEaiE
-00007a80: 6373 5265 7175 6573 7445 6373 2854 6561  csRequestEcs(Tea
-00007a90: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00007aa0: 5f5f 696e 6974 5f5f 2873 656c 662c 2069  __init__(self, i
-00007ab0: 6d61 6765 5f69 643d 4e6f 6e65 2c20 696e  mage_id=None, in
-00007ac0: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
-00007ad0: 6964 7468 5f69 6e3d 4e6f 6e65 2c20 696e  idth_in=None, in
-00007ae0: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
-00007af0: 6964 7468 5f6f 7574 3d4e 6f6e 652c 206e  idth_out=None, n
-00007b00: 616d 653d 4e6f 6e65 2c0a 2020 2020 2020  ame=None,.      
-00007b10: 2020 2020 2020 2020 2020 2070 6173 7377             passw
-00007b20: 6f72 643d 4e6f 6e65 2c20 7379 7374 656d  ord=None, system
-00007b30: 5f64 6973 6b5f 6361 7465 676f 7279 3d4e  _disk_category=N
-00007b40: 6f6e 652c 2073 7973 7465 6d5f 6469 736b  one, system_disk
-00007b50: 5f73 697a 653d 4e6f 6e65 2c20 7479 7065  _size=None, type
-00007b60: 3d4e 6f6e 652c 207a 6f6e 655f 6964 3d4e  =None, zone_id=N
-00007b70: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-00007b80: 6c66 2e69 6d61 6765 5f69 6420 3d20 696d  lf.image_id = im
-00007b90: 6167 655f 6964 2020 2320 7479 7065 3a20  age_id  # type: 
-00007ba0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-00007bb0: 2e69 6e74 6572 6e65 745f 6d61 785f 6261  .internet_max_ba
-00007bc0: 6e64 7769 6474 685f 696e 203d 2069 6e74  ndwidth_in = int
-00007bd0: 6572 6e65 745f 6d61 785f 6261 6e64 7769  ernet_max_bandwi
-00007be0: 6474 685f 696e 2020 2320 7479 7065 3a20  dth_in  # type: 
-00007bf0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-00007c00: 2e69 6e74 6572 6e65 745f 6d61 785f 6261  .internet_max_ba
-00007c10: 6e64 7769 6474 685f 6f75 7420 3d20 696e  ndwidth_out = in
-00007c20: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
-00007c30: 6964 7468 5f6f 7574 2020 2320 7479 7065  idth_out  # type
-00007c40: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-00007c50: 6c66 2e6e 616d 6520 3d20 6e61 6d65 2020  lf.name = name  
-00007c60: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00007c70: 2020 2020 7365 6c66 2e70 6173 7377 6f72      self.passwor
-00007c80: 6420 3d20 7061 7373 776f 7264 2020 2320  d = password  # 
-00007c90: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-00007ca0: 2020 7365 6c66 2e73 7973 7465 6d5f 6469    self.system_di
-00007cb0: 736b 5f63 6174 6567 6f72 7920 3d20 7379  sk_category = sy
-00007cc0: 7374 656d 5f64 6973 6b5f 6361 7465 676f  stem_disk_catego
-00007cd0: 7279 2020 2320 7479 7065 3a20 7374 720a  ry  # type: str.
-00007ce0: 2020 2020 2020 2020 7365 6c66 2e73 7973          self.sys
-00007cf0: 7465 6d5f 6469 736b 5f73 697a 6520 3d20  tem_disk_size = 
-00007d00: 7379 7374 656d 5f64 6973 6b5f 7369 7a65  system_disk_size
-00007d10: 2020 2320 7479 7065 3a20 6c6f 6e67 0a20    # type: long. 
-00007d20: 2020 2020 2020 2073 656c 662e 7479 7065         self.type
-00007d30: 203d 2074 7970 6520 2023 2074 7970 653a   = type  # type:
-00007d40: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
-00007d50: 662e 7a6f 6e65 5f69 6420 3d20 7a6f 6e65  f.zone_id = zone
-00007d60: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
-00007d70: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00007d80: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00007d90: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00007da0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00007db0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00007dc0: 6572 2843 7265 6174 6545 6169 4563 7352  er(CreateEaiEcsR
-00007dd0: 6571 7565 7374 4563 732c 2073 656c 6629  equestEcs, self)
-00007de0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00007df0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-00007e00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007e10: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-00007e20: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00007e30: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00007e40: 6966 2073 656c 662e 696d 6167 655f 6964  if self.image_id
-00007e50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00007e60: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00007e70: 5b27 496d 6167 6549 6427 5d20 3d20 7365  ['ImageId'] = se
-00007e80: 6c66 2e69 6d61 6765 5f69 640a 2020 2020  lf.image_id.    
-00007e90: 2020 2020 6966 2073 656c 662e 696e 7465      if self.inte
-00007ea0: 726e 6574 5f6d 6178 5f62 616e 6477 6964  rnet_max_bandwid
-00007eb0: 7468 5f69 6e20 6973 206e 6f74 204e 6f6e  th_in is not Non
-00007ec0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00007ed0: 6573 756c 745b 2749 6e74 6572 6e65 744d  esult['InternetM
-00007ee0: 6178 4261 6e64 7769 6474 6849 6e27 5d20  axBandwidthIn'] 
-00007ef0: 3d20 7365 6c66 2e69 6e74 6572 6e65 745f  = self.internet_
-00007f00: 6d61 785f 6261 6e64 7769 6474 685f 696e  max_bandwidth_in
-00007f10: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00007f20: 2e69 6e74 6572 6e65 745f 6d61 785f 6261  .internet_max_ba
-00007f30: 6e64 7769 6474 685f 6f75 7420 6973 206e  ndwidth_out is n
-00007f40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00007f50: 2020 2020 2072 6573 756c 745b 2749 6e74       result['Int
-00007f60: 6572 6e65 744d 6178 4261 6e64 7769 6474  ernetMaxBandwidt
-00007f70: 684f 7574 275d 203d 2073 656c 662e 696e  hOut'] = self.in
-00007f80: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
-00007f90: 6964 7468 5f6f 7574 0a20 2020 2020 2020  idth_out.       
-00007fa0: 2069 6620 7365 6c66 2e6e 616d 6520 6973   if self.name is
-00007fb0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00007fc0: 2020 2020 2020 2072 6573 756c 745b 274e         result['N
-00007fd0: 616d 6527 5d20 3d20 7365 6c66 2e6e 616d  ame'] = self.nam
-00007fe0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00007ff0: 662e 7061 7373 776f 7264 2069 7320 6e6f  f.password is no
-00008000: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00008010: 2020 2020 7265 7375 6c74 5b27 5061 7373      result['Pass
-00008020: 776f 7264 275d 203d 2073 656c 662e 7061  word'] = self.pa
-00008030: 7373 776f 7264 0a20 2020 2020 2020 2069  ssword.        i
-00008040: 6620 7365 6c66 2e73 7973 7465 6d5f 6469  f self.system_di
-00008050: 736b 5f63 6174 6567 6f72 7920 6973 206e  sk_category is n
-00008060: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00008070: 2020 2020 2072 6573 756c 745b 2753 7973       result['Sys
-00008080: 7465 6d44 6973 6b43 6174 6567 6f72 7927  temDiskCategory'
-00008090: 5d20 3d20 7365 6c66 2e73 7973 7465 6d5f  ] = self.system_
-000080a0: 6469 736b 5f63 6174 6567 6f72 790a 2020  disk_category.  
-000080b0: 2020 2020 2020 6966 2073 656c 662e 7379        if self.sy
-000080c0: 7374 656d 5f64 6973 6b5f 7369 7a65 2069  stem_disk_size i
-000080d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000080e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000080f0: 5379 7374 656d 4469 736b 5369 7a65 275d  SystemDiskSize']
-00008100: 203d 2073 656c 662e 7379 7374 656d 5f64   = self.system_d
-00008110: 6973 6b5f 7369 7a65 0a20 2020 2020 2020  isk_size.       
-00008120: 2069 6620 7365 6c66 2e74 7970 6520 6973   if self.type is
-00008130: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00008140: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
-00008150: 7970 6527 5d20 3d20 7365 6c66 2e74 7970  ype'] = self.typ
-00008160: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00008170: 662e 7a6f 6e65 5f69 6420 6973 206e 6f74  f.zone_id is not
-00008180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00008190: 2020 2072 6573 756c 745b 275a 6f6e 6549     result['ZoneI
-000081a0: 6427 5d20 3d20 7365 6c66 2e7a 6f6e 655f  d'] = self.zone_
-000081b0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-000081c0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-000081d0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000081e0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-000081f0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00008200: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00008210: 6574 2827 496d 6167 6549 6427 2920 6973  et('ImageId') is
-00008220: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00008230: 2020 2020 2020 2073 656c 662e 696d 6167         self.imag
-00008240: 655f 6964 203d 206d 2e67 6574 2827 496d  e_id = m.get('Im
-00008250: 6167 6549 6427 290a 2020 2020 2020 2020  ageId').        
-00008260: 6966 206d 2e67 6574 2827 496e 7465 726e  if m.get('Intern
-00008270: 6574 4d61 7842 616e 6477 6964 7468 496e  etMaxBandwidthIn
-00008280: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00008290: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000082a0: 2e69 6e74 6572 6e65 745f 6d61 785f 6261  .internet_max_ba
-000082b0: 6e64 7769 6474 685f 696e 203d 206d 2e67  ndwidth_in = m.g
-000082c0: 6574 2827 496e 7465 726e 6574 4d61 7842  et('InternetMaxB
-000082d0: 616e 6477 6964 7468 496e 2729 0a20 2020  andwidthIn').   
-000082e0: 2020 2020 2069 6620 6d2e 6765 7428 2749       if m.get('I
-000082f0: 6e74 6572 6e65 744d 6178 4261 6e64 7769  nternetMaxBandwi
-00008300: 6474 684f 7574 2729 2069 7320 6e6f 7420  dthOut') is not 
-00008310: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00008320: 2020 7365 6c66 2e69 6e74 6572 6e65 745f    self.internet_
-00008330: 6d61 785f 6261 6e64 7769 6474 685f 6f75  max_bandwidth_ou
-00008340: 7420 3d20 6d2e 6765 7428 2749 6e74 6572  t = m.get('Inter
-00008350: 6e65 744d 6178 4261 6e64 7769 6474 684f  netMaxBandwidthO
-00008360: 7574 2729 0a20 2020 2020 2020 2069 6620  ut').        if 
-00008370: 6d2e 6765 7428 274e 616d 6527 2920 6973  m.get('Name') is
-00008380: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00008390: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
-000083a0: 203d 206d 2e67 6574 2827 4e61 6d65 2729   = m.get('Name')
-000083b0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000083c0: 7428 2750 6173 7377 6f72 6427 2920 6973  t('Password') is
-000083d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000083e0: 2020 2020 2020 2073 656c 662e 7061 7373         self.pass
-000083f0: 776f 7264 203d 206d 2e67 6574 2827 5061  word = m.get('Pa
-00008400: 7373 776f 7264 2729 0a20 2020 2020 2020  ssword').       
-00008410: 2069 6620 6d2e 6765 7428 2753 7973 7465   if m.get('Syste
-00008420: 6d44 6973 6b43 6174 6567 6f72 7927 2920  mDiskCategory') 
-00008430: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00008440: 2020 2020 2020 2020 2073 656c 662e 7379           self.sy
-00008450: 7374 656d 5f64 6973 6b5f 6361 7465 676f  stem_disk_catego
-00008460: 7279 203d 206d 2e67 6574 2827 5379 7374  ry = m.get('Syst
-00008470: 656d 4469 736b 4361 7465 676f 7279 2729  emDiskCategory')
-00008480: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00008490: 7428 2753 7973 7465 6d44 6973 6b53 697a  t('SystemDiskSiz
-000084a0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-000084b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000084c0: 662e 7379 7374 656d 5f64 6973 6b5f 7369  f.system_disk_si
-000084d0: 7a65 203d 206d 2e67 6574 2827 5379 7374  ze = m.get('Syst
-000084e0: 656d 4469 736b 5369 7a65 2729 0a20 2020  emDiskSize').   
-000084f0: 2020 2020 2069 6620 6d2e 6765 7428 2754       if m.get('T
-00008500: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
-00008510: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00008520: 656c 662e 7479 7065 203d 206d 2e67 6574  elf.type = m.get
-00008530: 2827 5479 7065 2729 0a20 2020 2020 2020  ('Type').       
-00008540: 2069 6620 6d2e 6765 7428 275a 6f6e 6549   if m.get('ZoneI
-00008550: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00008560: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008570: 662e 7a6f 6e65 5f69 6420 3d20 6d2e 6765  f.zone_id = m.ge
-00008580: 7428 275a 6f6e 6549 6427 290a 2020 2020  t('ZoneId').    
-00008590: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-000085a0: 0a0a 636c 6173 7320 4372 6561 7465 4561  ..class CreateEa
-000085b0: 6945 6373 5265 7175 6573 7428 5465 614d  iEcsRequest(TeaM
-000085c0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000085d0: 5f69 6e69 745f 5f28 7365 6c66 2c20 636c  _init__(self, cl
-000085e0: 6965 6e74 5f74 6f6b 656e 3d4e 6f6e 652c  ient_token=None,
-000085f0: 2065 6169 735f 6e61 6d65 3d4e 6f6e 652c   eais_name=None,
-00008600: 2065 6169 735f 7479 7065 3d4e 6f6e 652c   eais_type=None,
-00008610: 2065 6373 3d4e 6f6e 652c 2072 6567 696f   ecs=None, regio
-00008620: 6e5f 6964 3d4e 6f6e 652c 0a20 2020 2020  n_id=None,.     
-00008630: 2020 2020 2020 2020 2020 2020 7265 736f              reso
-00008640: 7572 6365 5f67 726f 7570 5f69 643d 4e6f  urce_group_id=No
-00008650: 6e65 2c20 7365 6375 7269 7479 5f67 726f  ne, security_gro
-00008660: 7570 5f69 643d 4e6f 6e65 2c20 765f 7377  up_id=None, v_sw
-00008670: 6974 6368 5f69 643d 4e6f 6e65 293a 0a20  itch_id=None):. 
-00008680: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
-00008690: 6e74 5f74 6f6b 656e 203d 2063 6c69 656e  nt_token = clien
-000086a0: 745f 746f 6b65 6e20 2023 2074 7970 653a  t_token  # type:
-000086b0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
-000086c0: 662e 6561 6973 5f6e 616d 6520 3d20 6561  f.eais_name = ea
-000086d0: 6973 5f6e 616d 6520 2023 2074 7970 653a  is_name  # type:
-000086e0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
-000086f0: 662e 6561 6973 5f74 7970 6520 3d20 6561  f.eais_type = ea
-00008700: 6973 5f74 7970 6520 2023 2074 7970 653a  is_type  # type:
-00008710: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
-00008720: 662e 6563 7320 3d20 6563 7320 2023 2074  f.ecs = ecs  # t
-00008730: 7970 653a 2043 7265 6174 6545 6169 4563  ype: CreateEaiEc
-00008740: 7352 6571 7565 7374 4563 730a 2020 2020  sRequestEcs.    
-00008750: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
-00008760: 6964 203d 2072 6567 696f 6e5f 6964 2020  id = region_id  
-00008770: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00008780: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
-00008790: 655f 6772 6f75 705f 6964 203d 2072 6573  e_group_id = res
-000087a0: 6f75 7263 655f 6772 6f75 705f 6964 2020  ource_group_id  
-000087b0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-000087c0: 2020 2020 7365 6c66 2e73 6563 7572 6974      self.securit
-000087d0: 795f 6772 6f75 705f 6964 203d 2073 6563  y_group_id = sec
-000087e0: 7572 6974 795f 6772 6f75 705f 6964 2020  urity_group_id  
-000087f0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00008800: 2020 2020 7365 6c66 2e76 5f73 7769 7463      self.v_switc
-00008810: 685f 6964 203d 2076 5f73 7769 7463 685f  h_id = v_switch_
-00008820: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-00008830: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00008840: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00008850: 2069 6620 7365 6c66 2e65 6373 3a0a 2020   if self.ecs:.  
-00008860: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-00008870: 6373 2e76 616c 6964 6174 6528 290a 0a20  cs.validate().. 
-00008880: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00008890: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-000088a0: 7020 3d20 7375 7065 7228 4372 6561 7465  p = super(Create
-000088b0: 4561 6945 6373 5265 7175 6573 742c 2073  EaiEcsRequest, s
-000088c0: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
-000088d0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-000088e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000088f0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-00008900: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-00008910: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-00008920: 2020 2020 6966 2073 656c 662e 636c 6965      if self.clie
-00008930: 6e74 5f74 6f6b 656e 2069 7320 6e6f 7420  nt_token is not 
-00008940: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00008950: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-00008960: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e63  Token'] = self.c
-00008970: 6c69 656e 745f 746f 6b65 6e0a 2020 2020  lient_token.    
-00008980: 2020 2020 6966 2073 656c 662e 6561 6973      if self.eais
-00008990: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
-000089a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000089b0: 6573 756c 745b 2745 6169 734e 616d 6527  esult['EaisName'
-000089c0: 5d20 3d20 7365 6c66 2e65 6169 735f 6e61  ] = self.eais_na
-000089d0: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
-000089e0: 6c66 2e65 6169 735f 7479 7065 2069 7320  lf.eais_type is 
-000089f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00008a00: 2020 2020 2020 7265 7375 6c74 5b27 4561        result['Ea
-00008a10: 6973 5479 7065 275d 203d 2073 656c 662e  isType'] = self.
-00008a20: 6561 6973 5f74 7970 650a 2020 2020 2020  eais_type.      
-00008a30: 2020 6966 2073 656c 662e 6563 7320 6973    if self.ecs is
-00008a40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00008a50: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
-00008a60: 6373 275d 203d 2073 656c 662e 6563 732e  cs'] = self.ecs.
-00008a70: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00008a80: 2069 6620 7365 6c66 2e72 6567 696f 6e5f   if self.region_
-00008a90: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00008aa0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00008ab0: 6c74 5b27 5265 6769 6f6e 4964 275d 203d  lt['RegionId'] =
-00008ac0: 2073 656c 662e 7265 6769 6f6e 5f69 640a   self.region_id.
-00008ad0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00008ae0: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-00008af0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00008b00: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00008b10: 745b 2752 6573 6f75 7263 6547 726f 7570  t['ResourceGroup
-00008b20: 4964 275d 203d 2073 656c 662e 7265 736f  Id'] = self.reso
-00008b30: 7572 6365 5f67 726f 7570 5f69 640a 2020  urce_group_id.  
-00008b40: 2020 2020 2020 6966 2073 656c 662e 7365        if self.se
-00008b50: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
-00008b60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00008b70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00008b80: 2753 6563 7572 6974 7947 726f 7570 4964  'SecurityGroupId
-00008b90: 275d 203d 2073 656c 662e 7365 6375 7269  '] = self.securi
-00008ba0: 7479 5f67 726f 7570 5f69 640a 2020 2020  ty_group_id.    
-00008bb0: 2020 2020 6966 2073 656c 662e 765f 7377      if self.v_sw
-00008bc0: 6974 6368 5f69 6420 6973 206e 6f74 204e  itch_id is not N
-00008bd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00008be0: 2072 6573 756c 745b 2756 5377 6974 6368   result['VSwitch
-00008bf0: 4964 275d 203d 2073 656c 662e 765f 7377  Id'] = self.v_sw
-00008c00: 6974 6368 5f69 640a 2020 2020 2020 2020  itch_id.        
-00008c10: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00008c20: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00008c30: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
-00008c40: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00008c50: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00008c60: 6620 6d2e 6765 7428 2743 6c69 656e 7454  f m.get('ClientT
-00008c70: 6f6b 656e 2729 2069 7320 6e6f 7420 4e6f  oken') is not No
-00008c80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00008c90: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
-00008ca0: 6e20 3d20 6d2e 6765 7428 2743 6c69 656e  n = m.get('Clien
-00008cb0: 7454 6f6b 656e 2729 0a20 2020 2020 2020  tToken').       
-00008cc0: 2069 6620 6d2e 6765 7428 2745 6169 734e   if m.get('EaisN
-00008cd0: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
-00008ce0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00008cf0: 656c 662e 6561 6973 5f6e 616d 6520 3d20  elf.eais_name = 
-00008d00: 6d2e 6765 7428 2745 6169 734e 616d 6527  m.get('EaisName'
-00008d10: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00008d20: 6574 2827 4561 6973 5479 7065 2729 2069  et('EaisType') i
-00008d30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00008d40: 2020 2020 2020 2020 7365 6c66 2e65 6169          self.eai
-00008d50: 735f 7479 7065 203d 206d 2e67 6574 2827  s_type = m.get('
-00008d60: 4561 6973 5479 7065 2729 0a20 2020 2020  EaisType').     
-00008d70: 2020 2069 6620 6d2e 6765 7428 2745 6373     if m.get('Ecs
-00008d80: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00008d90: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00008da0: 5f6d 6f64 656c 203d 2043 7265 6174 6545  _model = CreateE
-00008db0: 6169 4563 7352 6571 7565 7374 4563 7328  aiEcsRequestEcs(
-00008dc0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00008dd0: 6c66 2e65 6373 203d 2074 656d 705f 6d6f  lf.ecs = temp_mo
-00008de0: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
-00008df0: 4563 7327 5d29 0a20 2020 2020 2020 2069  Ecs']).        i
-00008e00: 6620 6d2e 6765 7428 2752 6567 696f 6e49  f m.get('RegionI
-00008e10: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00008e20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008e30: 662e 7265 6769 6f6e 5f69 6420 3d20 6d2e  f.region_id = m.
-00008e40: 6765 7428 2752 6567 696f 6e49 6427 290a  get('RegionId').
-00008e50: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00008e60: 2827 5265 736f 7572 6365 4772 6f75 7049  ('ResourceGroupI
-00008e70: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00008e80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008e90: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
-00008ea0: 5f69 6420 3d20 6d2e 6765 7428 2752 6573  _id = m.get('Res
-00008eb0: 6f75 7263 6547 726f 7570 4964 2729 0a20  ourceGroupId'). 
-00008ec0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00008ed0: 2753 6563 7572 6974 7947 726f 7570 4964  'SecurityGroupId
-00008ee0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00008ef0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008f00: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
-00008f10: 6964 203d 206d 2e67 6574 2827 5365 6375  id = m.get('Secu
-00008f20: 7269 7479 4772 6f75 7049 6427 290a 2020  rityGroupId').  
-00008f30: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00008f40: 5653 7769 7463 6849 6427 2920 6973 206e  VSwitchId') is n
-00008f50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00008f60: 2020 2020 2073 656c 662e 765f 7377 6974       self.v_swit
-00008f70: 6368 5f69 6420 3d20 6d2e 6765 7428 2756  ch_id = m.get('V
-00008f80: 5377 6974 6368 4964 2729 0a20 2020 2020  SwitchId').     
-00008f90: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00008fa0: 0a63 6c61 7373 2043 7265 6174 6545 6169  .class CreateEai
-00008fb0: 4563 7353 6872 696e 6b52 6571 7565 7374  EcsShrinkRequest
-00008fc0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00008fd0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00008fe0: 662c 2063 6c69 656e 745f 746f 6b65 6e3d  f, client_token=
-00008ff0: 4e6f 6e65 2c20 6561 6973 5f6e 616d 653d  None, eais_name=
-00009000: 4e6f 6e65 2c20 6561 6973 5f74 7970 653d  None, eais_type=
-00009010: 4e6f 6e65 2c20 6563 735f 7368 7269 6e6b  None, ecs_shrink
-00009020: 3d4e 6f6e 652c 2072 6567 696f 6e5f 6964  =None, region_id
-00009030: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00009040: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-00009050: 5f67 726f 7570 5f69 643d 4e6f 6e65 2c20  _group_id=None, 
-00009060: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
-00009070: 643d 4e6f 6e65 2c20 765f 7377 6974 6368  d=None, v_switch
-00009080: 5f69 643d 4e6f 6e65 293a 0a20 2020 2020  _id=None):.     
-00009090: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
-000090a0: 6f6b 656e 203d 2063 6c69 656e 745f 746f  oken = client_to
-000090b0: 6b65 6e20 2023 2074 7970 653a 2073 7472  ken  # type: str
-000090c0: 0a20 2020 2020 2020 2073 656c 662e 6561  .        self.ea
-000090d0: 6973 5f6e 616d 6520 3d20 6561 6973 5f6e  is_name = eais_n
-000090e0: 616d 6520 2023 2074 7970 653a 2073 7472  ame  # type: str
-000090f0: 0a20 2020 2020 2020 2073 656c 662e 6561  .        self.ea
-00009100: 6973 5f74 7970 6520 3d20 6561 6973 5f74  is_type = eais_t
-00009110: 7970 6520 2023 2074 7970 653a 2073 7472  ype  # type: str
-00009120: 0a20 2020 2020 2020 2073 656c 662e 6563  .        self.ec
-00009130: 735f 7368 7269 6e6b 203d 2065 6373 5f73  s_shrink = ecs_s
-00009140: 6872 696e 6b20 2023 2074 7970 653a 2073  hrink  # type: s
-00009150: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-00009160: 7265 6769 6f6e 5f69 6420 3d20 7265 6769  region_id = regi
-00009170: 6f6e 5f69 6420 2023 2074 7970 653a 2073  on_id  # type: s
-00009180: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-00009190: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-000091a0: 6420 3d20 7265 736f 7572 6365 5f67 726f  d = resource_gro
-000091b0: 7570 5f69 6420 2023 2074 7970 653a 2073  up_id  # type: s
-000091c0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-000091d0: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
-000091e0: 6420 3d20 7365 6375 7269 7479 5f67 726f  d = security_gro
-000091f0: 7570 5f69 6420 2023 2074 7970 653a 2073  up_id  # type: s
-00009200: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-00009210: 765f 7377 6974 6368 5f69 6420 3d20 765f  v_switch_id = v_
-00009220: 7377 6974 6368 5f69 6420 2023 2074 7970  switch_id  # typ
-00009230: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
-00009240: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-00009250: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00009260: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00009270: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00009280: 203d 2073 7570 6572 2843 7265 6174 6545   = super(CreateE
-00009290: 6169 4563 7353 6872 696e 6b52 6571 7565  aiEcsShrinkReque
-000092a0: 7374 2c20 7365 6c66 292e 746f 5f6d 6170  st, self).to_map
-000092b0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-000092c0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-000092d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000092e0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-000092f0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-00009300: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00009310: 2e63 6c69 656e 745f 746f 6b65 6e20 6973  .client_token is
-00009320: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00009330: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
-00009340: 6c69 656e 7454 6f6b 656e 275d 203d 2073  lientToken'] = s
-00009350: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
-00009360: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00009370: 2e65 6169 735f 6e61 6d65 2069 7320 6e6f  .eais_name is no
-00009380: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00009390: 2020 2020 7265 7375 6c74 5b27 4561 6973      result['Eais
-000093a0: 4e61 6d65 275d 203d 2073 656c 662e 6561  Name'] = self.ea
-000093b0: 6973 5f6e 616d 650a 2020 2020 2020 2020  is_name.        
-000093c0: 6966 2073 656c 662e 6561 6973 5f74 7970  if self.eais_typ
-000093d0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-000093e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000093f0: 745b 2745 6169 7354 7970 6527 5d20 3d20  t['EaisType'] = 
-00009400: 7365 6c66 2e65 6169 735f 7479 7065 0a20  self.eais_type. 
-00009410: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-00009420: 6373 5f73 6872 696e 6b20 6973 206e 6f74  cs_shrink is not
-00009430: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00009440: 2020 2072 6573 756c 745b 2745 6373 275d     result['Ecs']
-00009450: 203d 2073 656c 662e 6563 735f 7368 7269   = self.ecs_shri
-00009460: 6e6b 0a20 2020 2020 2020 2069 6620 7365  nk.        if se
-00009470: 6c66 2e72 6567 696f 6e5f 6964 2069 7320  lf.region_id is 
-00009480: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00009490: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-000094a0: 6769 6f6e 4964 275d 203d 2073 656c 662e  gionId'] = self.
-000094b0: 7265 6769 6f6e 5f69 640a 2020 2020 2020  region_id.      
-000094c0: 2020 6966 2073 656c 662e 7265 736f 7572    if self.resour
-000094d0: 6365 5f67 726f 7570 5f69 6420 6973 206e  ce_group_id is n
-000094e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000094f0: 2020 2020 2072 6573 756c 745b 2752 6573       result['Res
-00009500: 6f75 7263 6547 726f 7570 4964 275d 203d  ourceGroupId'] =
-00009510: 2073 656c 662e 7265 736f 7572 6365 5f67   self.resource_g
-00009520: 726f 7570 5f69 640a 2020 2020 2020 2020  roup_id.        
-00009530: 6966 2073 656c 662e 7365 6375 7269 7479  if self.security
-00009540: 5f67 726f 7570 5f69 6420 6973 206e 6f74  _group_id is not
-00009550: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00009560: 2020 2072 6573 756c 745b 2753 6563 7572     result['Secur
-00009570: 6974 7947 726f 7570 4964 275d 203d 2073  ityGroupId'] = s
-00009580: 656c 662e 7365 6375 7269 7479 5f67 726f  elf.security_gro
-00009590: 7570 5f69 640a 2020 2020 2020 2020 6966  up_id.        if
-000095a0: 2073 656c 662e 765f 7377 6974 6368 5f69   self.v_switch_i
-000095b0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000095c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000095d0: 745b 2756 5377 6974 6368 4964 275d 203d  t['VSwitchId'] =
-000095e0: 2073 656c 662e 765f 7377 6974 6368 5f69   self.v_switch_i
-000095f0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
-00009600: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-00009610: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-00009620: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
-00009630: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00009640: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00009650: 7428 2743 6c69 656e 7454 6f6b 656e 2729  t('ClientToken')
-00009660: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00009670: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00009680: 6c69 656e 745f 746f 6b65 6e20 3d20 6d2e  lient_token = m.
-00009690: 6765 7428 2743 6c69 656e 7454 6f6b 656e  get('ClientToken
-000096a0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-000096b0: 6765 7428 2745 6169 734e 616d 6527 2920  get('EaisName') 
-000096c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000096d0: 2020 2020 2020 2020 2073 656c 662e 6561           self.ea
-000096e0: 6973 5f6e 616d 6520 3d20 6d2e 6765 7428  is_name = m.get(
-000096f0: 2745 6169 734e 616d 6527 290a 2020 2020  'EaisName').    
-00009700: 2020 2020 6966 206d 2e67 6574 2827 4561      if m.get('Ea
-00009710: 6973 5479 7065 2729 2069 7320 6e6f 7420  isType') is not 
-00009720: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00009730: 2020 7365 6c66 2e65 6169 735f 7479 7065    self.eais_type
-00009740: 203d 206d 2e67 6574 2827 4561 6973 5479   = m.get('EaisTy
-00009750: 7065 2729 0a20 2020 2020 2020 2069 6620  pe').        if 
-00009760: 6d2e 6765 7428 2745 6373 2729 2069 7320  m.get('Ecs') is 
-00009770: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00009780: 2020 2020 2020 7365 6c66 2e65 6373 5f73        self.ecs_s
-00009790: 6872 696e 6b20 3d20 6d2e 6765 7428 2745  hrink = m.get('E
-000097a0: 6373 2729 0a20 2020 2020 2020 2069 6620  cs').        if 
-000097b0: 6d2e 6765 7428 2752 6567 696f 6e49 6427  m.get('RegionId'
-000097c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000097d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000097e0: 7265 6769 6f6e 5f69 6420 3d20 6d2e 6765  region_id = m.ge
-000097f0: 7428 2752 6567 696f 6e49 6427 290a 2020  t('RegionId').  
-00009800: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00009810: 5265 736f 7572 6365 4772 6f75 7049 6427  ResourceGroupId'
-00009820: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00009830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009840: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-00009850: 6420 3d20 6d2e 6765 7428 2752 6573 6f75  d = m.get('Resou
-00009860: 7263 6547 726f 7570 4964 2729 0a20 2020  rceGroupId').   
-00009870: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
-00009880: 6563 7572 6974 7947 726f 7570 4964 2729  ecurityGroupId')
-00009890: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000098a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-000098b0: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
-000098c0: 203d 206d 2e67 6574 2827 5365 6375 7269   = m.get('Securi
-000098d0: 7479 4772 6f75 7049 6427 290a 2020 2020  tyGroupId').    
-000098e0: 2020 2020 6966 206d 2e67 6574 2827 5653      if m.get('VS
-000098f0: 7769 7463 6849 6427 2920 6973 206e 6f74  witchId') is not
-00009900: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00009910: 2020 2073 656c 662e 765f 7377 6974 6368     self.v_switch
-00009920: 5f69 6420 3d20 6d2e 6765 7428 2756 5377  _id = m.get('VSw
-00009930: 6974 6368 4964 2729 0a20 2020 2020 2020  itchId').       
-00009940: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-00009950: 6c61 7373 2043 7265 6174 6545 6169 4563  lass CreateEaiEc
-00009960: 7352 6573 706f 6e73 6542 6f64 7928 5465  sResponseBody(Te
-00009970: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00009980: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00009990: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
-000099a0: 6964 3d4e 6f6e 652c 2065 6c61 7374 6963  id=None, elastic
-000099b0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
-000099c0: 7461 6e63 655f 6964 3d4e 6f6e 652c 2072  tance_id=None, r
-000099d0: 6571 7565 7374 5f69 643d 4e6f 6e65 293a  equest_id=None):
-000099e0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
-000099f0: 6965 6e74 5f69 6e73 7461 6e63 655f 6964  ient_instance_id
-00009a00: 203d 2063 6c69 656e 745f 696e 7374 616e   = client_instan
-00009a10: 6365 5f69 6420 2023 2074 7970 653a 2073  ce_id  # type: s
-00009a20: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-00009a30: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
-00009a40: 7465 645f 696e 7374 616e 6365 5f69 6420  ted_instance_id 
-00009a50: 3d20 656c 6173 7469 635f 6163 6365 6c65  = elastic_accele
-00009a60: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-00009a70: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
-00009a80: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
-00009a90: 6573 745f 6964 203d 2072 6571 7565 7374  est_id = request
-00009aa0: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
-00009ab0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00009ac0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00009ad0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00009ae0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00009af0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00009b00: 6572 2843 7265 6174 6545 6169 4563 7352  er(CreateEaiEcsR
-00009b10: 6573 706f 6e73 6542 6f64 792c 2073 656c  esponseBody, sel
-00009b20: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-00009b30: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00009b40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00009b50: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00009b60: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00009b70: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00009b80: 2020 6966 2073 656c 662e 636c 6965 6e74    if self.client
-00009b90: 5f69 6e73 7461 6e63 655f 6964 2069 7320  _instance_id is 
-00009ba0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00009bb0: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
-00009bc0: 6965 6e74 496e 7374 616e 6365 4964 275d  ientInstanceId']
-00009bd0: 203d 2073 656c 662e 636c 6965 6e74 5f69   = self.client_i
-00009be0: 6e73 7461 6e63 655f 6964 0a20 2020 2020  nstance_id.     
-00009bf0: 2020 2069 6620 7365 6c66 2e65 6c61 7374     if self.elast
-00009c00: 6963 5f61 6363 656c 6572 6174 6564 5f69  ic_accelerated_i
-00009c10: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
-00009c20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00009c30: 2020 2020 7265 7375 6c74 5b27 456c 6173      result['Elas
-00009c40: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
-00009c50: 7374 616e 6365 4964 275d 203d 2073 656c  stanceId'] = sel
-00009c60: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-00009c70: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-00009c80: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00009c90: 662e 7265 7175 6573 745f 6964 2069 7320  f.request_id is 
-00009ca0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00009cb0: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-00009cc0: 7175 6573 7449 6427 5d20 3d20 7365 6c66  questId'] = self
-00009cd0: 2e72 6571 7565 7374 5f69 640a 2020 2020  .request_id.    
-00009ce0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00009cf0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00009d00: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-00009d10: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00009d20: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00009d30: 2020 2069 6620 6d2e 6765 7428 2743 6c69     if m.get('Cli
-00009d40: 656e 7449 6e73 7461 6e63 6549 6427 2920  entInstanceId') 
-00009d50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00009d60: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-00009d70: 6965 6e74 5f69 6e73 7461 6e63 655f 6964  ient_instance_id
-00009d80: 203d 206d 2e67 6574 2827 436c 6965 6e74   = m.get('Client
-00009d90: 496e 7374 616e 6365 4964 2729 0a20 2020  InstanceId').   
-00009da0: 2020 2020 2069 6620 6d2e 6765 7428 2745       if m.get('E
-00009db0: 6c61 7374 6963 4163 6365 6c65 7261 7465  lasticAccelerate
-00009dc0: 6449 6e73 7461 6e63 6549 6427 2920 6973  dInstanceId') is
-00009dd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00009de0: 2020 2020 2020 2073 656c 662e 656c 6173         self.elas
-00009df0: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
-00009e00: 696e 7374 616e 6365 5f69 6420 3d20 6d2e  instance_id = m.
-00009e10: 6765 7428 2745 6c61 7374 6963 4163 6365  get('ElasticAcce
-00009e20: 6c65 7261 7465 6449 6e73 7461 6e63 6549  leratedInstanceI
-00009e30: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00009e40: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-00009e50: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00009e60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009e70: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
-00009e80: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
-00009e90: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00009ea0: 656c 660a 0a0a 636c 6173 7320 4372 6561  elf...class Crea
-00009eb0: 7465 4561 6945 6373 5265 7370 6f6e 7365  teEaiEcsResponse
-00009ec0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00009ed0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00009ee0: 662c 2068 6561 6465 7273 3d4e 6f6e 652c  f, headers=None,
-00009ef0: 2073 7461 7475 735f 636f 6465 3d4e 6f6e   status_code=Non
-00009f00: 652c 2062 6f64 793d 4e6f 6e65 293a 0a20  e, body=None):. 
-00009f10: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00009f20: 6572 7320 3d20 6865 6164 6572 7320 2023  ers = headers  #
-00009f30: 2074 7970 653a 2064 6963 745b 7374 722c   type: dict[str,
-00009f40: 2073 7472 5d0a 2020 2020 2020 2020 7365   str].        se
-00009f50: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-00009f60: 2073 7461 7475 735f 636f 6465 2020 2320   status_code  # 
-00009f70: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
-00009f80: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-00009f90: 6479 2020 2320 7479 7065 3a20 4372 6561  dy  # type: Crea
-00009fa0: 7465 4561 6945 6373 5265 7370 6f6e 7365  teEaiEcsResponse
-00009fb0: 426f 6479 0a0a 2020 2020 6465 6620 7661  Body..    def va
-00009fc0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-00009fd0: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-00009fe0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-00009ff0: 662e 6865 6164 6572 732c 2027 6865 6164  f.headers, 'head
-0000a000: 6572 7327 290a 2020 2020 2020 2020 7365  ers').        se
-0000a010: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-0000a020: 6972 6564 2873 656c 662e 7374 6174 7573  ired(self.status
-0000a030: 5f63 6f64 652c 2027 7374 6174 7573 5f63  _code, 'status_c
-0000a040: 6f64 6527 290a 2020 2020 2020 2020 7365  ode').        se
-0000a050: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-0000a060: 6972 6564 2873 656c 662e 626f 6479 2c20  ired(self.body, 
-0000a070: 2762 6f64 7927 290a 2020 2020 2020 2020  'body').        
-0000a080: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-0000a090: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-0000a0a0: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-0000a0b0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0000a0c0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0000a0d0: 6170 203d 2073 7570 6572 2843 7265 6174  ap = super(Creat
-0000a0e0: 6545 6169 4563 7352 6573 706f 6e73 652c  eEaiEcsResponse,
-0000a0f0: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-0000a100: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0000a110: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000a120: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000a130: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0000a140: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0000a150: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-0000a160: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-0000a170: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000a180: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-0000a190: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-0000a1a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000a1b0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-0000a1c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000a1d0: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-0000a1e0: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-0000a1f0: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-0000a200: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0000a210: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-0000a220: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000a230: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-0000a240: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-0000a250: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0000a260: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0000a270: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-0000a280: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0000a290: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0000a2a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0000a2b0: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
-0000a2c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000a2d0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-0000a2e0: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-0000a2f0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0000a300: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-0000a310: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0000a320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a330: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-0000a340: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-0000a350: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0000a360: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-0000a370: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000a380: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-0000a390: 2043 7265 6174 6545 6169 4563 7352 6573   CreateEaiEcsRes
-0000a3a0: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
-0000a3b0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0000a3c0: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-0000a3d0: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-0000a3e0: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-0000a3f0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2043  n self...class C
-0000a400: 7265 6174 6545 6169 4a75 7079 7465 7252  reateEaiJupyterR
-0000a410: 6571 7565 7374 456e 7669 726f 6e6d 656e  equestEnvironmen
-0000a420: 7456 6172 2854 6561 4d6f 6465 6c29 3a0a  tVar(TeaModel):.
-0000a430: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000a440: 2873 656c 662c 206b 6579 3d4e 6f6e 652c  (self, key=None,
-0000a450: 2076 616c 7565 3d4e 6f6e 6529 3a0a 2020   value=None):.  
-0000a460: 2020 2020 2020 7365 6c66 2e6b 6579 203d        self.key =
-0000a470: 206b 6579 2020 2320 7479 7065 3a20 7374   key  # type: st
-0000a480: 720a 2020 2020 2020 2020 7365 6c66 2e76  r.        self.v
-0000a490: 616c 7565 203d 2076 616c 7565 2020 2320  alue = value  # 
-0000a4a0: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
-0000a4b0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0000a4c0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0000a4d0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0000a4e0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0000a4f0: 6d61 7020 3d20 7375 7065 7228 4372 6561  map = super(Crea
-0000a500: 7465 4561 694a 7570 7974 6572 5265 7175  teEaiJupyterRequ
-0000a510: 6573 7445 6e76 6972 6f6e 6d65 6e74 5661  estEnvironmentVa
-0000a520: 722c 2073 656c 6629 2e74 6f5f 6d61 7028  r, self).to_map(
-0000a530: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-0000a540: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-0000a550: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000a560: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-0000a570: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-0000a580: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000a590: 6b65 7920 6973 206e 6f74 204e 6f6e 653a  key is not None:
-0000a5a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000a5b0: 756c 745b 274b 6579 275d 203d 2073 656c  ult['Key'] = sel
-0000a5c0: 662e 6b65 790a 2020 2020 2020 2020 6966  f.key.        if
-0000a5d0: 2073 656c 662e 7661 6c75 6520 6973 206e   self.value is n
-0000a5e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000a5f0: 2020 2020 2072 6573 756c 745b 2756 616c       result['Val
-0000a600: 7565 275d 203d 2073 656c 662e 7661 6c75  ue'] = self.valu
-0000a610: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-0000a620: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-0000a630: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-0000a640: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
-0000a650: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-0000a660: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0000a670: 7428 274b 6579 2729 2069 7320 6e6f 7420  t('Key') is not 
-0000a680: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000a690: 2020 7365 6c66 2e6b 6579 203d 206d 2e67    self.key = m.g
-0000a6a0: 6574 2827 4b65 7927 290a 2020 2020 2020  et('Key').      
-0000a6b0: 2020 6966 206d 2e67 6574 2827 5661 6c75    if m.get('Valu
-0000a6c0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-0000a6d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000a6e0: 662e 7661 6c75 6520 3d20 6d2e 6765 7428  f.value = m.get(
-0000a6f0: 2756 616c 7565 2729 0a20 2020 2020 2020  'Value').       
-0000a700: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0000a710: 6c61 7373 2043 7265 6174 6545 6169 4a75  lass CreateEaiJu
-0000a720: 7079 7465 7252 6571 7565 7374 2854 6561  pyterRequest(Tea
-0000a730: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0000a740: 5f5f 696e 6974 5f5f 2873 656c 662c 2063  __init__(self, c
-0000a750: 6c69 656e 745f 746f 6b65 6e3d 4e6f 6e65  lient_token=None
-0000a760: 2c20 6561 6973 5f74 7970 653d 4e6f 6e65  , eais_type=None
-0000a770: 2c20 656e 7669 726f 6e6d 656e 745f 7661  , environment_va
-0000a780: 723d 4e6f 6e65 2c20 7265 6769 6f6e 5f69  r=None, region_i
-0000a790: 643d 4e6f 6e65 2c0a 2020 2020 2020 2020  d=None,.        
-0000a7a0: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
-0000a7b0: 655f 6772 6f75 705f 6964 3d4e 6f6e 652c  e_group_id=None,
-0000a7c0: 2073 6563 7572 6974 795f 6772 6f75 705f   security_group_
-0000a7d0: 6964 3d4e 6f6e 652c 2076 5f73 7769 7463  id=None, v_switc
-0000a7e0: 685f 6964 3d4e 6f6e 6529 3a0a 2020 2020  h_id=None):.    
-0000a7f0: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
-0000a800: 746f 6b65 6e20 3d20 636c 6965 6e74 5f74  token = client_t
-0000a810: 6f6b 656e 2020 2320 7479 7065 3a20 7374  oken  # type: st
-0000a820: 720a 2020 2020 2020 2020 7365 6c66 2e65  r.        self.e
-0000a830: 6169 735f 7479 7065 203d 2065 6169 735f  ais_type = eais_
-0000a840: 7479 7065 2020 2320 7479 7065 3a20 7374  type  # type: st
-0000a850: 720a 2020 2020 2020 2020 7365 6c66 2e65  r.        self.e
-0000a860: 6e76 6972 6f6e 6d65 6e74 5f76 6172 203d  nvironment_var =
-0000a870: 2065 6e76 6972 6f6e 6d65 6e74 5f76 6172   environment_var
-0000a880: 2020 2320 7479 7065 3a20 6c69 7374 5b43    # type: list[C
-0000a890: 7265 6174 6545 6169 4a75 7079 7465 7252  reateEaiJupyterR
-0000a8a0: 6571 7565 7374 456e 7669 726f 6e6d 656e  equestEnvironmen
-0000a8b0: 7456 6172 5d0a 2020 2020 2020 2020 7365  tVar].        se
-0000a8c0: 6c66 2e72 6567 696f 6e5f 6964 203d 2072  lf.region_id = r
-0000a8d0: 6567 696f 6e5f 6964 2020 2320 7479 7065  egion_id  # type
-0000a8e0: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-0000a8f0: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
-0000a900: 705f 6964 203d 2072 6573 6f75 7263 655f  p_id = resource_
-0000a910: 6772 6f75 705f 6964 2020 2320 7479 7065  group_id  # type
-0000a920: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-0000a930: 6c66 2e73 6563 7572 6974 795f 6772 6f75  lf.security_grou
-0000a940: 705f 6964 203d 2073 6563 7572 6974 795f  p_id = security_
-0000a950: 6772 6f75 705f 6964 2020 2320 7479 7065  group_id  # type
-0000a960: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-0000a970: 6c66 2e76 5f73 7769 7463 685f 6964 203d  lf.v_switch_id =
-0000a980: 2076 5f73 7769 7463 685f 6964 2020 2320   v_switch_id  # 
-0000a990: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
-0000a9a0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0000a9b0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-0000a9c0: 6c66 2e65 6e76 6972 6f6e 6d65 6e74 5f76  lf.environment_v
-0000a9d0: 6172 3a0a 2020 2020 2020 2020 2020 2020  ar:.            
-0000a9e0: 666f 7220 6b20 696e 2073 656c 662e 656e  for k in self.en
-0000a9f0: 7669 726f 6e6d 656e 745f 7661 723a 0a20  vironment_var:. 
-0000aa00: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000aa10: 6620 6b3a 0a20 2020 2020 2020 2020 2020  f k:.           
-0000aa20: 2020 2020 2020 2020 206b 2e76 616c 6964           k.valid
-0000aa30: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-0000aa40: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-0000aa50: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-0000aa60: 7228 4372 6561 7465 4561 694a 7570 7974  r(CreateEaiJupyt
-0000aa70: 6572 5265 7175 6573 742c 2073 656c 6629  erRequest, self)
-0000aa80: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0000aa90: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0000aaa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000aab0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0000aac0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0000aad0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0000aae0: 6966 2073 656c 662e 636c 6965 6e74 5f74  if self.client_t
-0000aaf0: 6f6b 656e 2069 7320 6e6f 7420 4e6f 6e65  oken is not None
-0000ab00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000ab10: 7375 6c74 5b27 436c 6965 6e74 546f 6b65  sult['ClientToke
-0000ab20: 6e27 5d20 3d20 7365 6c66 2e63 6c69 656e  n'] = self.clien
-0000ab30: 745f 746f 6b65 6e0a 2020 2020 2020 2020  t_token.        
-0000ab40: 6966 2073 656c 662e 6561 6973 5f74 7970  if self.eais_typ
-0000ab50: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-0000ab60: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000ab70: 745b 2745 6169 7354 7970 6527 5d20 3d20  t['EaisType'] = 
-0000ab80: 7365 6c66 2e65 6169 735f 7479 7065 0a20  self.eais_type. 
-0000ab90: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
-0000aba0: 6e76 6972 6f6e 6d65 6e74 5661 7227 5d20  nvironmentVar'] 
-0000abb0: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
-0000abc0: 7365 6c66 2e65 6e76 6972 6f6e 6d65 6e74  self.environment
-0000abd0: 5f76 6172 2069 7320 6e6f 7420 4e6f 6e65  _var is not None
-0000abe0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0000abf0: 7220 6b20 696e 2073 656c 662e 656e 7669  r k in self.envi
-0000ac00: 726f 6e6d 656e 745f 7661 723a 0a20 2020  ronment_var:.   
-0000ac10: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0000ac20: 756c 745b 2745 6e76 6972 6f6e 6d65 6e74  ult['Environment
-0000ac30: 5661 7227 5d2e 6170 7065 6e64 286b 2e74  Var'].append(k.t
-0000ac40: 6f5f 6d61 7028 2920 6966 206b 2065 6c73  o_map() if k els
-0000ac50: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
-0000ac60: 6966 2073 656c 662e 7265 6769 6f6e 5f69  if self.region_i
-0000ac70: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-0000ac80: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000ac90: 745b 2752 6567 696f 6e49 6427 5d20 3d20  t['RegionId'] = 
-0000aca0: 7365 6c66 2e72 6567 696f 6e5f 6964 0a20  self.region_id. 
-0000acb0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000acc0: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-0000acd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000ace0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000acf0: 5b27 5265 736f 7572 6365 4772 6f75 7049  ['ResourceGroupI
-0000ad00: 6427 5d20 3d20 7365 6c66 2e72 6573 6f75  d'] = self.resou
-0000ad10: 7263 655f 6772 6f75 705f 6964 0a20 2020  rce_group_id.   
-0000ad20: 2020 2020 2069 6620 7365 6c66 2e73 6563       if self.sec
-0000ad30: 7572 6974 795f 6772 6f75 705f 6964 2069  urity_group_id i
-0000ad40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000ad50: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0000ad60: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
-0000ad70: 5d20 3d20 7365 6c66 2e73 6563 7572 6974  ] = self.securit
-0000ad80: 795f 6772 6f75 705f 6964 0a20 2020 2020  y_group_id.     
-0000ad90: 2020 2069 6620 7365 6c66 2e76 5f73 7769     if self.v_swi
-0000ada0: 7463 685f 6964 2069 7320 6e6f 7420 4e6f  tch_id is not No
-0000adb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000adc0: 7265 7375 6c74 5b27 5653 7769 7463 6849  result['VSwitchI
-0000add0: 6427 5d20 3d20 7365 6c66 2e76 5f73 7769  d'] = self.v_swi
-0000ade0: 7463 685f 6964 0a20 2020 2020 2020 2072  tch_id.        r
-0000adf0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-0000ae00: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-0000ae10: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
-0000ae20: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0000ae30: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0000ae40: 206d 2e67 6574 2827 436c 6965 6e74 546f   m.get('ClientTo
-0000ae50: 6b65 6e27 2920 6973 206e 6f74 204e 6f6e  ken') is not Non
-0000ae60: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000ae70: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
-0000ae80: 203d 206d 2e67 6574 2827 436c 6965 6e74   = m.get('Client
-0000ae90: 546f 6b65 6e27 290a 2020 2020 2020 2020  Token').        
-0000aea0: 6966 206d 2e67 6574 2827 4561 6973 5479  if m.get('EaisTy
-0000aeb0: 7065 2729 2069 7320 6e6f 7420 4e6f 6e65  pe') is not None
-0000aec0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000aed0: 6c66 2e65 6169 735f 7479 7065 203d 206d  lf.eais_type = m
-0000aee0: 2e67 6574 2827 4561 6973 5479 7065 2729  .get('EaisType')
-0000aef0: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-0000af00: 7669 726f 6e6d 656e 745f 7661 7220 3d20  vironment_var = 
-0000af10: 5b5d 0a20 2020 2020 2020 2069 6620 6d2e  [].        if m.
-0000af20: 6765 7428 2745 6e76 6972 6f6e 6d65 6e74  get('Environment
-0000af30: 5661 7227 2920 6973 206e 6f74 204e 6f6e  Var') is not Non
-0000af40: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-0000af50: 6f72 206b 2069 6e20 6d2e 6765 7428 2745  or k in m.get('E
-0000af60: 6e76 6972 6f6e 6d65 6e74 5661 7227 293a  nvironmentVar'):
-0000af70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000af80: 2074 656d 705f 6d6f 6465 6c20 3d20 4372   temp_model = Cr
-0000af90: 6561 7465 4561 694a 7570 7974 6572 5265  eateEaiJupyterRe
-0000afa0: 7175 6573 7445 6e76 6972 6f6e 6d65 6e74  questEnvironment
-0000afb0: 5661 7228 290a 2020 2020 2020 2020 2020  Var().          
-0000afc0: 2020 2020 2020 7365 6c66 2e65 6e76 6972        self.envir
-0000afd0: 6f6e 6d65 6e74 5f76 6172 2e61 7070 656e  onment_var.appen
-0000afe0: 6428 7465 6d70 5f6d 6f64 656c 2e66 726f  d(temp_model.fro
-0000aff0: 6d5f 6d61 7028 6b29 290a 2020 2020 2020  m_map(k)).      
-0000b000: 2020 6966 206d 2e67 6574 2827 5265 6769    if m.get('Regi
-0000b010: 6f6e 4964 2729 2069 7320 6e6f 7420 4e6f  onId') is not No
-0000b020: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000b030: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
-0000b040: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
-0000b050: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0000b060: 6765 7428 2752 6573 6f75 7263 6547 726f  get('ResourceGro
-0000b070: 7570 4964 2729 2069 7320 6e6f 7420 4e6f  upId') is not No
-0000b080: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000b090: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
-0000b0a0: 6f75 705f 6964 203d 206d 2e67 6574 2827  oup_id = m.get('
-0000b0b0: 5265 736f 7572 6365 4772 6f75 7049 6427  ResourceGroupId'
-0000b0c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0000b0d0: 6574 2827 5365 6375 7269 7479 4772 6f75  et('SecurityGrou
-0000b0e0: 7049 6427 2920 6973 206e 6f74 204e 6f6e  pId') is not Non
-0000b0f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000b100: 656c 662e 7365 6375 7269 7479 5f67 726f  elf.security_gro
-0000b110: 7570 5f69 6420 3d20 6d2e 6765 7428 2753  up_id = m.get('S
-0000b120: 6563 7572 6974 7947 726f 7570 4964 2729  ecurityGroupId')
-0000b130: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0000b140: 7428 2756 5377 6974 6368 4964 2729 2069  t('VSwitchId') i
-0000b150: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000b160: 2020 2020 2020 2020 7365 6c66 2e76 5f73          self.v_s
-0000b170: 7769 7463 685f 6964 203d 206d 2e67 6574  witch_id = m.get
-0000b180: 2827 5653 7769 7463 6849 6427 290a 2020  ('VSwitchId').  
-0000b190: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000b1a0: 660a 0a0a 636c 6173 7320 4372 6561 7465  f...class Create
-0000b1b0: 4561 694a 7570 7974 6572 5368 7269 6e6b  EaiJupyterShrink
-0000b1c0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
-0000b1d0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-0000b1e0: 745f 5f28 7365 6c66 2c20 636c 6965 6e74  t__(self, client
-0000b1f0: 5f74 6f6b 656e 3d4e 6f6e 652c 2065 6169  _token=None, eai
-0000b200: 735f 7479 7065 3d4e 6f6e 652c 2065 6e76  s_type=None, env
-0000b210: 6972 6f6e 6d65 6e74 5f76 6172 5f73 6872  ironment_var_shr
-0000b220: 696e 6b3d 4e6f 6e65 2c20 7265 6769 6f6e  ink=None, region
-0000b230: 5f69 643d 4e6f 6e65 2c0a 2020 2020 2020  _id=None,.      
-0000b240: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
-0000b250: 7263 655f 6772 6f75 705f 6964 3d4e 6f6e  rce_group_id=Non
-0000b260: 652c 2073 6563 7572 6974 795f 6772 6f75  e, security_grou
-0000b270: 705f 6964 3d4e 6f6e 652c 2076 5f73 7769  p_id=None, v_swi
-0000b280: 7463 685f 6964 3d4e 6f6e 6529 3a0a 2020  tch_id=None):.  
-0000b290: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-0000b2a0: 745f 746f 6b65 6e20 3d20 636c 6965 6e74  t_token = client
-0000b2b0: 5f74 6f6b 656e 2020 2320 7479 7065 3a20  _token  # type: 
-0000b2c0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-0000b2d0: 2e65 6169 735f 7479 7065 203d 2065 6169  .eais_type = eai
-0000b2e0: 735f 7479 7065 2020 2320 7479 7065 3a20  s_type  # type: 
-0000b2f0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-0000b300: 2e65 6e76 6972 6f6e 6d65 6e74 5f76 6172  .environment_var
-0000b310: 5f73 6872 696e 6b20 3d20 656e 7669 726f  _shrink = enviro
-0000b320: 6e6d 656e 745f 7661 725f 7368 7269 6e6b  nment_var_shrink
-0000b330: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-0000b340: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-0000b350: 6e5f 6964 203d 2072 6567 696f 6e5f 6964  n_id = region_id
-0000b360: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-0000b370: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
-0000b380: 7263 655f 6772 6f75 705f 6964 203d 2072  rce_group_id = r
-0000b390: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-0000b3a0: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-0000b3b0: 2020 2020 2020 7365 6c66 2e73 6563 7572        self.secur
-0000b3c0: 6974 795f 6772 6f75 705f 6964 203d 2073  ity_group_id = s
-0000b3d0: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
-0000b3e0: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-0000b3f0: 2020 2020 2020 7365 6c66 2e76 5f73 7769        self.v_swi
-0000b400: 7463 685f 6964 203d 2076 5f73 7769 7463  tch_id = v_switc
-0000b410: 685f 6964 2020 2320 7479 7065 3a20 7374  h_id  # type: st
-0000b420: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
-0000b430: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-0000b440: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-0000b450: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0000b460: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0000b470: 7065 7228 4372 6561 7465 4561 694a 7570  per(CreateEaiJup
-0000b480: 7974 6572 5368 7269 6e6b 5265 7175 6573  yterShrinkReques
-0000b490: 742c 2073 656c 6629 2e74 6f5f 6d61 7028  t, self).to_map(
-0000b4a0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-0000b4b0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-0000b4c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b4d0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-0000b4e0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-0000b4f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b500: 636c 6965 6e74 5f74 6f6b 656e 2069 7320  client_token is 
-0000b510: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000b520: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
-0000b530: 6965 6e74 546f 6b65 6e27 5d20 3d20 7365  ientToken'] = se
-0000b540: 6c66 2e63 6c69 656e 745f 746f 6b65 6e0a  lf.client_token.
-0000b550: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b560: 6561 6973 5f74 7970 6520 6973 206e 6f74  eais_type is not
-0000b570: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000b580: 2020 2072 6573 756c 745b 2745 6169 7354     result['EaisT
-0000b590: 7970 6527 5d20 3d20 7365 6c66 2e65 6169  ype'] = self.eai
-0000b5a0: 735f 7479 7065 0a20 2020 2020 2020 2069  s_type.        i
-0000b5b0: 6620 7365 6c66 2e65 6e76 6972 6f6e 6d65  f self.environme
-0000b5c0: 6e74 5f76 6172 5f73 6872 696e 6b20 6973  nt_var_shrink is
-0000b5d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000b5e0: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
-0000b5f0: 6e76 6972 6f6e 6d65 6e74 5661 7227 5d20  nvironmentVar'] 
-0000b600: 3d20 7365 6c66 2e65 6e76 6972 6f6e 6d65  = self.environme
-0000b610: 6e74 5f76 6172 5f73 6872 696e 6b0a 2020  nt_var_shrink.  
-0000b620: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-0000b630: 6769 6f6e 5f69 6420 6973 206e 6f74 204e  gion_id is not N
-0000b640: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000b650: 2072 6573 756c 745b 2752 6567 696f 6e49   result['RegionI
-0000b660: 6427 5d20 3d20 7365 6c66 2e72 6567 696f  d'] = self.regio
-0000b670: 6e5f 6964 0a20 2020 2020 2020 2069 6620  n_id.        if 
-0000b680: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
-0000b690: 6f75 705f 6964 2069 7320 6e6f 7420 4e6f  oup_id is not No
-0000b6a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000b6b0: 7265 7375 6c74 5b27 5265 736f 7572 6365  result['Resource
-0000b6c0: 4772 6f75 7049 6427 5d20 3d20 7365 6c66  GroupId'] = self
-0000b6d0: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
-0000b6e0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-0000b6f0: 6c66 2e73 6563 7572 6974 795f 6772 6f75  lf.security_grou
-0000b700: 705f 6964 2069 7320 6e6f 7420 4e6f 6e65  p_id is not None
-0000b710: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000b720: 7375 6c74 5b27 5365 6375 7269 7479 4772  sult['SecurityGr
-0000b730: 6f75 7049 6427 5d20 3d20 7365 6c66 2e73  oupId'] = self.s
-0000b740: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
-0000b750: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000b760: 2e76 5f73 7769 7463 685f 6964 2069 7320  .v_switch_id is 
-0000b770: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000b780: 2020 2020 2020 7265 7375 6c74 5b27 5653        result['VS
-0000b790: 7769 7463 6849 6427 5d20 3d20 7365 6c66  witchId'] = self
-0000b7a0: 2e76 5f73 7769 7463 685f 6964 0a20 2020  .v_switch_id.   
-0000b7b0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0000b7c0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0000b7d0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
-0000b7e0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0000b7f0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0000b800: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
-0000b810: 6965 6e74 546f 6b65 6e27 2920 6973 206e  ientToken') is n
-0000b820: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000b830: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-0000b840: 5f74 6f6b 656e 203d 206d 2e67 6574 2827  _token = m.get('
-0000b850: 436c 6965 6e74 546f 6b65 6e27 290a 2020  ClientToken').  
-0000b860: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0000b870: 4561 6973 5479 7065 2729 2069 7320 6e6f  EaisType') is no
-0000b880: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000b890: 2020 2020 7365 6c66 2e65 6169 735f 7479      self.eais_ty
-0000b8a0: 7065 203d 206d 2e67 6574 2827 4561 6973  pe = m.get('Eais
-0000b8b0: 5479 7065 2729 0a20 2020 2020 2020 2069  Type').        i
-0000b8c0: 6620 6d2e 6765 7428 2745 6e76 6972 6f6e  f m.get('Environ
-0000b8d0: 6d65 6e74 5661 7227 2920 6973 206e 6f74  mentVar') is not
-0000b8e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000b8f0: 2020 2073 656c 662e 656e 7669 726f 6e6d     self.environm
-0000b900: 656e 745f 7661 725f 7368 7269 6e6b 203d  ent_var_shrink =
-0000b910: 206d 2e67 6574 2827 456e 7669 726f 6e6d   m.get('Environm
-0000b920: 656e 7456 6172 2729 0a20 2020 2020 2020  entVar').       
-0000b930: 2069 6620 6d2e 6765 7428 2752 6567 696f   if m.get('Regio
-0000b940: 6e49 6427 2920 6973 206e 6f74 204e 6f6e  nId') is not Non
-0000b950: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000b960: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
-0000b970: 6d2e 6765 7428 2752 6567 696f 6e49 6427  m.get('RegionId'
-0000b980: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0000b990: 6574 2827 5265 736f 7572 6365 4772 6f75  et('ResourceGrou
-0000b9a0: 7049 6427 2920 6973 206e 6f74 204e 6f6e  pId') is not Non
-0000b9b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000b9c0: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
-0000b9d0: 7570 5f69 6420 3d20 6d2e 6765 7428 2752  up_id = m.get('R
-0000b9e0: 6573 6f75 7263 6547 726f 7570 4964 2729  esourceGroupId')
-0000b9f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0000ba00: 7428 2753 6563 7572 6974 7947 726f 7570  t('SecurityGroup
-0000ba10: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-0000ba20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000ba30: 6c66 2e73 6563 7572 6974 795f 6772 6f75  lf.security_grou
-0000ba40: 705f 6964 203d 206d 2e67 6574 2827 5365  p_id = m.get('Se
-0000ba50: 6375 7269 7479 4772 6f75 7049 6427 290a  curityGroupId').
-0000ba60: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0000ba70: 2827 5653 7769 7463 6849 6427 2920 6973  ('VSwitchId') is
-0000ba80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000ba90: 2020 2020 2020 2073 656c 662e 765f 7377         self.v_sw
-0000baa0: 6974 6368 5f69 6420 3d20 6d2e 6765 7428  itch_id = m.get(
-0000bab0: 2756 5377 6974 6368 4964 2729 0a20 2020  'VSwitchId').   
-0000bac0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000bad0: 0a0a 0a63 6c61 7373 2043 7265 6174 6545  ...class CreateE
-0000bae0: 6169 4a75 7079 7465 7252 6573 706f 6e73  aiJupyterRespons
-0000baf0: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
-0000bb00: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000bb10: 5f28 7365 6c66 2c20 656c 6173 7469 635f  _(self, elastic_
-0000bb20: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
-0000bb30: 616e 6365 5f69 643d 4e6f 6e65 2c20 7265  ance_id=None, re
-0000bb40: 7175 6573 745f 6964 3d4e 6f6e 6529 3a0a  quest_id=None):.
-0000bb50: 2020 2020 2020 2020 7365 6c66 2e65 6c61          self.ela
-0000bb60: 7374 6963 5f61 6363 656c 6572 6174 6564  stic_accelerated
-0000bb70: 5f69 6e73 7461 6e63 655f 6964 203d 2065  _instance_id = e
-0000bb80: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
-0000bb90: 6564 5f69 6e73 7461 6e63 655f 6964 2020  ed_instance_id  
-0000bba0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-0000bbb0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-0000bbc0: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
-0000bbd0: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
-0000bbe0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0000bbf0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0000bc00: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-0000bc10: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0000bc20: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0000bc30: 4372 6561 7465 4561 694a 7570 7974 6572  CreateEaiJupyter
-0000bc40: 5265 7370 6f6e 7365 426f 6479 2c20 7365  ResponseBody, se
-0000bc50: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
-0000bc60: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-0000bc70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000bc80: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-0000bc90: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-0000bca0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0000bcb0: 2020 2069 6620 7365 6c66 2e65 6c61 7374     if self.elast
-0000bcc0: 6963 5f61 6363 656c 6572 6174 6564 5f69  ic_accelerated_i
-0000bcd0: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
-0000bce0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000bcf0: 2020 2020 7265 7375 6c74 5b27 456c 6173      result['Elas
-0000bd00: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
-0000bd10: 7374 616e 6365 4964 275d 203d 2073 656c  stanceId'] = sel
-0000bd20: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-0000bd30: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-0000bd40: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-0000bd50: 662e 7265 7175 6573 745f 6964 2069 7320  f.request_id is 
-0000bd60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000bd70: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-0000bd80: 7175 6573 7449 6427 5d20 3d20 7365 6c66  questId'] = self
-0000bd90: 2e72 6571 7565 7374 5f69 640a 2020 2020  .request_id.    
-0000bda0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0000bdb0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-0000bdc0: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-0000bdd0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0000bde0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0000bdf0: 2020 2069 6620 6d2e 6765 7428 2745 6c61     if m.get('Ela
-0000be00: 7374 6963 4163 6365 6c65 7261 7465 6449  sticAcceleratedI
-0000be10: 6e73 7461 6e63 6549 6427 2920 6973 206e  nstanceId') is n
-0000be20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000be30: 2020 2020 2073 656c 662e 656c 6173 7469       self.elasti
-0000be40: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
-0000be50: 7374 616e 6365 5f69 6420 3d20 6d2e 6765  stance_id = m.ge
-0000be60: 7428 2745 6c61 7374 6963 4163 6365 6c65  t('ElasticAccele
-0000be70: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
-0000be80: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0000be90: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
-0000bea0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000beb0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0000bec0: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
-0000bed0: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
-0000bee0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000bef0: 660a 0a0a 636c 6173 7320 4372 6561 7465  f...class Create
-0000bf00: 4561 694a 7570 7974 6572 5265 7370 6f6e  EaiJupyterRespon
-0000bf10: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-0000bf20: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000bf30: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
-0000bf40: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
-0000bf50: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
-0000bf60: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
-0000bf70: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
-0000bf80: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
-0000bf90: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
-0000bfa0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0000bfb0: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
-0000bfc0: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
-0000bfd0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-0000bfe0: 626f 6479 2020 2320 7479 7065 3a20 4372  body  # type: Cr
-0000bff0: 6561 7465 4561 694a 7570 7974 6572 5265  eateEaiJupyterRe
-0000c000: 7370 6f6e 7365 426f 6479 0a0a 2020 2020  sponseBody..    
-0000c010: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0000c020: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-0000c030: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0000c040: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
-0000c050: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
-0000c060: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0000c070: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0000c080: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
-0000c090: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
-0000c0a0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0000c0b0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0000c0c0: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
-0000c0d0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-0000c0e0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-0000c0f0: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-0000c100: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-0000c110: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0000c120: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0000c130: 2843 7265 6174 6545 6169 4a75 7079 7465  (CreateEaiJupyte
-0000c140: 7252 6573 706f 6e73 652c 2073 656c 6629  rResponse, self)
-0000c150: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0000c160: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0000c170: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000c180: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0000c190: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0000c1a0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0000c1b0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-0000c1c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000c1d0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000c1e0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-0000c1f0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-0000c200: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-0000c210: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-0000c220: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000c230: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-0000c240: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-0000c250: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-0000c260: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-0000c270: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000c280: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-0000c290: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-0000c2a0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0000c2b0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0000c2c0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0000c2d0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-0000c2e0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0000c2f0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0000c300: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
-0000c310: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-0000c320: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c330: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
-0000c340: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
-0000c350: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
-0000c360: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
-0000c370: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000c380: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-0000c390: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
-0000c3a0: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
-0000c3b0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-0000c3c0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-0000c3d0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-0000c3e0: 6d70 5f6d 6f64 656c 203d 2043 7265 6174  mp_model = Creat
-0000c3f0: 6545 6169 4a75 7079 7465 7252 6573 706f  eEaiJupyterRespo
-0000c400: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
-0000c410: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-0000c420: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
-0000c430: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
-0000c440: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000c450: 7365 6c66 0a0a 0a63 6c61 7373 2044 656c  self...class Del
-0000c460: 6574 6545 6169 5265 7175 6573 7428 5465  eteEaiRequest(Te
-0000c470: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-0000c480: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-0000c490: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
-0000c4a0: 7465 645f 696e 7374 616e 6365 5f69 643d  ted_instance_id=
-0000c4b0: 4e6f 6e65 2c20 666f 7263 653d 4e6f 6e65  None, force=None
-0000c4c0: 2c20 7265 6769 6f6e 5f69 643d 4e6f 6e65  , region_id=None
-0000c4d0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0000c4e0: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
-0000c4f0: 7465 645f 696e 7374 616e 6365 5f69 6420  ted_instance_id 
-0000c500: 3d20 656c 6173 7469 635f 6163 6365 6c65  = elastic_accele
-0000c510: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-0000c520: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
-0000c530: 2020 2020 2020 2073 656c 662e 666f 7263         self.forc
-0000c540: 6520 3d20 666f 7263 6520 2023 2074 7970  e = force  # typ
-0000c550: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
-0000c560: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
-0000c570: 2072 6567 696f 6e5f 6964 2020 2320 7479   region_id  # ty
-0000c580: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
-0000c590: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0000c5a0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0000c5b0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0000c5c0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0000c5d0: 7020 3d20 7375 7065 7228 4465 6c65 7465  p = super(Delete
-0000c5e0: 4561 6952 6571 7565 7374 2c20 7365 6c66  EaiRequest, self
-0000c5f0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0000c600: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0000c610: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000c620: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0000c630: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0000c640: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0000c650: 2069 6620 7365 6c66 2e65 6c61 7374 6963   if self.elastic
-0000c660: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
-0000c670: 7461 6e63 655f 6964 2069 7320 6e6f 7420  tance_id is not 
-0000c680: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000c690: 2020 7265 7375 6c74 5b27 456c 6173 7469    result['Elasti
-0000c6a0: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
-0000c6b0: 616e 6365 4964 275d 203d 2073 656c 662e  anceId'] = self.
-0000c6c0: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
-0000c6d0: 7465 645f 696e 7374 616e 6365 5f69 640a  ted_instance_id.
-0000c6e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000c6f0: 666f 7263 6520 6973 206e 6f74 204e 6f6e  force is not Non
-0000c700: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000c710: 6573 756c 745b 2746 6f72 6365 275d 203d  esult['Force'] =
-0000c720: 2073 656c 662e 666f 7263 650a 2020 2020   self.force.    
-0000c730: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
-0000c740: 6f6e 5f69 6420 6973 206e 6f74 204e 6f6e  on_id is not Non
-0000c750: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000c760: 6573 756c 745b 2752 6567 696f 6e49 6427  esult['RegionId'
-0000c770: 5d20 3d20 7365 6c66 2e72 6567 696f 6e5f  ] = self.region_
-0000c780: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-0000c790: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0000c7a0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0000c7b0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-0000c7c0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-0000c7d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0000c7e0: 6574 2827 456c 6173 7469 6341 6363 656c  et('ElasticAccel
-0000c7f0: 6572 6174 6564 496e 7374 616e 6365 4964  eratedInstanceId
-0000c800: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0000c810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c820: 2e65 6c61 7374 6963 5f61 6363 656c 6572  .elastic_acceler
-0000c830: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
-0000c840: 203d 206d 2e67 6574 2827 456c 6173 7469   = m.get('Elasti
-0000c850: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
-0000c860: 616e 6365 4964 2729 0a20 2020 2020 2020  anceId').       
-0000c870: 2069 6620 6d2e 6765 7428 2746 6f72 6365   if m.get('Force
-0000c880: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0000c890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c8a0: 2e66 6f72 6365 203d 206d 2e67 6574 2827  .force = m.get('
-0000c8b0: 466f 7263 6527 290a 2020 2020 2020 2020  Force').        
-0000c8c0: 6966 206d 2e67 6574 2827 5265 6769 6f6e  if m.get('Region
-0000c8d0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-0000c8e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000c8f0: 6c66 2e72 6567 696f 6e5f 6964 203d 206d  lf.region_id = m
-0000c900: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
-0000c910: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000c920: 7365 6c66 0a0a 0a63 6c61 7373 2044 656c  self...class Del
-0000c930: 6574 6545 6169 5265 7370 6f6e 7365 426f  eteEaiResponseBo
-0000c940: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
-0000c950: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000c960: 656c 662c 2072 6571 7565 7374 5f69 643d  elf, request_id=
-0000c970: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-0000c980: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-0000c990: 2072 6571 7565 7374 5f69 6420 2023 2074   request_id  # t
-0000c9a0: 7970 653a 2073 7472 0a0a 2020 2020 6465  ype: str..    de
-0000c9b0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0000c9c0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0000c9d0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0000c9e0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0000c9f0: 6170 203d 2073 7570 6572 2844 656c 6574  ap = super(Delet
-0000ca00: 6545 6169 5265 7370 6f6e 7365 426f 6479  eEaiResponseBody
-0000ca10: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
-0000ca20: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0000ca30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000ca40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000ca50: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0000ca60: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0000ca70: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000ca80: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
-0000ca90: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000caa0: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
-0000cab0: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
-0000cac0: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
-0000cad0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0000cae0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0000caf0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-0000cb00: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0000cb10: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0000cb20: 6966 206d 2e67 6574 2827 5265 7175 6573  if m.get('Reques
-0000cb30: 7449 6427 2920 6973 206e 6f74 204e 6f6e  tId') is not Non
-0000cb40: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000cb50: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-0000cb60: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
-0000cb70: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
-0000cb80: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-0000cb90: 4465 6c65 7465 4561 6952 6573 706f 6e73  DeleteEaiRespons
-0000cba0: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
-0000cbb0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-0000cbc0: 6c66 2c20 6865 6164 6572 733d 4e6f 6e65  lf, headers=None
-0000cbd0: 2c20 7374 6174 7573 5f63 6f64 653d 4e6f  , status_code=No
-0000cbe0: 6e65 2c20 626f 6479 3d4e 6f6e 6529 3a0a  ne, body=None):.
-0000cbf0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0000cc00: 6465 7273 203d 2068 6561 6465 7273 2020  ders = headers  
-0000cc10: 2320 7479 7065 3a20 6469 6374 5b73 7472  # type: dict[str
-0000cc20: 2c20 7374 725d 0a20 2020 2020 2020 2073  , str].        s
-0000cc30: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0000cc40: 3d20 7374 6174 7573 5f63 6f64 6520 2023  = status_code  #
-0000cc50: 2074 7970 653a 2069 6e74 0a20 2020 2020   type: int.     
-0000cc60: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-0000cc70: 6f64 7920 2023 2074 7970 653a 2044 656c  ody  # type: Del
-0000cc80: 6574 6545 6169 5265 7370 6f6e 7365 426f  eteEaiResponseBo
-0000cc90: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
-0000cca0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-0000ccb0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0000ccc0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0000ccd0: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
-0000cce0: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
-0000ccf0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0000cd00: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
-0000cd10: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
-0000cd20: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
-0000cd30: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0000cd40: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
-0000cd50: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
-0000cd60: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-0000cd70: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0000cd80: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-0000cd90: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0000cda0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0000cdb0: 203d 2073 7570 6572 2844 656c 6574 6545   = super(DeleteE
-0000cdc0: 6169 5265 7370 6f6e 7365 2c20 7365 6c66  aiResponse, self
-0000cdd0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0000cde0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0000cdf0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000ce00: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0000ce10: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0000ce20: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0000ce30: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-0000ce40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000ce50: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000ce60: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-0000ce70: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-0000ce80: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-0000ce90: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-0000cea0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000ceb0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-0000cec0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-0000ced0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-0000cee0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-0000cef0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000cf00: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-0000cf10: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-0000cf20: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0000cf30: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0000cf40: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0000cf50: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-0000cf60: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-0000cf70: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-0000cf80: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-0000cf90: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-0000cfa0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000cfb0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-0000cfc0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-0000cfd0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0000cfe0: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-0000cff0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000d000: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0000d010: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-0000d020: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-0000d030: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-0000d040: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-0000d050: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-0000d060: 656d 705f 6d6f 6465 6c20 3d20 4465 6c65  emp_model = Dele
-0000d070: 7465 4561 6952 6573 706f 6e73 6542 6f64  teEaiResponseBod
-0000d080: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-0000d090: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-0000d0a0: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-0000d0b0: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-0000d0c0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0000d0d0: 0a63 6c61 7373 2044 656c 6574 6545 6169  .class DeleteEai
-0000d0e0: 416c 6c52 6571 7565 7374 2854 6561 4d6f  AllRequest(TeaMo
-0000d0f0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0000d100: 696e 6974 5f5f 2873 656c 662c 2063 6c69  init__(self, cli
-0000d110: 656e 745f 696e 7374 616e 6365 5f69 643d  ent_instance_id=
-0000d120: 4e6f 6e65 2c20 656c 6173 7469 635f 6163  None, elastic_ac
-0000d130: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
-0000d140: 6365 5f69 643d 4e6f 6e65 2c20 7265 6769  ce_id=None, regi
-0000d150: 6f6e 5f69 643d 4e6f 6e65 293a 0a20 2020  on_id=None):.   
-0000d160: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-0000d170: 5f69 6e73 7461 6e63 655f 6964 203d 2063  _instance_id = c
-0000d180: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
-0000d190: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
-0000d1a0: 2020 2020 2020 2073 656c 662e 656c 6173         self.elas
-0000d1b0: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
-0000d1c0: 696e 7374 616e 6365 5f69 6420 3d20 656c  instance_id = el
-0000d1d0: 6173 7469 635f 6163 6365 6c65 7261 7465  astic_accelerate
-0000d1e0: 645f 696e 7374 616e 6365 5f69 6420 2023  d_instance_id  #
-0000d1f0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0000d200: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
-0000d210: 6420 3d20 7265 6769 6f6e 5f69 6420 2023  d = region_id  #
-0000d220: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
-0000d230: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0000d240: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-0000d250: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-0000d260: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000d270: 5f6d 6170 203d 2073 7570 6572 2844 656c  _map = super(Del
-0000d280: 6574 6545 6169 416c 6c52 6571 7565 7374  eteEaiAllRequest
-0000d290: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
-0000d2a0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0000d2b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000d2c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d2d0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0000d2e0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0000d2f0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000d300: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
-0000d310: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-0000d320: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000d330: 745b 2743 6c69 656e 7449 6e73 7461 6e63  t['ClientInstanc
-0000d340: 6549 6427 5d20 3d20 7365 6c66 2e63 6c69  eId'] = self.cli
-0000d350: 656e 745f 696e 7374 616e 6365 5f69 640a  ent_instance_id.
-0000d360: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d370: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
-0000d380: 7465 645f 696e 7374 616e 6365 5f69 6420  ted_instance_id 
-0000d390: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000d3a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000d3b0: 2745 6c61 7374 6963 4163 6365 6c65 7261  'ElasticAccelera
-0000d3c0: 7465 6449 6e73 7461 6e63 6549 6427 5d20  tedInstanceId'] 
-0000d3d0: 3d20 7365 6c66 2e65 6c61 7374 6963 5f61  = self.elastic_a
-0000d3e0: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
-0000d3f0: 6e63 655f 6964 0a20 2020 2020 2020 2069  nce_id.        i
-0000d400: 6620 7365 6c66 2e72 6567 696f 6e5f 6964  f self.region_id
-0000d410: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000d420: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000d430: 5b27 5265 6769 6f6e 4964 275d 203d 2073  ['RegionId'] = s
-0000d440: 656c 662e 7265 6769 6f6e 5f69 640a 2020  elf.region_id.  
-0000d450: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0000d460: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0000d470: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
-0000d480: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0000d490: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0000d4a0: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
-0000d4b0: 6c69 656e 7449 6e73 7461 6e63 6549 6427  lientInstanceId'
-0000d4c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0000d4d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d4e0: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
-0000d4f0: 6964 203d 206d 2e67 6574 2827 436c 6965  id = m.get('Clie
-0000d500: 6e74 496e 7374 616e 6365 4964 2729 0a20  ntInstanceId'). 
-0000d510: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0000d520: 2745 6c61 7374 6963 4163 6365 6c65 7261  'ElasticAccelera
-0000d530: 7465 6449 6e73 7461 6e63 6549 6427 2920  tedInstanceId') 
-0000d540: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000d550: 2020 2020 2020 2020 2073 656c 662e 656c           self.el
-0000d560: 6173 7469 635f 6163 6365 6c65 7261 7465  astic_accelerate
-0000d570: 645f 696e 7374 616e 6365 5f69 6420 3d20  d_instance_id = 
-0000d580: 6d2e 6765 7428 2745 6c61 7374 6963 4163  m.get('ElasticAc
-0000d590: 6365 6c65 7261 7465 6449 6e73 7461 6e63  celeratedInstanc
-0000d5a0: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
-0000d5b0: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
-0000d5c0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0000d5d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d5e0: 2e72 6567 696f 6e5f 6964 203d 206d 2e67  .region_id = m.g
-0000d5f0: 6574 2827 5265 6769 6f6e 4964 2729 0a20  et('RegionId'). 
-0000d600: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000d610: 6c66 0a0a 0a63 6c61 7373 2044 656c 6574  lf...class Delet
-0000d620: 6545 6169 416c 6c52 6573 706f 6e73 6542  eEaiAllResponseB
-0000d630: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
-0000d640: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0000d650: 7365 6c66 2c20 7265 7175 6573 745f 6964  self, request_id
-0000d660: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0000d670: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-0000d680: 3d20 7265 7175 6573 745f 6964 2020 2320  = request_id  # 
-0000d690: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
-0000d6a0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0000d6b0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0000d6c0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0000d6d0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0000d6e0: 6d61 7020 3d20 7375 7065 7228 4465 6c65  map = super(Dele
-0000d6f0: 7465 4561 6941 6c6c 5265 7370 6f6e 7365  teEaiAllResponse
-0000d700: 426f 6479 2c20 7365 6c66 292e 746f 5f6d  Body, self).to_m
-0000d710: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0000d720: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0000d730: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000d740: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0000d750: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0000d760: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0000d770: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
-0000d780: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000d790: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-0000d7a0: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
-0000d7b0: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
-0000d7c0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0000d7d0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0000d7e0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
-0000d7f0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0000d800: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0000d810: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-0000d820: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
-0000d830: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000d840: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-0000d850: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
-0000d860: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
-0000d870: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-0000d880: 6173 7320 4465 6c65 7465 4561 6941 6c6c  ass DeleteEaiAll
-0000d890: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-0000d8a0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-0000d8b0: 6974 5f5f 2873 656c 662c 2068 6561 6465  it__(self, heade
-0000d8c0: 7273 3d4e 6f6e 652c 2073 7461 7475 735f  rs=None, status_
-0000d8d0: 636f 6465 3d4e 6f6e 652c 2062 6f64 793d  code=None, body=
-0000d8e0: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-0000d8f0: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-0000d900: 6164 6572 7320 2023 2074 7970 653a 2064  aders  # type: d
-0000d910: 6963 745b 7374 722c 2073 7472 5d0a 2020  ict[str, str].  
-0000d920: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0000d930: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-0000d940: 636f 6465 2020 2320 7479 7065 3a20 696e  code  # type: in
-0000d950: 740a 2020 2020 2020 2020 7365 6c66 2e62  t.        self.b
-0000d960: 6f64 7920 3d20 626f 6479 2020 2320 7479  ody = body  # ty
-0000d970: 7065 3a20 4465 6c65 7465 4561 6941 6c6c  pe: DeleteEaiAll
-0000d980: 5265 7370 6f6e 7365 426f 6479 0a0a 2020  ResponseBody..  
-0000d990: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0000d9a0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-0000d9b0: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-0000d9c0: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
-0000d9d0: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
-0000d9e0: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0000d9f0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-0000da00: 662e 7374 6174 7573 5f63 6f64 652c 2027  f.status_code, '
-0000da10: 7374 6174 7573 5f63 6f64 6527 290a 2020  status_code').  
-0000da20: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0000da30: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-0000da40: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
-0000da50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000da60: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-0000da70: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-0000da80: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-0000da90: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0000daa0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0000dab0: 6572 2844 656c 6574 6545 6169 416c 6c52  er(DeleteEaiAllR
-0000dac0: 6573 706f 6e73 652c 2073 656c 6629 2e74  esponse, self).t
-0000dad0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0000dae0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-0000daf0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000db00: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-0000db10: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-0000db20: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0000db30: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-0000db40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000db50: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-0000db60: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-0000db70: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-0000db80: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-0000db90: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-0000dba0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000dbb0: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-0000dbc0: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-0000dbd0: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
-0000dbe0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-0000dbf0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000dc00: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-0000dc10: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-0000dc20: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-0000dc30: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-0000dc40: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-0000dc50: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
-0000dc60: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0000dc70: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0000dc80: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-0000dc90: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0000dca0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000dcb0: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-0000dcc0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-0000dcd0: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-0000dce0: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-0000dcf0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000dd00: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-0000dd10: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-0000dd20: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-0000dd30: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-0000dd40: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0000dd50: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000dd60: 5f6d 6f64 656c 203d 2044 656c 6574 6545  _model = DeleteE
-0000dd70: 6169 416c 6c52 6573 706f 6e73 6542 6f64  aiAllResponseBod
-0000dd80: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-0000dd90: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-0000dda0: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-0000ddb0: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-0000ddc0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0000ddd0: 0a63 6c61 7373 2044 6573 6372 6962 6545  .class DescribeE
-0000dde0: 6169 7352 6571 7565 7374 2854 6561 4d6f  aisRequest(TeaMo
-0000ddf0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0000de00: 696e 6974 5f5f 2873 656c 662c 2065 6c61  init__(self, ela
-0000de10: 7374 6963 5f61 6363 656c 6572 6174 6564  stic_accelerated
-0000de20: 5f69 6e73 7461 6e63 655f 6964 733d 4e6f  _instance_ids=No
-0000de30: 6e65 2c20 696e 7374 616e 6365 5f6e 616d  ne, instance_nam
-0000de40: 653d 4e6f 6e65 2c20 696e 7374 616e 6365  e=None, instance
-0000de50: 5f74 7970 653d 4e6f 6e65 2c0a 2020 2020  _type=None,.    
-0000de60: 2020 2020 2020 2020 2020 2020 2070 6167               pag
-0000de70: 655f 6e75 6d62 6572 3d4e 6f6e 652c 2070  e_number=None, p
-0000de80: 6167 655f 7369 7a65 3d4e 6f6e 652c 2072  age_size=None, r
-0000de90: 6567 696f 6e5f 6964 3d4e 6f6e 652c 2072  egion_id=None, r
-0000dea0: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-0000deb0: 3d4e 6f6e 652c 2073 7461 7475 733d 4e6f  =None, status=No
-0000dec0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
-0000ded0: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-0000dee0: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-0000def0: 6473 203d 2065 6c61 7374 6963 5f61 6363  ds = elastic_acc
-0000df00: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
-0000df10: 655f 6964 7320 2023 2074 7970 653a 2073  e_ids  # type: s
-0000df20: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-0000df30: 696e 7374 616e 6365 5f6e 616d 6520 3d20  instance_name = 
-0000df40: 696e 7374 616e 6365 5f6e 616d 6520 2023  instance_name  #
-0000df50: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0000df60: 2020 2073 656c 662e 696e 7374 616e 6365     self.instance
-0000df70: 5f74 7970 6520 3d20 696e 7374 616e 6365  _type = instance
-0000df80: 5f74 7970 6520 2023 2074 7970 653a 2073  _type  # type: s
-0000df90: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-0000dfa0: 7061 6765 5f6e 756d 6265 7220 3d20 7061  page_number = pa
-0000dfb0: 6765 5f6e 756d 6265 7220 2023 2074 7970  ge_number  # typ
-0000dfc0: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
-0000dfd0: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
-0000dfe0: 7061 6765 5f73 697a 6520 2023 2074 7970  page_size  # typ
-0000dff0: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
-0000e000: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
-0000e010: 7265 6769 6f6e 5f69 6420 2023 2074 7970  region_id  # typ
-0000e020: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-0000e030: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
-0000e040: 7570 5f69 6420 3d20 7265 736f 7572 6365  up_id = resource
-0000e050: 5f67 726f 7570 5f69 6420 2023 2074 7970  _group_id  # typ
-0000e060: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-0000e070: 656c 662e 7374 6174 7573 203d 2073 7461  elf.status = sta
-0000e080: 7475 7320 2023 2074 7970 653a 2073 7472  tus  # type: str
-0000e090: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0000e0a0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0000e0b0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-0000e0c0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0000e0d0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0000e0e0: 6572 2844 6573 6372 6962 6545 6169 7352  er(DescribeEaisR
-0000e0f0: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
-0000e100: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0000e110: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0000e120: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000e130: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0000e140: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0000e150: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0000e160: 7365 6c66 2e65 6c61 7374 6963 5f61 6363  self.elastic_acc
-0000e170: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
-0000e180: 655f 6964 7320 6973 206e 6f74 204e 6f6e  e_ids is not Non
-0000e190: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000e1a0: 6573 756c 745b 2745 6c61 7374 6963 4163  esult['ElasticAc
-0000e1b0: 6365 6c65 7261 7465 6449 6e73 7461 6e63  celeratedInstanc
-0000e1c0: 6549 6473 275d 203d 2073 656c 662e 656c  eIds'] = self.el
-0000e1d0: 6173 7469 635f 6163 6365 6c65 7261 7465  astic_accelerate
-0000e1e0: 645f 696e 7374 616e 6365 5f69 6473 0a20  d_instance_ids. 
-0000e1f0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-0000e200: 6e73 7461 6e63 655f 6e61 6d65 2069 7320  nstance_name is 
-0000e210: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000e220: 2020 2020 2020 7265 7375 6c74 5b27 496e        result['In
-0000e230: 7374 616e 6365 4e61 6d65 275d 203d 2073  stanceName'] = s
-0000e240: 656c 662e 696e 7374 616e 6365 5f6e 616d  elf.instance_nam
-0000e250: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0000e260: 662e 696e 7374 616e 6365 5f74 7970 6520  f.instance_type 
-0000e270: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000e280: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000e290: 2749 6e73 7461 6e63 6554 7970 6527 5d20  'InstanceType'] 
-0000e2a0: 3d20 7365 6c66 2e69 6e73 7461 6e63 655f  = self.instance_
-0000e2b0: 7479 7065 0a20 2020 2020 2020 2069 6620  type.        if 
-0000e2c0: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
-0000e2d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e2e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000e2f0: 5b27 5061 6765 4e75 6d62 6572 275d 203d  ['PageNumber'] =
-0000e300: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
-0000e310: 720a 2020 2020 2020 2020 6966 2073 656c  r.        if sel
-0000e320: 662e 7061 6765 5f73 697a 6520 6973 206e  f.page_size is n
-0000e330: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000e340: 2020 2020 2072 6573 756c 745b 2750 6167       result['Pag
-0000e350: 6553 697a 6527 5d20 3d20 7365 6c66 2e70  eSize'] = self.p
-0000e360: 6167 655f 7369 7a65 0a20 2020 2020 2020  age_size.       
-0000e370: 2069 6620 7365 6c66 2e72 6567 696f 6e5f   if self.region_
-0000e380: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0000e390: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000e3a0: 6c74 5b27 5265 6769 6f6e 4964 275d 203d  lt['RegionId'] =
-0000e3b0: 2073 656c 662e 7265 6769 6f6e 5f69 640a   self.region_id.
-0000e3c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000e3d0: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-0000e3e0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-0000e3f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000e400: 745b 2752 6573 6f75 7263 6547 726f 7570  t['ResourceGroup
-0000e410: 4964 275d 203d 2073 656c 662e 7265 736f  Id'] = self.reso
-0000e420: 7572 6365 5f67 726f 7570 5f69 640a 2020  urce_group_id.  
-0000e430: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-0000e440: 6174 7573 2069 7320 6e6f 7420 4e6f 6e65  atus is not None
-0000e450: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000e460: 7375 6c74 5b27 5374 6174 7573 275d 203d  sult['Status'] =
-0000e470: 2073 656c 662e 7374 6174 7573 0a20 2020   self.status.   
-0000e480: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0000e490: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0000e4a0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
-0000e4b0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0000e4c0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0000e4d0: 2020 2020 6966 206d 2e67 6574 2827 456c      if m.get('El
-0000e4e0: 6173 7469 6341 6363 656c 6572 6174 6564  asticAccelerated
-0000e4f0: 496e 7374 616e 6365 4964 7327 2920 6973  InstanceIds') is
-0000e500: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000e510: 2020 2020 2020 2073 656c 662e 656c 6173         self.elas
-0000e520: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
-0000e530: 696e 7374 616e 6365 5f69 6473 203d 206d  instance_ids = m
-0000e540: 2e67 6574 2827 456c 6173 7469 6341 6363  .get('ElasticAcc
-0000e550: 656c 6572 6174 6564 496e 7374 616e 6365  eleratedInstance
-0000e560: 4964 7327 290a 2020 2020 2020 2020 6966  Ids').        if
-0000e570: 206d 2e67 6574 2827 496e 7374 616e 6365   m.get('Instance
-0000e580: 4e61 6d65 2729 2069 7320 6e6f 7420 4e6f  Name') is not No
-0000e590: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000e5a0: 7365 6c66 2e69 6e73 7461 6e63 655f 6e61  self.instance_na
-0000e5b0: 6d65 203d 206d 2e67 6574 2827 496e 7374  me = m.get('Inst
-0000e5c0: 616e 6365 4e61 6d65 2729 0a20 2020 2020  anceName').     
-0000e5d0: 2020 2069 6620 6d2e 6765 7428 2749 6e73     if m.get('Ins
-0000e5e0: 7461 6e63 6554 7970 6527 2920 6973 206e  tanceType') is n
-0000e5f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000e600: 2020 2020 2073 656c 662e 696e 7374 616e       self.instan
-0000e610: 6365 5f74 7970 6520 3d20 6d2e 6765 7428  ce_type = m.get(
-0000e620: 2749 6e73 7461 6e63 6554 7970 6527 290a  'InstanceType').
-0000e630: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0000e640: 2827 5061 6765 4e75 6d62 6572 2729 2069  ('PageNumber') i
-0000e650: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000e660: 2020 2020 2020 2020 7365 6c66 2e70 6167          self.pag
-0000e670: 655f 6e75 6d62 6572 203d 206d 2e67 6574  e_number = m.get
-0000e680: 2827 5061 6765 4e75 6d62 6572 2729 0a20  ('PageNumber'). 
-0000e690: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0000e6a0: 2750 6167 6553 697a 6527 2920 6973 206e  'PageSize') is n
-0000e6b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000e6c0: 2020 2020 2073 656c 662e 7061 6765 5f73       self.page_s
-0000e6d0: 697a 6520 3d20 6d2e 6765 7428 2750 6167  ize = m.get('Pag
-0000e6e0: 6553 697a 6527 290a 2020 2020 2020 2020  eSize').        
-0000e6f0: 6966 206d 2e67 6574 2827 5265 6769 6f6e  if m.get('Region
-0000e700: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-0000e710: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000e720: 6c66 2e72 6567 696f 6e5f 6964 203d 206d  lf.region_id = m
-0000e730: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
-0000e740: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0000e750: 7428 2752 6573 6f75 7263 6547 726f 7570  t('ResourceGroup
-0000e760: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-0000e770: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000e780: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
-0000e790: 705f 6964 203d 206d 2e67 6574 2827 5265  p_id = m.get('Re
-0000e7a0: 736f 7572 6365 4772 6f75 7049 6427 290a  sourceGroupId').
-0000e7b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0000e7c0: 2827 5374 6174 7573 2729 2069 7320 6e6f  ('Status') is no
-0000e7d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000e7e0: 2020 2020 7365 6c66 2e73 7461 7475 7320      self.status 
-0000e7f0: 3d20 6d2e 6765 7428 2753 7461 7475 7327  = m.get('Status'
-0000e800: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000e810: 2073 656c 660a 0a0a 636c 6173 7320 4465   self...class De
-0000e820: 7363 7269 6265 4561 6973 5265 7370 6f6e  scribeEaisRespon
-0000e830: 7365 426f 6479 496e 7374 616e 6365 7349  seBodyInstancesI
-0000e840: 6e73 7461 6e63 6554 6167 7354 6167 2854  nstanceTagsTag(T
-0000e850: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-0000e860: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0000e870: 2074 6167 5f6b 6579 3d4e 6f6e 652c 2074   tag_key=None, t
-0000e880: 6167 5f76 616c 7565 3d4e 6f6e 6529 3a0a  ag_value=None):.
-0000e890: 2020 2020 2020 2020 7365 6c66 2e74 6167          self.tag
-0000e8a0: 5f6b 6579 203d 2074 6167 5f6b 6579 2020  _key = tag_key  
-0000e8b0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-0000e8c0: 2020 2020 7365 6c66 2e74 6167 5f76 616c      self.tag_val
-0000e8d0: 7565 203d 2074 6167 5f76 616c 7565 2020  ue = tag_value  
-0000e8e0: 2320 7479 7065 3a20 7374 720a 0a20 2020  # type: str..   
-0000e8f0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0000e900: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-0000e910: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-0000e920: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0000e930: 205f 6d61 7020 3d20 7375 7065 7228 4465   _map = super(De
-0000e940: 7363 7269 6265 4561 6973 5265 7370 6f6e  scribeEaisRespon
-0000e950: 7365 426f 6479 496e 7374 616e 6365 7349  seBodyInstancesI
-0000e960: 6e73 7461 6e63 6554 6167 7354 6167 2c20  nstanceTagsTag, 
-0000e970: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
-0000e980: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-0000e990: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000e9a0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-0000e9b0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-0000e9c0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-0000e9d0: 2020 2020 2069 6620 7365 6c66 2e74 6167       if self.tag
-0000e9e0: 5f6b 6579 2069 7320 6e6f 7420 4e6f 6e65  _key is not None
-0000e9f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000ea00: 7375 6c74 5b27 5461 674b 6579 275d 203d  sult['TagKey'] =
-0000ea10: 2073 656c 662e 7461 675f 6b65 790a 2020   self.tag_key.  
-0000ea20: 2020 2020 2020 6966 2073 656c 662e 7461        if self.ta
-0000ea30: 675f 7661 6c75 6520 6973 206e 6f74 204e  g_value is not N
-0000ea40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000ea50: 2072 6573 756c 745b 2754 6167 5661 6c75   result['TagValu
-0000ea60: 6527 5d20 3d20 7365 6c66 2e74 6167 5f76  e'] = self.tag_v
-0000ea70: 616c 7565 0a20 2020 2020 2020 2072 6574  alue.        ret
-0000ea80: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0000ea90: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0000eaa0: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-0000eab0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0000eac0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0000ead0: 2e67 6574 2827 5461 674b 6579 2729 2069  .get('TagKey') i
-0000eae0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000eaf0: 2020 2020 2020 2020 7365 6c66 2e74 6167          self.tag
-0000eb00: 5f6b 6579 203d 206d 2e67 6574 2827 5461  _key = m.get('Ta
-0000eb10: 674b 6579 2729 0a20 2020 2020 2020 2069  gKey').        i
-0000eb20: 6620 6d2e 6765 7428 2754 6167 5661 6c75  f m.get('TagValu
-0000eb30: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-0000eb40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000eb50: 662e 7461 675f 7661 6c75 6520 3d20 6d2e  f.tag_value = m.
-0000eb60: 6765 7428 2754 6167 5661 6c75 6527 290a  get('TagValue').
-0000eb70: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000eb80: 656c 660a 0a0a 636c 6173 7320 4465 7363  elf...class Desc
-0000eb90: 7269 6265 4561 6973 5265 7370 6f6e 7365  ribeEaisResponse
-0000eba0: 426f 6479 496e 7374 616e 6365 7349 6e73  BodyInstancesIns
-0000ebb0: 7461 6e63 6554 6167 7328 5465 614d 6f64  tanceTags(TeaMod
-0000ebc0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-0000ebd0: 6e69 745f 5f28 7365 6c66 2c20 7461 673d  nit__(self, tag=
-0000ebe0: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-0000ebf0: 656c 662e 7461 6720 3d20 7461 6720 2023  elf.tag = tag  #
-0000ec00: 2074 7970 653a 206c 6973 745b 4465 7363   type: list[Desc
-0000ec10: 7269 6265 4561 6973 5265 7370 6f6e 7365  ribeEaisResponse
-0000ec20: 426f 6479 496e 7374 616e 6365 7349 6e73  BodyInstancesIns
-0000ec30: 7461 6e63 6554 6167 7354 6167 5d0a 0a20  tanceTagsTag].. 
-0000ec40: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0000ec50: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-0000ec60: 6620 7365 6c66 2e74 6167 3a0a 2020 2020  f self.tag:.    
-0000ec70: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-0000ec80: 2073 656c 662e 7461 673a 0a20 2020 2020   self.tag:.     
-0000ec90: 2020 2020 2020 2020 2020 2069 6620 6b3a             if k:
-0000eca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ecb0: 2020 2020 206b 2e76 616c 6964 6174 6528       k.validate(
-0000ecc0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-0000ecd0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0000ece0: 205f 6d61 7020 3d20 7375 7065 7228 4465   _map = super(De
-0000ecf0: 7363 7269 6265 4561 6973 5265 7370 6f6e  scribeEaisRespon
-0000ed00: 7365 426f 6479 496e 7374 616e 6365 7349  seBodyInstancesI
-0000ed10: 6e73 7461 6e63 6554 6167 732c 2073 656c  nstanceTags, sel
-0000ed20: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-0000ed30: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0000ed40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000ed50: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0000ed60: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0000ed70: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0000ed80: 2020 7265 7375 6c74 5b27 5461 6727 5d20    result['Tag'] 
-0000ed90: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
-0000eda0: 7365 6c66 2e74 6167 2069 7320 6e6f 7420  self.tag is not 
-0000edb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000edc0: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
-0000edd0: 7461 673a 0a20 2020 2020 2020 2020 2020  tag:.           
-0000ede0: 2020 2020 2072 6573 756c 745b 2754 6167       result['Tag
-0000edf0: 275d 2e61 7070 656e 6428 6b2e 746f 5f6d  '].append(k.to_m
-0000ee00: 6170 2829 2069 6620 6b20 656c 7365 204e  ap() if k else N
-0000ee10: 6f6e 6529 0a20 2020 2020 2020 2072 6574  one).        ret
-0000ee20: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0000ee30: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0000ee40: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-0000ee50: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0000ee60: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-0000ee70: 2e74 6167 203d 205b 5d0a 2020 2020 2020  .tag = [].      
-0000ee80: 2020 6966 206d 2e67 6574 2827 5461 6727    if m.get('Tag'
-0000ee90: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0000eea0: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-0000eeb0: 2069 6e20 6d2e 6765 7428 2754 6167 2729   in m.get('Tag')
-0000eec0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000eed0: 2020 7465 6d70 5f6d 6f64 656c 203d 2044    temp_model = D
-0000eee0: 6573 6372 6962 6545 6169 7352 6573 706f  escribeEaisRespo
-0000eef0: 6e73 6542 6f64 7949 6e73 7461 6e63 6573  nseBodyInstances
-0000ef00: 496e 7374 616e 6365 5461 6773 5461 6728  InstanceTagsTag(
-0000ef10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ef20: 2020 7365 6c66 2e74 6167 2e61 7070 656e    self.tag.appen
-0000ef30: 6428 7465 6d70 5f6d 6f64 656c 2e66 726f  d(temp_model.fro
-0000ef40: 6d5f 6d61 7028 6b29 290a 2020 2020 2020  m_map(k)).      
-0000ef50: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0000ef60: 636c 6173 7320 4465 7363 7269 6265 4561  class DescribeEa
-0000ef70: 6973 5265 7370 6f6e 7365 426f 6479 496e  isResponseBodyIn
-0000ef80: 7374 616e 6365 7349 6e73 7461 6e63 6528  stancesInstance(
-0000ef90: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0000efa0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0000efb0: 2c20 6361 7465 676f 7279 3d4e 6f6e 652c  , category=None,
-0000efc0: 2063 6c69 656e 745f 696e 7374 616e 6365   client_instance
-0000efd0: 5f69 643d 4e6f 6e65 2c20 636c 6965 6e74  _id=None, client
-0000efe0: 5f69 6e73 7461 6e63 655f 6e61 6d65 3d4e  _instance_name=N
-0000eff0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0000f000: 2020 2020 2020 636c 6965 6e74 5f69 6e73        client_ins
-0000f010: 7461 6e63 655f 7479 7065 3d4e 6f6e 652c  tance_type=None,
-0000f020: 2063 7265 6174 696f 6e5f 7469 6d65 3d4e   creation_time=N
-0000f030: 6f6e 652c 2064 6573 6372 6970 7469 6f6e  one, description
-0000f040: 3d4e 6f6e 652c 2065 6c61 7374 6963 5f61  =None, elastic_a
-0000f050: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
-0000f060: 6e63 655f 6964 3d4e 6f6e 652c 0a20 2020  nce_id=None,.   
-0000f070: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000f080: 7374 616e 6365 5f6e 616d 653d 4e6f 6e65  stance_name=None
-0000f090: 2c20 696e 7374 616e 6365 5f74 7970 653d  , instance_type=
-0000f0a0: 4e6f 6e65 2c20 6a75 7079 7465 725f 7572  None, jupyter_ur
-0000f0b0: 6c3d 4e6f 6e65 2c20 7265 6769 6f6e 5f69  l=None, region_i
-0000f0c0: 643d 4e6f 6e65 2c20 7265 736f 7572 6365  d=None, resource
-0000f0d0: 5f67 726f 7570 5f69 643d 4e6f 6e65 2c0a  _group_id=None,.
-0000f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f0f0: 2073 6563 7572 6974 795f 6772 6f75 705f   security_group_
-0000f100: 6964 3d4e 6f6e 652c 2073 7461 7274 5f74  id=None, start_t
-0000f110: 696d 653d 4e6f 6e65 2c20 7374 6174 7573  ime=None, status
-0000f120: 3d4e 6f6e 652c 2074 6167 733d 4e6f 6e65  =None, tags=None
-0000f130: 2c20 765f 7377 6974 6368 5f69 643d 4e6f  , v_switch_id=No
-0000f140: 6e65 2c20 7a6f 6e65 5f69 643d 4e6f 6e65  ne, zone_id=None
-0000f150: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0000f160: 6361 7465 676f 7279 203d 2063 6174 6567  category = categ
-0000f170: 6f72 7920 2023 2074 7970 653a 2073 7472  ory  # type: str
-0000f180: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
-0000f190: 6965 6e74 5f69 6e73 7461 6e63 655f 6964  ient_instance_id
-0000f1a0: 203d 2063 6c69 656e 745f 696e 7374 616e   = client_instan
-0000f1b0: 6365 5f69 6420 2023 2074 7970 653a 2073  ce_id  # type: s
-0000f1c0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-0000f1d0: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
-0000f1e0: 6e61 6d65 203d 2063 6c69 656e 745f 696e  name = client_in
-0000f1f0: 7374 616e 6365 5f6e 616d 6520 2023 2074  stance_name  # t
-0000f200: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
-0000f210: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
-0000f220: 7461 6e63 655f 7479 7065 203d 2063 6c69  tance_type = cli
-0000f230: 656e 745f 696e 7374 616e 6365 5f74 7970  ent_instance_typ
-0000f240: 6520 2023 2074 7970 653a 2073 7472 0a20  e  # type: str. 
-0000f250: 2020 2020 2020 2073 656c 662e 6372 6561         self.crea
-0000f260: 7469 6f6e 5f74 696d 6520 3d20 6372 6561  tion_time = crea
-0000f270: 7469 6f6e 5f74 696d 6520 2023 2074 7970  tion_time  # typ
-0000f280: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-0000f290: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
-0000f2a0: 3d20 6465 7363 7269 7074 696f 6e20 2023  = description  #
-0000f2b0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0000f2c0: 2020 2073 656c 662e 656c 6173 7469 635f     self.elastic_
-0000f2d0: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
-0000f2e0: 616e 6365 5f69 6420 3d20 656c 6173 7469  ance_id = elasti
-0000f2f0: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
-0000f300: 7374 616e 6365 5f69 6420 2023 2074 7970  stance_id  # typ
-0000f310: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-0000f320: 656c 662e 696e 7374 616e 6365 5f6e 616d  elf.instance_nam
-0000f330: 6520 3d20 696e 7374 616e 6365 5f6e 616d  e = instance_nam
-0000f340: 6520 2023 2074 7970 653a 2073 7472 0a20  e  # type: str. 
-0000f350: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
-0000f360: 616e 6365 5f74 7970 6520 3d20 696e 7374  ance_type = inst
-0000f370: 616e 6365 5f74 7970 6520 2023 2074 7970  ance_type  # typ
-0000f380: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-0000f390: 656c 662e 6a75 7079 7465 725f 7572 6c20  elf.jupyter_url 
-0000f3a0: 3d20 6a75 7079 7465 725f 7572 6c20 2023  = jupyter_url  #
-0000f3b0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0000f3c0: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
-0000f3d0: 6420 3d20 7265 6769 6f6e 5f69 6420 2023  d = region_id  #
-0000f3e0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0000f3f0: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
-0000f400: 5f67 726f 7570 5f69 6420 3d20 7265 736f  _group_id = reso
-0000f410: 7572 6365 5f67 726f 7570 5f69 6420 2023  urce_group_id  #
-0000f420: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0000f430: 2020 2073 656c 662e 7365 6375 7269 7479     self.security
-0000f440: 5f67 726f 7570 5f69 6420 3d20 7365 6375  _group_id = secu
-0000f450: 7269 7479 5f67 726f 7570 5f69 6420 2023  rity_group_id  #
-0000f460: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0000f470: 2020 2073 656c 662e 7374 6172 745f 7469     self.start_ti
-0000f480: 6d65 203d 2073 7461 7274 5f74 696d 6520  me = start_time 
-0000f490: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-0000f4a0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-0000f4b0: 203d 2073 7461 7475 7320 2023 2074 7970   = status  # typ
-0000f4c0: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-0000f4d0: 656c 662e 7461 6773 203d 2074 6167 7320  elf.tags = tags 
-0000f4e0: 2023 2074 7970 653a 2044 6573 6372 6962   # type: Describ
-0000f4f0: 6545 6169 7352 6573 706f 6e73 6542 6f64  eEaisResponseBod
-0000f500: 7949 6e73 7461 6e63 6573 496e 7374 616e  yInstancesInstan
-0000f510: 6365 5461 6773 0a20 2020 2020 2020 2073  ceTags.        s
-0000f520: 656c 662e 765f 7377 6974 6368 5f69 6420  elf.v_switch_id 
-0000f530: 3d20 765f 7377 6974 6368 5f69 6420 2023  = v_switch_id  #
-0000f540: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0000f550: 2020 2073 656c 662e 7a6f 6e65 5f69 6420     self.zone_id 
-0000f560: 3d20 7a6f 6e65 5f69 6420 2023 2074 7970  = zone_id  # typ
-0000f570: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
-0000f580: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0000f590: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f5a0: 7461 6773 3a0a 2020 2020 2020 2020 2020  tags:.          
-0000f5b0: 2020 7365 6c66 2e74 6167 732e 7661 6c69    self.tags.vali
-0000f5c0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-0000f5d0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0000f5e0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0000f5f0: 6572 2844 6573 6372 6962 6545 6169 7352  er(DescribeEaisR
-0000f600: 6573 706f 6e73 6542 6f64 7949 6e73 7461  esponseBodyInsta
-0000f610: 6e63 6573 496e 7374 616e 6365 2c20 7365  ncesInstance, se
-0000f620: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
-0000f630: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-0000f640: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000f650: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-0000f660: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-0000f670: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0000f680: 2020 2069 6620 7365 6c66 2e63 6174 6567     if self.categ
-0000f690: 6f72 7920 6973 206e 6f74 204e 6f6e 653a  ory is not None:
-0000f6a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000f6b0: 756c 745b 2743 6174 6567 6f72 7927 5d20  ult['Category'] 
-0000f6c0: 3d20 7365 6c66 2e63 6174 6567 6f72 790a  = self.category.
-0000f6d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f6e0: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
-0000f6f0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0000f700: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000f710: 6c74 5b27 436c 6965 6e74 496e 7374 616e  lt['ClientInstan
-0000f720: 6365 4964 275d 203d 2073 656c 662e 636c  ceId'] = self.cl
-0000f730: 6965 6e74 5f69 6e73 7461 6e63 655f 6964  ient_instance_id
-0000f740: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000f750: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
-0000f760: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
-0000f770: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000f780: 6573 756c 745b 2743 6c69 656e 7449 6e73  esult['ClientIns
-0000f790: 7461 6e63 654e 616d 6527 5d20 3d20 7365  tanceName'] = se
-0000f7a0: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
-0000f7b0: 6365 5f6e 616d 650a 2020 2020 2020 2020  ce_name.        
-0000f7c0: 6966 2073 656c 662e 636c 6965 6e74 5f69  if self.client_i
-0000f7d0: 6e73 7461 6e63 655f 7479 7065 2069 7320  nstance_type is 
-0000f7e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000f7f0: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
-0000f800: 6965 6e74 496e 7374 616e 6365 5479 7065  ientInstanceType
-0000f810: 275d 203d 2073 656c 662e 636c 6965 6e74  '] = self.client
-0000f820: 5f69 6e73 7461 6e63 655f 7479 7065 0a20  _instance_type. 
-0000f830: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0000f840: 7265 6174 696f 6e5f 7469 6d65 2069 7320  reation_time is 
-0000f850: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000f860: 2020 2020 2020 7265 7375 6c74 5b27 4372        result['Cr
-0000f870: 6561 7469 6f6e 5469 6d65 275d 203d 2073  eationTime'] = s
-0000f880: 656c 662e 6372 6561 7469 6f6e 5f74 696d  elf.creation_tim
-0000f890: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0000f8a0: 662e 6465 7363 7269 7074 696f 6e20 6973  f.description is
-0000f8b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000f8c0: 2020 2020 2020 2072 6573 756c 745b 2744         result['D
-0000f8d0: 6573 6372 6970 7469 6f6e 275d 203d 2073  escription'] = s
-0000f8e0: 656c 662e 6465 7363 7269 7074 696f 6e0a  elf.description.
-0000f8f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f900: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
-0000f910: 7465 645f 696e 7374 616e 6365 5f69 6420  ted_instance_id 
-0000f920: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000f930: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000f940: 2745 6c61 7374 6963 4163 6365 6c65 7261  'ElasticAccelera
-0000f950: 7465 6449 6e73 7461 6e63 6549 6427 5d20  tedInstanceId'] 
-0000f960: 3d20 7365 6c66 2e65 6c61 7374 6963 5f61  = self.elastic_a
-0000f970: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
-0000f980: 6e63 655f 6964 0a20 2020 2020 2020 2069  nce_id.        i
-0000f990: 6620 7365 6c66 2e69 6e73 7461 6e63 655f  f self.instance_
-0000f9a0: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-0000f9b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000f9c0: 7375 6c74 5b27 496e 7374 616e 6365 4e61  sult['InstanceNa
-0000f9d0: 6d65 275d 203d 2073 656c 662e 696e 7374  me'] = self.inst
-0000f9e0: 616e 6365 5f6e 616d 650a 2020 2020 2020  ance_name.      
-0000f9f0: 2020 6966 2073 656c 662e 696e 7374 616e    if self.instan
-0000fa00: 6365 5f74 7970 6520 6973 206e 6f74 204e  ce_type is not N
-0000fa10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000fa20: 2072 6573 756c 745b 2749 6e73 7461 6e63   result['Instanc
-0000fa30: 6554 7970 6527 5d20 3d20 7365 6c66 2e69  eType'] = self.i
-0000fa40: 6e73 7461 6e63 655f 7479 7065 0a20 2020  nstance_type.   
-0000fa50: 2020 2020 2069 6620 7365 6c66 2e6a 7570       if self.jup
-0000fa60: 7974 6572 5f75 726c 2069 7320 6e6f 7420  yter_url is not 
-0000fa70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000fa80: 2020 7265 7375 6c74 5b27 4a75 7079 7465    result['Jupyte
-0000fa90: 7255 726c 275d 203d 2073 656c 662e 6a75  rUrl'] = self.ju
-0000faa0: 7079 7465 725f 7572 6c0a 2020 2020 2020  pyter_url.      
-0000fab0: 2020 6966 2073 656c 662e 7265 6769 6f6e    if self.region
-0000fac0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-0000fad0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000fae0: 756c 745b 2752 6567 696f 6e49 6427 5d20  ult['RegionId'] 
-0000faf0: 3d20 7365 6c66 2e72 6567 696f 6e5f 6964  = self.region_id
-0000fb00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000fb10: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
-0000fb20: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0000fb30: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000fb40: 6c74 5b27 5265 736f 7572 6365 4772 6f75  lt['ResourceGrou
-0000fb50: 7049 6427 5d20 3d20 7365 6c66 2e72 6573  pId'] = self.res
-0000fb60: 6f75 7263 655f 6772 6f75 705f 6964 0a20  ource_group_id. 
-0000fb70: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0000fb80: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
-0000fb90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000fba0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000fbb0: 5b27 5365 6375 7269 7479 4772 6f75 7049  ['SecurityGroupI
-0000fbc0: 6427 5d20 3d20 7365 6c66 2e73 6563 7572  d'] = self.secur
-0000fbd0: 6974 795f 6772 6f75 705f 6964 0a20 2020  ity_group_id.   
-0000fbe0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-0000fbf0: 7274 5f74 696d 6520 6973 206e 6f74 204e  rt_time is not N
-0000fc00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000fc10: 2072 6573 756c 745b 2753 7461 7274 5469   result['StartTi
-0000fc20: 6d65 275d 203d 2073 656c 662e 7374 6172  me'] = self.star
-0000fc30: 745f 7469 6d65 0a20 2020 2020 2020 2069  t_time.        i
-0000fc40: 6620 7365 6c66 2e73 7461 7475 7320 6973  f self.status is
-0000fc50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000fc60: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
-0000fc70: 7461 7475 7327 5d20 3d20 7365 6c66 2e73  tatus'] = self.s
-0000fc80: 7461 7475 730a 2020 2020 2020 2020 6966  tatus.        if
-0000fc90: 2073 656c 662e 7461 6773 2069 7320 6e6f   self.tags is no
-0000fca0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000fcb0: 2020 2020 7265 7375 6c74 5b27 5461 6773      result['Tags
-0000fcc0: 275d 203d 2073 656c 662e 7461 6773 2e74  '] = self.tags.t
-0000fcd0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0000fce0: 6966 2073 656c 662e 765f 7377 6974 6368  if self.v_switch
-0000fcf0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-0000fd00: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000fd10: 756c 745b 2756 5377 6974 6368 4964 275d  ult['VSwitchId']
-0000fd20: 203d 2073 656c 662e 765f 7377 6974 6368   = self.v_switch
-0000fd30: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-0000fd40: 656c 662e 7a6f 6e65 5f69 6420 6973 206e  elf.zone_id is n
-0000fd50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000fd60: 2020 2020 2072 6573 756c 745b 275a 6f6e       result['Zon
-0000fd70: 6549 6427 5d20 3d20 7365 6c66 2e7a 6f6e  eId'] = self.zon
-0000fd80: 655f 6964 0a20 2020 2020 2020 2072 6574  e_id.        ret
-0000fd90: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0000fda0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0000fdb0: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-0000fdc0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0000fdd0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0000fde0: 2e67 6574 2827 4361 7465 676f 7279 2729  .get('Category')
-0000fdf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000fe00: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000fe10: 6174 6567 6f72 7920 3d20 6d2e 6765 7428  ategory = m.get(
-0000fe20: 2743 6174 6567 6f72 7927 290a 2020 2020  'Category').    
-0000fe30: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
-0000fe40: 6965 6e74 496e 7374 616e 6365 4964 2729  ientInstanceId')
-0000fe50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000fe60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000fe70: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
-0000fe80: 6420 3d20 6d2e 6765 7428 2743 6c69 656e  d = m.get('Clien
-0000fe90: 7449 6e73 7461 6e63 6549 6427 290a 2020  tInstanceId').  
-0000fea0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0000feb0: 436c 6965 6e74 496e 7374 616e 6365 4e61  ClientInstanceNa
-0000fec0: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
-0000fed0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000fee0: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
-0000fef0: 6365 5f6e 616d 6520 3d20 6d2e 6765 7428  ce_name = m.get(
-0000ff00: 2743 6c69 656e 7449 6e73 7461 6e63 654e  'ClientInstanceN
-0000ff10: 616d 6527 290a 2020 2020 2020 2020 6966  ame').        if
-0000ff20: 206d 2e67 6574 2827 436c 6965 6e74 496e   m.get('ClientIn
-0000ff30: 7374 616e 6365 5479 7065 2729 2069 7320  stanceType') is 
-0000ff40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000ff50: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-0000ff60: 745f 696e 7374 616e 6365 5f74 7970 6520  t_instance_type 
-0000ff70: 3d20 6d2e 6765 7428 2743 6c69 656e 7449  = m.get('ClientI
-0000ff80: 6e73 7461 6e63 6554 7970 6527 290a 2020  nstanceType').  
-0000ff90: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0000ffa0: 4372 6561 7469 6f6e 5469 6d65 2729 2069  CreationTime') i
-0000ffb0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000ffc0: 2020 2020 2020 2020 7365 6c66 2e63 7265          self.cre
-0000ffd0: 6174 696f 6e5f 7469 6d65 203d 206d 2e67  ation_time = m.g
-0000ffe0: 6574 2827 4372 6561 7469 6f6e 5469 6d65  et('CreationTime
-0000fff0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00010000: 6765 7428 2744 6573 6372 6970 7469 6f6e  get('Description
-00010010: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00010020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010030: 2e64 6573 6372 6970 7469 6f6e 203d 206d  .description = m
-00010040: 2e67 6574 2827 4465 7363 7269 7074 696f  .get('Descriptio
-00010050: 6e27 290a 2020 2020 2020 2020 6966 206d  n').        if m
-00010060: 2e67 6574 2827 456c 6173 7469 6341 6363  .get('ElasticAcc
-00010070: 656c 6572 6174 6564 496e 7374 616e 6365  eleratedInstance
-00010080: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00010090: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000100a0: 6c66 2e65 6c61 7374 6963 5f61 6363 656c  lf.elastic_accel
-000100b0: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
-000100c0: 6964 203d 206d 2e67 6574 2827 456c 6173  id = m.get('Elas
-000100d0: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
-000100e0: 7374 616e 6365 4964 2729 0a20 2020 2020  stanceId').     
-000100f0: 2020 2069 6620 6d2e 6765 7428 2749 6e73     if m.get('Ins
-00010100: 7461 6e63 654e 616d 6527 2920 6973 206e  tanceName') is n
-00010110: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00010120: 2020 2020 2073 656c 662e 696e 7374 616e       self.instan
-00010130: 6365 5f6e 616d 6520 3d20 6d2e 6765 7428  ce_name = m.get(
-00010140: 2749 6e73 7461 6e63 654e 616d 6527 290a  'InstanceName').
-00010150: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00010160: 2827 496e 7374 616e 6365 5479 7065 2729  ('InstanceType')
-00010170: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00010180: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-00010190: 6e73 7461 6e63 655f 7479 7065 203d 206d  nstance_type = m
-000101a0: 2e67 6574 2827 496e 7374 616e 6365 5479  .get('InstanceTy
-000101b0: 7065 2729 0a20 2020 2020 2020 2069 6620  pe').        if 
-000101c0: 6d2e 6765 7428 274a 7570 7974 6572 5572  m.get('JupyterUr
-000101d0: 6c27 2920 6973 206e 6f74 204e 6f6e 653a  l') is not None:
-000101e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000101f0: 662e 6a75 7079 7465 725f 7572 6c20 3d20  f.jupyter_url = 
-00010200: 6d2e 6765 7428 274a 7570 7974 6572 5572  m.get('JupyterUr
-00010210: 6c27 290a 2020 2020 2020 2020 6966 206d  l').        if m
-00010220: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
-00010230: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00010240: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00010250: 6567 696f 6e5f 6964 203d 206d 2e67 6574  egion_id = m.get
-00010260: 2827 5265 6769 6f6e 4964 2729 0a20 2020  ('RegionId').   
-00010270: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-00010280: 6573 6f75 7263 6547 726f 7570 4964 2729  esourceGroupId')
-00010290: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000102a0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000102b0: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-000102c0: 203d 206d 2e67 6574 2827 5265 736f 7572   = m.get('Resour
-000102d0: 6365 4772 6f75 7049 6427 290a 2020 2020  ceGroupId').    
-000102e0: 2020 2020 6966 206d 2e67 6574 2827 5365      if m.get('Se
-000102f0: 6375 7269 7479 4772 6f75 7049 6427 2920  curityGroupId') 
-00010300: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00010310: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00010320: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
-00010330: 3d20 6d2e 6765 7428 2753 6563 7572 6974  = m.get('Securit
-00010340: 7947 726f 7570 4964 2729 0a20 2020 2020  yGroupId').     
-00010350: 2020 2069 6620 6d2e 6765 7428 2753 7461     if m.get('Sta
-00010360: 7274 5469 6d65 2729 2069 7320 6e6f 7420  rtTime') is not 
-00010370: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00010380: 2020 7365 6c66 2e73 7461 7274 5f74 696d    self.start_tim
-00010390: 6520 3d20 6d2e 6765 7428 2753 7461 7274  e = m.get('Start
-000103a0: 5469 6d65 2729 0a20 2020 2020 2020 2069  Time').        i
-000103b0: 6620 6d2e 6765 7428 2753 7461 7475 7327  f m.get('Status'
-000103c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000103d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000103e0: 7374 6174 7573 203d 206d 2e67 6574 2827  status = m.get('
-000103f0: 5374 6174 7573 2729 0a20 2020 2020 2020  Status').       
-00010400: 2069 6620 6d2e 6765 7428 2754 6167 7327   if m.get('Tags'
-00010410: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00010420: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-00010430: 6d6f 6465 6c20 3d20 4465 7363 7269 6265  model = Describe
-00010440: 4561 6973 5265 7370 6f6e 7365 426f 6479  EaisResponseBody
-00010450: 496e 7374 616e 6365 7349 6e73 7461 6e63  InstancesInstanc
-00010460: 6554 6167 7328 290a 2020 2020 2020 2020  eTags().        
-00010470: 2020 2020 7365 6c66 2e74 6167 7320 3d20      self.tags = 
-00010480: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-00010490: 6d61 7028 6d5b 2754 6167 7327 5d29 0a20  map(m['Tags']). 
-000104a0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000104b0: 2756 5377 6974 6368 4964 2729 2069 7320  'VSwitchId') is 
-000104c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000104d0: 2020 2020 2020 7365 6c66 2e76 5f73 7769        self.v_swi
-000104e0: 7463 685f 6964 203d 206d 2e67 6574 2827  tch_id = m.get('
-000104f0: 5653 7769 7463 6849 6427 290a 2020 2020  VSwitchId').    
-00010500: 2020 2020 6966 206d 2e67 6574 2827 5a6f      if m.get('Zo
-00010510: 6e65 4964 2729 2069 7320 6e6f 7420 4e6f  neId') is not No
-00010520: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00010530: 7365 6c66 2e7a 6f6e 655f 6964 203d 206d  self.zone_id = m
-00010540: 2e67 6574 2827 5a6f 6e65 4964 2729 0a20  .get('ZoneId'). 
-00010550: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00010560: 6c66 0a0a 0a63 6c61 7373 2044 6573 6372  lf...class Descr
-00010570: 6962 6545 6169 7352 6573 706f 6e73 6542  ibeEaisResponseB
-00010580: 6f64 7949 6e73 7461 6e63 6573 2854 6561  odyInstances(Tea
-00010590: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-000105a0: 5f5f 696e 6974 5f5f 2873 656c 662c 2069  __init__(self, i
-000105b0: 6e73 7461 6e63 653d 4e6f 6e65 293a 0a20  nstance=None):. 
-000105c0: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
-000105d0: 616e 6365 203d 2069 6e73 7461 6e63 6520  ance = instance 
-000105e0: 2023 2074 7970 653a 206c 6973 745b 4465   # type: list[De
-000105f0: 7363 7269 6265 4561 6973 5265 7370 6f6e  scribeEaisRespon
-00010600: 7365 426f 6479 496e 7374 616e 6365 7349  seBodyInstancesI
-00010610: 6e73 7461 6e63 655d 0a0a 2020 2020 6465  nstance]..    de
-00010620: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00010630: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00010640: 662e 696e 7374 616e 6365 3a0a 2020 2020  f.instance:.    
-00010650: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00010660: 2073 656c 662e 696e 7374 616e 6365 3a0a   self.instance:.
-00010670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010680: 6966 206b 3a0a 2020 2020 2020 2020 2020  if k:.          
-00010690: 2020 2020 2020 2020 2020 6b2e 7661 6c69            k.vali
-000106a0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-000106b0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-000106c0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-000106d0: 6572 2844 6573 6372 6962 6545 6169 7352  er(DescribeEaisR
-000106e0: 6573 706f 6e73 6542 6f64 7949 6e73 7461  esponseBodyInsta
-000106f0: 6e63 6573 2c20 7365 6c66 292e 746f 5f6d  nces, self).to_m
-00010700: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00010710: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00010720: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00010730: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00010740: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00010750: 2829 0a20 2020 2020 2020 2072 6573 756c  ().        resul
-00010760: 745b 2749 6e73 7461 6e63 6527 5d20 3d20  t['Instance'] = 
-00010770: 5b5d 0a20 2020 2020 2020 2069 6620 7365  [].        if se
-00010780: 6c66 2e69 6e73 7461 6e63 6520 6973 206e  lf.instance is n
-00010790: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000107a0: 2020 2020 2066 6f72 206b 2069 6e20 7365       for k in se
-000107b0: 6c66 2e69 6e73 7461 6e63 653a 0a20 2020  lf.instance:.   
-000107c0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-000107d0: 756c 745b 2749 6e73 7461 6e63 6527 5d2e  ult['Instance'].
-000107e0: 6170 7065 6e64 286b 2e74 6f5f 6d61 7028  append(k.to_map(
-000107f0: 2920 6966 206b 2065 6c73 6520 4e6f 6e65  ) if k else None
-00010800: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00010810: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-00010820: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-00010830: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
-00010840: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00010850: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00010860: 7374 616e 6365 203d 205b 5d0a 2020 2020  stance = [].    
-00010870: 2020 2020 6966 206d 2e67 6574 2827 496e      if m.get('In
-00010880: 7374 616e 6365 2729 2069 7320 6e6f 7420  stance') is not 
-00010890: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000108a0: 2020 666f 7220 6b20 696e 206d 2e67 6574    for k in m.get
-000108b0: 2827 496e 7374 616e 6365 2729 3a0a 2020  ('Instance'):.  
-000108c0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-000108d0: 6d70 5f6d 6f64 656c 203d 2044 6573 6372  mp_model = Descr
-000108e0: 6962 6545 6169 7352 6573 706f 6e73 6542  ibeEaisResponseB
-000108f0: 6f64 7949 6e73 7461 6e63 6573 496e 7374  odyInstancesInst
-00010900: 616e 6365 2829 0a20 2020 2020 2020 2020  ance().         
-00010910: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
-00010920: 616e 6365 2e61 7070 656e 6428 7465 6d70  ance.append(temp
-00010930: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-00010940: 6b29 290a 2020 2020 2020 2020 7265 7475  k)).        retu
-00010950: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00010960: 4465 7363 7269 6265 4561 6973 5265 7370  DescribeEaisResp
-00010970: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
-00010980: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00010990: 6974 5f5f 2873 656c 662c 2069 6e73 7461  it__(self, insta
-000109a0: 6e63 6573 3d4e 6f6e 652c 2070 6167 655f  nces=None, page_
-000109b0: 6e75 6d62 6572 3d4e 6f6e 652c 2070 6167  number=None, pag
-000109c0: 655f 7369 7a65 3d4e 6f6e 652c 2072 6571  e_size=None, req
-000109d0: 7565 7374 5f69 643d 4e6f 6e65 2c20 746f  uest_id=None, to
-000109e0: 7461 6c5f 636f 756e 743d 4e6f 6e65 293a  tal_count=None):
-000109f0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00010a00: 7374 616e 6365 7320 3d20 696e 7374 616e  stances = instan
-00010a10: 6365 7320 2023 2074 7970 653a 2044 6573  ces  # type: Des
-00010a20: 6372 6962 6545 6169 7352 6573 706f 6e73  cribeEaisRespons
-00010a30: 6542 6f64 7949 6e73 7461 6e63 6573 0a20  eBodyInstances. 
-00010a40: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
-00010a50: 5f6e 756d 6265 7220 3d20 7061 6765 5f6e  _number = page_n
-00010a60: 756d 6265 7220 2023 2074 7970 653a 2069  umber  # type: i
-00010a70: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
-00010a80: 7061 6765 5f73 697a 6520 3d20 7061 6765  page_size = page
-00010a90: 5f73 697a 6520 2023 2074 7970 653a 2069  _size  # type: i
-00010aa0: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
-00010ab0: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
-00010ac0: 7565 7374 5f69 6420 2023 2074 7970 653a  uest_id  # type:
-00010ad0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
-00010ae0: 662e 746f 7461 6c5f 636f 756e 7420 3d20  f.total_count = 
-00010af0: 746f 7461 6c5f 636f 756e 7420 2023 2074  total_count  # t
-00010b00: 7970 653a 2069 6e74 0a0a 2020 2020 6465  ype: int..    de
-00010b10: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00010b20: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00010b30: 662e 696e 7374 616e 6365 733a 0a20 2020  f.instances:.   
-00010b40: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
-00010b50: 7374 616e 6365 732e 7661 6c69 6461 7465  stances.validate
-00010b60: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-00010b70: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-00010b80: 2020 5f6d 6170 203d 2073 7570 6572 2844    _map = super(D
-00010b90: 6573 6372 6962 6545 6169 7352 6573 706f  escribeEaisRespo
-00010ba0: 6e73 6542 6f64 792c 2073 656c 6629 2e74  nseBody, self).t
-00010bb0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00010bc0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00010bd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00010be0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-00010bf0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-00010c00: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00010c10: 2073 656c 662e 696e 7374 616e 6365 7320   self.instances 
-00010c20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00010c30: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00010c40: 2749 6e73 7461 6e63 6573 275d 203d 2073  'Instances'] = s
-00010c50: 656c 662e 696e 7374 616e 6365 732e 746f  elf.instances.to
-00010c60: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-00010c70: 6620 7365 6c66 2e70 6167 655f 6e75 6d62  f self.page_numb
-00010c80: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00010c90: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00010ca0: 6c74 5b27 5061 6765 4e75 6d62 6572 275d  lt['PageNumber']
-00010cb0: 203d 2073 656c 662e 7061 6765 5f6e 756d   = self.page_num
-00010cc0: 6265 720a 2020 2020 2020 2020 6966 2073  ber.        if s
-00010cd0: 656c 662e 7061 6765 5f73 697a 6520 6973  elf.page_size is
-00010ce0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00010cf0: 2020 2020 2020 2072 6573 756c 745b 2750         result['P
-00010d00: 6167 6553 697a 6527 5d20 3d20 7365 6c66  ageSize'] = self
-00010d10: 2e70 6167 655f 7369 7a65 0a20 2020 2020  .page_size.     
-00010d20: 2020 2069 6620 7365 6c66 2e72 6571 7565     if self.reque
-00010d30: 7374 5f69 6420 6973 206e 6f74 204e 6f6e  st_id is not Non
-00010d40: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00010d50: 6573 756c 745b 2752 6571 7565 7374 4964  esult['RequestId
-00010d60: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
-00010d70: 745f 6964 0a20 2020 2020 2020 2069 6620  t_id.        if 
-00010d80: 7365 6c66 2e74 6f74 616c 5f63 6f75 6e74  self.total_count
-00010d90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00010da0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00010db0: 5b27 546f 7461 6c43 6f75 6e74 275d 203d  ['TotalCount'] =
-00010dc0: 2073 656c 662e 746f 7461 6c5f 636f 756e   self.total_coun
-00010dd0: 740a 2020 2020 2020 2020 7265 7475 726e  t.        return
-00010de0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-00010df0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-00010e00: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
-00010e10: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00010e20: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00010e30: 7428 2749 6e73 7461 6e63 6573 2729 2069  t('Instances') i
-00010e40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00010e50: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-00010e60: 656c 203d 2044 6573 6372 6962 6545 6169  el = DescribeEai
-00010e70: 7352 6573 706f 6e73 6542 6f64 7949 6e73  sResponseBodyIns
-00010e80: 7461 6e63 6573 2829 0a20 2020 2020 2020  tances().       
-00010e90: 2020 2020 2073 656c 662e 696e 7374 616e       self.instan
-00010ea0: 6365 7320 3d20 7465 6d70 5f6d 6f64 656c  ces = temp_model
-00010eb0: 2e66 726f 6d5f 6d61 7028 6d5b 2749 6e73  .from_map(m['Ins
-00010ec0: 7461 6e63 6573 275d 290a 2020 2020 2020  tances']).      
-00010ed0: 2020 6966 206d 2e67 6574 2827 5061 6765    if m.get('Page
-00010ee0: 4e75 6d62 6572 2729 2069 7320 6e6f 7420  Number') is not 
-00010ef0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00010f00: 2020 7365 6c66 2e70 6167 655f 6e75 6d62    self.page_numb
-00010f10: 6572 203d 206d 2e67 6574 2827 5061 6765  er = m.get('Page
-00010f20: 4e75 6d62 6572 2729 0a20 2020 2020 2020  Number').       
-00010f30: 2069 6620 6d2e 6765 7428 2750 6167 6553   if m.get('PageS
-00010f40: 697a 6527 2920 6973 206e 6f74 204e 6f6e  ize') is not Non
-00010f50: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00010f60: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
-00010f70: 6d2e 6765 7428 2750 6167 6553 697a 6527  m.get('PageSize'
-00010f80: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00010f90: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
-00010fa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00010fb0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00010fc0: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
-00010fd0: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
-00010fe0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00010ff0: 546f 7461 6c43 6f75 6e74 2729 2069 7320  TotalCount') is 
-00011000: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00011010: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
-00011020: 5f63 6f75 6e74 203d 206d 2e67 6574 2827  _count = m.get('
-00011030: 546f 7461 6c43 6f75 6e74 2729 0a20 2020  TotalCount').   
-00011040: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00011050: 0a0a 0a63 6c61 7373 2044 6573 6372 6962  ...class Describ
-00011060: 6545 6169 7352 6573 706f 6e73 6528 5465  eEaisResponse(Te
-00011070: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00011080: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00011090: 6865 6164 6572 733d 4e6f 6e65 2c20 7374  headers=None, st
-000110a0: 6174 7573 5f63 6f64 653d 4e6f 6e65 2c20  atus_code=None, 
-000110b0: 626f 6479 3d4e 6f6e 6529 3a0a 2020 2020  body=None):.    
-000110c0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-000110d0: 203d 2068 6561 6465 7273 2020 2320 7479   = headers  # ty
-000110e0: 7065 3a20 6469 6374 5b73 7472 2c20 7374  pe: dict[str, st
-000110f0: 725d 0a20 2020 2020 2020 2073 656c 662e  r].        self.
-00011100: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
-00011110: 6174 7573 5f63 6f64 6520 2023 2074 7970  atus_code  # typ
-00011120: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
-00011130: 656c 662e 626f 6479 203d 2062 6f64 7920  elf.body = body 
-00011140: 2023 2074 7970 653a 2044 6573 6372 6962   # type: Describ
-00011150: 6545 6169 7352 6573 706f 6e73 6542 6f64  eEaisResponseBod
-00011160: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-00011170: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00011180: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-00011190: 5f72 6571 7569 7265 6428 7365 6c66 2e68  _required(self.h
-000111a0: 6561 6465 7273 2c20 2768 6561 6465 7273  eaders, 'headers
-000111b0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-000111c0: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-000111d0: 6428 7365 6c66 2e73 7461 7475 735f 636f  d(self.status_co
-000111e0: 6465 2c20 2773 7461 7475 735f 636f 6465  de, 'status_code
-000111f0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00011200: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-00011210: 6428 7365 6c66 2e62 6f64 792c 2027 626f  d(self.body, 'bo
-00011220: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
-00011230: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-00011240: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00011250: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-00011260: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-00011270: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-00011280: 3d20 7375 7065 7228 4465 7363 7269 6265  = super(Describe
-00011290: 4561 6973 5265 7370 6f6e 7365 2c20 7365  EaisResponse, se
-000112a0: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
-000112b0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-000112c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000112d0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-000112e0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-000112f0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00011300: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-00011310: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-00011320: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00011330: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-00011340: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-00011350: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00011360: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-00011370: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00011380: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-00011390: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-000113a0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-000113b0: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-000113c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000113d0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000113e0: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-000113f0: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-00011400: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00011410: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00011420: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-00011430: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00011440: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00011450: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-00011460: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-00011470: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00011480: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-00011490: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-000114a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000114b0: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-000114c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000114d0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-000114e0: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-000114f0: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-00011500: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00011510: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-00011520: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00011530: 2074 656d 705f 6d6f 6465 6c20 3d20 4465   temp_model = De
-00011540: 7363 7269 6265 4561 6973 5265 7370 6f6e  scribeEaisRespon
-00011550: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
-00011560: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-00011570: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-00011580: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-00011590: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000115a0: 656c 660a 0a0a 636c 6173 7320 4465 7363  elf...class Desc
-000115b0: 7269 6265 5265 6769 6f6e 7352 6573 706f  ribeRegionsRespo
-000115c0: 6e73 6542 6f64 7952 6567 696f 6e73 5265  nseBodyRegionsRe
-000115d0: 6769 6f6e 2854 6561 4d6f 6465 6c29 3a0a  gion(TeaModel):.
-000115e0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000115f0: 2873 656c 662c 206c 6f63 616c 5f6e 616d  (self, local_nam
-00011600: 653d 4e6f 6e65 2c20 7265 6769 6f6e 5f65  e=None, region_e
-00011610: 6e64 706f 696e 743d 4e6f 6e65 2c20 7265  ndpoint=None, re
-00011620: 6769 6f6e 5f69 643d 4e6f 6e65 293a 0a20  gion_id=None):. 
-00011630: 2020 2020 2020 2073 656c 662e 6c6f 6361         self.loca
-00011640: 6c5f 6e61 6d65 203d 206c 6f63 616c 5f6e  l_name = local_n
-00011650: 616d 6520 2023 2074 7970 653a 2073 7472  ame  # type: str
-00011660: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00011670: 6769 6f6e 5f65 6e64 706f 696e 7420 3d20  gion_endpoint = 
-00011680: 7265 6769 6f6e 5f65 6e64 706f 696e 7420  region_endpoint 
-00011690: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-000116a0: 2020 2020 2073 656c 662e 7265 6769 6f6e       self.region
-000116b0: 5f69 6420 3d20 7265 6769 6f6e 5f69 6420  _id = region_id 
-000116c0: 2023 2074 7970 653a 2073 7472 0a0a 2020   # type: str..  
-000116d0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-000116e0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-000116f0: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-00011700: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-00011710: 2020 5f6d 6170 203d 2073 7570 6572 2844    _map = super(D
-00011720: 6573 6372 6962 6552 6567 696f 6e73 5265  escribeRegionsRe
-00011730: 7370 6f6e 7365 426f 6479 5265 6769 6f6e  sponseBodyRegion
-00011740: 7352 6567 696f 6e2c 2073 656c 6629 2e74  sRegion, self).t
-00011750: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00011760: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00011770: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00011780: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-00011790: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000117a0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000117b0: 2073 656c 662e 6c6f 6361 6c5f 6e61 6d65   self.local_name
-000117c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000117d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000117e0: 5b27 4c6f 6361 6c4e 616d 6527 5d20 3d20  ['LocalName'] = 
-000117f0: 7365 6c66 2e6c 6f63 616c 5f6e 616d 650a  self.local_name.
-00011800: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00011810: 7265 6769 6f6e 5f65 6e64 706f 696e 7420  region_endpoint 
-00011820: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00011830: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00011840: 2752 6567 696f 6e45 6e64 706f 696e 7427  'RegionEndpoint'
-00011850: 5d20 3d20 7365 6c66 2e72 6567 696f 6e5f  ] = self.region_
-00011860: 656e 6470 6f69 6e74 0a20 2020 2020 2020  endpoint.       
-00011870: 2069 6620 7365 6c66 2e72 6567 696f 6e5f   if self.region_
-00011880: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00011890: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000118a0: 6c74 5b27 5265 6769 6f6e 4964 275d 203d  lt['RegionId'] =
-000118b0: 2073 656c 662e 7265 6769 6f6e 5f69 640a   self.region_id.
-000118c0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000118d0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-000118e0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
-000118f0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00011900: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00011910: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00011920: 274c 6f63 616c 4e61 6d65 2729 2069 7320  'LocalName') is 
-00011930: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00011940: 2020 2020 2020 7365 6c66 2e6c 6f63 616c        self.local
-00011950: 5f6e 616d 6520 3d20 6d2e 6765 7428 274c  _name = m.get('L
-00011960: 6f63 616c 4e61 6d65 2729 0a20 2020 2020  ocalName').     
-00011970: 2020 2069 6620 6d2e 6765 7428 2752 6567     if m.get('Reg
-00011980: 696f 6e45 6e64 706f 696e 7427 2920 6973  ionEndpoint') is
-00011990: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000119a0: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
-000119b0: 6f6e 5f65 6e64 706f 696e 7420 3d20 6d2e  on_endpoint = m.
-000119c0: 6765 7428 2752 6567 696f 6e45 6e64 706f  get('RegionEndpo
-000119d0: 696e 7427 290a 2020 2020 2020 2020 6966  int').        if
-000119e0: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
-000119f0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00011a00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011a10: 2e72 6567 696f 6e5f 6964 203d 206d 2e67  .region_id = m.g
-00011a20: 6574 2827 5265 6769 6f6e 4964 2729 0a20  et('RegionId'). 
-00011a30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00011a40: 6c66 0a0a 0a63 6c61 7373 2044 6573 6372  lf...class Descr
-00011a50: 6962 6552 6567 696f 6e73 5265 7370 6f6e  ibeRegionsRespon
-00011a60: 7365 426f 6479 5265 6769 6f6e 7328 5465  seBodyRegions(Te
-00011a70: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00011a80: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00011a90: 7265 6769 6f6e 3d4e 6f6e 6529 3a0a 2020  region=None):.  
-00011aa0: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-00011ab0: 6e20 3d20 7265 6769 6f6e 2020 2320 7479  n = region  # ty
-00011ac0: 7065 3a20 6c69 7374 5b44 6573 6372 6962  pe: list[Describ
-00011ad0: 6552 6567 696f 6e73 5265 7370 6f6e 7365  eRegionsResponse
-00011ae0: 426f 6479 5265 6769 6f6e 7352 6567 696f  BodyRegionsRegio
-00011af0: 6e5d 0a0a 2020 2020 6465 6620 7661 6c69  n]..    def vali
-00011b00: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00011b10: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
-00011b20: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-00011b30: 666f 7220 6b20 696e 2073 656c 662e 7265  for k in self.re
-00011b40: 6769 6f6e 3a0a 2020 2020 2020 2020 2020  gion:.          
-00011b50: 2020 2020 2020 6966 206b 3a0a 2020 2020        if k:.    
-00011b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b70: 6b2e 7661 6c69 6461 7465 2829 0a0a 2020  k.validate()..  
-00011b80: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00011b90: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00011ba0: 203d 2073 7570 6572 2844 6573 6372 6962   = super(Describ
-00011bb0: 6552 6567 696f 6e73 5265 7370 6f6e 7365  eRegionsResponse
-00011bc0: 426f 6479 5265 6769 6f6e 732c 2073 656c  BodyRegions, sel
-00011bd0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-00011be0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00011bf0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00011c00: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00011c10: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00011c20: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00011c30: 2020 7265 7375 6c74 5b27 5265 6769 6f6e    result['Region
-00011c40: 275d 203d 205b 5d0a 2020 2020 2020 2020  '] = [].        
-00011c50: 6966 2073 656c 662e 7265 6769 6f6e 2069  if self.region i
-00011c60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00011c70: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00011c80: 2073 656c 662e 7265 6769 6f6e 3a0a 2020   self.region:.  
-00011c90: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00011ca0: 7375 6c74 5b27 5265 6769 6f6e 275d 2e61  sult['Region'].a
-00011cb0: 7070 656e 6428 6b2e 746f 5f6d 6170 2829  ppend(k.to_map()
-00011cc0: 2069 6620 6b20 656c 7365 204e 6f6e 6529   if k else None)
-00011cd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011ce0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-00011cf0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-00011d00: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00011d10: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00011d20: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
-00011d30: 696f 6e20 3d20 5b5d 0a20 2020 2020 2020  ion = [].       
-00011d40: 2069 6620 6d2e 6765 7428 2752 6567 696f   if m.get('Regio
-00011d50: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
-00011d60: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00011d70: 206b 2069 6e20 6d2e 6765 7428 2752 6567   k in m.get('Reg
-00011d80: 696f 6e27 293a 0a20 2020 2020 2020 2020  ion'):.         
-00011d90: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-00011da0: 6c20 3d20 4465 7363 7269 6265 5265 6769  l = DescribeRegi
-00011db0: 6f6e 7352 6573 706f 6e73 6542 6f64 7952  onsResponseBodyR
-00011dc0: 6567 696f 6e73 5265 6769 6f6e 2829 0a20  egionsRegion(). 
-00011dd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011de0: 656c 662e 7265 6769 6f6e 2e61 7070 656e  elf.region.appen
-00011df0: 6428 7465 6d70 5f6d 6f64 656c 2e66 726f  d(temp_model.fro
-00011e00: 6d5f 6d61 7028 6b29 290a 2020 2020 2020  m_map(k)).      
-00011e10: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00011e20: 636c 6173 7320 4465 7363 7269 6265 5265  class DescribeRe
-00011e30: 6769 6f6e 7352 6573 706f 6e73 6542 6f64  gionsResponseBod
-00011e40: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
-00011e50: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00011e60: 6c66 2c20 7265 6769 6f6e 733d 4e6f 6e65  lf, regions=None
-00011e70: 2c20 7265 7175 6573 745f 6964 3d4e 6f6e  , request_id=Non
-00011e80: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-00011e90: 2e72 6567 696f 6e73 203d 2072 6567 696f  .regions = regio
-00011ea0: 6e73 2020 2320 7479 7065 3a20 4465 7363  ns  # type: Desc
-00011eb0: 7269 6265 5265 6769 6f6e 7352 6573 706f  ribeRegionsRespo
-00011ec0: 6e73 6542 6f64 7952 6567 696f 6e73 0a20  nseBodyRegions. 
-00011ed0: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
-00011ee0: 6573 745f 6964 203d 2072 6571 7565 7374  est_id = request
-00011ef0: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
-00011f00: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00011f10: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00011f20: 2020 6966 2073 656c 662e 7265 6769 6f6e    if self.region
-00011f30: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00011f40: 656c 662e 7265 6769 6f6e 732e 7661 6c69  elf.regions.vali
-00011f50: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-00011f60: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00011f70: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00011f80: 6572 2844 6573 6372 6962 6552 6567 696f  er(DescribeRegio
-00011f90: 6e73 5265 7370 6f6e 7365 426f 6479 2c20  nsResponseBody, 
-00011fa0: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
-00011fb0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00011fc0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00011fd0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00011fe0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00011ff0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00012000: 2020 2020 2069 6620 7365 6c66 2e72 6567       if self.reg
-00012010: 696f 6e73 2069 7320 6e6f 7420 4e6f 6e65  ions is not None
-00012020: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00012030: 7375 6c74 5b27 5265 6769 6f6e 7327 5d20  sult['Regions'] 
-00012040: 3d20 7365 6c66 2e72 6567 696f 6e73 2e74  = self.regions.t
-00012050: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00012060: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
-00012070: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00012080: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00012090: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
-000120a0: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
-000120b0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
-000120c0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-000120d0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-000120e0: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
-000120f0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00012100: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00012110: 7428 2752 6567 696f 6e73 2729 2069 7320  t('Regions') is 
-00012120: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00012130: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-00012140: 203d 2044 6573 6372 6962 6552 6567 696f   = DescribeRegio
-00012150: 6e73 5265 7370 6f6e 7365 426f 6479 5265  nsResponseBodyRe
-00012160: 6769 6f6e 7328 290a 2020 2020 2020 2020  gions().        
-00012170: 2020 2020 7365 6c66 2e72 6567 696f 6e73      self.regions
-00012180: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-00012190: 6f6d 5f6d 6170 286d 5b27 5265 6769 6f6e  om_map(m['Region
-000121a0: 7327 5d29 0a20 2020 2020 2020 2069 6620  s']).        if 
-000121b0: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-000121c0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000121d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000121e0: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
-000121f0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-00012200: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012210: 7365 6c66 0a0a 0a63 6c61 7373 2044 6573  self...class Des
-00012220: 6372 6962 6552 6567 696f 6e73 5265 7370  cribeRegionsResp
-00012230: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-00012240: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00012250: 2873 656c 662c 2068 6561 6465 7273 3d4e  (self, headers=N
-00012260: 6f6e 652c 2073 7461 7475 735f 636f 6465  one, status_code
-00012270: 3d4e 6f6e 652c 2062 6f64 793d 4e6f 6e65  =None, body=None
-00012280: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00012290: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-000122a0: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
-000122b0: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
-000122c0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-000122d0: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-000122e0: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
-000122f0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-00012300: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
-00012310: 4465 7363 7269 6265 5265 6769 6f6e 7352  DescribeRegionsR
-00012320: 6573 706f 6e73 6542 6f64 790a 0a20 2020  esponseBody..   
-00012330: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00012340: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00012350: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00012360: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
-00012370: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
-00012380: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00012390: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-000123a0: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
-000123b0: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
-000123c0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-000123d0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-000123e0: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
-000123f0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00012400: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-00012410: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-00012420: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-00012430: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00012440: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00012450: 7228 4465 7363 7269 6265 5265 6769 6f6e  r(DescribeRegion
-00012460: 7352 6573 706f 6e73 652c 2073 656c 6629  sResponse, self)
-00012470: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00012480: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-00012490: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000124a0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-000124b0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-000124c0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000124d0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-000124e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000124f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00012500: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-00012510: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-00012520: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-00012530: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-00012540: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00012550: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-00012560: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-00012570: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-00012580: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-00012590: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000125a0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-000125b0: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-000125c0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000125d0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000125e0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000125f0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-00012600: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00012610: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00012620: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
-00012630: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-00012640: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012650: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
-00012660: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
-00012670: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
-00012680: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
-00012690: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000126a0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-000126b0: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
-000126c0: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
-000126d0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-000126e0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-000126f0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-00012700: 6d70 5f6d 6f64 656c 203d 2044 6573 6372  mp_model = Descr
-00012710: 6962 6552 6567 696f 6e73 5265 7370 6f6e  ibeRegionsRespon
-00012720: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
-00012730: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-00012740: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-00012750: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-00012760: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00012770: 656c 660a 0a0a 636c 6173 7320 4465 7461  elf...class Deta
-00012780: 6368 4561 6952 6571 7565 7374 2854 6561  chEaiRequest(Tea
-00012790: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-000127a0: 5f5f 696e 6974 5f5f 2873 656c 662c 2065  __init__(self, e
-000127b0: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
-000127c0: 6564 5f69 6e73 7461 6e63 655f 6964 3d4e  ed_instance_id=N
-000127d0: 6f6e 652c 2072 6567 696f 6e5f 6964 3d4e  one, region_id=N
-000127e0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-000127f0: 6c66 2e65 6c61 7374 6963 5f61 6363 656c  lf.elastic_accel
-00012800: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
-00012810: 6964 203d 2065 6c61 7374 6963 5f61 6363  id = elastic_acc
-00012820: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
-00012830: 655f 6964 2020 2320 7479 7065 3a20 7374  e_id  # type: st
-00012840: 720a 2020 2020 2020 2020 7365 6c66 2e72  r.        self.r
-00012850: 6567 696f 6e5f 6964 203d 2072 6567 696f  egion_id = regio
-00012860: 6e5f 6964 2020 2320 7479 7065 3a20 7374  n_id  # type: st
-00012870: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
-00012880: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00012890: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-000128a0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-000128b0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-000128c0: 7065 7228 4465 7461 6368 4561 6952 6571  per(DetachEaiReq
-000128d0: 7565 7374 2c20 7365 6c66 292e 746f 5f6d  uest, self).to_m
-000128e0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-000128f0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00012900: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00012910: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00012920: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00012930: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00012940: 6c66 2e65 6c61 7374 6963 5f61 6363 656c  lf.elastic_accel
-00012950: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
-00012960: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00012970: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00012980: 6c74 5b27 456c 6173 7469 6341 6363 656c  lt['ElasticAccel
-00012990: 6572 6174 6564 496e 7374 616e 6365 4964  eratedInstanceId
-000129a0: 275d 203d 2073 656c 662e 656c 6173 7469  '] = self.elasti
-000129b0: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
-000129c0: 7374 616e 6365 5f69 640a 2020 2020 2020  stance_id.      
-000129d0: 2020 6966 2073 656c 662e 7265 6769 6f6e    if self.region
-000129e0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-000129f0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00012a00: 756c 745b 2752 6567 696f 6e49 6427 5d20  ult['RegionId'] 
-00012a10: 3d20 7365 6c66 2e72 6567 696f 6e5f 6964  = self.region_id
-00012a20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012a30: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-00012a40: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-00012a50: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-00012a60: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00012a70: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00012a80: 2827 456c 6173 7469 6341 6363 656c 6572  ('ElasticAcceler
-00012a90: 6174 6564 496e 7374 616e 6365 4964 2729  atedInstanceId')
-00012aa0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00012ab0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-00012ac0: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
-00012ad0: 6564 5f69 6e73 7461 6e63 655f 6964 203d  ed_instance_id =
-00012ae0: 206d 2e67 6574 2827 456c 6173 7469 6341   m.get('ElasticA
-00012af0: 6363 656c 6572 6174 6564 496e 7374 616e  cceleratedInstan
-00012b00: 6365 4964 2729 0a20 2020 2020 2020 2069  ceId').        i
-00012b10: 6620 6d2e 6765 7428 2752 6567 696f 6e49  f m.get('RegionI
-00012b20: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00012b30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012b40: 662e 7265 6769 6f6e 5f69 6420 3d20 6d2e  f.region_id = m.
-00012b50: 6765 7428 2752 6567 696f 6e49 6427 290a  get('RegionId').
-00012b60: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00012b70: 656c 660a 0a0a 636c 6173 7320 4465 7461  elf...class Deta
-00012b80: 6368 4561 6952 6573 706f 6e73 6542 6f64  chEaiResponseBod
-00012b90: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
-00012ba0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00012bb0: 6c66 2c20 7265 7175 6573 745f 6964 3d4e  lf, request_id=N
-00012bc0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-00012bd0: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-00012be0: 7265 7175 6573 745f 6964 2020 2320 7479  request_id  # ty
-00012bf0: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
-00012c00: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-00012c10: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00012c20: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00012c30: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00012c40: 7020 3d20 7375 7065 7228 4465 7461 6368  p = super(Detach
-00012c50: 4561 6952 6573 706f 6e73 6542 6f64 792c  EaiResponseBody,
-00012c60: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-00012c70: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00012c80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00012c90: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00012ca0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00012cb0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00012cc0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-00012cd0: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
-00012ce0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00012cf0: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
-00012d00: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
-00012d10: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
-00012d20: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00012d30: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00012d40: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
-00012d50: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00012d60: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00012d70: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
-00012d80: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00012d90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012da0: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-00012db0: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-00012dc0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00012dd0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2044  n self...class D
-00012de0: 6574 6163 6845 6169 5265 7370 6f6e 7365  etachEaiResponse
-00012df0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00012e00: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00012e10: 662c 2068 6561 6465 7273 3d4e 6f6e 652c  f, headers=None,
-00012e20: 2073 7461 7475 735f 636f 6465 3d4e 6f6e   status_code=Non
-00012e30: 652c 2062 6f64 793d 4e6f 6e65 293a 0a20  e, body=None):. 
-00012e40: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-00012e50: 6572 7320 3d20 6865 6164 6572 7320 2023  ers = headers  #
-00012e60: 2074 7970 653a 2064 6963 745b 7374 722c   type: dict[str,
-00012e70: 2073 7472 5d0a 2020 2020 2020 2020 7365   str].        se
-00012e80: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-00012e90: 2073 7461 7475 735f 636f 6465 2020 2320   status_code  # 
-00012ea0: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
-00012eb0: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-00012ec0: 6479 2020 2320 7479 7065 3a20 4465 7461  dy  # type: Deta
-00012ed0: 6368 4561 6952 6573 706f 6e73 6542 6f64  chEaiResponseBod
-00012ee0: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-00012ef0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00012f00: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-00012f10: 5f72 6571 7569 7265 6428 7365 6c66 2e68  _required(self.h
-00012f20: 6561 6465 7273 2c20 2768 6561 6465 7273  eaders, 'headers
-00012f30: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00012f40: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-00012f50: 6428 7365 6c66 2e73 7461 7475 735f 636f  d(self.status_co
-00012f60: 6465 2c20 2773 7461 7475 735f 636f 6465  de, 'status_code
-00012f70: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00012f80: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-00012f90: 6428 7365 6c66 2e62 6f64 792c 2027 626f  d(self.body, 'bo
-00012fa0: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
-00012fb0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-00012fc0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00012fd0: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-00012fe0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-00012ff0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-00013000: 3d20 7375 7065 7228 4465 7461 6368 4561  = super(DetachEa
-00013010: 6952 6573 706f 6e73 652c 2073 656c 6629  iResponse, self)
-00013020: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00013030: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-00013040: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00013050: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-00013060: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00013070: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00013080: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-00013090: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000130a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000130b0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-000130c0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-000130d0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-000130e0: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-000130f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00013100: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-00013110: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-00013120: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-00013130: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-00013140: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00013150: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-00013160: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-00013170: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00013180: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00013190: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000131a0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-000131b0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-000131c0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-000131d0: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
-000131e0: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-000131f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013200: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
-00013210: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
-00013220: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
-00013230: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
-00013240: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00013250: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00013260: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
-00013270: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
-00013280: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-00013290: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-000132a0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-000132b0: 6d70 5f6d 6f64 656c 203d 2044 6574 6163  mp_model = Detac
-000132c0: 6845 6169 5265 7370 6f6e 7365 426f 6479  hEaiResponseBody
-000132d0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-000132e0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-000132f0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-00013300: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-00013310: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00013320: 636c 6173 7320 4765 7449 6e73 7461 6e63  class GetInstanc
-00013330: 654d 6574 7269 6373 5265 7175 6573 7428  eMetricsRequest(
-00013340: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00013350: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00013360: 2c20 656e 645f 7469 6d65 3d4e 6f6e 652c  , end_time=None,
-00013370: 2069 6e73 7461 6e63 655f 6964 3d4e 6f6e   instance_id=Non
-00013380: 652c 206d 6574 7269 635f 7479 7065 3d4e  e, metric_type=N
-00013390: 6f6e 652c 2073 7461 7274 5f74 696d 653d  one, start_time=
-000133a0: 4e6f 6e65 2c20 7469 6d65 5f73 7465 703d  None, time_step=
-000133b0: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-000133c0: 656c 662e 656e 645f 7469 6d65 203d 2065  elf.end_time = e
-000133d0: 6e64 5f74 696d 6520 2023 2074 7970 653a  nd_time  # type:
-000133e0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
-000133f0: 662e 696e 7374 616e 6365 5f69 6420 3d20  f.instance_id = 
-00013400: 696e 7374 616e 6365 5f69 6420 2023 2074  instance_id  # t
-00013410: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
-00013420: 2073 656c 662e 6d65 7472 6963 5f74 7970   self.metric_typ
-00013430: 6520 3d20 6d65 7472 6963 5f74 7970 6520  e = metric_type 
-00013440: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-00013450: 2020 2020 2073 656c 662e 7374 6172 745f       self.start_
-00013460: 7469 6d65 203d 2073 7461 7274 5f74 696d  time = start_tim
-00013470: 6520 2023 2074 7970 653a 2073 7472 0a20  e  # type: str. 
-00013480: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
-00013490: 5f73 7465 7020 3d20 7469 6d65 5f73 7465  _step = time_ste
-000134a0: 7020 2023 2074 7970 653a 2073 7472 0a0a  p  # type: str..
-000134b0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-000134c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000134d0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-000134e0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-000134f0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00013500: 2847 6574 496e 7374 616e 6365 4d65 7472  (GetInstanceMetr
-00013510: 6963 7352 6571 7565 7374 2c20 7365 6c66  icsRequest, self
-00013520: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00013530: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00013540: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00013550: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00013560: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00013570: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00013580: 2069 6620 7365 6c66 2e65 6e64 5f74 696d   if self.end_tim
-00013590: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-000135a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000135b0: 745b 2745 6e64 5469 6d65 275d 203d 2073  t['EndTime'] = s
-000135c0: 656c 662e 656e 645f 7469 6d65 0a20 2020  elf.end_time.   
-000135d0: 2020 2020 2069 6620 7365 6c66 2e69 6e73       if self.ins
-000135e0: 7461 6e63 655f 6964 2069 7320 6e6f 7420  tance_id is not 
-000135f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00013600: 2020 7265 7375 6c74 5b27 496e 7374 616e    result['Instan
-00013610: 6365 4964 275d 203d 2073 656c 662e 696e  ceId'] = self.in
-00013620: 7374 616e 6365 5f69 640a 2020 2020 2020  stance_id.      
-00013630: 2020 6966 2073 656c 662e 6d65 7472 6963    if self.metric
-00013640: 5f74 7970 6520 6973 206e 6f74 204e 6f6e  _type is not Non
-00013650: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00013660: 6573 756c 745b 274d 6574 7269 6354 7970  esult['MetricTyp
-00013670: 6527 5d20 3d20 7365 6c66 2e6d 6574 7269  e'] = self.metri
-00013680: 635f 7479 7065 0a20 2020 2020 2020 2069  c_type.        i
-00013690: 6620 7365 6c66 2e73 7461 7274 5f74 696d  f self.start_tim
-000136a0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-000136b0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000136c0: 745b 2753 7461 7274 5469 6d65 275d 203d  t['StartTime'] =
-000136d0: 2073 656c 662e 7374 6172 745f 7469 6d65   self.start_time
-000136e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000136f0: 2e74 696d 655f 7374 6570 2069 7320 6e6f  .time_step is no
-00013700: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00013710: 2020 2020 7265 7375 6c74 5b27 5469 6d65      result['Time
-00013720: 5374 6570 275d 203d 2073 656c 662e 7469  Step'] = self.ti
-00013730: 6d65 5f73 7465 700a 2020 2020 2020 2020  me_step.        
-00013740: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00013750: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00013760: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
-00013770: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00013780: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00013790: 6620 6d2e 6765 7428 2745 6e64 5469 6d65  f m.get('EndTime
-000137a0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000137b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000137c0: 2e65 6e64 5f74 696d 6520 3d20 6d2e 6765  .end_time = m.ge
-000137d0: 7428 2745 6e64 5469 6d65 2729 0a20 2020  t('EndTime').   
-000137e0: 2020 2020 2069 6620 6d2e 6765 7428 2749       if m.get('I
-000137f0: 6e73 7461 6e63 6549 6427 2920 6973 206e  nstanceId') is n
-00013800: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00013810: 2020 2020 2073 656c 662e 696e 7374 616e       self.instan
-00013820: 6365 5f69 6420 3d20 6d2e 6765 7428 2749  ce_id = m.get('I
-00013830: 6e73 7461 6e63 6549 6427 290a 2020 2020  nstanceId').    
-00013840: 2020 2020 6966 206d 2e67 6574 2827 4d65      if m.get('Me
-00013850: 7472 6963 5479 7065 2729 2069 7320 6e6f  tricType') is no
-00013860: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00013870: 2020 2020 7365 6c66 2e6d 6574 7269 635f      self.metric_
-00013880: 7479 7065 203d 206d 2e67 6574 2827 4d65  type = m.get('Me
-00013890: 7472 6963 5479 7065 2729 0a20 2020 2020  tricType').     
-000138a0: 2020 2069 6620 6d2e 6765 7428 2753 7461     if m.get('Sta
-000138b0: 7274 5469 6d65 2729 2069 7320 6e6f 7420  rtTime') is not 
-000138c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000138d0: 2020 7365 6c66 2e73 7461 7274 5f74 696d    self.start_tim
-000138e0: 6520 3d20 6d2e 6765 7428 2753 7461 7274  e = m.get('Start
-000138f0: 5469 6d65 2729 0a20 2020 2020 2020 2069  Time').        i
-00013900: 6620 6d2e 6765 7428 2754 696d 6553 7465  f m.get('TimeSte
-00013910: 7027 2920 6973 206e 6f74 204e 6f6e 653a  p') is not None:
-00013920: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013930: 662e 7469 6d65 5f73 7465 7020 3d20 6d2e  f.time_step = m.
-00013940: 6765 7428 2754 696d 6553 7465 7027 290a  get('TimeStep').
-00013950: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00013960: 656c 660a 0a0a 636c 6173 7320 4765 7449  elf...class GetI
-00013970: 6e73 7461 6e63 654d 6574 7269 6373 5265  nstanceMetricsRe
-00013980: 7370 6f6e 7365 426f 6479 506f 644d 6574  sponseBodyPodMet
-00013990: 7269 6373 4d65 7472 6963 7328 5465 614d  ricsMetrics(TeaM
-000139a0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-000139b0: 5f69 6e69 745f 5f28 7365 6c66 2c20 7469  _init__(self, ti
-000139c0: 6d65 3d4e 6f6e 652c 2076 616c 7565 3d4e  me=None, value=N
-000139d0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-000139e0: 6c66 2e74 696d 6520 3d20 7469 6d65 2020  lf.time = time  
-000139f0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00013a00: 2020 2020 7365 6c66 2e76 616c 7565 203d      self.value =
-00013a10: 2076 616c 7565 2020 2320 7479 7065 3a20   value  # type: 
-00013a20: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
-00013a30: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00013a40: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00013a50: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00013a60: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00013a70: 7375 7065 7228 4765 7449 6e73 7461 6e63  super(GetInstanc
-00013a80: 654d 6574 7269 6373 5265 7370 6f6e 7365  eMetricsResponse
-00013a90: 426f 6479 506f 644d 6574 7269 6373 4d65  BodyPodMetricsMe
-00013aa0: 7472 6963 732c 2073 656c 6629 2e74 6f5f  trics, self).to_
-00013ab0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00013ac0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00013ad0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00013ae0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00013af0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00013b00: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00013b10: 656c 662e 7469 6d65 2069 7320 6e6f 7420  elf.time is not 
-00013b20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00013b30: 2020 7265 7375 6c74 5b27 5469 6d65 275d    result['Time']
-00013b40: 203d 2073 656c 662e 7469 6d65 0a20 2020   = self.time.   
-00013b50: 2020 2020 2069 6620 7365 6c66 2e76 616c       if self.val
-00013b60: 7565 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ue is not None:.
-00013b70: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00013b80: 6c74 5b27 5661 6c75 6527 5d20 3d20 7365  lt['Value'] = se
-00013b90: 6c66 2e76 616c 7565 0a20 2020 2020 2020  lf.value.       
-00013ba0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00013bb0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-00013bc0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-00013bd0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00013be0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00013bf0: 6966 206d 2e67 6574 2827 5469 6d65 2729  if m.get('Time')
-00013c00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00013c10: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00013c20: 696d 6520 3d20 6d2e 6765 7428 2754 696d  ime = m.get('Tim
-00013c30: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-00013c40: 2e67 6574 2827 5661 6c75 6527 2920 6973  .get('Value') is
-00013c50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00013c60: 2020 2020 2020 2073 656c 662e 7661 6c75         self.valu
-00013c70: 6520 3d20 6d2e 6765 7428 2756 616c 7565  e = m.get('Value
-00013c80: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00013c90: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2047  n self...class G
-00013ca0: 6574 496e 7374 616e 6365 4d65 7472 6963  etInstanceMetric
-00013cb0: 7352 6573 706f 6e73 6542 6f64 7950 6f64  sResponseBodyPod
-00013cc0: 4d65 7472 6963 7328 5465 614d 6f64 656c  Metrics(TeaModel
-00013cd0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00013ce0: 745f 5f28 7365 6c66 2c20 6d65 7472 6963  t__(self, metric
-00013cf0: 733d 4e6f 6e65 2c20 706f 645f 6964 3d4e  s=None, pod_id=N
-00013d00: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-00013d10: 6c66 2e6d 6574 7269 6373 203d 206d 6574  lf.metrics = met
-00013d20: 7269 6373 2020 2320 7479 7065 3a20 6c69  rics  # type: li
-00013d30: 7374 5b47 6574 496e 7374 616e 6365 4d65  st[GetInstanceMe
-00013d40: 7472 6963 7352 6573 706f 6e73 6542 6f64  tricsResponseBod
-00013d50: 7950 6f64 4d65 7472 6963 734d 6574 7269  yPodMetricsMetri
-00013d60: 6373 5d0a 2020 2020 2020 2020 2320 506f  cs].        # Po
-00013d70: 6420 4944 e380 820a 2020 2020 2020 2020  d ID....        
-00013d80: 7365 6c66 2e70 6f64 5f69 6420 3d20 706f  self.pod_id = po
-00013d90: 645f 6964 2020 2320 7479 7065 3a20 7374  d_id  # type: st
-00013da0: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
-00013db0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00013dc0: 2020 2069 6620 7365 6c66 2e6d 6574 7269     if self.metri
-00013dd0: 6373 3a0a 2020 2020 2020 2020 2020 2020  cs:.            
-00013de0: 666f 7220 6b20 696e 2073 656c 662e 6d65  for k in self.me
-00013df0: 7472 6963 733a 0a20 2020 2020 2020 2020  trics:.         
-00013e00: 2020 2020 2020 2069 6620 6b3a 0a20 2020         if k:.   
-00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e20: 206b 2e76 616c 6964 6174 6528 290a 0a20   k.validate().. 
-00013e30: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00013e40: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00013e50: 7020 3d20 7375 7065 7228 4765 7449 6e73  p = super(GetIns
-00013e60: 7461 6e63 654d 6574 7269 6373 5265 7370  tanceMetricsResp
-00013e70: 6f6e 7365 426f 6479 506f 644d 6574 7269  onseBodyPodMetri
-00013e80: 6373 2c20 7365 6c66 292e 746f 5f6d 6170  cs, self).to_map
-00013e90: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-00013ea0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-00013eb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00013ec0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-00013ed0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-00013ee0: 0a20 2020 2020 2020 2072 6573 756c 745b  .        result[
-00013ef0: 274d 6574 7269 6373 275d 203d 205b 5d0a  'Metrics'] = [].
-00013f00: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00013f10: 6d65 7472 6963 7320 6973 206e 6f74 204e  metrics is not N
-00013f20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00013f30: 2066 6f72 206b 2069 6e20 7365 6c66 2e6d   for k in self.m
-00013f40: 6574 7269 6373 3a0a 2020 2020 2020 2020  etrics:.        
-00013f50: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00013f60: 4d65 7472 6963 7327 5d2e 6170 7065 6e64  Metrics'].append
-00013f70: 286b 2e74 6f5f 6d61 7028 2920 6966 206b  (k.to_map() if k
-00013f80: 2065 6c73 6520 4e6f 6e65 290a 2020 2020   else None).    
-00013f90: 2020 2020 6966 2073 656c 662e 706f 645f      if self.pod_
-00013fa0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00013fb0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00013fc0: 6c74 5b27 506f 6449 6427 5d20 3d20 7365  lt['PodId'] = se
-00013fd0: 6c66 2e70 6f64 5f69 640a 2020 2020 2020  lf.pod_id.      
-00013fe0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00013ff0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00014000: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-00014010: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00014020: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-00014030: 2073 656c 662e 6d65 7472 6963 7320 3d20   self.metrics = 
-00014040: 5b5d 0a20 2020 2020 2020 2069 6620 6d2e  [].        if m.
-00014050: 6765 7428 274d 6574 7269 6373 2729 2069  get('Metrics') i
-00014060: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00014070: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00014080: 206d 2e67 6574 2827 4d65 7472 6963 7327   m.get('Metrics'
-00014090: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000140a0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-000140b0: 4765 7449 6e73 7461 6e63 654d 6574 7269  GetInstanceMetri
-000140c0: 6373 5265 7370 6f6e 7365 426f 6479 506f  csResponseBodyPo
-000140d0: 644d 6574 7269 6373 4d65 7472 6963 7328  dMetricsMetrics(
-000140e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000140f0: 2020 7365 6c66 2e6d 6574 7269 6373 2e61    self.metrics.a
-00014100: 7070 656e 6428 7465 6d70 5f6d 6f64 656c  ppend(temp_model
-00014110: 2e66 726f 6d5f 6d61 7028 6b29 290a 2020  .from_map(k)).  
-00014120: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00014130: 506f 6449 6427 2920 6973 206e 6f74 204e  PodId') is not N
-00014140: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00014150: 2073 656c 662e 706f 645f 6964 203d 206d   self.pod_id = m
-00014160: 2e67 6574 2827 506f 6449 6427 290a 2020  .get('PodId').  
-00014170: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00014180: 660a 0a0a 636c 6173 7320 4765 7449 6e73  f...class GetIns
-00014190: 7461 6e63 654d 6574 7269 6373 5265 7370  tanceMetricsResp
-000141a0: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
-000141b0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-000141c0: 6974 5f5f 2873 656c 662c 2069 6e73 7461  it__(self, insta
-000141d0: 6e63 655f 6964 3d4e 6f6e 652c 2070 6f64  nce_id=None, pod
-000141e0: 5f6d 6574 7269 6373 3d4e 6f6e 652c 2072  _metrics=None, r
-000141f0: 6571 7565 7374 5f69 643d 4e6f 6e65 293a  equest_id=None):
-00014200: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00014210: 7374 616e 6365 5f69 6420 3d20 696e 7374  stance_id = inst
-00014220: 616e 6365 5f69 6420 2023 2074 7970 653a  ance_id  # type:
-00014230: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
-00014240: 662e 706f 645f 6d65 7472 6963 7320 3d20  f.pod_metrics = 
-00014250: 706f 645f 6d65 7472 6963 7320 2023 2074  pod_metrics  # t
-00014260: 7970 653a 206c 6973 745b 4765 7449 6e73  ype: list[GetIns
-00014270: 7461 6e63 654d 6574 7269 6373 5265 7370  tanceMetricsResp
-00014280: 6f6e 7365 426f 6479 506f 644d 6574 7269  onseBodyPodMetri
-00014290: 6373 5d0a 2020 2020 2020 2020 7365 6c66  cs].        self
-000142a0: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
-000142b0: 7175 6573 745f 6964 2020 2320 7479 7065  quest_id  # type
-000142c0: 3a20 7374 720a 0a20 2020 2064 6566 2076  : str..    def v
-000142d0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-000142e0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-000142f0: 6f64 5f6d 6574 7269 6373 3a0a 2020 2020  od_metrics:.    
-00014300: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00014310: 2073 656c 662e 706f 645f 6d65 7472 6963   self.pod_metric
-00014320: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00014330: 2020 2069 6620 6b3a 0a20 2020 2020 2020     if k:.       
-00014340: 2020 2020 2020 2020 2020 2020 206b 2e76               k.v
-00014350: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
-00014360: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00014370: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00014380: 7375 7065 7228 4765 7449 6e73 7461 6e63  super(GetInstanc
-00014390: 654d 6574 7269 6373 5265 7370 6f6e 7365  eMetricsResponse
-000143a0: 426f 6479 2c20 7365 6c66 292e 746f 5f6d  Body, self).to_m
-000143b0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-000143c0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-000143d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000143e0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-000143f0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00014400: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00014410: 6c66 2e69 6e73 7461 6e63 655f 6964 2069  lf.instance_id i
-00014420: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00014430: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00014440: 496e 7374 616e 6365 4964 275d 203d 2073  InstanceId'] = s
-00014450: 656c 662e 696e 7374 616e 6365 5f69 640a  elf.instance_id.
-00014460: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00014470: 506f 644d 6574 7269 6373 275d 203d 205b  PodMetrics'] = [
-00014480: 5d0a 2020 2020 2020 2020 6966 2073 656c  ].        if sel
-00014490: 662e 706f 645f 6d65 7472 6963 7320 6973  f.pod_metrics is
-000144a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000144b0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-000144c0: 7365 6c66 2e70 6f64 5f6d 6574 7269 6373  self.pod_metrics
-000144d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000144e0: 2020 7265 7375 6c74 5b27 506f 644d 6574    result['PodMet
-000144f0: 7269 6373 275d 2e61 7070 656e 6428 6b2e  rics'].append(k.
-00014500: 746f 5f6d 6170 2829 2069 6620 6b20 656c  to_map() if k el
-00014510: 7365 204e 6f6e 6529 0a20 2020 2020 2020  se None).       
-00014520: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
-00014530: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00014540: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00014550: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
-00014560: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
-00014570: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-00014580: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00014590: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-000145a0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-000145b0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-000145c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000145d0: 6574 2827 496e 7374 616e 6365 4964 2729  et('InstanceId')
-000145e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000145f0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-00014600: 6e73 7461 6e63 655f 6964 203d 206d 2e67  nstance_id = m.g
-00014610: 6574 2827 496e 7374 616e 6365 4964 2729  et('InstanceId')
-00014620: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
-00014630: 645f 6d65 7472 6963 7320 3d20 5b5d 0a20  d_metrics = []. 
-00014640: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00014650: 2750 6f64 4d65 7472 6963 7327 2920 6973  'PodMetrics') is
-00014660: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00014670: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-00014680: 6d2e 6765 7428 2750 6f64 4d65 7472 6963  m.get('PodMetric
-00014690: 7327 293a 0a20 2020 2020 2020 2020 2020  s'):.           
-000146a0: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-000146b0: 3d20 4765 7449 6e73 7461 6e63 654d 6574  = GetInstanceMet
-000146c0: 7269 6373 5265 7370 6f6e 7365 426f 6479  ricsResponseBody
-000146d0: 506f 644d 6574 7269 6373 2829 0a20 2020  PodMetrics().   
-000146e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000146f0: 662e 706f 645f 6d65 7472 6963 732e 6170  f.pod_metrics.ap
-00014700: 7065 6e64 2874 656d 705f 6d6f 6465 6c2e  pend(temp_model.
-00014710: 6672 6f6d 5f6d 6170 286b 2929 0a20 2020  from_map(k)).   
-00014720: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-00014730: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
-00014740: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00014750: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-00014760: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
-00014770: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
-00014780: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-00014790: 6c61 7373 2047 6574 496e 7374 616e 6365  lass GetInstance
-000147a0: 4d65 7472 6963 7352 6573 706f 6e73 6528  MetricsResponse(
-000147b0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-000147c0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000147d0: 2c20 6865 6164 6572 733d 4e6f 6e65 2c20  , headers=None, 
-000147e0: 7374 6174 7573 5f63 6f64 653d 4e6f 6e65  status_code=None
-000147f0: 2c20 626f 6479 3d4e 6f6e 6529 3a0a 2020  , body=None):.  
-00014800: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-00014810: 7273 203d 2068 6561 6465 7273 2020 2320  rs = headers  # 
-00014820: 7479 7065 3a20 6469 6374 5b73 7472 2c20  type: dict[str, 
-00014830: 7374 725d 0a20 2020 2020 2020 2073 656c  str].        sel
-00014840: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-00014850: 7374 6174 7573 5f63 6f64 6520 2023 2074  status_code  # t
-00014860: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
-00014870: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-00014880: 7920 2023 2074 7970 653a 2047 6574 496e  y  # type: GetIn
-00014890: 7374 616e 6365 4d65 7472 6963 7352 6573  stanceMetricsRes
-000148a0: 706f 6e73 6542 6f64 790a 0a20 2020 2064  ponseBody..    d
-000148b0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000148c0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000148d0: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-000148e0: 6428 7365 6c66 2e68 6561 6465 7273 2c20  d(self.headers, 
-000148f0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00014900: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-00014910: 5f72 6571 7569 7265 6428 7365 6c66 2e73  _required(self.s
-00014920: 7461 7475 735f 636f 6465 2c20 2773 7461  tatus_code, 'sta
-00014930: 7475 735f 636f 6465 2729 0a20 2020 2020  tus_code').     
-00014940: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-00014950: 5f72 6571 7569 7265 6428 7365 6c66 2e62  _required(self.b
-00014960: 6f64 792c 2027 626f 6479 2729 0a20 2020  ody, 'body').   
-00014970: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00014980: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-00014990: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-000149a0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-000149b0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-000149c0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-000149d0: 4765 7449 6e73 7461 6e63 654d 6574 7269  GetInstanceMetri
-000149e0: 6373 5265 7370 6f6e 7365 2c20 7365 6c66  csResponse, self
-000149f0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00014a00: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00014a10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00014a20: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00014a30: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00014a40: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00014a50: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-00014a60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00014a70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00014a80: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-00014a90: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-00014aa0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-00014ab0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-00014ac0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00014ad0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-00014ae0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-00014af0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-00014b00: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-00014b10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00014b20: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00014b30: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00014b40: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00014b50: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00014b60: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00014b70: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-00014b80: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00014b90: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-00014ba0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-00014bb0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-00014bc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00014bd0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-00014be0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-00014bf0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00014c00: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-00014c10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00014c20: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00014c30: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-00014c40: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-00014c50: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-00014c60: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-00014c70: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-00014c80: 656d 705f 6d6f 6465 6c20 3d20 4765 7449  emp_model = GetI
-00014c90: 6e73 7461 6e63 654d 6574 7269 6373 5265  nstanceMetricsRe
-00014ca0: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
-00014cb0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-00014cc0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-00014cd0: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-00014ce0: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-00014cf0: 726e 2073 656c 660a 0a0a                 rn self...
+00006570: 2020 2073 656c 662e 636f 6d6d 616e 6420     self.command 
+00006580: 3d20 6d2e 6765 7428 2743 6f6d 6d61 6e64  = m.get('Command
+00006590: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000065a0: 6765 7428 2749 6d61 6765 2729 2069 7320  get('Image') is 
+000065b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000065c0: 2020 2020 2020 7365 6c66 2e69 6d61 6765        self.image
+000065d0: 203d 206d 2e67 6574 2827 496d 6167 6527   = m.get('Image'
+000065e0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000065f0: 6574 2827 4e61 6d65 2729 2069 7320 6e6f  et('Name') is no
+00006600: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00006610: 2020 2020 7365 6c66 2e6e 616d 6520 3d20      self.name = 
+00006620: 6d2e 6765 7428 274e 616d 6527 290a 2020  m.get('Name').  
+00006630: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00006640: 566f 6c75 6d65 7327 2920 6973 206e 6f74  Volumes') is not
+00006650: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00006660: 2020 2073 656c 662e 766f 6c75 6d65 7320     self.volumes 
+00006670: 3d20 6d2e 6765 7428 2756 6f6c 756d 6573  = m.get('Volumes
+00006680: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+00006690: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2043  n self...class C
+000066a0: 7265 6174 6545 6169 4563 6952 6571 7565  reateEaiEciReque
+000066b0: 7374 4563 6928 5465 614d 6f64 656c 293a  stEci(TeaModel):
+000066c0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000066d0: 5f28 7365 6c66 2c20 636f 6e74 6169 6e65  _(self, containe
+000066e0: 723d 4e6f 6e65 2c20 6569 705f 6964 3d4e  r=None, eip_id=N
+000066f0: 6f6e 652c 206e 616d 653d 4e6f 6e65 2c20  one, name=None, 
+00006700: 7479 7065 3d4e 6f6e 652c 2076 6f6c 756d  type=None, volum
+00006710: 653d 4e6f 6e65 293a 0a20 2020 2020 2020  e=None):.       
+00006720: 2073 656c 662e 636f 6e74 6169 6e65 7220   self.container 
+00006730: 3d20 636f 6e74 6169 6e65 7220 2023 2074  = container  # t
+00006740: 7970 653a 2043 7265 6174 6545 6169 4563  ype: CreateEaiEc
+00006750: 6952 6571 7565 7374 4563 6943 6f6e 7461  iRequestEciConta
+00006760: 696e 6572 0a20 2020 2020 2020 2073 656c  iner.        sel
+00006770: 662e 6569 705f 6964 203d 2065 6970 5f69  f.eip_id = eip_i
+00006780: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
+00006790: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
+000067a0: 203d 206e 616d 6520 2023 2074 7970 653a   = name  # type:
+000067b0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+000067c0: 662e 7479 7065 203d 2074 7970 6520 2023  f.type = type  #
+000067d0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
+000067e0: 2020 2073 656c 662e 766f 6c75 6d65 203d     self.volume =
+000067f0: 2076 6f6c 756d 6520 2023 2074 7970 653a   volume  # type:
+00006800: 2073 7472 0a0a 2020 2020 6465 6620 7661   str..    def va
+00006810: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00006820: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00006830: 6e74 6169 6e65 723a 0a20 2020 2020 2020  ntainer:.       
+00006840: 2020 2020 2073 656c 662e 636f 6e74 6169       self.contai
+00006850: 6e65 722e 7661 6c69 6461 7465 2829 0a0a  ner.validate()..
+00006860: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00006870: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00006880: 6170 203d 2073 7570 6572 2843 7265 6174  ap = super(Creat
+00006890: 6545 6169 4563 6952 6571 7565 7374 4563  eEaiEciRequestEc
+000068a0: 692c 2073 656c 6629 2e74 6f5f 6d61 7028  i, self).to_map(
+000068b0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+000068c0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000068d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000068e0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000068f0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00006900: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00006910: 636f 6e74 6169 6e65 7220 6973 206e 6f74  container is not
+00006920: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00006930: 2020 2072 6573 756c 745b 2743 6f6e 7461     result['Conta
+00006940: 696e 6572 275d 203d 2073 656c 662e 636f  iner'] = self.co
+00006950: 6e74 6169 6e65 722e 746f 5f6d 6170 2829  ntainer.to_map()
+00006960: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00006970: 2e65 6970 5f69 6420 6973 206e 6f74 204e  .eip_id is not N
+00006980: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00006990: 2072 6573 756c 745b 2745 6970 4964 275d   result['EipId']
+000069a0: 203d 2073 656c 662e 6569 705f 6964 0a20   = self.eip_id. 
+000069b0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+000069c0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+000069d0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000069e0: 756c 745b 274e 616d 6527 5d20 3d20 7365  ult['Name'] = se
+000069f0: 6c66 2e6e 616d 650a 2020 2020 2020 2020  lf.name.        
+00006a00: 6966 2073 656c 662e 7479 7065 2069 7320  if self.type is 
+00006a10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00006a20: 2020 2020 2020 7265 7375 6c74 5b27 5479        result['Ty
+00006a30: 7065 275d 203d 2073 656c 662e 7479 7065  pe'] = self.type
+00006a40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00006a50: 2e76 6f6c 756d 6520 6973 206e 6f74 204e  .volume is not N
+00006a60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00006a70: 2072 6573 756c 745b 2756 6f6c 756d 6527   result['Volume'
+00006a80: 5d20 3d20 7365 6c66 2e76 6f6c 756d 650a  ] = self.volume.
+00006a90: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00006aa0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00006ab0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+00006ac0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00006ad0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00006ae0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00006af0: 2743 6f6e 7461 696e 6572 2729 2069 7320  'Container') is 
+00006b00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00006b10: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00006b20: 203d 2043 7265 6174 6545 6169 4563 6952   = CreateEaiEciR
+00006b30: 6571 7565 7374 4563 6943 6f6e 7461 696e  equestEciContain
+00006b40: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
+00006b50: 2073 656c 662e 636f 6e74 6169 6e65 7220   self.container 
+00006b60: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+00006b70: 6d5f 6d61 7028 6d5b 2743 6f6e 7461 696e  m_map(m['Contain
+00006b80: 6572 275d 290a 2020 2020 2020 2020 6966  er']).        if
+00006b90: 206d 2e67 6574 2827 4569 7049 6427 2920   m.get('EipId') 
+00006ba0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00006bb0: 2020 2020 2020 2020 2073 656c 662e 6569           self.ei
+00006bc0: 705f 6964 203d 206d 2e67 6574 2827 4569  p_id = m.get('Ei
+00006bd0: 7049 6427 290a 2020 2020 2020 2020 6966  pId').        if
+00006be0: 206d 2e67 6574 2827 4e61 6d65 2729 2069   m.get('Name') i
+00006bf0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00006c00: 2020 2020 2020 2020 7365 6c66 2e6e 616d          self.nam
+00006c10: 6520 3d20 6d2e 6765 7428 274e 616d 6527  e = m.get('Name'
+00006c20: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00006c30: 6574 2827 5479 7065 2729 2069 7320 6e6f  et('Type') is no
+00006c40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00006c50: 2020 2020 7365 6c66 2e74 7970 6520 3d20      self.type = 
+00006c60: 6d2e 6765 7428 2754 7970 6527 290a 2020  m.get('Type').  
+00006c70: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00006c80: 566f 6c75 6d65 2729 2069 7320 6e6f 7420  Volume') is not 
+00006c90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00006ca0: 2020 7365 6c66 2e76 6f6c 756d 6520 3d20    self.volume = 
+00006cb0: 6d2e 6765 7428 2756 6f6c 756d 6527 290a  m.get('Volume').
+00006cc0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00006cd0: 656c 660a 0a0a 636c 6173 7320 4372 6561  elf...class Crea
+00006ce0: 7465 4561 6945 6369 5265 7175 6573 7428  teEaiEciRequest(
+00006cf0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00006d00: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00006d10: 2c20 636c 6965 6e74 5f74 6f6b 656e 3d4e  , client_token=N
+00006d20: 6f6e 652c 2065 6169 735f 6e61 6d65 3d4e  one, eais_name=N
+00006d30: 6f6e 652c 2065 6169 735f 7479 7065 3d4e  one, eais_type=N
+00006d40: 6f6e 652c 2065 6369 3d4e 6f6e 652c 2072  one, eci=None, r
+00006d50: 6567 696f 6e5f 6964 3d4e 6f6e 652c 0a20  egion_id=None,. 
+00006d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d70: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
+00006d80: 643d 4e6f 6e65 2c20 7365 6375 7269 7479  d=None, security
+00006d90: 5f67 726f 7570 5f69 643d 4e6f 6e65 2c20  _group_id=None, 
+00006da0: 765f 7377 6974 6368 5f69 643d 4e6f 6e65  v_switch_id=None
+00006db0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00006dc0: 636c 6965 6e74 5f74 6f6b 656e 203d 2063  client_token = c
+00006dd0: 6c69 656e 745f 746f 6b65 6e20 2023 2074  lient_token  # t
+00006de0: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00006df0: 2073 656c 662e 6561 6973 5f6e 616d 6520   self.eais_name 
+00006e00: 3d20 6561 6973 5f6e 616d 6520 2023 2074  = eais_name  # t
+00006e10: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00006e20: 2073 656c 662e 6561 6973 5f74 7970 6520   self.eais_type 
+00006e30: 3d20 6561 6973 5f74 7970 6520 2023 2074  = eais_type  # t
+00006e40: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00006e50: 2073 656c 662e 6563 6920 3d20 6563 6920   self.eci = eci 
+00006e60: 2023 2074 7970 653a 2043 7265 6174 6545   # type: CreateE
+00006e70: 6169 4563 6952 6571 7565 7374 4563 690a  aiEciRequestEci.
+00006e80: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
+00006e90: 696f 6e5f 6964 203d 2072 6567 696f 6e5f  ion_id = region_
+00006ea0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+00006eb0: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+00006ec0: 6f75 7263 655f 6772 6f75 705f 6964 203d  ource_group_id =
+00006ed0: 2072 6573 6f75 7263 655f 6772 6f75 705f   resource_group_
+00006ee0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+00006ef0: 2020 2020 2020 2020 7365 6c66 2e73 6563          self.sec
+00006f00: 7572 6974 795f 6772 6f75 705f 6964 203d  urity_group_id =
+00006f10: 2073 6563 7572 6974 795f 6772 6f75 705f   security_group_
+00006f20: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+00006f30: 2020 2020 2020 2020 7365 6c66 2e76 5f73          self.v_s
+00006f40: 7769 7463 685f 6964 203d 2076 5f73 7769  witch_id = v_swi
+00006f50: 7463 685f 6964 2020 2320 7479 7065 3a20  tch_id  # type: 
+00006f60: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
+00006f70: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00006f80: 2020 2020 2069 6620 7365 6c66 2e65 6369       if self.eci
+00006f90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00006fa0: 6c66 2e65 6369 2e76 616c 6964 6174 6528  lf.eci.validate(
+00006fb0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+00006fc0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00006fd0: 205f 6d61 7020 3d20 7375 7065 7228 4372   _map = super(Cr
+00006fe0: 6561 7465 4561 6945 6369 5265 7175 6573  eateEaiEciReques
+00006ff0: 742c 2073 656c 6629 2e74 6f5f 6d61 7028  t, self).to_map(
+00007000: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00007010: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00007020: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007030: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00007040: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00007050: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00007060: 636c 6965 6e74 5f74 6f6b 656e 2069 7320  client_token is 
+00007070: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00007080: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
+00007090: 6965 6e74 546f 6b65 6e27 5d20 3d20 7365  ientToken'] = se
+000070a0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e0a  lf.client_token.
+000070b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000070c0: 6561 6973 5f6e 616d 6520 6973 206e 6f74  eais_name is not
+000070d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000070e0: 2020 2072 6573 756c 745b 2745 6169 734e     result['EaisN
+000070f0: 616d 6527 5d20 3d20 7365 6c66 2e65 6169  ame'] = self.eai
+00007100: 735f 6e61 6d65 0a20 2020 2020 2020 2069  s_name.        i
+00007110: 6620 7365 6c66 2e65 6169 735f 7479 7065  f self.eais_type
+00007120: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00007130: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00007140: 5b27 4561 6973 5479 7065 275d 203d 2073  ['EaisType'] = s
+00007150: 656c 662e 6561 6973 5f74 7970 650a 2020  elf.eais_type.  
+00007160: 2020 2020 2020 6966 2073 656c 662e 6563        if self.ec
+00007170: 6920 6973 206e 6f74 204e 6f6e 653a 0a20  i is not None:. 
+00007180: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00007190: 745b 2745 6369 275d 203d 2073 656c 662e  t['Eci'] = self.
+000071a0: 6563 692e 746f 5f6d 6170 2829 0a20 2020  eci.to_map().   
+000071b0: 2020 2020 2069 6620 7365 6c66 2e72 6567       if self.reg
+000071c0: 696f 6e5f 6964 2069 7320 6e6f 7420 4e6f  ion_id is not No
+000071d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000071e0: 7265 7375 6c74 5b27 5265 6769 6f6e 4964  result['RegionId
+000071f0: 275d 203d 2073 656c 662e 7265 6769 6f6e  '] = self.region
+00007200: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00007210: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
+00007220: 7570 5f69 6420 6973 206e 6f74 204e 6f6e  up_id is not Non
+00007230: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00007240: 6573 756c 745b 2752 6573 6f75 7263 6547  esult['ResourceG
+00007250: 726f 7570 4964 275d 203d 2073 656c 662e  roupId'] = self.
+00007260: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
+00007270: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+00007280: 662e 7365 6375 7269 7479 5f67 726f 7570  f.security_group
+00007290: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+000072a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000072b0: 756c 745b 2753 6563 7572 6974 7947 726f  ult['SecurityGro
+000072c0: 7570 4964 275d 203d 2073 656c 662e 7365  upId'] = self.se
+000072d0: 6375 7269 7479 5f67 726f 7570 5f69 640a  curity_group_id.
+000072e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000072f0: 765f 7377 6974 6368 5f69 6420 6973 206e  v_switch_id is n
+00007300: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00007310: 2020 2020 2072 6573 756c 745b 2756 5377       result['VSw
+00007320: 6974 6368 4964 275d 203d 2073 656c 662e  itchId'] = self.
+00007330: 765f 7377 6974 6368 5f69 640a 2020 2020  v_switch_id.    
+00007340: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00007350: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+00007360: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
+00007370: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+00007380: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+00007390: 2020 2069 6620 6d2e 6765 7428 2743 6c69     if m.get('Cli
+000073a0: 656e 7454 6f6b 656e 2729 2069 7320 6e6f  entToken') is no
+000073b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000073c0: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
+000073d0: 746f 6b65 6e20 3d20 6d2e 6765 7428 2743  token = m.get('C
+000073e0: 6c69 656e 7454 6f6b 656e 2729 0a20 2020  lientToken').   
+000073f0: 2020 2020 2069 6620 6d2e 6765 7428 2745       if m.get('E
+00007400: 6169 734e 616d 6527 2920 6973 206e 6f74  aisName') is not
+00007410: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00007420: 2020 2073 656c 662e 6561 6973 5f6e 616d     self.eais_nam
+00007430: 6520 3d20 6d2e 6765 7428 2745 6169 734e  e = m.get('EaisN
+00007440: 616d 6527 290a 2020 2020 2020 2020 6966  ame').        if
+00007450: 206d 2e67 6574 2827 4561 6973 5479 7065   m.get('EaisType
+00007460: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00007470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007480: 2e65 6169 735f 7479 7065 203d 206d 2e67  .eais_type = m.g
+00007490: 6574 2827 4561 6973 5479 7065 2729 0a20  et('EaisType'). 
+000074a0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000074b0: 2745 6369 2729 2069 7320 6e6f 7420 4e6f  'Eci') is not No
+000074c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000074d0: 7465 6d70 5f6d 6f64 656c 203d 2043 7265  temp_model = Cre
+000074e0: 6174 6545 6169 4563 6952 6571 7565 7374  ateEaiEciRequest
+000074f0: 4563 6928 290a 2020 2020 2020 2020 2020  Eci().          
+00007500: 2020 7365 6c66 2e65 6369 203d 2074 656d    self.eci = tem
+00007510: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00007520: 286d 5b27 4563 6927 5d29 0a20 2020 2020  (m['Eci']).     
+00007530: 2020 2069 6620 6d2e 6765 7428 2752 6567     if m.get('Reg
+00007540: 696f 6e49 6427 2920 6973 206e 6f74 204e  ionId') is not N
+00007550: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007560: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+00007570: 3d20 6d2e 6765 7428 2752 6567 696f 6e49  = m.get('RegionI
+00007580: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+00007590: 2e67 6574 2827 5265 736f 7572 6365 4772  .get('ResourceGr
+000075a0: 6f75 7049 6427 2920 6973 206e 6f74 204e  oupId') is not N
+000075b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000075c0: 2073 656c 662e 7265 736f 7572 6365 5f67   self.resource_g
+000075d0: 726f 7570 5f69 6420 3d20 6d2e 6765 7428  roup_id = m.get(
+000075e0: 2752 6573 6f75 7263 6547 726f 7570 4964  'ResourceGroupId
+000075f0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00007600: 6765 7428 2753 6563 7572 6974 7947 726f  get('SecurityGro
+00007610: 7570 4964 2729 2069 7320 6e6f 7420 4e6f  upId') is not No
+00007620: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00007630: 7365 6c66 2e73 6563 7572 6974 795f 6772  self.security_gr
+00007640: 6f75 705f 6964 203d 206d 2e67 6574 2827  oup_id = m.get('
+00007650: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
+00007660: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00007670: 6574 2827 5653 7769 7463 6849 6427 2920  et('VSwitchId') 
+00007680: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007690: 2020 2020 2020 2020 2073 656c 662e 765f           self.v_
+000076a0: 7377 6974 6368 5f69 6420 3d20 6d2e 6765  switch_id = m.ge
+000076b0: 7428 2756 5377 6974 6368 4964 2729 0a20  t('VSwitchId'). 
+000076c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000076d0: 6c66 0a0a 0a63 6c61 7373 2043 7265 6174  lf...class Creat
+000076e0: 6545 6169 4563 6953 6872 696e 6b52 6571  eEaiEciShrinkReq
+000076f0: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+00007700: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00007710: 2873 656c 662c 2063 6c69 656e 745f 746f  (self, client_to
+00007720: 6b65 6e3d 4e6f 6e65 2c20 6561 6973 5f6e  ken=None, eais_n
+00007730: 616d 653d 4e6f 6e65 2c20 6561 6973 5f74  ame=None, eais_t
+00007740: 7970 653d 4e6f 6e65 2c20 6563 695f 7368  ype=None, eci_sh
+00007750: 7269 6e6b 3d4e 6f6e 652c 2072 6567 696f  rink=None, regio
+00007760: 6e5f 6964 3d4e 6f6e 652c 0a20 2020 2020  n_id=None,.     
+00007770: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+00007780: 7572 6365 5f67 726f 7570 5f69 643d 4e6f  urce_group_id=No
+00007790: 6e65 2c20 7365 6375 7269 7479 5f67 726f  ne, security_gro
+000077a0: 7570 5f69 643d 4e6f 6e65 2c20 765f 7377  up_id=None, v_sw
+000077b0: 6974 6368 5f69 643d 4e6f 6e65 293a 0a20  itch_id=None):. 
+000077c0: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+000077d0: 6e74 5f74 6f6b 656e 203d 2063 6c69 656e  nt_token = clien
+000077e0: 745f 746f 6b65 6e20 2023 2074 7970 653a  t_token  # type:
+000077f0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00007800: 662e 6561 6973 5f6e 616d 6520 3d20 6561  f.eais_name = ea
+00007810: 6973 5f6e 616d 6520 2023 2074 7970 653a  is_name  # type:
+00007820: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00007830: 662e 6561 6973 5f74 7970 6520 3d20 6561  f.eais_type = ea
+00007840: 6973 5f74 7970 6520 2023 2074 7970 653a  is_type  # type:
+00007850: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00007860: 662e 6563 695f 7368 7269 6e6b 203d 2065  f.eci_shrink = e
+00007870: 6369 5f73 6872 696e 6b20 2023 2074 7970  ci_shrink  # typ
+00007880: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+00007890: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
+000078a0: 7265 6769 6f6e 5f69 6420 2023 2074 7970  region_id  # typ
+000078b0: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+000078c0: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
+000078d0: 7570 5f69 6420 3d20 7265 736f 7572 6365  up_id = resource
+000078e0: 5f67 726f 7570 5f69 6420 2023 2074 7970  _group_id  # typ
+000078f0: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+00007900: 656c 662e 7365 6375 7269 7479 5f67 726f  elf.security_gro
+00007910: 7570 5f69 6420 3d20 7365 6375 7269 7479  up_id = security
+00007920: 5f67 726f 7570 5f69 6420 2023 2074 7970  _group_id  # typ
+00007930: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+00007940: 656c 662e 765f 7377 6974 6368 5f69 6420  elf.v_switch_id 
+00007950: 3d20 765f 7377 6974 6368 5f69 6420 2023  = v_switch_id  #
+00007960: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
+00007970: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00007980: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00007990: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+000079a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000079b0: 5f6d 6170 203d 2073 7570 6572 2843 7265  _map = super(Cre
+000079c0: 6174 6545 6169 4563 6953 6872 696e 6b52  ateEaiEciShrinkR
+000079d0: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
+000079e0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000079f0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00007a00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00007a10: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00007a20: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00007a30: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00007a40: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
+00007a50: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+00007a60: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00007a70: 745b 2743 6c69 656e 7454 6f6b 656e 275d  t['ClientToken']
+00007a80: 203d 2073 656c 662e 636c 6965 6e74 5f74   = self.client_t
+00007a90: 6f6b 656e 0a20 2020 2020 2020 2069 6620  oken.        if 
+00007aa0: 7365 6c66 2e65 6169 735f 6e61 6d65 2069  self.eais_name i
+00007ab0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00007ac0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00007ad0: 4561 6973 4e61 6d65 275d 203d 2073 656c  EaisName'] = sel
+00007ae0: 662e 6561 6973 5f6e 616d 650a 2020 2020  f.eais_name.    
+00007af0: 2020 2020 6966 2073 656c 662e 6561 6973      if self.eais
+00007b00: 5f74 7970 6520 6973 206e 6f74 204e 6f6e  _type is not Non
+00007b10: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00007b20: 6573 756c 745b 2745 6169 7354 7970 6527  esult['EaisType'
+00007b30: 5d20 3d20 7365 6c66 2e65 6169 735f 7479  ] = self.eais_ty
+00007b40: 7065 0a20 2020 2020 2020 2069 6620 7365  pe.        if se
+00007b50: 6c66 2e65 6369 5f73 6872 696e 6b20 6973  lf.eci_shrink is
+00007b60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00007b70: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
+00007b80: 6369 275d 203d 2073 656c 662e 6563 695f  ci'] = self.eci_
+00007b90: 7368 7269 6e6b 0a20 2020 2020 2020 2069  shrink.        i
+00007ba0: 6620 7365 6c66 2e72 6567 696f 6e5f 6964  f self.region_id
+00007bb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00007bc0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00007bd0: 5b27 5265 6769 6f6e 4964 275d 203d 2073  ['RegionId'] = s
+00007be0: 656c 662e 7265 6769 6f6e 5f69 640a 2020  elf.region_id.  
+00007bf0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+00007c00: 736f 7572 6365 5f67 726f 7570 5f69 6420  source_group_id 
+00007c10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007c20: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00007c30: 2752 6573 6f75 7263 6547 726f 7570 4964  'ResourceGroupId
+00007c40: 275d 203d 2073 656c 662e 7265 736f 7572  '] = self.resour
+00007c50: 6365 5f67 726f 7570 5f69 640a 2020 2020  ce_group_id.    
+00007c60: 2020 2020 6966 2073 656c 662e 7365 6375      if self.secu
+00007c70: 7269 7479 5f67 726f 7570 5f69 6420 6973  rity_group_id is
+00007c80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00007c90: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
+00007ca0: 6563 7572 6974 7947 726f 7570 4964 275d  ecurityGroupId']
+00007cb0: 203d 2073 656c 662e 7365 6375 7269 7479   = self.security
+00007cc0: 5f67 726f 7570 5f69 640a 2020 2020 2020  _group_id.      
+00007cd0: 2020 6966 2073 656c 662e 765f 7377 6974    if self.v_swit
+00007ce0: 6368 5f69 6420 6973 206e 6f74 204e 6f6e  ch_id is not Non
+00007cf0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00007d00: 6573 756c 745b 2756 5377 6974 6368 4964  esult['VSwitchId
+00007d10: 275d 203d 2073 656c 662e 765f 7377 6974  '] = self.v_swit
+00007d20: 6368 5f69 640a 2020 2020 2020 2020 7265  ch_id.        re
+00007d30: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00007d40: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00007d50: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+00007d60: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00007d70: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00007d80: 6d2e 6765 7428 2743 6c69 656e 7454 6f6b  m.get('ClientTok
+00007d90: 656e 2729 2069 7320 6e6f 7420 4e6f 6e65  en') is not None
+00007da0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00007db0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
+00007dc0: 3d20 6d2e 6765 7428 2743 6c69 656e 7454  = m.get('ClientT
+00007dd0: 6f6b 656e 2729 0a20 2020 2020 2020 2069  oken').        i
+00007de0: 6620 6d2e 6765 7428 2745 6169 734e 616d  f m.get('EaisNam
+00007df0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00007e00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007e10: 662e 6561 6973 5f6e 616d 6520 3d20 6d2e  f.eais_name = m.
+00007e20: 6765 7428 2745 6169 734e 616d 6527 290a  get('EaisName').
+00007e30: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00007e40: 2827 4561 6973 5479 7065 2729 2069 7320  ('EaisType') is 
+00007e50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00007e60: 2020 2020 2020 7365 6c66 2e65 6169 735f        self.eais_
+00007e70: 7479 7065 203d 206d 2e67 6574 2827 4561  type = m.get('Ea
+00007e80: 6973 5479 7065 2729 0a20 2020 2020 2020  isType').       
+00007e90: 2069 6620 6d2e 6765 7428 2745 6369 2729   if m.get('Eci')
+00007ea0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00007eb0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+00007ec0: 6369 5f73 6872 696e 6b20 3d20 6d2e 6765  ci_shrink = m.ge
+00007ed0: 7428 2745 6369 2729 0a20 2020 2020 2020  t('Eci').       
+00007ee0: 2069 6620 6d2e 6765 7428 2752 6567 696f   if m.get('Regio
+00007ef0: 6e49 6427 2920 6973 206e 6f74 204e 6f6e  nId') is not Non
+00007f00: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00007f10: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
+00007f20: 6d2e 6765 7428 2752 6567 696f 6e49 6427  m.get('RegionId'
+00007f30: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00007f40: 6574 2827 5265 736f 7572 6365 4772 6f75  et('ResourceGrou
+00007f50: 7049 6427 2920 6973 206e 6f74 204e 6f6e  pId') is not Non
+00007f60: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00007f70: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
+00007f80: 7570 5f69 6420 3d20 6d2e 6765 7428 2752  up_id = m.get('R
+00007f90: 6573 6f75 7263 6547 726f 7570 4964 2729  esourceGroupId')
+00007fa0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00007fb0: 7428 2753 6563 7572 6974 7947 726f 7570  t('SecurityGroup
+00007fc0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00007fd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00007fe0: 6c66 2e73 6563 7572 6974 795f 6772 6f75  lf.security_grou
+00007ff0: 705f 6964 203d 206d 2e67 6574 2827 5365  p_id = m.get('Se
+00008000: 6375 7269 7479 4772 6f75 7049 6427 290a  curityGroupId').
+00008010: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00008020: 2827 5653 7769 7463 6849 6427 2920 6973  ('VSwitchId') is
+00008030: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00008040: 2020 2020 2020 2073 656c 662e 765f 7377         self.v_sw
+00008050: 6974 6368 5f69 6420 3d20 6d2e 6765 7428  itch_id = m.get(
+00008060: 2756 5377 6974 6368 4964 2729 0a20 2020  'VSwitchId').   
+00008070: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00008080: 0a0a 0a63 6c61 7373 2043 7265 6174 6545  ...class CreateE
+00008090: 6169 4563 6952 6573 706f 6e73 6542 6f64  aiEciResponseBod
+000080a0: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+000080b0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000080c0: 6c66 2c20 636c 6965 6e74 5f69 6e73 7461  lf, client_insta
+000080d0: 6e63 655f 6964 3d4e 6f6e 652c 2065 6c61  nce_id=None, ela
+000080e0: 7374 6963 5f61 6363 656c 6572 6174 6564  stic_accelerated
+000080f0: 5f69 6e73 7461 6e63 655f 6964 3d4e 6f6e  _instance_id=Non
+00008100: 652c 2072 6571 7565 7374 5f69 643d 4e6f  e, request_id=No
+00008110: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+00008120: 662e 636c 6965 6e74 5f69 6e73 7461 6e63  f.client_instanc
+00008130: 655f 6964 203d 2063 6c69 656e 745f 696e  e_id = client_in
+00008140: 7374 616e 6365 5f69 6420 2023 2074 7970  stance_id  # typ
+00008150: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+00008160: 656c 662e 656c 6173 7469 635f 6163 6365  elf.elastic_acce
+00008170: 6c65 7261 7465 645f 696e 7374 616e 6365  lerated_instance
+00008180: 5f69 6420 3d20 656c 6173 7469 635f 6163  _id = elastic_ac
+00008190: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+000081a0: 6365 5f69 6420 2023 2074 7970 653a 2073  ce_id  # type: s
+000081b0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+000081c0: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
+000081d0: 7565 7374 5f69 6420 2023 2074 7970 653a  uest_id  # type:
+000081e0: 2073 7472 0a0a 2020 2020 6465 6620 7661   str..    def va
+000081f0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00008200: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00008210: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00008220: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00008230: 2073 7570 6572 2843 7265 6174 6545 6169   super(CreateEai
+00008240: 4563 6952 6573 706f 6e73 6542 6f64 792c  EciResponseBody,
+00008250: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
+00008260: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+00008270: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00008280: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008290: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+000082a0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+000082b0: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
+000082c0: 6965 6e74 5f69 6e73 7461 6e63 655f 6964  ient_instance_id
+000082d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000082e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000082f0: 5b27 436c 6965 6e74 496e 7374 616e 6365  ['ClientInstance
+00008300: 4964 275d 203d 2073 656c 662e 636c 6965  Id'] = self.clie
+00008310: 6e74 5f69 6e73 7461 6e63 655f 6964 0a20  nt_instance_id. 
+00008320: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+00008330: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+00008340: 6564 5f69 6e73 7461 6e63 655f 6964 2069  ed_instance_id i
+00008350: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00008360: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00008370: 456c 6173 7469 6341 6363 656c 6572 6174  ElasticAccelerat
+00008380: 6564 496e 7374 616e 6365 4964 275d 203d  edInstanceId'] =
+00008390: 2073 656c 662e 656c 6173 7469 635f 6163   self.elastic_ac
+000083a0: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+000083b0: 6365 5f69 640a 2020 2020 2020 2020 6966  ce_id.        if
+000083c0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+000083d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000083e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000083f0: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
+00008400: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
+00008410: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00008420: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00008430: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+00008440: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00008450: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00008460: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00008470: 2743 6c69 656e 7449 6e73 7461 6e63 6549  'ClientInstanceI
+00008480: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00008490: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000084a0: 662e 636c 6965 6e74 5f69 6e73 7461 6e63  f.client_instanc
+000084b0: 655f 6964 203d 206d 2e67 6574 2827 436c  e_id = m.get('Cl
+000084c0: 6965 6e74 496e 7374 616e 6365 4964 2729  ientInstanceId')
+000084d0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000084e0: 7428 2745 6c61 7374 6963 4163 6365 6c65  t('ElasticAccele
+000084f0: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
+00008500: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00008510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008520: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
+00008530: 7465 645f 696e 7374 616e 6365 5f69 6420  ted_instance_id 
+00008540: 3d20 6d2e 6765 7428 2745 6c61 7374 6963  = m.get('Elastic
+00008550: 4163 6365 6c65 7261 7465 6449 6e73 7461  AcceleratedInsta
+00008560: 6e63 6549 6427 290a 2020 2020 2020 2020  nceId').        
+00008570: 6966 206d 2e67 6574 2827 5265 7175 6573  if m.get('Reques
+00008580: 7449 6427 2920 6973 206e 6f74 204e 6f6e  tId') is not Non
+00008590: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000085a0: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+000085b0: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+000085c0: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
+000085d0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+000085e0: 4372 6561 7465 4561 6945 6369 5265 7370  CreateEaiEciResp
+000085f0: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+00008600: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00008610: 2873 656c 662c 2068 6561 6465 7273 3d4e  (self, headers=N
+00008620: 6f6e 652c 2073 7461 7475 735f 636f 6465  one, status_code
+00008630: 3d4e 6f6e 652c 2062 6f64 793d 4e6f 6e65  =None, body=None
+00008640: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00008650: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+00008660: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
+00008670: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
+00008680: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+00008690: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
+000086a0: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
+000086b0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+000086c0: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
+000086d0: 4372 6561 7465 4561 6945 6369 5265 7370  CreateEaiEciResp
+000086e0: 6f6e 7365 426f 6479 0a0a 2020 2020 6465  onseBody..    de
+000086f0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00008700: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
+00008710: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00008720: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
+00008730: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+00008740: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00008750: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
+00008760: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
+00008770: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
+00008780: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00008790: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
+000087a0: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
+000087b0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+000087c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000087d0: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+000087e0: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+000087f0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00008800: 2020 5f6d 6170 203d 2073 7570 6572 2843    _map = super(C
+00008810: 7265 6174 6545 6169 4563 6952 6573 706f  reateEaiEciRespo
+00008820: 6e73 652c 2073 656c 6629 2e74 6f5f 6d61  nse, self).to_ma
+00008830: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00008840: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00008850: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00008860: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+00008870: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00008880: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00008890: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+000088a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000088b0: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+000088c0: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+000088d0: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+000088e0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+000088f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00008900: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00008910: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+00008920: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00008930: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00008940: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+00008950: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00008960: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+00008970: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+00008980: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00008990: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000089a0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000089b0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+000089c0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000089d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000089e0: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
+000089f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00008a00: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+00008a10: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
+00008a20: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
+00008a30: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
+00008a40: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
+00008a50: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00008a60: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00008a70: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
+00008a80: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
+00008a90: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
+00008aa0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00008ab0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+00008ac0: 656c 203d 2043 7265 6174 6545 6169 4563  el = CreateEaiEc
+00008ad0: 6952 6573 706f 6e73 6542 6f64 7928 290a  iResponseBody().
+00008ae0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00008af0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+00008b00: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+00008b10: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+00008b20: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00008b30: 7373 2043 7265 6174 6545 6169 4563 7352  ss CreateEaiEcsR
+00008b40: 6571 7565 7374 4563 7328 5465 614d 6f64  equestEcs(TeaMod
+00008b50: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00008b60: 6e69 745f 5f28 7365 6c66 2c20 696d 6167  nit__(self, imag
+00008b70: 655f 6964 3d4e 6f6e 652c 2069 6e74 6572  e_id=None, inter
+00008b80: 6e65 745f 6d61 785f 6261 6e64 7769 6474  net_max_bandwidt
+00008b90: 685f 696e 3d4e 6f6e 652c 2069 6e74 6572  h_in=None, inter
+00008ba0: 6e65 745f 6d61 785f 6261 6e64 7769 6474  net_max_bandwidt
+00008bb0: 685f 6f75 743d 4e6f 6e65 2c20 6e61 6d65  h_out=None, name
+00008bc0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+00008bd0: 2020 2020 2020 2020 7061 7373 776f 7264          password
+00008be0: 3d4e 6f6e 652c 2073 7973 7465 6d5f 6469  =None, system_di
+00008bf0: 736b 5f63 6174 6567 6f72 793d 4e6f 6e65  sk_category=None
+00008c00: 2c20 7379 7374 656d 5f64 6973 6b5f 7369  , system_disk_si
+00008c10: 7a65 3d4e 6f6e 652c 2074 7970 653d 4e6f  ze=None, type=No
+00008c20: 6e65 2c20 7a6f 6e65 5f69 643d 4e6f 6e65  ne, zone_id=None
+00008c30: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00008c40: 696d 6167 655f 6964 203d 2069 6d61 6765  image_id = image
+00008c50: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
+00008c60: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00008c70: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
+00008c80: 6964 7468 5f69 6e20 3d20 696e 7465 726e  idth_in = intern
+00008c90: 6574 5f6d 6178 5f62 616e 6477 6964 7468  et_max_bandwidth
+00008ca0: 5f69 6e20 2023 2074 7970 653a 2073 7472  _in  # type: str
+00008cb0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00008cc0: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
+00008cd0: 6964 7468 5f6f 7574 203d 2069 6e74 6572  idth_out = inter
+00008ce0: 6e65 745f 6d61 785f 6261 6e64 7769 6474  net_max_bandwidt
+00008cf0: 685f 6f75 7420 2023 2074 7970 653a 2073  h_out  # type: s
+00008d00: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+00008d10: 6e61 6d65 203d 206e 616d 6520 2023 2074  name = name  # t
+00008d20: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00008d30: 2073 656c 662e 7061 7373 776f 7264 203d   self.password =
+00008d40: 2070 6173 7377 6f72 6420 2023 2074 7970   password  # typ
+00008d50: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+00008d60: 656c 662e 7379 7374 656d 5f64 6973 6b5f  elf.system_disk_
+00008d70: 6361 7465 676f 7279 203d 2073 7973 7465  category = syste
+00008d80: 6d5f 6469 736b 5f63 6174 6567 6f72 7920  m_disk_category 
+00008d90: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00008da0: 2020 2020 2073 656c 662e 7379 7374 656d       self.system
+00008db0: 5f64 6973 6b5f 7369 7a65 203d 2073 7973  _disk_size = sys
+00008dc0: 7465 6d5f 6469 736b 5f73 697a 6520 2023  tem_disk_size  #
+00008dd0: 2074 7970 653a 206c 6f6e 670a 2020 2020   type: long.    
+00008de0: 2020 2020 7365 6c66 2e74 7970 6520 3d20      self.type = 
+00008df0: 7479 7065 2020 2320 7479 7065 3a20 7374  type  # type: st
+00008e00: 720a 2020 2020 2020 2020 7365 6c66 2e7a  r.        self.z
+00008e10: 6f6e 655f 6964 203d 207a 6f6e 655f 6964  one_id = zone_id
+00008e20: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
+00008e30: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+00008e40: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00008e50: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+00008e60: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00008e70: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00008e80: 4372 6561 7465 4561 6945 6373 5265 7175  CreateEaiEcsRequ
+00008e90: 6573 7445 6373 2c20 7365 6c66 292e 746f  estEcs, self).to
+00008ea0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00008eb0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00008ec0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00008ed0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00008ee0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00008ef0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00008f00: 7365 6c66 2e69 6d61 6765 5f69 6420 6973  self.image_id is
+00008f10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00008f20: 2020 2020 2020 2072 6573 756c 745b 2749         result['I
+00008f30: 6d61 6765 4964 275d 203d 2073 656c 662e  mageId'] = self.
+00008f40: 696d 6167 655f 6964 0a20 2020 2020 2020  image_id.       
+00008f50: 2069 6620 7365 6c66 2e69 6e74 6572 6e65   if self.interne
+00008f60: 745f 6d61 785f 6261 6e64 7769 6474 685f  t_max_bandwidth_
+00008f70: 696e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  in is not None:.
+00008f80: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00008f90: 6c74 5b27 496e 7465 726e 6574 4d61 7842  lt['InternetMaxB
+00008fa0: 616e 6477 6964 7468 496e 275d 203d 2073  andwidthIn'] = s
+00008fb0: 656c 662e 696e 7465 726e 6574 5f6d 6178  elf.internet_max
+00008fc0: 5f62 616e 6477 6964 7468 5f69 6e0a 2020  _bandwidth_in.  
+00008fd0: 2020 2020 2020 6966 2073 656c 662e 696e        if self.in
+00008fe0: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
+00008ff0: 6964 7468 5f6f 7574 2069 7320 6e6f 7420  idth_out is not 
+00009000: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00009010: 2020 7265 7375 6c74 5b27 496e 7465 726e    result['Intern
+00009020: 6574 4d61 7842 616e 6477 6964 7468 4f75  etMaxBandwidthOu
+00009030: 7427 5d20 3d20 7365 6c66 2e69 6e74 6572  t'] = self.inter
+00009040: 6e65 745f 6d61 785f 6261 6e64 7769 6474  net_max_bandwidt
+00009050: 685f 6f75 740a 2020 2020 2020 2020 6966  h_out.        if
+00009060: 2073 656c 662e 6e61 6d65 2069 7320 6e6f   self.name is no
+00009070: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00009080: 2020 2020 7265 7375 6c74 5b27 4e61 6d65      result['Name
+00009090: 275d 203d 2073 656c 662e 6e61 6d65 0a20  '] = self.name. 
+000090a0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+000090b0: 6173 7377 6f72 6420 6973 206e 6f74 204e  assword is not N
+000090c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000090d0: 2072 6573 756c 745b 2750 6173 7377 6f72   result['Passwor
+000090e0: 6427 5d20 3d20 7365 6c66 2e70 6173 7377  d'] = self.passw
+000090f0: 6f72 640a 2020 2020 2020 2020 6966 2073  ord.        if s
+00009100: 656c 662e 7379 7374 656d 5f64 6973 6b5f  elf.system_disk_
+00009110: 6361 7465 676f 7279 2069 7320 6e6f 7420  category is not 
+00009120: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00009130: 2020 7265 7375 6c74 5b27 5379 7374 656d    result['System
+00009140: 4469 736b 4361 7465 676f 7279 275d 203d  DiskCategory'] =
+00009150: 2073 656c 662e 7379 7374 656d 5f64 6973   self.system_dis
+00009160: 6b5f 6361 7465 676f 7279 0a20 2020 2020  k_category.     
+00009170: 2020 2069 6620 7365 6c66 2e73 7973 7465     if self.syste
+00009180: 6d5f 6469 736b 5f73 697a 6520 6973 206e  m_disk_size is n
+00009190: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000091a0: 2020 2020 2072 6573 756c 745b 2753 7973       result['Sys
+000091b0: 7465 6d44 6973 6b53 697a 6527 5d20 3d20  temDiskSize'] = 
+000091c0: 7365 6c66 2e73 7973 7465 6d5f 6469 736b  self.system_disk
+000091d0: 5f73 697a 650a 2020 2020 2020 2020 6966  _size.        if
+000091e0: 2073 656c 662e 7479 7065 2069 7320 6e6f   self.type is no
+000091f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00009200: 2020 2020 7265 7375 6c74 5b27 5479 7065      result['Type
+00009210: 275d 203d 2073 656c 662e 7479 7065 0a20  '] = self.type. 
+00009220: 2020 2020 2020 2069 6620 7365 6c66 2e7a         if self.z
+00009230: 6f6e 655f 6964 2069 7320 6e6f 7420 4e6f  one_id is not No
+00009240: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00009250: 7265 7375 6c74 5b27 5a6f 6e65 4964 275d  result['ZoneId']
+00009260: 203d 2073 656c 662e 7a6f 6e65 5f69 640a   = self.zone_id.
+00009270: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00009280: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00009290: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+000092a0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+000092b0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+000092c0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000092d0: 2749 6d61 6765 4964 2729 2069 7320 6e6f  'ImageId') is no
+000092e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000092f0: 2020 2020 7365 6c66 2e69 6d61 6765 5f69      self.image_i
+00009300: 6420 3d20 6d2e 6765 7428 2749 6d61 6765  d = m.get('Image
+00009310: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+00009320: 6d2e 6765 7428 2749 6e74 6572 6e65 744d  m.get('InternetM
+00009330: 6178 4261 6e64 7769 6474 6849 6e27 2920  axBandwidthIn') 
+00009340: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00009350: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
+00009360: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
+00009370: 6964 7468 5f69 6e20 3d20 6d2e 6765 7428  idth_in = m.get(
+00009380: 2749 6e74 6572 6e65 744d 6178 4261 6e64  'InternetMaxBand
+00009390: 7769 6474 6849 6e27 290a 2020 2020 2020  widthIn').      
+000093a0: 2020 6966 206d 2e67 6574 2827 496e 7465    if m.get('Inte
+000093b0: 726e 6574 4d61 7842 616e 6477 6964 7468  rnetMaxBandwidth
+000093c0: 4f75 7427 2920 6973 206e 6f74 204e 6f6e  Out') is not Non
+000093d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000093e0: 656c 662e 696e 7465 726e 6574 5f6d 6178  elf.internet_max
+000093f0: 5f62 616e 6477 6964 7468 5f6f 7574 203d  _bandwidth_out =
+00009400: 206d 2e67 6574 2827 496e 7465 726e 6574   m.get('Internet
+00009410: 4d61 7842 616e 6477 6964 7468 4f75 7427  MaxBandwidthOut'
+00009420: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00009430: 6574 2827 4e61 6d65 2729 2069 7320 6e6f  et('Name') is no
+00009440: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00009450: 2020 2020 7365 6c66 2e6e 616d 6520 3d20      self.name = 
+00009460: 6d2e 6765 7428 274e 616d 6527 290a 2020  m.get('Name').  
+00009470: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00009480: 5061 7373 776f 7264 2729 2069 7320 6e6f  Password') is no
+00009490: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000094a0: 2020 2020 7365 6c66 2e70 6173 7377 6f72      self.passwor
+000094b0: 6420 3d20 6d2e 6765 7428 2750 6173 7377  d = m.get('Passw
+000094c0: 6f72 6427 290a 2020 2020 2020 2020 6966  ord').        if
+000094d0: 206d 2e67 6574 2827 5379 7374 656d 4469   m.get('SystemDi
+000094e0: 736b 4361 7465 676f 7279 2729 2069 7320  skCategory') is 
+000094f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00009500: 2020 2020 2020 7365 6c66 2e73 7973 7465        self.syste
+00009510: 6d5f 6469 736b 5f63 6174 6567 6f72 7920  m_disk_category 
+00009520: 3d20 6d2e 6765 7428 2753 7973 7465 6d44  = m.get('SystemD
+00009530: 6973 6b43 6174 6567 6f72 7927 290a 2020  iskCategory').  
+00009540: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00009550: 5379 7374 656d 4469 736b 5369 7a65 2729  SystemDiskSize')
+00009560: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00009570: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00009580: 7973 7465 6d5f 6469 736b 5f73 697a 6520  ystem_disk_size 
+00009590: 3d20 6d2e 6765 7428 2753 7973 7465 6d44  = m.get('SystemD
+000095a0: 6973 6b53 697a 6527 290a 2020 2020 2020  iskSize').      
+000095b0: 2020 6966 206d 2e67 6574 2827 5479 7065    if m.get('Type
+000095c0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000095d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000095e0: 2e74 7970 6520 3d20 6d2e 6765 7428 2754  .type = m.get('T
+000095f0: 7970 6527 290a 2020 2020 2020 2020 6966  ype').        if
+00009600: 206d 2e67 6574 2827 5a6f 6e65 4964 2729   m.get('ZoneId')
+00009610: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00009620: 2020 2020 2020 2020 2020 7365 6c66 2e7a            self.z
+00009630: 6f6e 655f 6964 203d 206d 2e67 6574 2827  one_id = m.get('
+00009640: 5a6f 6e65 4964 2729 0a20 2020 2020 2020  ZoneId').       
+00009650: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00009660: 6c61 7373 2043 7265 6174 6545 6169 4563  lass CreateEaiEc
+00009670: 7352 6571 7565 7374 2854 6561 4d6f 6465  sRequest(TeaMode
+00009680: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00009690: 6974 5f5f 2873 656c 662c 2063 6c69 656e  it__(self, clien
+000096a0: 745f 746f 6b65 6e3d 4e6f 6e65 2c20 6561  t_token=None, ea
+000096b0: 6973 5f6e 616d 653d 4e6f 6e65 2c20 6561  is_name=None, ea
+000096c0: 6973 5f74 7970 653d 4e6f 6e65 2c20 6563  is_type=None, ec
+000096d0: 733d 4e6f 6e65 2c20 7265 6769 6f6e 5f69  s=None, region_i
+000096e0: 643d 4e6f 6e65 2c0a 2020 2020 2020 2020  d=None,.        
+000096f0: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
+00009700: 655f 6772 6f75 705f 6964 3d4e 6f6e 652c  e_group_id=None,
+00009710: 2073 6563 7572 6974 795f 6772 6f75 705f   security_group_
+00009720: 6964 3d4e 6f6e 652c 2076 5f73 7769 7463  id=None, v_switc
+00009730: 685f 6964 3d4e 6f6e 6529 3a0a 2020 2020  h_id=None):.    
+00009740: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
+00009750: 746f 6b65 6e20 3d20 636c 6965 6e74 5f74  token = client_t
+00009760: 6f6b 656e 2020 2320 7479 7065 3a20 7374  oken  # type: st
+00009770: 720a 2020 2020 2020 2020 7365 6c66 2e65  r.        self.e
+00009780: 6169 735f 6e61 6d65 203d 2065 6169 735f  ais_name = eais_
+00009790: 6e61 6d65 2020 2320 7479 7065 3a20 7374  name  # type: st
+000097a0: 720a 2020 2020 2020 2020 7365 6c66 2e65  r.        self.e
+000097b0: 6169 735f 7479 7065 203d 2065 6169 735f  ais_type = eais_
+000097c0: 7479 7065 2020 2320 7479 7065 3a20 7374  type  # type: st
+000097d0: 720a 2020 2020 2020 2020 7365 6c66 2e65  r.        self.e
+000097e0: 6373 203d 2065 6373 2020 2320 7479 7065  cs = ecs  # type
+000097f0: 3a20 4372 6561 7465 4561 6945 6373 5265  : CreateEaiEcsRe
+00009800: 7175 6573 7445 6373 0a20 2020 2020 2020  questEcs.       
+00009810: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+00009820: 3d20 7265 6769 6f6e 5f69 6420 2023 2074  = region_id  # t
+00009830: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00009840: 2073 656c 662e 7265 736f 7572 6365 5f67   self.resource_g
+00009850: 726f 7570 5f69 6420 3d20 7265 736f 7572  roup_id = resour
+00009860: 6365 5f67 726f 7570 5f69 6420 2023 2074  ce_group_id  # t
+00009870: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00009880: 2073 656c 662e 7365 6375 7269 7479 5f67   self.security_g
+00009890: 726f 7570 5f69 6420 3d20 7365 6375 7269  roup_id = securi
+000098a0: 7479 5f67 726f 7570 5f69 6420 2023 2074  ty_group_id  # t
+000098b0: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+000098c0: 2073 656c 662e 765f 7377 6974 6368 5f69   self.v_switch_i
+000098d0: 6420 3d20 765f 7377 6974 6368 5f69 6420  d = v_switch_id 
+000098e0: 2023 2074 7970 653a 2073 7472 0a0a 2020   # type: str..  
+000098f0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00009900: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+00009910: 2073 656c 662e 6563 733a 0a20 2020 2020   self.ecs:.     
+00009920: 2020 2020 2020 2073 656c 662e 6563 732e         self.ecs.
+00009930: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+00009940: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00009950: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00009960: 2073 7570 6572 2843 7265 6174 6545 6169   super(CreateEai
+00009970: 4563 7352 6571 7565 7374 2c20 7365 6c66  EcsRequest, self
+00009980: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00009990: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+000099a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000099b0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+000099c0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000099d0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000099e0: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
+000099f0: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
+00009a00: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00009a10: 6573 756c 745b 2743 6c69 656e 7454 6f6b  esult['ClientTok
+00009a20: 656e 275d 203d 2073 656c 662e 636c 6965  en'] = self.clie
+00009a30: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
+00009a40: 2069 6620 7365 6c66 2e65 6169 735f 6e61   if self.eais_na
+00009a50: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+00009a60: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00009a70: 6c74 5b27 4561 6973 4e61 6d65 275d 203d  lt['EaisName'] =
+00009a80: 2073 656c 662e 6561 6973 5f6e 616d 650a   self.eais_name.
+00009a90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00009aa0: 6561 6973 5f74 7970 6520 6973 206e 6f74  eais_type is not
+00009ab0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00009ac0: 2020 2072 6573 756c 745b 2745 6169 7354     result['EaisT
+00009ad0: 7970 6527 5d20 3d20 7365 6c66 2e65 6169  ype'] = self.eai
+00009ae0: 735f 7479 7065 0a20 2020 2020 2020 2069  s_type.        i
+00009af0: 6620 7365 6c66 2e65 6373 2069 7320 6e6f  f self.ecs is no
+00009b00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00009b10: 2020 2020 7265 7375 6c74 5b27 4563 7327      result['Ecs'
+00009b20: 5d20 3d20 7365 6c66 2e65 6373 2e74 6f5f  ] = self.ecs.to_
+00009b30: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00009b40: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+00009b50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00009b60: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00009b70: 2752 6567 696f 6e49 6427 5d20 3d20 7365  'RegionId'] = se
+00009b80: 6c66 2e72 6567 696f 6e5f 6964 0a20 2020  lf.region_id.   
+00009b90: 2020 2020 2069 6620 7365 6c66 2e72 6573       if self.res
+00009ba0: 6f75 7263 655f 6772 6f75 705f 6964 2069  ource_group_id i
+00009bb0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00009bc0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00009bd0: 5265 736f 7572 6365 4772 6f75 7049 6427  ResourceGroupId'
+00009be0: 5d20 3d20 7365 6c66 2e72 6573 6f75 7263  ] = self.resourc
+00009bf0: 655f 6772 6f75 705f 6964 0a20 2020 2020  e_group_id.     
+00009c00: 2020 2069 6620 7365 6c66 2e73 6563 7572     if self.secur
+00009c10: 6974 795f 6772 6f75 705f 6964 2069 7320  ity_group_id is 
+00009c20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00009c30: 2020 2020 2020 7265 7375 6c74 5b27 5365        result['Se
+00009c40: 6375 7269 7479 4772 6f75 7049 6427 5d20  curityGroupId'] 
+00009c50: 3d20 7365 6c66 2e73 6563 7572 6974 795f  = self.security_
+00009c60: 6772 6f75 705f 6964 0a20 2020 2020 2020  group_id.       
+00009c70: 2069 6620 7365 6c66 2e76 5f73 7769 7463   if self.v_switc
+00009c80: 685f 6964 2069 7320 6e6f 7420 4e6f 6e65  h_id is not None
+00009c90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00009ca0: 7375 6c74 5b27 5653 7769 7463 6849 6427  sult['VSwitchId'
+00009cb0: 5d20 3d20 7365 6c66 2e76 5f73 7769 7463  ] = self.v_switc
+00009cc0: 685f 6964 0a20 2020 2020 2020 2072 6574  h_id.        ret
+00009cd0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00009ce0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00009cf0: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+00009d00: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00009d10: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00009d20: 2e67 6574 2827 436c 6965 6e74 546f 6b65  .get('ClientToke
+00009d30: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
+00009d40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009d50: 662e 636c 6965 6e74 5f74 6f6b 656e 203d  f.client_token =
+00009d60: 206d 2e67 6574 2827 436c 6965 6e74 546f   m.get('ClientTo
+00009d70: 6b65 6e27 290a 2020 2020 2020 2020 6966  ken').        if
+00009d80: 206d 2e67 6574 2827 4561 6973 4e61 6d65   m.get('EaisName
+00009d90: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00009da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009db0: 2e65 6169 735f 6e61 6d65 203d 206d 2e67  .eais_name = m.g
+00009dc0: 6574 2827 4561 6973 4e61 6d65 2729 0a20  et('EaisName'). 
+00009dd0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00009de0: 2745 6169 7354 7970 6527 2920 6973 206e  'EaisType') is n
+00009df0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00009e00: 2020 2020 2073 656c 662e 6561 6973 5f74       self.eais_t
+00009e10: 7970 6520 3d20 6d2e 6765 7428 2745 6169  ype = m.get('Eai
+00009e20: 7354 7970 6527 290a 2020 2020 2020 2020  sType').        
+00009e30: 6966 206d 2e67 6574 2827 4563 7327 2920  if m.get('Ecs') 
+00009e40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00009e50: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+00009e60: 6465 6c20 3d20 4372 6561 7465 4561 6945  del = CreateEaiE
+00009e70: 6373 5265 7175 6573 7445 6373 2829 0a20  csRequestEcs(). 
+00009e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009e90: 6563 7320 3d20 7465 6d70 5f6d 6f64 656c  ecs = temp_model
+00009ea0: 2e66 726f 6d5f 6d61 7028 6d5b 2745 6373  .from_map(m['Ecs
+00009eb0: 275d 290a 2020 2020 2020 2020 6966 206d  ']).        if m
+00009ec0: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
+00009ed0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00009ee0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00009ef0: 6567 696f 6e5f 6964 203d 206d 2e67 6574  egion_id = m.get
+00009f00: 2827 5265 6769 6f6e 4964 2729 0a20 2020  ('RegionId').   
+00009f10: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+00009f20: 6573 6f75 7263 6547 726f 7570 4964 2729  esourceGroupId')
+00009f30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00009f40: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00009f50: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
+00009f60: 203d 206d 2e67 6574 2827 5265 736f 7572   = m.get('Resour
+00009f70: 6365 4772 6f75 7049 6427 290a 2020 2020  ceGroupId').    
+00009f80: 2020 2020 6966 206d 2e67 6574 2827 5365      if m.get('Se
+00009f90: 6375 7269 7479 4772 6f75 7049 6427 2920  curityGroupId') 
+00009fa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00009fb0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00009fc0: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
+00009fd0: 3d20 6d2e 6765 7428 2753 6563 7572 6974  = m.get('Securit
+00009fe0: 7947 726f 7570 4964 2729 0a20 2020 2020  yGroupId').     
+00009ff0: 2020 2069 6620 6d2e 6765 7428 2756 5377     if m.get('VSw
+0000a000: 6974 6368 4964 2729 2069 7320 6e6f 7420  itchId') is not 
+0000a010: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000a020: 2020 7365 6c66 2e76 5f73 7769 7463 685f    self.v_switch_
+0000a030: 6964 203d 206d 2e67 6574 2827 5653 7769  id = m.get('VSwi
+0000a040: 7463 6849 6427 290a 2020 2020 2020 2020  tchId').        
+0000a050: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+0000a060: 6173 7320 4372 6561 7465 4561 6945 6373  ass CreateEaiEcs
+0000a070: 5368 7269 6e6b 5265 7175 6573 7428 5465  ShrinkRequest(Te
+0000a080: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0000a090: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0000a0a0: 636c 6965 6e74 5f74 6f6b 656e 3d4e 6f6e  client_token=Non
+0000a0b0: 652c 2065 6169 735f 6e61 6d65 3d4e 6f6e  e, eais_name=Non
+0000a0c0: 652c 2065 6169 735f 7479 7065 3d4e 6f6e  e, eais_type=Non
+0000a0d0: 652c 2065 6373 5f73 6872 696e 6b3d 4e6f  e, ecs_shrink=No
+0000a0e0: 6e65 2c20 7265 6769 6f6e 5f69 643d 4e6f  ne, region_id=No
+0000a0f0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0000a100: 2020 2020 2072 6573 6f75 7263 655f 6772       resource_gr
+0000a110: 6f75 705f 6964 3d4e 6f6e 652c 2073 6563  oup_id=None, sec
+0000a120: 7572 6974 795f 6772 6f75 705f 6964 3d4e  urity_group_id=N
+0000a130: 6f6e 652c 2076 5f73 7769 7463 685f 6964  one, v_switch_id
+0000a140: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0000a150: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
+0000a160: 6e20 3d20 636c 6965 6e74 5f74 6f6b 656e  n = client_token
+0000a170: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+0000a180: 2020 2020 2020 7365 6c66 2e65 6169 735f        self.eais_
+0000a190: 6e61 6d65 203d 2065 6169 735f 6e61 6d65  name = eais_name
+0000a1a0: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+0000a1b0: 2020 2020 2020 7365 6c66 2e65 6169 735f        self.eais_
+0000a1c0: 7479 7065 203d 2065 6169 735f 7479 7065  type = eais_type
+0000a1d0: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+0000a1e0: 2020 2020 2020 7365 6c66 2e65 6373 5f73        self.ecs_s
+0000a1f0: 6872 696e 6b20 3d20 6563 735f 7368 7269  hrink = ecs_shri
+0000a200: 6e6b 2020 2320 7479 7065 3a20 7374 720a  nk  # type: str.
+0000a210: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
+0000a220: 696f 6e5f 6964 203d 2072 6567 696f 6e5f  ion_id = region_
+0000a230: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+0000a240: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+0000a250: 6f75 7263 655f 6772 6f75 705f 6964 203d  ource_group_id =
+0000a260: 2072 6573 6f75 7263 655f 6772 6f75 705f   resource_group_
+0000a270: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+0000a280: 2020 2020 2020 2020 7365 6c66 2e73 6563          self.sec
+0000a290: 7572 6974 795f 6772 6f75 705f 6964 203d  urity_group_id =
+0000a2a0: 2073 6563 7572 6974 795f 6772 6f75 705f   security_group_
+0000a2b0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+0000a2c0: 2020 2020 2020 2020 7365 6c66 2e76 5f73          self.v_s
+0000a2d0: 7769 7463 685f 6964 203d 2076 5f73 7769  witch_id = v_swi
+0000a2e0: 7463 685f 6964 2020 2320 7479 7065 3a20  tch_id  # type: 
+0000a2f0: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
+0000a300: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0000a310: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+0000a320: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0000a330: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0000a340: 7375 7065 7228 4372 6561 7465 4561 6945  super(CreateEaiE
+0000a350: 6373 5368 7269 6e6b 5265 7175 6573 742c  csShrinkRequest,
+0000a360: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
+0000a370: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+0000a380: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000a390: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000a3a0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+0000a3b0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+0000a3c0: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
+0000a3d0: 6965 6e74 5f74 6f6b 656e 2069 7320 6e6f  ient_token is no
+0000a3e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000a3f0: 2020 2020 7265 7375 6c74 5b27 436c 6965      result['Clie
+0000a400: 6e74 546f 6b65 6e27 5d20 3d20 7365 6c66  ntToken'] = self
+0000a410: 2e63 6c69 656e 745f 746f 6b65 6e0a 2020  .client_token.  
+0000a420: 2020 2020 2020 6966 2073 656c 662e 6561        if self.ea
+0000a430: 6973 5f6e 616d 6520 6973 206e 6f74 204e  is_name is not N
+0000a440: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000a450: 2072 6573 756c 745b 2745 6169 734e 616d   result['EaisNam
+0000a460: 6527 5d20 3d20 7365 6c66 2e65 6169 735f  e'] = self.eais_
+0000a470: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
+0000a480: 7365 6c66 2e65 6169 735f 7479 7065 2069  self.eais_type i
+0000a490: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000a4a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0000a4b0: 4561 6973 5479 7065 275d 203d 2073 656c  EaisType'] = sel
+0000a4c0: 662e 6561 6973 5f74 7970 650a 2020 2020  f.eais_type.    
+0000a4d0: 2020 2020 6966 2073 656c 662e 6563 735f      if self.ecs_
+0000a4e0: 7368 7269 6e6b 2069 7320 6e6f 7420 4e6f  shrink is not No
+0000a4f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000a500: 7265 7375 6c74 5b27 4563 7327 5d20 3d20  result['Ecs'] = 
+0000a510: 7365 6c66 2e65 6373 5f73 6872 696e 6b0a  self.ecs_shrink.
+0000a520: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000a530: 7265 6769 6f6e 5f69 6420 6973 206e 6f74  region_id is not
+0000a540: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000a550: 2020 2072 6573 756c 745b 2752 6567 696f     result['Regio
+0000a560: 6e49 6427 5d20 3d20 7365 6c66 2e72 6567  nId'] = self.reg
+0000a570: 696f 6e5f 6964 0a20 2020 2020 2020 2069  ion_id.        i
+0000a580: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
+0000a590: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
+0000a5a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000a5b0: 2020 7265 7375 6c74 5b27 5265 736f 7572    result['Resour
+0000a5c0: 6365 4772 6f75 7049 6427 5d20 3d20 7365  ceGroupId'] = se
+0000a5d0: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
+0000a5e0: 705f 6964 0a20 2020 2020 2020 2069 6620  p_id.        if 
+0000a5f0: 7365 6c66 2e73 6563 7572 6974 795f 6772  self.security_gr
+0000a600: 6f75 705f 6964 2069 7320 6e6f 7420 4e6f  oup_id is not No
+0000a610: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000a620: 7265 7375 6c74 5b27 5365 6375 7269 7479  result['Security
+0000a630: 4772 6f75 7049 6427 5d20 3d20 7365 6c66  GroupId'] = self
+0000a640: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
+0000a650: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+0000a660: 6c66 2e76 5f73 7769 7463 685f 6964 2069  lf.v_switch_id i
+0000a670: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000a680: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0000a690: 5653 7769 7463 6849 6427 5d20 3d20 7365  VSwitchId'] = se
+0000a6a0: 6c66 2e76 5f73 7769 7463 685f 6964 0a20  lf.v_switch_id. 
+0000a6b0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000a6c0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0000a6d0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+0000a6e0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+0000a6f0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+0000a700: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0000a710: 436c 6965 6e74 546f 6b65 6e27 2920 6973  ClientToken') is
+0000a720: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000a730: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+0000a740: 6e74 5f74 6f6b 656e 203d 206d 2e67 6574  nt_token = m.get
+0000a750: 2827 436c 6965 6e74 546f 6b65 6e27 290a  ('ClientToken').
+0000a760: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0000a770: 2827 4561 6973 4e61 6d65 2729 2069 7320  ('EaisName') is 
+0000a780: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000a790: 2020 2020 2020 7365 6c66 2e65 6169 735f        self.eais_
+0000a7a0: 6e61 6d65 203d 206d 2e67 6574 2827 4561  name = m.get('Ea
+0000a7b0: 6973 4e61 6d65 2729 0a20 2020 2020 2020  isName').       
+0000a7c0: 2069 6620 6d2e 6765 7428 2745 6169 7354   if m.get('EaisT
+0000a7d0: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
+0000a7e0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000a7f0: 656c 662e 6561 6973 5f74 7970 6520 3d20  elf.eais_type = 
+0000a800: 6d2e 6765 7428 2745 6169 7354 7970 6527  m.get('EaisType'
+0000a810: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0000a820: 6574 2827 4563 7327 2920 6973 206e 6f74  et('Ecs') is not
+0000a830: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000a840: 2020 2073 656c 662e 6563 735f 7368 7269     self.ecs_shri
+0000a850: 6e6b 203d 206d 2e67 6574 2827 4563 7327  nk = m.get('Ecs'
+0000a860: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0000a870: 6574 2827 5265 6769 6f6e 4964 2729 2069  et('RegionId') i
+0000a880: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000a890: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
+0000a8a0: 696f 6e5f 6964 203d 206d 2e67 6574 2827  ion_id = m.get('
+0000a8b0: 5265 6769 6f6e 4964 2729 0a20 2020 2020  RegionId').     
+0000a8c0: 2020 2069 6620 6d2e 6765 7428 2752 6573     if m.get('Res
+0000a8d0: 6f75 7263 6547 726f 7570 4964 2729 2069  ourceGroupId') i
+0000a8e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000a8f0: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+0000a900: 6f75 7263 655f 6772 6f75 705f 6964 203d  ource_group_id =
+0000a910: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+0000a920: 4772 6f75 7049 6427 290a 2020 2020 2020  GroupId').      
+0000a930: 2020 6966 206d 2e67 6574 2827 5365 6375    if m.get('Secu
+0000a940: 7269 7479 4772 6f75 7049 6427 2920 6973  rityGroupId') is
+0000a950: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000a960: 2020 2020 2020 2073 656c 662e 7365 6375         self.secu
+0000a970: 7269 7479 5f67 726f 7570 5f69 6420 3d20  rity_group_id = 
+0000a980: 6d2e 6765 7428 2753 6563 7572 6974 7947  m.get('SecurityG
+0000a990: 726f 7570 4964 2729 0a20 2020 2020 2020  roupId').       
+0000a9a0: 2069 6620 6d2e 6765 7428 2756 5377 6974   if m.get('VSwit
+0000a9b0: 6368 4964 2729 2069 7320 6e6f 7420 4e6f  chId') is not No
+0000a9c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000a9d0: 7365 6c66 2e76 5f73 7769 7463 685f 6964  self.v_switch_id
+0000a9e0: 203d 206d 2e67 6574 2827 5653 7769 7463   = m.get('VSwitc
+0000a9f0: 6849 6427 290a 2020 2020 2020 2020 7265  hId').        re
+0000aa00: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0000aa10: 7320 4372 6561 7465 4561 6945 6373 5265  s CreateEaiEcsRe
+0000aa20: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
+0000aa30: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+0000aa40: 696e 6974 5f5f 2873 656c 662c 2063 6c69  init__(self, cli
+0000aa50: 656e 745f 696e 7374 616e 6365 5f69 643d  ent_instance_id=
+0000aa60: 4e6f 6e65 2c20 656c 6173 7469 635f 6163  None, elastic_ac
+0000aa70: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+0000aa80: 6365 5f69 643d 4e6f 6e65 2c20 7265 7175  ce_id=None, requ
+0000aa90: 6573 745f 6964 3d4e 6f6e 6529 3a0a 2020  est_id=None):.  
+0000aaa0: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
+0000aab0: 745f 696e 7374 616e 6365 5f69 6420 3d20  t_instance_id = 
+0000aac0: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
+0000aad0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+0000aae0: 2020 2020 2020 2020 7365 6c66 2e65 6c61          self.ela
+0000aaf0: 7374 6963 5f61 6363 656c 6572 6174 6564  stic_accelerated
+0000ab00: 5f69 6e73 7461 6e63 655f 6964 203d 2065  _instance_id = e
+0000ab10: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+0000ab20: 6564 5f69 6e73 7461 6e63 655f 6964 2020  ed_instance_id  
+0000ab30: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+0000ab40: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+0000ab50: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
+0000ab60: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
+0000ab70: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0000ab80: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+0000ab90: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+0000aba0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+0000abb0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+0000abc0: 4372 6561 7465 4561 6945 6373 5265 7370  CreateEaiEcsResp
+0000abd0: 6f6e 7365 426f 6479 2c20 7365 6c66 292e  onseBody, self).
+0000abe0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0000abf0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0000ac00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000ac10: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0000ac20: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000ac30: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0000ac40: 6620 7365 6c66 2e63 6c69 656e 745f 696e  f self.client_in
+0000ac50: 7374 616e 6365 5f69 6420 6973 206e 6f74  stance_id is not
+0000ac60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000ac70: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
+0000ac80: 7449 6e73 7461 6e63 6549 6427 5d20 3d20  tInstanceId'] = 
+0000ac90: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
+0000aca0: 616e 6365 5f69 640a 2020 2020 2020 2020  ance_id.        
+0000acb0: 6966 2073 656c 662e 656c 6173 7469 635f  if self.elastic_
+0000acc0: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
+0000acd0: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
+0000ace0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000acf0: 2072 6573 756c 745b 2745 6c61 7374 6963   result['Elastic
+0000ad00: 4163 6365 6c65 7261 7465 6449 6e73 7461  AcceleratedInsta
+0000ad10: 6e63 6549 6427 5d20 3d20 7365 6c66 2e65  nceId'] = self.e
+0000ad20: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+0000ad30: 6564 5f69 6e73 7461 6e63 655f 6964 0a20  ed_instance_id. 
+0000ad40: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000ad50: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
+0000ad60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000ad70: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
+0000ad80: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
+0000ad90: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+0000ada0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0000adb0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+0000adc0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+0000add0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0000ade0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0000adf0: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
+0000ae00: 496e 7374 616e 6365 4964 2729 2069 7320  InstanceId') is 
+0000ae10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000ae20: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
+0000ae30: 745f 696e 7374 616e 6365 5f69 6420 3d20  t_instance_id = 
+0000ae40: 6d2e 6765 7428 2743 6c69 656e 7449 6e73  m.get('ClientIns
+0000ae50: 7461 6e63 6549 6427 290a 2020 2020 2020  tanceId').      
+0000ae60: 2020 6966 206d 2e67 6574 2827 456c 6173    if m.get('Elas
+0000ae70: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
+0000ae80: 7374 616e 6365 4964 2729 2069 7320 6e6f  stanceId') is no
+0000ae90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000aea0: 2020 2020 7365 6c66 2e65 6c61 7374 6963      self.elastic
+0000aeb0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+0000aec0: 7461 6e63 655f 6964 203d 206d 2e67 6574  tance_id = m.get
+0000aed0: 2827 456c 6173 7469 6341 6363 656c 6572  ('ElasticAcceler
+0000aee0: 6174 6564 496e 7374 616e 6365 4964 2729  atedInstanceId')
+0000aef0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0000af00: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
+0000af10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000af20: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+0000af30: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
+0000af40: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
+0000af50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000af60: 0a0a 0a63 6c61 7373 2043 7265 6174 6545  ...class CreateE
+0000af70: 6169 4563 7352 6573 706f 6e73 6528 5465  aiEcsResponse(Te
+0000af80: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0000af90: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0000afa0: 6865 6164 6572 733d 4e6f 6e65 2c20 7374  headers=None, st
+0000afb0: 6174 7573 5f63 6f64 653d 4e6f 6e65 2c20  atus_code=None, 
+0000afc0: 626f 6479 3d4e 6f6e 6529 3a0a 2020 2020  body=None):.    
+0000afd0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+0000afe0: 203d 2068 6561 6465 7273 2020 2320 7479   = headers  # ty
+0000aff0: 7065 3a20 6469 6374 5b73 7472 2c20 7374  pe: dict[str, st
+0000b000: 725d 0a20 2020 2020 2020 2073 656c 662e  r].        self.
+0000b010: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+0000b020: 6174 7573 5f63 6f64 6520 2023 2074 7970  atus_code  # typ
+0000b030: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
+0000b040: 656c 662e 626f 6479 203d 2062 6f64 7920  elf.body = body 
+0000b050: 2023 2074 7970 653a 2043 7265 6174 6545   # type: CreateE
+0000b060: 6169 4563 7352 6573 706f 6e73 6542 6f64  aiEcsResponseBod
+0000b070: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+0000b080: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+0000b090: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+0000b0a0: 5f72 6571 7569 7265 6428 7365 6c66 2e68  _required(self.h
+0000b0b0: 6561 6465 7273 2c20 2768 6561 6465 7273  eaders, 'headers
+0000b0c0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0000b0d0: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+0000b0e0: 6428 7365 6c66 2e73 7461 7475 735f 636f  d(self.status_co
+0000b0f0: 6465 2c20 2773 7461 7475 735f 636f 6465  de, 'status_code
+0000b100: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0000b110: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+0000b120: 6428 7365 6c66 2e62 6f64 792c 2027 626f  d(self.body, 'bo
+0000b130: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
+0000b140: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+0000b150: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0000b160: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+0000b170: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0000b180: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0000b190: 3d20 7375 7065 7228 4372 6561 7465 4561  = super(CreateEa
+0000b1a0: 6945 6373 5265 7370 6f6e 7365 2c20 7365  iEcsResponse, se
+0000b1b0: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+0000b1c0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0000b1d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000b1e0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0000b1f0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0000b200: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0000b210: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
+0000b220: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
+0000b230: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000b240: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
+0000b250: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
+0000b260: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+0000b270: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
+0000b280: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000b290: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
+0000b2a0: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
+0000b2b0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+0000b2c0: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
+0000b2d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000b2e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0000b2f0: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
+0000b300: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
+0000b310: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0000b320: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+0000b330: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
+0000b340: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0000b350: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0000b360: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
+0000b370: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
+0000b380: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000b390: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
+0000b3a0: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
+0000b3b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0000b3c0: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
+0000b3d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000b3e0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000b3f0: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
+0000b400: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
+0000b410: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0000b420: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+0000b430: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000b440: 2074 656d 705f 6d6f 6465 6c20 3d20 4372   temp_model = Cr
+0000b450: 6561 7465 4561 6945 6373 5265 7370 6f6e  eateEaiEcsRespon
+0000b460: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
+0000b470: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+0000b480: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+0000b490: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+0000b4a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000b4b0: 656c 660a 0a0a 636c 6173 7320 4372 6561  elf...class Crea
+0000b4c0: 7465 4561 694a 7570 7974 6572 5265 7175  teEaiJupyterRequ
+0000b4d0: 6573 7445 6e76 6972 6f6e 6d65 6e74 5661  estEnvironmentVa
+0000b4e0: 7228 5465 614d 6f64 656c 293a 0a20 2020  r(TeaModel):.   
+0000b4f0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0000b500: 6c66 2c20 6b65 793d 4e6f 6e65 2c20 7661  lf, key=None, va
+0000b510: 6c75 653d 4e6f 6e65 293a 0a20 2020 2020  lue=None):.     
+0000b520: 2020 2073 656c 662e 6b65 7920 3d20 6b65     self.key = ke
+0000b530: 7920 2023 2074 7970 653a 2073 7472 0a20  y  # type: str. 
+0000b540: 2020 2020 2020 2073 656c 662e 7661 6c75         self.valu
+0000b550: 6520 3d20 7661 6c75 6520 2023 2074 7970  e = value  # typ
+0000b560: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
+0000b570: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+0000b580: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0000b590: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0000b5a0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0000b5b0: 203d 2073 7570 6572 2843 7265 6174 6545   = super(CreateE
+0000b5c0: 6169 4a75 7079 7465 7252 6571 7565 7374  aiJupyterRequest
+0000b5d0: 456e 7669 726f 6e6d 656e 7456 6172 2c20  EnvironmentVar, 
+0000b5e0: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+0000b5f0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0000b600: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000b610: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0000b620: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0000b630: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0000b640: 2020 2020 2069 6620 7365 6c66 2e6b 6579       if self.key
+0000b650: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000b660: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000b670: 5b27 4b65 7927 5d20 3d20 7365 6c66 2e6b  ['Key'] = self.k
+0000b680: 6579 0a20 2020 2020 2020 2069 6620 7365  ey.        if se
+0000b690: 6c66 2e76 616c 7565 2069 7320 6e6f 7420  lf.value is not 
+0000b6a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000b6b0: 2020 7265 7375 6c74 5b27 5661 6c75 6527    result['Value'
+0000b6c0: 5d20 3d20 7365 6c66 2e76 616c 7565 0a20  ] = self.value. 
+0000b6d0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000b6e0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0000b6f0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+0000b700: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+0000b710: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+0000b720: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0000b730: 4b65 7927 2920 6973 206e 6f74 204e 6f6e  Key') is not Non
+0000b740: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000b750: 656c 662e 6b65 7920 3d20 6d2e 6765 7428  elf.key = m.get(
+0000b760: 274b 6579 2729 0a20 2020 2020 2020 2069  'Key').        i
+0000b770: 6620 6d2e 6765 7428 2756 616c 7565 2729  f m.get('Value')
+0000b780: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000b790: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+0000b7a0: 616c 7565 203d 206d 2e67 6574 2827 5661  alue = m.get('Va
+0000b7b0: 6c75 6527 290a 2020 2020 2020 2020 7265  lue').        re
+0000b7c0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0000b7d0: 7320 4372 6561 7465 4561 694a 7570 7974  s CreateEaiJupyt
+0000b7e0: 6572 5265 7175 6573 7428 5465 614d 6f64  erRequest(TeaMod
+0000b7f0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+0000b800: 6e69 745f 5f28 7365 6c66 2c20 636c 6965  nit__(self, clie
+0000b810: 6e74 5f74 6f6b 656e 3d4e 6f6e 652c 2065  nt_token=None, e
+0000b820: 6169 735f 6e61 6d65 3d4e 6f6e 652c 2065  ais_name=None, e
+0000b830: 6169 735f 7479 7065 3d4e 6f6e 652c 2065  ais_type=None, e
+0000b840: 6e76 6972 6f6e 6d65 6e74 5f76 6172 3d4e  nvironment_var=N
+0000b850: 6f6e 652c 2072 6567 696f 6e5f 6964 3d4e  one, region_id=N
+0000b860: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0000b870: 2020 2020 2020 7265 736f 7572 6365 5f67        resource_g
+0000b880: 726f 7570 5f69 643d 4e6f 6e65 2c20 7365  roup_id=None, se
+0000b890: 6375 7269 7479 5f67 726f 7570 5f69 643d  curity_group_id=
+0000b8a0: 4e6f 6e65 2c20 765f 7377 6974 6368 5f69  None, v_switch_i
+0000b8b0: 643d 4e6f 6e65 293a 0a20 2020 2020 2020  d=None):.       
+0000b8c0: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+0000b8d0: 656e 203d 2063 6c69 656e 745f 746f 6b65  en = client_toke
+0000b8e0: 6e20 2023 2074 7970 653a 2073 7472 0a20  n  # type: str. 
+0000b8f0: 2020 2020 2020 2073 656c 662e 6561 6973         self.eais
+0000b900: 5f6e 616d 6520 3d20 6561 6973 5f6e 616d  _name = eais_nam
+0000b910: 6520 2023 2074 7970 653a 2073 7472 0a20  e  # type: str. 
+0000b920: 2020 2020 2020 2073 656c 662e 6561 6973         self.eais
+0000b930: 5f74 7970 6520 3d20 6561 6973 5f74 7970  _type = eais_typ
+0000b940: 6520 2023 2074 7970 653a 2073 7472 0a20  e  # type: str. 
+0000b950: 2020 2020 2020 2073 656c 662e 656e 7669         self.envi
+0000b960: 726f 6e6d 656e 745f 7661 7220 3d20 656e  ronment_var = en
+0000b970: 7669 726f 6e6d 656e 745f 7661 7220 2023  vironment_var  #
+0000b980: 2074 7970 653a 206c 6973 745b 4372 6561   type: list[Crea
+0000b990: 7465 4561 694a 7570 7974 6572 5265 7175  teEaiJupyterRequ
+0000b9a0: 6573 7445 6e76 6972 6f6e 6d65 6e74 5661  estEnvironmentVa
+0000b9b0: 725d 0a20 2020 2020 2020 2073 656c 662e  r].        self.
+0000b9c0: 7265 6769 6f6e 5f69 6420 3d20 7265 6769  region_id = regi
+0000b9d0: 6f6e 5f69 6420 2023 2074 7970 653a 2073  on_id  # type: s
+0000b9e0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+0000b9f0: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
+0000ba00: 6420 3d20 7265 736f 7572 6365 5f67 726f  d = resource_gro
+0000ba10: 7570 5f69 6420 2023 2074 7970 653a 2073  up_id  # type: s
+0000ba20: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+0000ba30: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
+0000ba40: 6420 3d20 7365 6375 7269 7479 5f67 726f  d = security_gro
+0000ba50: 7570 5f69 6420 2023 2074 7970 653a 2073  up_id  # type: s
+0000ba60: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+0000ba70: 765f 7377 6974 6368 5f69 6420 3d20 765f  v_switch_id = v_
+0000ba80: 7377 6974 6368 5f69 6420 2023 2074 7970  switch_id  # typ
+0000ba90: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
+0000baa0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+0000bab0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000bac0: 656e 7669 726f 6e6d 656e 745f 7661 723a  environment_var:
+0000bad0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000bae0: 206b 2069 6e20 7365 6c66 2e65 6e76 6972   k in self.envir
+0000baf0: 6f6e 6d65 6e74 5f76 6172 3a0a 2020 2020  onment_var:.    
+0000bb00: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+0000bb10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bb20: 2020 2020 2020 6b2e 7661 6c69 6461 7465        k.validate
+0000bb30: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+0000bb40: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+0000bb50: 2020 5f6d 6170 203d 2073 7570 6572 2843    _map = super(C
+0000bb60: 7265 6174 6545 6169 4a75 7079 7465 7252  reateEaiJupyterR
+0000bb70: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
+0000bb80: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0000bb90: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0000bba0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000bbb0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0000bbc0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0000bbd0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0000bbe0: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
+0000bbf0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+0000bc00: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0000bc10: 745b 2743 6c69 656e 7454 6f6b 656e 275d  t['ClientToken']
+0000bc20: 203d 2073 656c 662e 636c 6965 6e74 5f74   = self.client_t
+0000bc30: 6f6b 656e 0a20 2020 2020 2020 2069 6620  oken.        if 
+0000bc40: 7365 6c66 2e65 6169 735f 6e61 6d65 2069  self.eais_name i
+0000bc50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000bc60: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0000bc70: 4561 6973 4e61 6d65 275d 203d 2073 656c  EaisName'] = sel
+0000bc80: 662e 6561 6973 5f6e 616d 650a 2020 2020  f.eais_name.    
+0000bc90: 2020 2020 6966 2073 656c 662e 6561 6973      if self.eais
+0000bca0: 5f74 7970 6520 6973 206e 6f74 204e 6f6e  _type is not Non
+0000bcb0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000bcc0: 6573 756c 745b 2745 6169 7354 7970 6527  esult['EaisType'
+0000bcd0: 5d20 3d20 7365 6c66 2e65 6169 735f 7479  ] = self.eais_ty
+0000bce0: 7065 0a20 2020 2020 2020 2072 6573 756c  pe.        resul
+0000bcf0: 745b 2745 6e76 6972 6f6e 6d65 6e74 5661  t['EnvironmentVa
+0000bd00: 7227 5d20 3d20 5b5d 0a20 2020 2020 2020  r'] = [].       
+0000bd10: 2069 6620 7365 6c66 2e65 6e76 6972 6f6e   if self.environ
+0000bd20: 6d65 6e74 5f76 6172 2069 7320 6e6f 7420  ment_var is not 
+0000bd30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000bd40: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
+0000bd50: 656e 7669 726f 6e6d 656e 745f 7661 723a  environment_var:
+0000bd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bd70: 2072 6573 756c 745b 2745 6e76 6972 6f6e   result['Environ
+0000bd80: 6d65 6e74 5661 7227 5d2e 6170 7065 6e64  mentVar'].append
+0000bd90: 286b 2e74 6f5f 6d61 7028 2920 6966 206b  (k.to_map() if k
+0000bda0: 2065 6c73 6520 4e6f 6e65 290a 2020 2020   else None).    
+0000bdb0: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
+0000bdc0: 6f6e 5f69 6420 6973 206e 6f74 204e 6f6e  on_id is not Non
+0000bdd0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000bde0: 6573 756c 745b 2752 6567 696f 6e49 6427  esult['RegionId'
+0000bdf0: 5d20 3d20 7365 6c66 2e72 6567 696f 6e5f  ] = self.region_
+0000be00: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+0000be10: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
+0000be20: 705f 6964 2069 7320 6e6f 7420 4e6f 6e65  p_id is not None
+0000be30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000be40: 7375 6c74 5b27 5265 736f 7572 6365 4772  sult['ResourceGr
+0000be50: 6f75 7049 6427 5d20 3d20 7365 6c66 2e72  oupId'] = self.r
+0000be60: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
+0000be70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000be80: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
+0000be90: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0000bea0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000beb0: 6c74 5b27 5365 6375 7269 7479 4772 6f75  lt['SecurityGrou
+0000bec0: 7049 6427 5d20 3d20 7365 6c66 2e73 6563  pId'] = self.sec
+0000bed0: 7572 6974 795f 6772 6f75 705f 6964 0a20  urity_group_id. 
+0000bee0: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+0000bef0: 5f73 7769 7463 685f 6964 2069 7320 6e6f  _switch_id is no
+0000bf00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000bf10: 2020 2020 7265 7375 6c74 5b27 5653 7769      result['VSwi
+0000bf20: 7463 6849 6427 5d20 3d20 7365 6c66 2e76  tchId'] = self.v
+0000bf30: 5f73 7769 7463 685f 6964 0a20 2020 2020  _switch_id.     
+0000bf40: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0000bf50: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0000bf60: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+0000bf70: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0000bf80: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0000bf90: 2020 6966 206d 2e67 6574 2827 436c 6965    if m.get('Clie
+0000bfa0: 6e74 546f 6b65 6e27 2920 6973 206e 6f74  ntToken') is not
+0000bfb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000bfc0: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
+0000bfd0: 6f6b 656e 203d 206d 2e67 6574 2827 436c  oken = m.get('Cl
+0000bfe0: 6965 6e74 546f 6b65 6e27 290a 2020 2020  ientToken').    
+0000bff0: 2020 2020 6966 206d 2e67 6574 2827 4561      if m.get('Ea
+0000c000: 6973 4e61 6d65 2729 2069 7320 6e6f 7420  isName') is not 
+0000c010: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000c020: 2020 7365 6c66 2e65 6169 735f 6e61 6d65    self.eais_name
+0000c030: 203d 206d 2e67 6574 2827 4561 6973 4e61   = m.get('EaisNa
+0000c040: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
+0000c050: 6d2e 6765 7428 2745 6169 7354 7970 6527  m.get('EaisType'
+0000c060: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0000c070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c080: 6561 6973 5f74 7970 6520 3d20 6d2e 6765  eais_type = m.ge
+0000c090: 7428 2745 6169 7354 7970 6527 290a 2020  t('EaisType').  
+0000c0a0: 2020 2020 2020 7365 6c66 2e65 6e76 6972        self.envir
+0000c0b0: 6f6e 6d65 6e74 5f76 6172 203d 205b 5d0a  onment_var = [].
+0000c0c0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0000c0d0: 2827 456e 7669 726f 6e6d 656e 7456 6172  ('EnvironmentVar
+0000c0e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0000c0f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000c100: 6b20 696e 206d 2e67 6574 2827 456e 7669  k in m.get('Envi
+0000c110: 726f 6e6d 656e 7456 6172 2729 3a0a 2020  ronmentVar'):.  
+0000c120: 2020 2020 2020 2020 2020 2020 2020 7465                te
+0000c130: 6d70 5f6d 6f64 656c 203d 2043 7265 6174  mp_model = Creat
+0000c140: 6545 6169 4a75 7079 7465 7252 6571 7565  eEaiJupyterReque
+0000c150: 7374 456e 7669 726f 6e6d 656e 7456 6172  stEnvironmentVar
+0000c160: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000c170: 2020 2073 656c 662e 656e 7669 726f 6e6d     self.environm
+0000c180: 656e 745f 7661 722e 6170 7065 6e64 2874  ent_var.append(t
+0000c190: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+0000c1a0: 6170 286b 2929 0a20 2020 2020 2020 2069  ap(k)).        i
+0000c1b0: 6620 6d2e 6765 7428 2752 6567 696f 6e49  f m.get('RegionI
+0000c1c0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0000c1d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c1e0: 662e 7265 6769 6f6e 5f69 6420 3d20 6d2e  f.region_id = m.
+0000c1f0: 6765 7428 2752 6567 696f 6e49 6427 290a  get('RegionId').
+0000c200: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0000c210: 2827 5265 736f 7572 6365 4772 6f75 7049  ('ResourceGroupI
+0000c220: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0000c230: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000c240: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
+0000c250: 5f69 6420 3d20 6d2e 6765 7428 2752 6573  _id = m.get('Res
+0000c260: 6f75 7263 6547 726f 7570 4964 2729 0a20  ourceGroupId'). 
+0000c270: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0000c280: 2753 6563 7572 6974 7947 726f 7570 4964  'SecurityGroupId
+0000c290: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0000c2a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c2b0: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
+0000c2c0: 6964 203d 206d 2e67 6574 2827 5365 6375  id = m.get('Secu
+0000c2d0: 7269 7479 4772 6f75 7049 6427 290a 2020  rityGroupId').  
+0000c2e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0000c2f0: 5653 7769 7463 6849 6427 2920 6973 206e  VSwitchId') is n
+0000c300: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000c310: 2020 2020 2073 656c 662e 765f 7377 6974       self.v_swit
+0000c320: 6368 5f69 6420 3d20 6d2e 6765 7428 2756  ch_id = m.get('V
+0000c330: 5377 6974 6368 4964 2729 0a20 2020 2020  SwitchId').     
+0000c340: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0000c350: 0a63 6c61 7373 2043 7265 6174 6545 6169  .class CreateEai
+0000c360: 4a75 7079 7465 7253 6872 696e 6b52 6571  JupyterShrinkReq
+0000c370: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+0000c380: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000c390: 2873 656c 662c 2063 6c69 656e 745f 746f  (self, client_to
+0000c3a0: 6b65 6e3d 4e6f 6e65 2c20 6561 6973 5f6e  ken=None, eais_n
+0000c3b0: 616d 653d 4e6f 6e65 2c20 6561 6973 5f74  ame=None, eais_t
+0000c3c0: 7970 653d 4e6f 6e65 2c20 656e 7669 726f  ype=None, enviro
+0000c3d0: 6e6d 656e 745f 7661 725f 7368 7269 6e6b  nment_var_shrink
+0000c3e0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0000c3f0: 2020 2020 2020 2020 7265 6769 6f6e 5f69          region_i
+0000c400: 643d 4e6f 6e65 2c20 7265 736f 7572 6365  d=None, resource
+0000c410: 5f67 726f 7570 5f69 643d 4e6f 6e65 2c20  _group_id=None, 
+0000c420: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
+0000c430: 643d 4e6f 6e65 2c20 765f 7377 6974 6368  d=None, v_switch
+0000c440: 5f69 643d 4e6f 6e65 293a 0a20 2020 2020  _id=None):.     
+0000c450: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
+0000c460: 6f6b 656e 203d 2063 6c69 656e 745f 746f  oken = client_to
+0000c470: 6b65 6e20 2023 2074 7970 653a 2073 7472  ken  # type: str
+0000c480: 0a20 2020 2020 2020 2073 656c 662e 6561  .        self.ea
+0000c490: 6973 5f6e 616d 6520 3d20 6561 6973 5f6e  is_name = eais_n
+0000c4a0: 616d 6520 2023 2074 7970 653a 2073 7472  ame  # type: str
+0000c4b0: 0a20 2020 2020 2020 2073 656c 662e 6561  .        self.ea
+0000c4c0: 6973 5f74 7970 6520 3d20 6561 6973 5f74  is_type = eais_t
+0000c4d0: 7970 6520 2023 2074 7970 653a 2073 7472  ype  # type: str
+0000c4e0: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
+0000c4f0: 7669 726f 6e6d 656e 745f 7661 725f 7368  vironment_var_sh
+0000c500: 7269 6e6b 203d 2065 6e76 6972 6f6e 6d65  rink = environme
+0000c510: 6e74 5f76 6172 5f73 6872 696e 6b20 2023  nt_var_shrink  #
+0000c520: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
+0000c530: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
+0000c540: 6420 3d20 7265 6769 6f6e 5f69 6420 2023  d = region_id  #
+0000c550: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
+0000c560: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
+0000c570: 5f67 726f 7570 5f69 6420 3d20 7265 736f  _group_id = reso
+0000c580: 7572 6365 5f67 726f 7570 5f69 6420 2023  urce_group_id  #
+0000c590: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
+0000c5a0: 2020 2073 656c 662e 7365 6375 7269 7479     self.security
+0000c5b0: 5f67 726f 7570 5f69 6420 3d20 7365 6375  _group_id = secu
+0000c5c0: 7269 7479 5f67 726f 7570 5f69 6420 2023  rity_group_id  #
+0000c5d0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
+0000c5e0: 2020 2073 656c 662e 765f 7377 6974 6368     self.v_switch
+0000c5f0: 5f69 6420 3d20 765f 7377 6974 6368 5f69  _id = v_switch_i
+0000c600: 6420 2023 2074 7970 653a 2073 7472 0a0a  d  # type: str..
+0000c610: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0000c620: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000c630: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+0000c640: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0000c650: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0000c660: 2843 7265 6174 6545 6169 4a75 7079 7465  (CreateEaiJupyte
+0000c670: 7253 6872 696e 6b52 6571 7565 7374 2c20  rShrinkRequest, 
+0000c680: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+0000c690: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0000c6a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000c6b0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0000c6c0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0000c6d0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0000c6e0: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
+0000c6f0: 656e 745f 746f 6b65 6e20 6973 206e 6f74  ent_token is not
+0000c700: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000c710: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
+0000c720: 7454 6f6b 656e 275d 203d 2073 656c 662e  tToken'] = self.
+0000c730: 636c 6965 6e74 5f74 6f6b 656e 0a20 2020  client_token.   
+0000c740: 2020 2020 2069 6620 7365 6c66 2e65 6169       if self.eai
+0000c750: 735f 6e61 6d65 2069 7320 6e6f 7420 4e6f  s_name is not No
+0000c760: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000c770: 7265 7375 6c74 5b27 4561 6973 4e61 6d65  result['EaisName
+0000c780: 275d 203d 2073 656c 662e 6561 6973 5f6e  '] = self.eais_n
+0000c790: 616d 650a 2020 2020 2020 2020 6966 2073  ame.        if s
+0000c7a0: 656c 662e 6561 6973 5f74 7970 6520 6973  elf.eais_type is
+0000c7b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000c7c0: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
+0000c7d0: 6169 7354 7970 6527 5d20 3d20 7365 6c66  aisType'] = self
+0000c7e0: 2e65 6169 735f 7479 7065 0a20 2020 2020  .eais_type.     
+0000c7f0: 2020 2069 6620 7365 6c66 2e65 6e76 6972     if self.envir
+0000c800: 6f6e 6d65 6e74 5f76 6172 5f73 6872 696e  onment_var_shrin
+0000c810: 6b20 6973 206e 6f74 204e 6f6e 653a 0a20  k is not None:. 
+0000c820: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0000c830: 745b 2745 6e76 6972 6f6e 6d65 6e74 5661  t['EnvironmentVa
+0000c840: 7227 5d20 3d20 7365 6c66 2e65 6e76 6972  r'] = self.envir
+0000c850: 6f6e 6d65 6e74 5f76 6172 5f73 6872 696e  onment_var_shrin
+0000c860: 6b0a 2020 2020 2020 2020 6966 2073 656c  k.        if sel
+0000c870: 662e 7265 6769 6f6e 5f69 6420 6973 206e  f.region_id is n
+0000c880: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000c890: 2020 2020 2072 6573 756c 745b 2752 6567       result['Reg
+0000c8a0: 696f 6e49 6427 5d20 3d20 7365 6c66 2e72  ionId'] = self.r
+0000c8b0: 6567 696f 6e5f 6964 0a20 2020 2020 2020  egion_id.       
+0000c8c0: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
+0000c8d0: 655f 6772 6f75 705f 6964 2069 7320 6e6f  e_group_id is no
+0000c8e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000c8f0: 2020 2020 7265 7375 6c74 5b27 5265 736f      result['Reso
+0000c900: 7572 6365 4772 6f75 7049 6427 5d20 3d20  urceGroupId'] = 
+0000c910: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
+0000c920: 6f75 705f 6964 0a20 2020 2020 2020 2069  oup_id.        i
+0000c930: 6620 7365 6c66 2e73 6563 7572 6974 795f  f self.security_
+0000c940: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
+0000c950: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000c960: 2020 7265 7375 6c74 5b27 5365 6375 7269    result['Securi
+0000c970: 7479 4772 6f75 7049 6427 5d20 3d20 7365  tyGroupId'] = se
+0000c980: 6c66 2e73 6563 7572 6974 795f 6772 6f75  lf.security_grou
+0000c990: 705f 6964 0a20 2020 2020 2020 2069 6620  p_id.        if 
+0000c9a0: 7365 6c66 2e76 5f73 7769 7463 685f 6964  self.v_switch_id
+0000c9b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000c9c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000c9d0: 5b27 5653 7769 7463 6849 6427 5d20 3d20  ['VSwitchId'] = 
+0000c9e0: 7365 6c66 2e76 5f73 7769 7463 685f 6964  self.v_switch_id
+0000c9f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000ca00: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0000ca10: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+0000ca20: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0000ca30: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+0000ca40: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0000ca50: 2827 436c 6965 6e74 546f 6b65 6e27 2920  ('ClientToken') 
+0000ca60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000ca70: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
+0000ca80: 6965 6e74 5f74 6f6b 656e 203d 206d 2e67  ient_token = m.g
+0000ca90: 6574 2827 436c 6965 6e74 546f 6b65 6e27  et('ClientToken'
+0000caa0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0000cab0: 6574 2827 4561 6973 4e61 6d65 2729 2069  et('EaisName') i
+0000cac0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000cad0: 2020 2020 2020 2020 7365 6c66 2e65 6169          self.eai
+0000cae0: 735f 6e61 6d65 203d 206d 2e67 6574 2827  s_name = m.get('
+0000caf0: 4561 6973 4e61 6d65 2729 0a20 2020 2020  EaisName').     
+0000cb00: 2020 2069 6620 6d2e 6765 7428 2745 6169     if m.get('Eai
+0000cb10: 7354 7970 6527 2920 6973 206e 6f74 204e  sType') is not N
+0000cb20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000cb30: 2073 656c 662e 6561 6973 5f74 7970 6520   self.eais_type 
+0000cb40: 3d20 6d2e 6765 7428 2745 6169 7354 7970  = m.get('EaisTyp
+0000cb50: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+0000cb60: 2e67 6574 2827 456e 7669 726f 6e6d 656e  .get('Environmen
+0000cb70: 7456 6172 2729 2069 7320 6e6f 7420 4e6f  tVar') is not No
+0000cb80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000cb90: 7365 6c66 2e65 6e76 6972 6f6e 6d65 6e74  self.environment
+0000cba0: 5f76 6172 5f73 6872 696e 6b20 3d20 6d2e  _var_shrink = m.
+0000cbb0: 6765 7428 2745 6e76 6972 6f6e 6d65 6e74  get('Environment
+0000cbc0: 5661 7227 290a 2020 2020 2020 2020 6966  Var').        if
+0000cbd0: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
+0000cbe0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0000cbf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cc00: 2e72 6567 696f 6e5f 6964 203d 206d 2e67  .region_id = m.g
+0000cc10: 6574 2827 5265 6769 6f6e 4964 2729 0a20  et('RegionId'). 
+0000cc20: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0000cc30: 2752 6573 6f75 7263 6547 726f 7570 4964  'ResourceGroupId
+0000cc40: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0000cc50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cc60: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
+0000cc70: 6964 203d 206d 2e67 6574 2827 5265 736f  id = m.get('Reso
+0000cc80: 7572 6365 4772 6f75 7049 6427 290a 2020  urceGroupId').  
+0000cc90: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0000cca0: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
+0000ccb0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0000ccc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ccd0: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
+0000cce0: 6420 3d20 6d2e 6765 7428 2753 6563 7572  d = m.get('Secur
+0000ccf0: 6974 7947 726f 7570 4964 2729 0a20 2020  ityGroupId').   
+0000cd00: 2020 2020 2069 6620 6d2e 6765 7428 2756       if m.get('V
+0000cd10: 5377 6974 6368 4964 2729 2069 7320 6e6f  SwitchId') is no
+0000cd20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000cd30: 2020 2020 7365 6c66 2e76 5f73 7769 7463      self.v_switc
+0000cd40: 685f 6964 203d 206d 2e67 6574 2827 5653  h_id = m.get('VS
+0000cd50: 7769 7463 6849 6427 290a 2020 2020 2020  witchId').      
+0000cd60: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+0000cd70: 636c 6173 7320 4372 6561 7465 4561 694a  class CreateEaiJ
+0000cd80: 7570 7974 6572 5265 7370 6f6e 7365 426f  upyterResponseBo
+0000cd90: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
+0000cda0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000cdb0: 656c 662c 2065 6c61 7374 6963 5f61 6363  elf, elastic_acc
+0000cdc0: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
+0000cdd0: 655f 6964 3d4e 6f6e 652c 2072 6571 7565  e_id=None, reque
+0000cde0: 7374 5f69 643d 4e6f 6e65 293a 0a20 2020  st_id=None):.   
+0000cdf0: 2020 2020 2073 656c 662e 656c 6173 7469       self.elasti
+0000ce00: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
+0000ce10: 7374 616e 6365 5f69 6420 3d20 656c 6173  stance_id = elas
+0000ce20: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
+0000ce30: 696e 7374 616e 6365 5f69 6420 2023 2074  instance_id  # t
+0000ce40: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+0000ce50: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+0000ce60: 203d 2072 6571 7565 7374 5f69 6420 2023   = request_id  #
+0000ce70: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
+0000ce80: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0000ce90: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0000cea0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0000ceb0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000cec0: 5f6d 6170 203d 2073 7570 6572 2843 7265  _map = super(Cre
+0000ced0: 6174 6545 6169 4a75 7079 7465 7252 6573  ateEaiJupyterRes
+0000cee0: 706f 6e73 6542 6f64 792c 2073 656c 6629  ponseBody, self)
+0000cef0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0000cf00: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0000cf10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000cf20: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0000cf30: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0000cf40: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0000cf50: 6966 2073 656c 662e 656c 6173 7469 635f  if self.elastic_
+0000cf60: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
+0000cf70: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
+0000cf80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000cf90: 2072 6573 756c 745b 2745 6c61 7374 6963   result['Elastic
+0000cfa0: 4163 6365 6c65 7261 7465 6449 6e73 7461  AcceleratedInsta
+0000cfb0: 6e63 6549 6427 5d20 3d20 7365 6c66 2e65  nceId'] = self.e
+0000cfc0: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+0000cfd0: 6564 5f69 6e73 7461 6e63 655f 6964 0a20  ed_instance_id. 
+0000cfe0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000cff0: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
+0000d000: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000d010: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
+0000d020: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
+0000d030: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+0000d040: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0000d050: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+0000d060: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+0000d070: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0000d080: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0000d090: 6966 206d 2e67 6574 2827 456c 6173 7469  if m.get('Elasti
+0000d0a0: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
+0000d0b0: 616e 6365 4964 2729 2069 7320 6e6f 7420  anceId') is not 
+0000d0c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000d0d0: 2020 7365 6c66 2e65 6c61 7374 6963 5f61    self.elastic_a
+0000d0e0: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
+0000d0f0: 6e63 655f 6964 203d 206d 2e67 6574 2827  nce_id = m.get('
+0000d100: 456c 6173 7469 6341 6363 656c 6572 6174  ElasticAccelerat
+0000d110: 6564 496e 7374 616e 6365 4964 2729 0a20  edInstanceId'). 
+0000d120: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0000d130: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
+0000d140: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000d150: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+0000d160: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
+0000d170: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
+0000d180: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0000d190: 0a63 6c61 7373 2043 7265 6174 6545 6169  .class CreateEai
+0000d1a0: 4a75 7079 7465 7252 6573 706f 6e73 6528  JupyterResponse(
+0000d1b0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+0000d1c0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0000d1d0: 2c20 6865 6164 6572 733d 4e6f 6e65 2c20  , headers=None, 
+0000d1e0: 7374 6174 7573 5f63 6f64 653d 4e6f 6e65  status_code=None
+0000d1f0: 2c20 626f 6479 3d4e 6f6e 6529 3a0a 2020  , body=None):.  
+0000d200: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+0000d210: 7273 203d 2068 6561 6465 7273 2020 2320  rs = headers  # 
+0000d220: 7479 7065 3a20 6469 6374 5b73 7472 2c20  type: dict[str, 
+0000d230: 7374 725d 0a20 2020 2020 2020 2073 656c  str].        sel
+0000d240: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+0000d250: 7374 6174 7573 5f63 6f64 6520 2023 2074  status_code  # t
+0000d260: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+0000d270: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+0000d280: 7920 2023 2074 7970 653a 2043 7265 6174  y  # type: Creat
+0000d290: 6545 6169 4a75 7079 7465 7252 6573 706f  eEaiJupyterRespo
+0000d2a0: 6e73 6542 6f64 790a 0a20 2020 2064 6566  nseBody..    def
+0000d2b0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+0000d2c0: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+0000d2d0: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+0000d2e0: 7365 6c66 2e68 6561 6465 7273 2c20 2768  self.headers, 'h
+0000d2f0: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+0000d300: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+0000d310: 6571 7569 7265 6428 7365 6c66 2e73 7461  equired(self.sta
+0000d320: 7475 735f 636f 6465 2c20 2773 7461 7475  tus_code, 'statu
+0000d330: 735f 636f 6465 2729 0a20 2020 2020 2020  s_code').       
+0000d340: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+0000d350: 6571 7569 7265 6428 7365 6c66 2e62 6f64  equired(self.bod
+0000d360: 792c 2027 626f 6479 2729 0a20 2020 2020  y, 'body').     
+0000d370: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+0000d380: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d390: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+0000d3a0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+0000d3b0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0000d3c0: 205f 6d61 7020 3d20 7375 7065 7228 4372   _map = super(Cr
+0000d3d0: 6561 7465 4561 694a 7570 7974 6572 5265  eateEaiJupyterRe
+0000d3e0: 7370 6f6e 7365 2c20 7365 6c66 292e 746f  sponse, self).to
+0000d3f0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0000d400: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0000d410: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000d420: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0000d430: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0000d440: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0000d450: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+0000d460: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000d470: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+0000d480: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+0000d490: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+0000d4a0: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+0000d4b0: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+0000d4c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000d4d0: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+0000d4e0: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+0000d4f0: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+0000d500: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+0000d510: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000d520: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+0000d530: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+0000d540: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+0000d550: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+0000d560: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+0000d570: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+0000d580: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0000d590: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0000d5a0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+0000d5b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000d5c0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+0000d5d0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+0000d5e0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+0000d5f0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+0000d600: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+0000d610: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000d620: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0000d630: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+0000d640: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+0000d650: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+0000d660: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0000d670: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+0000d680: 6d6f 6465 6c20 3d20 4372 6561 7465 4561  model = CreateEa
+0000d690: 694a 7570 7974 6572 5265 7370 6f6e 7365  iJupyterResponse
+0000d6a0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
+0000d6b0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+0000d6c0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+0000d6d0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+0000d6e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000d6f0: 660a 0a0a 636c 6173 7320 4372 6561 7465  f...class Create
+0000d700: 4561 6973 4569 5265 7175 6573 7428 5465  EaisEiRequest(Te
+0000d710: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0000d720: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0000d730: 636c 6965 6e74 5f74 6f6b 656e 3d4e 6f6e  client_token=Non
+0000d740: 652c 2069 6e73 7461 6e63 655f 6e61 6d65  e, instance_name
+0000d750: 3d4e 6f6e 652c 2069 6e73 7461 6e63 655f  =None, instance_
+0000d760: 7479 7065 3d4e 6f6e 652c 2072 6567 696f  type=None, regio
+0000d770: 6e5f 6964 3d4e 6f6e 652c 0a20 2020 2020  n_id=None,.     
+0000d780: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+0000d790: 7572 6365 5f67 726f 7570 5f69 643d 4e6f  urce_group_id=No
+0000d7a0: 6e65 2c20 7365 6375 7269 7479 5f67 726f  ne, security_gro
+0000d7b0: 7570 5f69 643d 4e6f 6e65 2c20 765f 7377  up_id=None, v_sw
+0000d7c0: 6974 6368 5f69 643d 4e6f 6e65 293a 0a20  itch_id=None):. 
+0000d7d0: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+0000d7e0: 6e74 5f74 6f6b 656e 203d 2063 6c69 656e  nt_token = clien
+0000d7f0: 745f 746f 6b65 6e20 2023 2074 7970 653a  t_token  # type:
+0000d800: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0000d810: 662e 696e 7374 616e 6365 5f6e 616d 6520  f.instance_name 
+0000d820: 3d20 696e 7374 616e 6365 5f6e 616d 6520  = instance_name 
+0000d830: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+0000d840: 2020 2020 2073 656c 662e 696e 7374 616e       self.instan
+0000d850: 6365 5f74 7970 6520 3d20 696e 7374 616e  ce_type = instan
+0000d860: 6365 5f74 7970 6520 2023 2074 7970 653a  ce_type  # type:
+0000d870: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0000d880: 662e 7265 6769 6f6e 5f69 6420 3d20 7265  f.region_id = re
+0000d890: 6769 6f6e 5f69 6420 2023 2074 7970 653a  gion_id  # type:
+0000d8a0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0000d8b0: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
+0000d8c0: 5f69 6420 3d20 7265 736f 7572 6365 5f67  _id = resource_g
+0000d8d0: 726f 7570 5f69 6420 2023 2074 7970 653a  roup_id  # type:
+0000d8e0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0000d8f0: 662e 7365 6375 7269 7479 5f67 726f 7570  f.security_group
+0000d900: 5f69 6420 3d20 7365 6375 7269 7479 5f67  _id = security_g
+0000d910: 726f 7570 5f69 6420 2023 2074 7970 653a  roup_id  # type:
+0000d920: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0000d930: 662e 765f 7377 6974 6368 5f69 6420 3d20  f.v_switch_id = 
+0000d940: 765f 7377 6974 6368 5f69 6420 2023 2074  v_switch_id  # t
+0000d950: 7970 653a 2073 7472 0a0a 2020 2020 6465  ype: str..    de
+0000d960: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+0000d970: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0000d980: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+0000d990: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+0000d9a0: 6170 203d 2073 7570 6572 2843 7265 6174  ap = super(Creat
+0000d9b0: 6545 6169 7345 6952 6571 7565 7374 2c20  eEaisEiRequest, 
+0000d9c0: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+0000d9d0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0000d9e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000d9f0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0000da00: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0000da10: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0000da20: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
+0000da30: 656e 745f 746f 6b65 6e20 6973 206e 6f74  ent_token is not
+0000da40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000da50: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
+0000da60: 7454 6f6b 656e 275d 203d 2073 656c 662e  tToken'] = self.
+0000da70: 636c 6965 6e74 5f74 6f6b 656e 0a20 2020  client_token.   
+0000da80: 2020 2020 2069 6620 7365 6c66 2e69 6e73       if self.ins
+0000da90: 7461 6e63 655f 6e61 6d65 2069 7320 6e6f  tance_name is no
+0000daa0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000dab0: 2020 2020 7265 7375 6c74 5b27 496e 7374      result['Inst
+0000dac0: 616e 6365 4e61 6d65 275d 203d 2073 656c  anceName'] = sel
+0000dad0: 662e 696e 7374 616e 6365 5f6e 616d 650a  f.instance_name.
+0000dae0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000daf0: 696e 7374 616e 6365 5f74 7970 6520 6973  instance_type is
+0000db00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000db10: 2020 2020 2020 2072 6573 756c 745b 2749         result['I
+0000db20: 6e73 7461 6e63 6554 7970 6527 5d20 3d20  nstanceType'] = 
+0000db30: 7365 6c66 2e69 6e73 7461 6e63 655f 7479  self.instance_ty
+0000db40: 7065 0a20 2020 2020 2020 2069 6620 7365  pe.        if se
+0000db50: 6c66 2e72 6567 696f 6e5f 6964 2069 7320  lf.region_id is 
+0000db60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000db70: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
+0000db80: 6769 6f6e 4964 275d 203d 2073 656c 662e  gionId'] = self.
+0000db90: 7265 6769 6f6e 5f69 640a 2020 2020 2020  region_id.      
+0000dba0: 2020 6966 2073 656c 662e 7265 736f 7572    if self.resour
+0000dbb0: 6365 5f67 726f 7570 5f69 6420 6973 206e  ce_group_id is n
+0000dbc0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000dbd0: 2020 2020 2072 6573 756c 745b 2752 6573       result['Res
+0000dbe0: 6f75 7263 6547 726f 7570 4964 275d 203d  ourceGroupId'] =
+0000dbf0: 2073 656c 662e 7265 736f 7572 6365 5f67   self.resource_g
+0000dc00: 726f 7570 5f69 640a 2020 2020 2020 2020  roup_id.        
+0000dc10: 6966 2073 656c 662e 7365 6375 7269 7479  if self.security
+0000dc20: 5f67 726f 7570 5f69 6420 6973 206e 6f74  _group_id is not
+0000dc30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000dc40: 2020 2072 6573 756c 745b 2753 6563 7572     result['Secur
+0000dc50: 6974 7947 726f 7570 4964 275d 203d 2073  ityGroupId'] = s
+0000dc60: 656c 662e 7365 6375 7269 7479 5f67 726f  elf.security_gro
+0000dc70: 7570 5f69 640a 2020 2020 2020 2020 6966  up_id.        if
+0000dc80: 2073 656c 662e 765f 7377 6974 6368 5f69   self.v_switch_i
+0000dc90: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+0000dca0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0000dcb0: 745b 2756 5377 6974 6368 4964 275d 203d  t['VSwitchId'] =
+0000dcc0: 2073 656c 662e 765f 7377 6974 6368 5f69   self.v_switch_i
+0000dcd0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+0000dce0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+0000dcf0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+0000dd00: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+0000dd10: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+0000dd20: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0000dd30: 7428 2743 6c69 656e 7454 6f6b 656e 2729  t('ClientToken')
+0000dd40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000dd50: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000dd60: 6c69 656e 745f 746f 6b65 6e20 3d20 6d2e  lient_token = m.
+0000dd70: 6765 7428 2743 6c69 656e 7454 6f6b 656e  get('ClientToken
+0000dd80: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0000dd90: 6765 7428 2749 6e73 7461 6e63 654e 616d  get('InstanceNam
+0000dda0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+0000ddb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ddc0: 662e 696e 7374 616e 6365 5f6e 616d 6520  f.instance_name 
+0000ddd0: 3d20 6d2e 6765 7428 2749 6e73 7461 6e63  = m.get('Instanc
+0000dde0: 654e 616d 6527 290a 2020 2020 2020 2020  eName').        
+0000ddf0: 6966 206d 2e67 6574 2827 496e 7374 616e  if m.get('Instan
+0000de00: 6365 5479 7065 2729 2069 7320 6e6f 7420  ceType') is not 
+0000de10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000de20: 2020 7365 6c66 2e69 6e73 7461 6e63 655f    self.instance_
+0000de30: 7479 7065 203d 206d 2e67 6574 2827 496e  type = m.get('In
+0000de40: 7374 616e 6365 5479 7065 2729 0a20 2020  stanceType').   
+0000de50: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+0000de60: 6567 696f 6e49 6427 2920 6973 206e 6f74  egionId') is not
+0000de70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000de80: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
+0000de90: 6420 3d20 6d2e 6765 7428 2752 6567 696f  d = m.get('Regio
+0000dea0: 6e49 6427 290a 2020 2020 2020 2020 6966  nId').        if
+0000deb0: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+0000dec0: 4772 6f75 7049 6427 2920 6973 206e 6f74  GroupId') is not
+0000ded0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000dee0: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
+0000def0: 5f67 726f 7570 5f69 6420 3d20 6d2e 6765  _group_id = m.ge
+0000df00: 7428 2752 6573 6f75 7263 6547 726f 7570  t('ResourceGroup
+0000df10: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0000df20: 6d2e 6765 7428 2753 6563 7572 6974 7947  m.get('SecurityG
+0000df30: 726f 7570 4964 2729 2069 7320 6e6f 7420  roupId') is not 
+0000df40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000df50: 2020 7365 6c66 2e73 6563 7572 6974 795f    self.security_
+0000df60: 6772 6f75 705f 6964 203d 206d 2e67 6574  group_id = m.get
+0000df70: 2827 5365 6375 7269 7479 4772 6f75 7049  ('SecurityGroupI
+0000df80: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+0000df90: 2e67 6574 2827 5653 7769 7463 6849 6427  .get('VSwitchId'
+0000dfa0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0000dfb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000dfc0: 765f 7377 6974 6368 5f69 6420 3d20 6d2e  v_switch_id = m.
+0000dfd0: 6765 7428 2756 5377 6974 6368 4964 2729  get('VSwitchId')
+0000dfe0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000dff0: 7365 6c66 0a0a 0a63 6c61 7373 2043 7265  self...class Cre
+0000e000: 6174 6545 6169 7345 6952 6573 706f 6e73  ateEaisEiRespons
+0000e010: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
+0000e020: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000e030: 5f28 7365 6c66 2c20 6569 5f69 6e73 7461  _(self, ei_insta
+0000e040: 6e63 655f 6964 3d4e 6f6e 652c 2072 6571  nce_id=None, req
+0000e050: 7565 7374 5f69 643d 4e6f 6e65 293a 0a20  uest_id=None):. 
+0000e060: 2020 2020 2020 2073 656c 662e 6569 5f69         self.ei_i
+0000e070: 6e73 7461 6e63 655f 6964 203d 2065 695f  nstance_id = ei_
+0000e080: 696e 7374 616e 6365 5f69 6420 2023 2074  instance_id  # t
+0000e090: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+0000e0a0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+0000e0b0: 203d 2072 6571 7565 7374 5f69 6420 2023   = request_id  #
+0000e0c0: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
+0000e0d0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0000e0e0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0000e0f0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0000e100: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000e110: 5f6d 6170 203d 2073 7570 6572 2843 7265  _map = super(Cre
+0000e120: 6174 6545 6169 7345 6952 6573 706f 6e73  ateEaisEiRespons
+0000e130: 6542 6f64 792c 2073 656c 6629 2e74 6f5f  eBody, self).to_
+0000e140: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+0000e150: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+0000e160: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000e170: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+0000e180: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+0000e190: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+0000e1a0: 656c 662e 6569 5f69 6e73 7461 6e63 655f  elf.ei_instance_
+0000e1b0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0000e1c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000e1d0: 6c74 5b27 4569 496e 7374 616e 6365 4964  lt['EiInstanceId
+0000e1e0: 275d 203d 2073 656c 662e 6569 5f69 6e73  '] = self.ei_ins
+0000e1f0: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+0000e200: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
+0000e210: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+0000e220: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000e230: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
+0000e240: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+0000e250: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+0000e260: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0000e270: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0000e280: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+0000e290: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+0000e2a0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0000e2b0: 6574 2827 4569 496e 7374 616e 6365 4964  et('EiInstanceId
+0000e2c0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0000e2d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e2e0: 2e65 695f 696e 7374 616e 6365 5f69 6420  .ei_instance_id 
+0000e2f0: 3d20 6d2e 6765 7428 2745 6949 6e73 7461  = m.get('EiInsta
+0000e300: 6e63 6549 6427 290a 2020 2020 2020 2020  nceId').        
+0000e310: 6966 206d 2e67 6574 2827 5265 7175 6573  if m.get('Reques
+0000e320: 7449 6427 2920 6973 206e 6f74 204e 6f6e  tId') is not Non
+0000e330: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000e340: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+0000e350: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+0000e360: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
+0000e370: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+0000e380: 4372 6561 7465 4561 6973 4569 5265 7370  CreateEaisEiResp
+0000e390: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+0000e3a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000e3b0: 2873 656c 662c 2068 6561 6465 7273 3d4e  (self, headers=N
+0000e3c0: 6f6e 652c 2073 7461 7475 735f 636f 6465  one, status_code
+0000e3d0: 3d4e 6f6e 652c 2062 6f64 793d 4e6f 6e65  =None, body=None
+0000e3e0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000e3f0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+0000e400: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
+0000e410: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
+0000e420: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0000e430: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
+0000e440: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
+0000e450: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+0000e460: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
+0000e470: 4372 6561 7465 4561 6973 4569 5265 7370  CreateEaisEiResp
+0000e480: 6f6e 7365 426f 6479 0a0a 2020 2020 6465  onseBody..    de
+0000e490: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+0000e4a0: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
+0000e4b0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+0000e4c0: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
+0000e4d0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+0000e4e0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+0000e4f0: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
+0000e500: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
+0000e510: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
+0000e520: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+0000e530: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
+0000e540: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
+0000e550: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+0000e560: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000e570: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+0000e580: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+0000e590: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+0000e5a0: 2020 5f6d 6170 203d 2073 7570 6572 2843    _map = super(C
+0000e5b0: 7265 6174 6545 6169 7345 6952 6573 706f  reateEaisEiRespo
+0000e5c0: 6e73 652c 2073 656c 6629 2e74 6f5f 6d61  nse, self).to_ma
+0000e5d0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+0000e5e0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+0000e5f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e600: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+0000e610: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+0000e620: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000e630: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+0000e640: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000e650: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+0000e660: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+0000e670: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+0000e680: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0000e690: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000e6a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0000e6b0: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+0000e6c0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0000e6d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000e6e0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+0000e6f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000e700: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+0000e710: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+0000e720: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+0000e730: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0000e740: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0000e750: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+0000e760: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+0000e770: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0000e780: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
+0000e790: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000e7a0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+0000e7b0: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
+0000e7c0: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
+0000e7d0: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
+0000e7e0: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
+0000e7f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000e800: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0000e810: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
+0000e820: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
+0000e830: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
+0000e840: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000e850: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+0000e860: 656c 203d 2043 7265 6174 6545 6169 7345  el = CreateEaisE
+0000e870: 6952 6573 706f 6e73 6542 6f64 7928 290a  iResponseBody().
+0000e880: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e890: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+0000e8a0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+0000e8b0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+0000e8c0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+0000e8d0: 7373 2044 656c 6574 6545 6169 5265 7175  ss DeleteEaiRequ
+0000e8e0: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+0000e8f0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000e900: 7365 6c66 2c20 656c 6173 7469 635f 6163  self, elastic_ac
+0000e910: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+0000e920: 6365 5f69 643d 4e6f 6e65 2c20 666f 7263  ce_id=None, forc
+0000e930: 653d 4e6f 6e65 2c20 7265 6769 6f6e 5f69  e=None, region_i
+0000e940: 643d 4e6f 6e65 293a 0a20 2020 2020 2020  d=None):.       
+0000e950: 2073 656c 662e 656c 6173 7469 635f 6163   self.elastic_ac
+0000e960: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+0000e970: 6365 5f69 6420 3d20 656c 6173 7469 635f  ce_id = elastic_
+0000e980: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
+0000e990: 616e 6365 5f69 6420 2023 2074 7970 653a  ance_id  # type:
+0000e9a0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0000e9b0: 662e 666f 7263 6520 3d20 666f 7263 6520  f.force = force 
+0000e9c0: 2023 2074 7970 653a 2062 6f6f 6c0a 2020   # type: bool.  
+0000e9d0: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
+0000e9e0: 6e5f 6964 203d 2072 6567 696f 6e5f 6964  n_id = region_id
+0000e9f0: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
+0000ea00: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0000ea10: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+0000ea20: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+0000ea30: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+0000ea40: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+0000ea50: 4465 6c65 7465 4561 6952 6571 7565 7374  DeleteEaiRequest
+0000ea60: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+0000ea70: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0000ea80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000ea90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000eaa0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0000eab0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0000eac0: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+0000ead0: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+0000eae0: 6564 5f69 6e73 7461 6e63 655f 6964 2069  ed_instance_id i
+0000eaf0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000eb00: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0000eb10: 456c 6173 7469 6341 6363 656c 6572 6174  ElasticAccelerat
+0000eb20: 6564 496e 7374 616e 6365 4964 275d 203d  edInstanceId'] =
+0000eb30: 2073 656c 662e 656c 6173 7469 635f 6163   self.elastic_ac
+0000eb40: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+0000eb50: 6365 5f69 640a 2020 2020 2020 2020 6966  ce_id.        if
+0000eb60: 2073 656c 662e 666f 7263 6520 6973 206e   self.force is n
+0000eb70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000eb80: 2020 2020 2072 6573 756c 745b 2746 6f72       result['For
+0000eb90: 6365 275d 203d 2073 656c 662e 666f 7263  ce'] = self.forc
+0000eba0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0000ebb0: 662e 7265 6769 6f6e 5f69 6420 6973 206e  f.region_id is n
+0000ebc0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000ebd0: 2020 2020 2072 6573 756c 745b 2752 6567       result['Reg
+0000ebe0: 696f 6e49 6427 5d20 3d20 7365 6c66 2e72  ionId'] = self.r
+0000ebf0: 6567 696f 6e5f 6964 0a20 2020 2020 2020  egion_id.       
+0000ec00: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0000ec10: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+0000ec20: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+0000ec30: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0000ec40: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0000ec50: 6966 206d 2e67 6574 2827 456c 6173 7469  if m.get('Elasti
+0000ec60: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
+0000ec70: 616e 6365 4964 2729 2069 7320 6e6f 7420  anceId') is not 
+0000ec80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000ec90: 2020 7365 6c66 2e65 6c61 7374 6963 5f61    self.elastic_a
+0000eca0: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
+0000ecb0: 6e63 655f 6964 203d 206d 2e67 6574 2827  nce_id = m.get('
+0000ecc0: 456c 6173 7469 6341 6363 656c 6572 6174  ElasticAccelerat
+0000ecd0: 6564 496e 7374 616e 6365 4964 2729 0a20  edInstanceId'). 
+0000ece0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0000ecf0: 2746 6f72 6365 2729 2069 7320 6e6f 7420  'Force') is not 
+0000ed00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000ed10: 2020 7365 6c66 2e66 6f72 6365 203d 206d    self.force = m
+0000ed20: 2e67 6574 2827 466f 7263 6527 290a 2020  .get('Force').  
+0000ed30: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0000ed40: 5265 6769 6f6e 4964 2729 2069 7320 6e6f  RegionId') is no
+0000ed50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000ed60: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
+0000ed70: 6964 203d 206d 2e67 6574 2827 5265 6769  id = m.get('Regi
+0000ed80: 6f6e 4964 2729 0a20 2020 2020 2020 2072  onId').        r
+0000ed90: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+0000eda0: 7373 2044 656c 6574 6545 6169 5265 7370  ss DeleteEaiResp
+0000edb0: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
+0000edc0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+0000edd0: 6974 5f5f 2873 656c 662c 2072 6571 7565  it__(self, reque
+0000ede0: 7374 5f69 643d 4e6f 6e65 293a 0a20 2020  st_id=None):.   
+0000edf0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+0000ee00: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
+0000ee10: 6420 2023 2074 7970 653a 2073 7472 0a0a  d  # type: str..
+0000ee20: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0000ee30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000ee40: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+0000ee50: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0000ee60: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0000ee70: 2844 656c 6574 6545 6169 5265 7370 6f6e  (DeleteEaiRespon
+0000ee80: 7365 426f 6479 2c20 7365 6c66 292e 746f  seBody, self).to
+0000ee90: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0000eea0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0000eeb0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000eec0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0000eed0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0000eee0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0000eef0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0000ef00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000ef10: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0000ef20: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+0000ef30: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+0000ef40: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000ef50: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0000ef60: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+0000ef70: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+0000ef80: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+0000ef90: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0000efa0: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
+0000efb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000efc0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+0000efd0: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
+0000efe0: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
+0000eff0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+0000f000: 636c 6173 7320 4465 6c65 7465 4561 6952  class DeleteEaiR
+0000f010: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
+0000f020: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0000f030: 745f 5f28 7365 6c66 2c20 6865 6164 6572  t__(self, header
+0000f040: 733d 4e6f 6e65 2c20 7374 6174 7573 5f63  s=None, status_c
+0000f050: 6f64 653d 4e6f 6e65 2c20 626f 6479 3d4e  ode=None, body=N
+0000f060: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+0000f070: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+0000f080: 6465 7273 2020 2320 7479 7065 3a20 6469  ders  # type: di
+0000f090: 6374 5b73 7472 2c20 7374 725d 0a20 2020  ct[str, str].   
+0000f0a0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+0000f0b0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+0000f0c0: 6f64 6520 2023 2074 7970 653a 2069 6e74  ode  # type: int
+0000f0d0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+0000f0e0: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
+0000f0f0: 653a 2044 656c 6574 6545 6169 5265 7370  e: DeleteEaiResp
+0000f100: 6f6e 7365 426f 6479 0a0a 2020 2020 6465  onseBody..    de
+0000f110: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+0000f120: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
+0000f130: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+0000f140: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
+0000f150: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+0000f160: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+0000f170: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
+0000f180: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
+0000f190: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
+0000f1a0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+0000f1b0: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
+0000f1c0: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
+0000f1d0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+0000f1e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000f1f0: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+0000f200: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+0000f210: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+0000f220: 2020 5f6d 6170 203d 2073 7570 6572 2844    _map = super(D
+0000f230: 656c 6574 6545 6169 5265 7370 6f6e 7365  eleteEaiResponse
+0000f240: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+0000f250: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0000f260: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000f270: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000f280: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0000f290: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0000f2a0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+0000f2b0: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+0000f2c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000f2d0: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+0000f2e0: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+0000f2f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000f300: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+0000f310: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000f320: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+0000f330: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+0000f340: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+0000f350: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+0000f360: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+0000f370: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000f380: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+0000f390: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+0000f3a0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000f3b0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0000f3c0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0000f3d0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0000f3e0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0000f3f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0000f400: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+0000f410: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000f420: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+0000f430: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+0000f440: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+0000f450: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0000f460: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0000f470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f480: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+0000f490: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0000f4a0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0000f4b0: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+0000f4c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000f4d0: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+0000f4e0: 3d20 4465 6c65 7465 4561 6952 6573 706f  = DeleteEaiRespo
+0000f4f0: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
+0000f500: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+0000f510: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+0000f520: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+0000f530: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000f540: 7365 6c66 0a0a 0a63 6c61 7373 2044 656c  self...class Del
+0000f550: 6574 6545 6169 416c 6c52 6571 7565 7374  eteEaiAllRequest
+0000f560: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+0000f570: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000f580: 662c 2063 6c69 656e 745f 696e 7374 616e  f, client_instan
+0000f590: 6365 5f69 643d 4e6f 6e65 2c20 656c 6173  ce_id=None, elas
+0000f5a0: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
+0000f5b0: 696e 7374 616e 6365 5f69 643d 4e6f 6e65  instance_id=None
+0000f5c0: 2c20 7265 6769 6f6e 5f69 643d 4e6f 6e65  , region_id=None
+0000f5d0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000f5e0: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
+0000f5f0: 6964 203d 2063 6c69 656e 745f 696e 7374  id = client_inst
+0000f600: 616e 6365 5f69 6420 2023 2074 7970 653a  ance_id  # type:
+0000f610: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0000f620: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
+0000f630: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
+0000f640: 6420 3d20 656c 6173 7469 635f 6163 6365  d = elastic_acce
+0000f650: 6c65 7261 7465 645f 696e 7374 616e 6365  lerated_instance
+0000f660: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
+0000f670: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0000f680: 6769 6f6e 5f69 6420 3d20 7265 6769 6f6e  gion_id = region
+0000f690: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
+0000f6a0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0000f6b0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0000f6c0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+0000f6d0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+0000f6e0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+0000f6f0: 6572 2844 656c 6574 6545 6169 416c 6c52  er(DeleteEaiAllR
+0000f700: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
+0000f710: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0000f720: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0000f730: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000f740: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0000f750: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0000f760: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0000f770: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
+0000f780: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
+0000f790: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000f7a0: 2072 6573 756c 745b 2743 6c69 656e 7449   result['ClientI
+0000f7b0: 6e73 7461 6e63 6549 6427 5d20 3d20 7365  nstanceId'] = se
+0000f7c0: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
+0000f7d0: 6365 5f69 640a 2020 2020 2020 2020 6966  ce_id.        if
+0000f7e0: 2073 656c 662e 656c 6173 7469 635f 6163   self.elastic_ac
+0000f7f0: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+0000f800: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
+0000f810: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000f820: 6573 756c 745b 2745 6c61 7374 6963 4163  esult['ElasticAc
+0000f830: 6365 6c65 7261 7465 6449 6e73 7461 6e63  celeratedInstanc
+0000f840: 6549 6427 5d20 3d20 7365 6c66 2e65 6c61  eId'] = self.ela
+0000f850: 7374 6963 5f61 6363 656c 6572 6174 6564  stic_accelerated
+0000f860: 5f69 6e73 7461 6e63 655f 6964 0a20 2020  _instance_id.   
+0000f870: 2020 2020 2069 6620 7365 6c66 2e72 6567       if self.reg
+0000f880: 696f 6e5f 6964 2069 7320 6e6f 7420 4e6f  ion_id is not No
+0000f890: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000f8a0: 7265 7375 6c74 5b27 5265 6769 6f6e 4964  result['RegionId
+0000f8b0: 275d 203d 2073 656c 662e 7265 6769 6f6e  '] = self.region
+0000f8c0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+0000f8d0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0000f8e0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0000f8f0: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+0000f900: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+0000f910: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+0000f920: 6765 7428 2743 6c69 656e 7449 6e73 7461  get('ClientInsta
+0000f930: 6e63 6549 6427 2920 6973 206e 6f74 204e  nceId') is not N
+0000f940: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000f950: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
+0000f960: 7461 6e63 655f 6964 203d 206d 2e67 6574  tance_id = m.get
+0000f970: 2827 436c 6965 6e74 496e 7374 616e 6365  ('ClientInstance
+0000f980: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0000f990: 6d2e 6765 7428 2745 6c61 7374 6963 4163  m.get('ElasticAc
+0000f9a0: 6365 6c65 7261 7465 6449 6e73 7461 6e63  celeratedInstanc
+0000f9b0: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+0000f9c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000f9d0: 656c 662e 656c 6173 7469 635f 6163 6365  elf.elastic_acce
+0000f9e0: 6c65 7261 7465 645f 696e 7374 616e 6365  lerated_instance
+0000f9f0: 5f69 6420 3d20 6d2e 6765 7428 2745 6c61  _id = m.get('Ela
+0000fa00: 7374 6963 4163 6365 6c65 7261 7465 6449  sticAcceleratedI
+0000fa10: 6e73 7461 6e63 6549 6427 290a 2020 2020  nstanceId').    
+0000fa20: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+0000fa30: 6769 6f6e 4964 2729 2069 7320 6e6f 7420  gionId') is not 
+0000fa40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000fa50: 2020 7365 6c66 2e72 6567 696f 6e5f 6964    self.region_id
+0000fa60: 203d 206d 2e67 6574 2827 5265 6769 6f6e   = m.get('Region
+0000fa70: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
+0000fa80: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+0000fa90: 2044 656c 6574 6545 6169 416c 6c52 6573   DeleteEaiAllRes
+0000faa0: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+0000fab0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+0000fac0: 6e69 745f 5f28 7365 6c66 2c20 7265 7175  nit__(self, requ
+0000fad0: 6573 745f 6964 3d4e 6f6e 6529 3a0a 2020  est_id=None):.  
+0000fae0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+0000faf0: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
+0000fb00: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+0000fb10: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0000fb20: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0000fb30: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+0000fb40: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0000fb50: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0000fb60: 7228 4465 6c65 7465 4561 6941 6c6c 5265  r(DeleteEaiAllRe
+0000fb70: 7370 6f6e 7365 426f 6479 2c20 7365 6c66  sponseBody, self
+0000fb80: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+0000fb90: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+0000fba0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000fbb0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+0000fbc0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0000fbd0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+0000fbe0: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
+0000fbf0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+0000fc00: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000fc10: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
+0000fc20: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+0000fc30: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+0000fc40: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0000fc50: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0000fc60: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+0000fc70: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+0000fc80: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0000fc90: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
+0000fca0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000fcb0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+0000fcc0: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
+0000fcd0: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
+0000fce0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000fcf0: 660a 0a0a 636c 6173 7320 4465 6c65 7465  f...class Delete
+0000fd00: 4561 6941 6c6c 5265 7370 6f6e 7365 2854  EaiAllResponse(T
+0000fd10: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0000fd20: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+0000fd30: 2068 6561 6465 7273 3d4e 6f6e 652c 2073   headers=None, s
+0000fd40: 7461 7475 735f 636f 6465 3d4e 6f6e 652c  tatus_code=None,
+0000fd50: 2062 6f64 793d 4e6f 6e65 293a 0a20 2020   body=None):.   
+0000fd60: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+0000fd70: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
+0000fd80: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
+0000fd90: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
+0000fda0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+0000fdb0: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
+0000fdc0: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
+0000fdd0: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+0000fde0: 2020 2320 7479 7065 3a20 4465 6c65 7465    # type: Delete
+0000fdf0: 4561 6941 6c6c 5265 7370 6f6e 7365 426f  EaiAllResponseBo
+0000fe00: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
+0000fe10: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+0000fe20: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+0000fe30: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+0000fe40: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
+0000fe50: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
+0000fe60: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+0000fe70: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
+0000fe80: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
+0000fe90: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
+0000fea0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+0000feb0: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
+0000fec0: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
+0000fed0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+0000fee0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+0000fef0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+0000ff00: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0000ff10: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0000ff20: 203d 2073 7570 6572 2844 656c 6574 6545   = super(DeleteE
+0000ff30: 6169 416c 6c52 6573 706f 6e73 652c 2073  aiAllResponse, s
+0000ff40: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
+0000ff50: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+0000ff60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000ff70: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+0000ff80: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+0000ff90: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+0000ffa0: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
+0000ffb0: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
+0000ffc0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000ffd0: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
+0000ffe0: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
+0000fff0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+00010000: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
+00010010: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00010020: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
+00010030: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
+00010040: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+00010050: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
+00010060: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00010070: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00010080: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
+00010090: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
+000100a0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000100b0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+000100c0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+000100d0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000100e0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000100f0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+00010100: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+00010110: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00010120: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00010130: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00010140: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00010150: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+00010160: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00010170: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00010180: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+00010190: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+000101a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000101b0: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+000101c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000101d0: 2020 7465 6d70 5f6d 6f64 656c 203d 2044    temp_model = D
+000101e0: 656c 6574 6545 6169 416c 6c52 6573 706f  eleteEaiAllRespo
+000101f0: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
+00010200: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00010210: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+00010220: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+00010230: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010240: 7365 6c66 0a0a 0a63 6c61 7373 2044 656c  self...class Del
+00010250: 6574 6545 6169 7345 6952 6571 7565 7374  eteEaisEiRequest
+00010260: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00010270: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00010280: 662c 2065 695f 696e 7374 616e 6365 5f69  f, ei_instance_i
+00010290: 643d 4e6f 6e65 2c20 666f 7263 653d 4e6f  d=None, force=No
+000102a0: 6e65 2c20 7265 6769 6f6e 5f69 643d 4e6f  ne, region_id=No
+000102b0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+000102c0: 662e 6569 5f69 6e73 7461 6e63 655f 6964  f.ei_instance_id
+000102d0: 203d 2065 695f 696e 7374 616e 6365 5f69   = ei_instance_i
+000102e0: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
+000102f0: 2020 2020 2020 2073 656c 662e 666f 7263         self.forc
+00010300: 6520 3d20 666f 7263 6520 2023 2074 7970  e = force  # typ
+00010310: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00010320: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
+00010330: 2072 6567 696f 6e5f 6964 2020 2320 7479   region_id  # ty
+00010340: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
+00010350: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00010360: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00010370: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00010380: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00010390: 7020 3d20 7375 7065 7228 4465 6c65 7465  p = super(Delete
+000103a0: 4561 6973 4569 5265 7175 6573 742c 2073  EaisEiRequest, s
+000103b0: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
+000103c0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+000103d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000103e0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+000103f0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00010400: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00010410: 2020 2020 6966 2073 656c 662e 6569 5f69      if self.ei_i
+00010420: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
+00010430: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00010440: 2020 2020 7265 7375 6c74 5b27 4569 496e      result['EiIn
+00010450: 7374 616e 6365 4964 275d 203d 2073 656c  stanceId'] = sel
+00010460: 662e 6569 5f69 6e73 7461 6e63 655f 6964  f.ei_instance_id
+00010470: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00010480: 2e66 6f72 6365 2069 7320 6e6f 7420 4e6f  .force is not No
+00010490: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000104a0: 7265 7375 6c74 5b27 466f 7263 6527 5d20  result['Force'] 
+000104b0: 3d20 7365 6c66 2e66 6f72 6365 0a20 2020  = self.force.   
+000104c0: 2020 2020 2069 6620 7365 6c66 2e72 6567       if self.reg
+000104d0: 696f 6e5f 6964 2069 7320 6e6f 7420 4e6f  ion_id is not No
+000104e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000104f0: 7265 7375 6c74 5b27 5265 6769 6f6e 4964  result['RegionId
+00010500: 275d 203d 2073 656c 662e 7265 6769 6f6e  '] = self.region
+00010510: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+00010520: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00010530: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00010540: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+00010550: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00010560: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00010570: 6765 7428 2745 6949 6e73 7461 6e63 6549  get('EiInstanceI
+00010580: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00010590: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000105a0: 662e 6569 5f69 6e73 7461 6e63 655f 6964  f.ei_instance_id
+000105b0: 203d 206d 2e67 6574 2827 4569 496e 7374   = m.get('EiInst
+000105c0: 616e 6365 4964 2729 0a20 2020 2020 2020  anceId').       
+000105d0: 2069 6620 6d2e 6765 7428 2746 6f72 6365   if m.get('Force
+000105e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000105f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010600: 2e66 6f72 6365 203d 206d 2e67 6574 2827  .force = m.get('
+00010610: 466f 7263 6527 290a 2020 2020 2020 2020  Force').        
+00010620: 6966 206d 2e67 6574 2827 5265 6769 6f6e  if m.get('Region
+00010630: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00010640: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00010650: 6c66 2e72 6567 696f 6e5f 6964 203d 206d  lf.region_id = m
+00010660: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
+00010670: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010680: 7365 6c66 0a0a 0a63 6c61 7373 2044 656c  self...class Del
+00010690: 6574 6545 6169 7345 6952 6573 706f 6e73  eteEaisEiRespons
+000106a0: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
+000106b0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000106c0: 5f28 7365 6c66 2c20 7265 7175 6573 745f  _(self, request_
+000106d0: 6964 3d4e 6f6e 6529 3a0a 2020 2020 2020  id=None):.      
+000106e0: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+000106f0: 6420 3d20 7265 7175 6573 745f 6964 2020  d = request_id  
+00010700: 2320 7479 7065 3a20 7374 720a 0a20 2020  # type: str..   
+00010710: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00010720: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00010730: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+00010740: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00010750: 205f 6d61 7020 3d20 7375 7065 7228 4465   _map = super(De
+00010760: 6c65 7465 4561 6973 4569 5265 7370 6f6e  leteEaisEiRespon
+00010770: 7365 426f 6479 2c20 7365 6c66 292e 746f  seBody, self).to
+00010780: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00010790: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000107a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000107b0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000107c0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000107d0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000107e0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+000107f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00010800: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00010810: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+00010820: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+00010830: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00010840: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00010850: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+00010860: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00010870: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00010880: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00010890: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
+000108a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000108b0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+000108c0: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
+000108d0: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
+000108e0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+000108f0: 636c 6173 7320 4465 6c65 7465 4561 6973  class DeleteEais
+00010900: 4569 5265 7370 6f6e 7365 2854 6561 4d6f  EiResponse(TeaMo
+00010910: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00010920: 696e 6974 5f5f 2873 656c 662c 2068 6561  init__(self, hea
+00010930: 6465 7273 3d4e 6f6e 652c 2073 7461 7475  ders=None, statu
+00010940: 735f 636f 6465 3d4e 6f6e 652c 2062 6f64  s_code=None, bod
+00010950: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
+00010960: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00010970: 6865 6164 6572 7320 2023 2074 7970 653a  headers  # type:
+00010980: 2064 6963 745b 7374 722c 2073 7472 5d0a   dict[str, str].
+00010990: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+000109a0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+000109b0: 735f 636f 6465 2020 2320 7479 7065 3a20  s_code  # type: 
+000109c0: 696e 740a 2020 2020 2020 2020 7365 6c66  int.        self
+000109d0: 2e62 6f64 7920 3d20 626f 6479 2020 2320  .body = body  # 
+000109e0: 7479 7065 3a20 4465 6c65 7465 4561 6973  type: DeleteEais
+000109f0: 4569 5265 7370 6f6e 7365 426f 6479 0a0a  EiResponseBody..
+00010a00: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00010a10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00010a20: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+00010a30: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
+00010a40: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
+00010a50: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00010a60: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+00010a70: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
+00010a80: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
+00010a90: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00010aa0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+00010ab0: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
+00010ac0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00010ad0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+00010ae0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+00010af0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+00010b00: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00010b10: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00010b20: 7570 6572 2844 656c 6574 6545 6169 7345  uper(DeleteEaisE
+00010b30: 6952 6573 706f 6e73 652c 2073 656c 6629  iResponse, self)
+00010b40: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00010b50: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00010b60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00010b70: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00010b80: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00010b90: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00010ba0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+00010bb0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00010bc0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00010bd0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+00010be0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+00010bf0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00010c00: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00010c10: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00010c20: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00010c30: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00010c40: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00010c50: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00010c60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00010c70: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+00010c80: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+00010c90: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00010ca0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00010cb0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00010cc0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+00010cd0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00010ce0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00010cf0: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+00010d00: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00010d10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010d20: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+00010d30: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+00010d40: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+00010d50: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+00010d60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00010d70: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00010d80: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+00010d90: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+00010da0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+00010db0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+00010dc0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00010dd0: 6d70 5f6d 6f64 656c 203d 2044 656c 6574  mp_model = Delet
+00010de0: 6545 6169 7345 6952 6573 706f 6e73 6542  eEaisEiResponseB
+00010df0: 6f64 7928 290a 2020 2020 2020 2020 2020  ody().          
+00010e00: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
+00010e10: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
+00010e20: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
+00010e30: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00010e40: 0a0a 0a63 6c61 7373 2044 6573 6372 6962  ...class Describ
+00010e50: 6545 6169 7352 6571 7565 7374 2854 6561  eEaisRequest(Tea
+00010e60: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+00010e70: 5f5f 696e 6974 5f5f 2873 656c 662c 2065  __init__(self, e
+00010e80: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+00010e90: 6564 5f69 6e73 7461 6e63 655f 6964 733d  ed_instance_ids=
+00010ea0: 4e6f 6e65 2c20 696e 7374 616e 6365 5f6e  None, instance_n
+00010eb0: 616d 653d 4e6f 6e65 2c20 696e 7374 616e  ame=None, instan
+00010ec0: 6365 5f74 7970 653d 4e6f 6e65 2c0a 2020  ce_type=None,.  
+00010ed0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00010ee0: 6167 655f 6e75 6d62 6572 3d4e 6f6e 652c  age_number=None,
+00010ef0: 2070 6167 655f 7369 7a65 3d4e 6f6e 652c   page_size=None,
+00010f00: 2072 6567 696f 6e5f 6964 3d4e 6f6e 652c   region_id=None,
+00010f10: 2072 6573 6f75 7263 655f 6772 6f75 705f   resource_group_
+00010f20: 6964 3d4e 6f6e 652c 2073 7461 7475 733d  id=None, status=
+00010f30: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
+00010f40: 656c 662e 656c 6173 7469 635f 6163 6365  elf.elastic_acce
+00010f50: 6c65 7261 7465 645f 696e 7374 616e 6365  lerated_instance
+00010f60: 5f69 6473 203d 2065 6c61 7374 6963 5f61  _ids = elastic_a
+00010f70: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
+00010f80: 6e63 655f 6964 7320 2023 2074 7970 653a  nce_ids  # type:
+00010f90: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00010fa0: 662e 696e 7374 616e 6365 5f6e 616d 6520  f.instance_name 
+00010fb0: 3d20 696e 7374 616e 6365 5f6e 616d 6520  = instance_name 
+00010fc0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00010fd0: 2020 2020 2073 656c 662e 696e 7374 616e       self.instan
+00010fe0: 6365 5f74 7970 6520 3d20 696e 7374 616e  ce_type = instan
+00010ff0: 6365 5f74 7970 6520 2023 2074 7970 653a  ce_type  # type:
+00011000: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00011010: 662e 7061 6765 5f6e 756d 6265 7220 3d20  f.page_number = 
+00011020: 7061 6765 5f6e 756d 6265 7220 2023 2074  page_number  # t
+00011030: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+00011040: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
+00011050: 3d20 7061 6765 5f73 697a 6520 2023 2074  = page_size  # t
+00011060: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+00011070: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+00011080: 3d20 7265 6769 6f6e 5f69 6420 2023 2074  = region_id  # t
+00011090: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+000110a0: 2073 656c 662e 7265 736f 7572 6365 5f67   self.resource_g
+000110b0: 726f 7570 5f69 6420 3d20 7265 736f 7572  roup_id = resour
+000110c0: 6365 5f67 726f 7570 5f69 6420 2023 2074  ce_group_id  # t
+000110d0: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+000110e0: 2073 656c 662e 7374 6174 7573 203d 2073   self.status = s
+000110f0: 7461 7475 7320 2023 2074 7970 653a 2073  tatus  # type: s
+00011100: 7472 0a0a 2020 2020 6465 6620 7661 6c69  tr..    def vali
+00011110: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00011120: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00011130: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00011140: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00011150: 7570 6572 2844 6573 6372 6962 6545 6169  uper(DescribeEai
+00011160: 7352 6571 7565 7374 2c20 7365 6c66 292e  sRequest, self).
+00011170: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00011180: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00011190: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000111a0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+000111b0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000111c0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000111d0: 6620 7365 6c66 2e65 6c61 7374 6963 5f61  f self.elastic_a
+000111e0: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
+000111f0: 6e63 655f 6964 7320 6973 206e 6f74 204e  nce_ids is not N
+00011200: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00011210: 2072 6573 756c 745b 2745 6c61 7374 6963   result['Elastic
+00011220: 4163 6365 6c65 7261 7465 6449 6e73 7461  AcceleratedInsta
+00011230: 6e63 6549 6473 275d 203d 2073 656c 662e  nceIds'] = self.
+00011240: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
+00011250: 7465 645f 696e 7374 616e 6365 5f69 6473  ted_instance_ids
+00011260: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00011270: 2e69 6e73 7461 6e63 655f 6e61 6d65 2069  .instance_name i
+00011280: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00011290: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000112a0: 496e 7374 616e 6365 4e61 6d65 275d 203d  InstanceName'] =
+000112b0: 2073 656c 662e 696e 7374 616e 6365 5f6e   self.instance_n
+000112c0: 616d 650a 2020 2020 2020 2020 6966 2073  ame.        if s
+000112d0: 656c 662e 696e 7374 616e 6365 5f74 7970  elf.instance_typ
+000112e0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000112f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00011300: 745b 2749 6e73 7461 6e63 6554 7970 6527  t['InstanceType'
+00011310: 5d20 3d20 7365 6c66 2e69 6e73 7461 6e63  ] = self.instanc
+00011320: 655f 7479 7065 0a20 2020 2020 2020 2069  e_type.        i
+00011330: 6620 7365 6c66 2e70 6167 655f 6e75 6d62  f self.page_numb
+00011340: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
+00011350: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00011360: 6c74 5b27 5061 6765 4e75 6d62 6572 275d  lt['PageNumber']
+00011370: 203d 2073 656c 662e 7061 6765 5f6e 756d   = self.page_num
+00011380: 6265 720a 2020 2020 2020 2020 6966 2073  ber.        if s
+00011390: 656c 662e 7061 6765 5f73 697a 6520 6973  elf.page_size is
+000113a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000113b0: 2020 2020 2020 2072 6573 756c 745b 2750         result['P
+000113c0: 6167 6553 697a 6527 5d20 3d20 7365 6c66  ageSize'] = self
+000113d0: 2e70 6167 655f 7369 7a65 0a20 2020 2020  .page_size.     
+000113e0: 2020 2069 6620 7365 6c66 2e72 6567 696f     if self.regio
+000113f0: 6e5f 6964 2069 7320 6e6f 7420 4e6f 6e65  n_id is not None
+00011400: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00011410: 7375 6c74 5b27 5265 6769 6f6e 4964 275d  sult['RegionId']
+00011420: 203d 2073 656c 662e 7265 6769 6f6e 5f69   = self.region_i
+00011430: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+00011440: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
+00011450: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00011460: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00011470: 756c 745b 2752 6573 6f75 7263 6547 726f  ult['ResourceGro
+00011480: 7570 4964 275d 203d 2073 656c 662e 7265  upId'] = self.re
+00011490: 736f 7572 6365 5f67 726f 7570 5f69 640a  source_group_id.
+000114a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000114b0: 7374 6174 7573 2069 7320 6e6f 7420 4e6f  status is not No
+000114c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000114d0: 7265 7375 6c74 5b27 5374 6174 7573 275d  result['Status']
+000114e0: 203d 2073 656c 662e 7374 6174 7573 0a20   = self.status. 
+000114f0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00011500: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00011510: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+00011520: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00011530: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00011540: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00011550: 456c 6173 7469 6341 6363 656c 6572 6174  ElasticAccelerat
+00011560: 6564 496e 7374 616e 6365 4964 7327 2920  edInstanceIds') 
+00011570: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00011580: 2020 2020 2020 2020 2073 656c 662e 656c           self.el
+00011590: 6173 7469 635f 6163 6365 6c65 7261 7465  astic_accelerate
+000115a0: 645f 696e 7374 616e 6365 5f69 6473 203d  d_instance_ids =
+000115b0: 206d 2e67 6574 2827 456c 6173 7469 6341   m.get('ElasticA
+000115c0: 6363 656c 6572 6174 6564 496e 7374 616e  cceleratedInstan
+000115d0: 6365 4964 7327 290a 2020 2020 2020 2020  ceIds').        
+000115e0: 6966 206d 2e67 6574 2827 496e 7374 616e  if m.get('Instan
+000115f0: 6365 4e61 6d65 2729 2069 7320 6e6f 7420  ceName') is not 
+00011600: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00011610: 2020 7365 6c66 2e69 6e73 7461 6e63 655f    self.instance_
+00011620: 6e61 6d65 203d 206d 2e67 6574 2827 496e  name = m.get('In
+00011630: 7374 616e 6365 4e61 6d65 2729 0a20 2020  stanceName').   
+00011640: 2020 2020 2069 6620 6d2e 6765 7428 2749       if m.get('I
+00011650: 6e73 7461 6e63 6554 7970 6527 2920 6973  nstanceType') is
+00011660: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00011670: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
+00011680: 616e 6365 5f74 7970 6520 3d20 6d2e 6765  ance_type = m.ge
+00011690: 7428 2749 6e73 7461 6e63 6554 7970 6527  t('InstanceType'
+000116a0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000116b0: 6574 2827 5061 6765 4e75 6d62 6572 2729  et('PageNumber')
+000116c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000116d0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+000116e0: 6167 655f 6e75 6d62 6572 203d 206d 2e67  age_number = m.g
+000116f0: 6574 2827 5061 6765 4e75 6d62 6572 2729  et('PageNumber')
+00011700: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00011710: 7428 2750 6167 6553 697a 6527 2920 6973  t('PageSize') is
+00011720: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00011730: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
+00011740: 5f73 697a 6520 3d20 6d2e 6765 7428 2750  _size = m.get('P
+00011750: 6167 6553 697a 6527 290a 2020 2020 2020  ageSize').      
+00011760: 2020 6966 206d 2e67 6574 2827 5265 6769    if m.get('Regi
+00011770: 6f6e 4964 2729 2069 7320 6e6f 7420 4e6f  onId') is not No
+00011780: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00011790: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
+000117a0: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
+000117b0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000117c0: 6765 7428 2752 6573 6f75 7263 6547 726f  get('ResourceGro
+000117d0: 7570 4964 2729 2069 7320 6e6f 7420 4e6f  upId') is not No
+000117e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000117f0: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
+00011800: 6f75 705f 6964 203d 206d 2e67 6574 2827  oup_id = m.get('
+00011810: 5265 736f 7572 6365 4772 6f75 7049 6427  ResourceGroupId'
+00011820: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00011830: 6574 2827 5374 6174 7573 2729 2069 7320  et('Status') is 
+00011840: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00011850: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00011860: 7320 3d20 6d2e 6765 7428 2753 7461 7475  s = m.get('Statu
+00011870: 7327 290a 2020 2020 2020 2020 7265 7475  s').        retu
+00011880: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00011890: 4465 7363 7269 6265 4561 6973 5265 7370  DescribeEaisResp
+000118a0: 6f6e 7365 426f 6479 496e 7374 616e 6365  onseBodyInstance
+000118b0: 7349 6e73 7461 6e63 6554 6167 7354 6167  sInstanceTagsTag
+000118c0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+000118d0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+000118e0: 662c 2074 6167 5f6b 6579 3d4e 6f6e 652c  f, tag_key=None,
+000118f0: 2074 6167 5f76 616c 7565 3d4e 6f6e 6529   tag_value=None)
+00011900: 3a0a 2020 2020 2020 2020 7365 6c66 2e74  :.        self.t
+00011910: 6167 5f6b 6579 203d 2074 6167 5f6b 6579  ag_key = tag_key
+00011920: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+00011930: 2020 2020 2020 7365 6c66 2e74 6167 5f76        self.tag_v
+00011940: 616c 7565 203d 2074 6167 5f76 616c 7565  alue = tag_value
+00011950: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
+00011960: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+00011970: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00011980: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+00011990: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+000119a0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+000119b0: 4465 7363 7269 6265 4561 6973 5265 7370  DescribeEaisResp
+000119c0: 6f6e 7365 426f 6479 496e 7374 616e 6365  onseBodyInstance
+000119d0: 7349 6e73 7461 6e63 6554 6167 7354 6167  sInstanceTagsTag
+000119e0: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+000119f0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00011a00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00011a10: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011a20: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00011a30: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00011a40: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00011a50: 6167 5f6b 6579 2069 7320 6e6f 7420 4e6f  ag_key is not No
+00011a60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00011a70: 7265 7375 6c74 5b27 5461 674b 6579 275d  result['TagKey']
+00011a80: 203d 2073 656c 662e 7461 675f 6b65 790a   = self.tag_key.
+00011a90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011aa0: 7461 675f 7661 6c75 6520 6973 206e 6f74  tag_value is not
+00011ab0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00011ac0: 2020 2072 6573 756c 745b 2754 6167 5661     result['TagVa
+00011ad0: 6c75 6527 5d20 3d20 7365 6c66 2e74 6167  lue'] = self.tag
+00011ae0: 5f76 616c 7565 0a20 2020 2020 2020 2072  _value.        r
+00011af0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00011b00: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00011b10: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
+00011b20: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00011b30: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00011b40: 206d 2e67 6574 2827 5461 674b 6579 2729   m.get('TagKey')
+00011b50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00011b60: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00011b70: 6167 5f6b 6579 203d 206d 2e67 6574 2827  ag_key = m.get('
+00011b80: 5461 674b 6579 2729 0a20 2020 2020 2020  TagKey').       
+00011b90: 2069 6620 6d2e 6765 7428 2754 6167 5661   if m.get('TagVa
+00011ba0: 6c75 6527 2920 6973 206e 6f74 204e 6f6e  lue') is not Non
+00011bb0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00011bc0: 656c 662e 7461 675f 7661 6c75 6520 3d20  elf.tag_value = 
+00011bd0: 6d2e 6765 7428 2754 6167 5661 6c75 6527  m.get('TagValue'
+00011be0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00011bf0: 2073 656c 660a 0a0a 636c 6173 7320 4465   self...class De
+00011c00: 7363 7269 6265 4561 6973 5265 7370 6f6e  scribeEaisRespon
+00011c10: 7365 426f 6479 496e 7374 616e 6365 7349  seBodyInstancesI
+00011c20: 6e73 7461 6e63 6554 6167 7328 5465 614d  nstanceTags(TeaM
+00011c30: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00011c40: 5f69 6e69 745f 5f28 7365 6c66 2c20 7461  _init__(self, ta
+00011c50: 673d 4e6f 6e65 293a 0a20 2020 2020 2020  g=None):.       
+00011c60: 2073 656c 662e 7461 6720 3d20 7461 6720   self.tag = tag 
+00011c70: 2023 2074 7970 653a 206c 6973 745b 4465   # type: list[De
+00011c80: 7363 7269 6265 4561 6973 5265 7370 6f6e  scribeEaisRespon
+00011c90: 7365 426f 6479 496e 7374 616e 6365 7349  seBodyInstancesI
+00011ca0: 6e73 7461 6e63 6554 6167 7354 6167 5d0a  nstanceTagsTag].
+00011cb0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00011cc0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00011cd0: 2069 6620 7365 6c66 2e74 6167 3a0a 2020   if self.tag:.  
+00011ce0: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+00011cf0: 696e 2073 656c 662e 7461 673a 0a20 2020  in self.tag:.   
+00011d00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011d10: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+00011d20: 2020 2020 2020 206b 2e76 616c 6964 6174         k.validat
+00011d30: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00011d40: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00011d50: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00011d60: 4465 7363 7269 6265 4561 6973 5265 7370  DescribeEaisResp
+00011d70: 6f6e 7365 426f 6479 496e 7374 616e 6365  onseBodyInstance
+00011d80: 7349 6e73 7461 6e63 6554 6167 732c 2073  sInstanceTags, s
+00011d90: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
+00011da0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00011db0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00011dc0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00011dd0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00011de0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00011df0: 2020 2020 7265 7375 6c74 5b27 5461 6727      result['Tag'
+00011e00: 5d20 3d20 5b5d 0a20 2020 2020 2020 2069  ] = [].        i
+00011e10: 6620 7365 6c66 2e74 6167 2069 7320 6e6f  f self.tag is no
+00011e20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00011e30: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
+00011e40: 662e 7461 673a 0a20 2020 2020 2020 2020  f.tag:.         
+00011e50: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
+00011e60: 6167 275d 2e61 7070 656e 6428 6b2e 746f  ag'].append(k.to
+00011e70: 5f6d 6170 2829 2069 6620 6b20 656c 7365  _map() if k else
+00011e80: 204e 6f6e 6529 0a20 2020 2020 2020 2072   None).        r
+00011e90: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00011ea0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00011eb0: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
+00011ec0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00011ed0: 6963 7428 290a 2020 2020 2020 2020 7365  ict().        se
+00011ee0: 6c66 2e74 6167 203d 205b 5d0a 2020 2020  lf.tag = [].    
+00011ef0: 2020 2020 6966 206d 2e67 6574 2827 5461      if m.get('Ta
+00011f00: 6727 2920 6973 206e 6f74 204e 6f6e 653a  g') is not None:
+00011f10: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00011f20: 206b 2069 6e20 6d2e 6765 7428 2754 6167   k in m.get('Tag
+00011f30: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+00011f40: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+00011f50: 2044 6573 6372 6962 6545 6169 7352 6573   DescribeEaisRes
+00011f60: 706f 6e73 6542 6f64 7949 6e73 7461 6e63  ponseBodyInstanc
+00011f70: 6573 496e 7374 616e 6365 5461 6773 5461  esInstanceTagsTa
+00011f80: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+00011f90: 2020 2020 7365 6c66 2e74 6167 2e61 7070      self.tag.app
+00011fa0: 656e 6428 7465 6d70 5f6d 6f64 656c 2e66  end(temp_model.f
+00011fb0: 726f 6d5f 6d61 7028 6b29 290a 2020 2020  rom_map(k)).    
+00011fc0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00011fd0: 0a0a 636c 6173 7320 4465 7363 7269 6265  ..class Describe
+00011fe0: 4561 6973 5265 7370 6f6e 7365 426f 6479  EaisResponseBody
+00011ff0: 496e 7374 616e 6365 7349 6e73 7461 6e63  InstancesInstanc
+00012000: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+00012010: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00012020: 6c66 2c20 6361 7465 676f 7279 3d4e 6f6e  lf, category=Non
+00012030: 652c 2063 6c69 656e 745f 696e 7374 616e  e, client_instan
+00012040: 6365 5f69 643d 4e6f 6e65 2c20 636c 6965  ce_id=None, clie
+00012050: 6e74 5f69 6e73 7461 6e63 655f 6e61 6d65  nt_instance_name
+00012060: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+00012070: 2020 2020 2020 2020 636c 6965 6e74 5f69          client_i
+00012080: 6e73 7461 6e63 655f 7479 7065 3d4e 6f6e  nstance_type=Non
+00012090: 652c 2063 7265 6174 696f 6e5f 7469 6d65  e, creation_time
+000120a0: 3d4e 6f6e 652c 2064 6573 6372 6970 7469  =None, descripti
+000120b0: 6f6e 3d4e 6f6e 652c 2065 6c61 7374 6963  on=None, elastic
+000120c0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+000120d0: 7461 6e63 655f 6964 3d4e 6f6e 652c 0a20  tance_id=None,. 
+000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120f0: 696e 7374 616e 6365 5f6e 616d 653d 4e6f  instance_name=No
+00012100: 6e65 2c20 696e 7374 616e 6365 5f74 7970  ne, instance_typ
+00012110: 653d 4e6f 6e65 2c20 6a75 7079 7465 725f  e=None, jupyter_
+00012120: 7572 6c3d 4e6f 6e65 2c20 7265 6769 6f6e  url=None, region
+00012130: 5f69 643d 4e6f 6e65 2c20 7265 736f 7572  _id=None, resour
+00012140: 6365 5f67 726f 7570 5f69 643d 4e6f 6e65  ce_group_id=None
+00012150: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012160: 2020 2073 6563 7572 6974 795f 6772 6f75     security_grou
+00012170: 705f 6964 3d4e 6f6e 652c 2073 7461 7274  p_id=None, start
+00012180: 5f74 696d 653d 4e6f 6e65 2c20 7374 6174  _time=None, stat
+00012190: 7573 3d4e 6f6e 652c 2074 6167 733d 4e6f  us=None, tags=No
+000121a0: 6e65 2c20 765f 7377 6974 6368 5f69 643d  ne, v_switch_id=
+000121b0: 4e6f 6e65 2c20 7a6f 6e65 5f69 643d 4e6f  None, zone_id=No
+000121c0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+000121d0: 662e 6361 7465 676f 7279 203d 2063 6174  f.category = cat
+000121e0: 6567 6f72 7920 2023 2074 7970 653a 2073  egory  # type: s
+000121f0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+00012200: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
+00012210: 6964 203d 2063 6c69 656e 745f 696e 7374  id = client_inst
+00012220: 616e 6365 5f69 6420 2023 2074 7970 653a  ance_id  # type:
+00012230: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00012240: 662e 636c 6965 6e74 5f69 6e73 7461 6e63  f.client_instanc
+00012250: 655f 6e61 6d65 203d 2063 6c69 656e 745f  e_name = client_
+00012260: 696e 7374 616e 6365 5f6e 616d 6520 2023  instance_name  #
+00012270: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
+00012280: 2020 2073 656c 662e 636c 6965 6e74 5f69     self.client_i
+00012290: 6e73 7461 6e63 655f 7479 7065 203d 2063  nstance_type = c
+000122a0: 6c69 656e 745f 696e 7374 616e 6365 5f74  lient_instance_t
+000122b0: 7970 6520 2023 2074 7970 653a 2073 7472  ype  # type: str
+000122c0: 0a20 2020 2020 2020 2073 656c 662e 6372  .        self.cr
+000122d0: 6561 7469 6f6e 5f74 696d 6520 3d20 6372  eation_time = cr
+000122e0: 6561 7469 6f6e 5f74 696d 6520 2023 2074  eation_time  # t
+000122f0: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00012300: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+00012310: 6e20 3d20 6465 7363 7269 7074 696f 6e20  n = description 
+00012320: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00012330: 2020 2020 2073 656c 662e 656c 6173 7469       self.elasti
+00012340: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
+00012350: 7374 616e 6365 5f69 6420 3d20 656c 6173  stance_id = elas
+00012360: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
+00012370: 696e 7374 616e 6365 5f69 6420 2023 2074  instance_id  # t
+00012380: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00012390: 2073 656c 662e 696e 7374 616e 6365 5f6e   self.instance_n
+000123a0: 616d 6520 3d20 696e 7374 616e 6365 5f6e  ame = instance_n
+000123b0: 616d 6520 2023 2074 7970 653a 2073 7472  ame  # type: str
+000123c0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+000123d0: 7374 616e 6365 5f74 7970 6520 3d20 696e  stance_type = in
+000123e0: 7374 616e 6365 5f74 7970 6520 2023 2074  stance_type  # t
+000123f0: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00012400: 2073 656c 662e 6a75 7079 7465 725f 7572   self.jupyter_ur
+00012410: 6c20 3d20 6a75 7079 7465 725f 7572 6c20  l = jupyter_url 
+00012420: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00012430: 2020 2020 2073 656c 662e 7265 6769 6f6e       self.region
+00012440: 5f69 6420 3d20 7265 6769 6f6e 5f69 6420  _id = region_id 
+00012450: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00012460: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+00012470: 6365 5f67 726f 7570 5f69 6420 3d20 7265  ce_group_id = re
+00012480: 736f 7572 6365 5f67 726f 7570 5f69 6420  source_group_id 
+00012490: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+000124a0: 2020 2020 2073 656c 662e 7365 6375 7269       self.securi
+000124b0: 7479 5f67 726f 7570 5f69 6420 3d20 7365  ty_group_id = se
+000124c0: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
+000124d0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+000124e0: 2020 2020 2073 656c 662e 7374 6172 745f       self.start_
+000124f0: 7469 6d65 203d 2073 7461 7274 5f74 696d  time = start_tim
+00012500: 6520 2023 2074 7970 653a 2073 7472 0a20  e  # type: str. 
+00012510: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00012520: 7573 203d 2073 7461 7475 7320 2023 2074  us = status  # t
+00012530: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+00012540: 2073 656c 662e 7461 6773 203d 2074 6167   self.tags = tag
+00012550: 7320 2023 2074 7970 653a 2044 6573 6372  s  # type: Descr
+00012560: 6962 6545 6169 7352 6573 706f 6e73 6542  ibeEaisResponseB
+00012570: 6f64 7949 6e73 7461 6e63 6573 496e 7374  odyInstancesInst
+00012580: 616e 6365 5461 6773 0a20 2020 2020 2020  anceTags.       
+00012590: 2073 656c 662e 765f 7377 6974 6368 5f69   self.v_switch_i
+000125a0: 6420 3d20 765f 7377 6974 6368 5f69 6420  d = v_switch_id 
+000125b0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+000125c0: 2020 2020 2073 656c 662e 7a6f 6e65 5f69       self.zone_i
+000125d0: 6420 3d20 7a6f 6e65 5f69 6420 2023 2074  d = zone_id  # t
+000125e0: 7970 653a 2073 7472 0a0a 2020 2020 6465  ype: str..    de
+000125f0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00012600: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00012610: 662e 7461 6773 3a0a 2020 2020 2020 2020  f.tags:.        
+00012620: 2020 2020 7365 6c66 2e74 6167 732e 7661      self.tags.va
+00012630: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+00012640: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00012650: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00012660: 7570 6572 2844 6573 6372 6962 6545 6169  uper(DescribeEai
+00012670: 7352 6573 706f 6e73 6542 6f64 7949 6e73  sResponseBodyIns
+00012680: 7461 6e63 6573 496e 7374 616e 6365 2c20  tancesInstance, 
+00012690: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+000126a0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000126b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000126c0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000126d0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000126e0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+000126f0: 2020 2020 2069 6620 7365 6c66 2e63 6174       if self.cat
+00012700: 6567 6f72 7920 6973 206e 6f74 204e 6f6e  egory is not Non
+00012710: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00012720: 6573 756c 745b 2743 6174 6567 6f72 7927  esult['Category'
+00012730: 5d20 3d20 7365 6c66 2e63 6174 6567 6f72  ] = self.categor
+00012740: 790a 2020 2020 2020 2020 6966 2073 656c  y.        if sel
+00012750: 662e 636c 6965 6e74 5f69 6e73 7461 6e63  f.client_instanc
+00012760: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+00012770: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00012780: 7375 6c74 5b27 436c 6965 6e74 496e 7374  sult['ClientInst
+00012790: 616e 6365 4964 275d 203d 2073 656c 662e  anceId'] = self.
+000127a0: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
+000127b0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+000127c0: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
+000127d0: 6365 5f6e 616d 6520 6973 206e 6f74 204e  ce_name is not N
+000127e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000127f0: 2072 6573 756c 745b 2743 6c69 656e 7449   result['ClientI
+00012800: 6e73 7461 6e63 654e 616d 6527 5d20 3d20  nstanceName'] = 
+00012810: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
+00012820: 616e 6365 5f6e 616d 650a 2020 2020 2020  ance_name.      
+00012830: 2020 6966 2073 656c 662e 636c 6965 6e74    if self.client
+00012840: 5f69 6e73 7461 6e63 655f 7479 7065 2069  _instance_type i
+00012850: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00012860: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00012870: 436c 6965 6e74 496e 7374 616e 6365 5479  ClientInstanceTy
+00012880: 7065 275d 203d 2073 656c 662e 636c 6965  pe'] = self.clie
+00012890: 6e74 5f69 6e73 7461 6e63 655f 7479 7065  nt_instance_type
+000128a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000128b0: 2e63 7265 6174 696f 6e5f 7469 6d65 2069  .creation_time i
+000128c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000128d0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000128e0: 4372 6561 7469 6f6e 5469 6d65 275d 203d  CreationTime'] =
+000128f0: 2073 656c 662e 6372 6561 7469 6f6e 5f74   self.creation_t
+00012900: 696d 650a 2020 2020 2020 2020 6966 2073  ime.        if s
+00012910: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
+00012920: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00012930: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00012940: 2744 6573 6372 6970 7469 6f6e 275d 203d  'Description'] =
+00012950: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+00012960: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
+00012970: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
+00012980: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
+00012990: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+000129a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000129b0: 745b 2745 6c61 7374 6963 4163 6365 6c65  t['ElasticAccele
+000129c0: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
+000129d0: 5d20 3d20 7365 6c66 2e65 6c61 7374 6963  ] = self.elastic
+000129e0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+000129f0: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+00012a00: 2069 6620 7365 6c66 2e69 6e73 7461 6e63   if self.instanc
+00012a10: 655f 6e61 6d65 2069 7320 6e6f 7420 4e6f  e_name is not No
+00012a20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00012a30: 7265 7375 6c74 5b27 496e 7374 616e 6365  result['Instance
+00012a40: 4e61 6d65 275d 203d 2073 656c 662e 696e  Name'] = self.in
+00012a50: 7374 616e 6365 5f6e 616d 650a 2020 2020  stance_name.    
+00012a60: 2020 2020 6966 2073 656c 662e 696e 7374      if self.inst
+00012a70: 616e 6365 5f74 7970 6520 6973 206e 6f74  ance_type is not
+00012a80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00012a90: 2020 2072 6573 756c 745b 2749 6e73 7461     result['Insta
+00012aa0: 6e63 6554 7970 6527 5d20 3d20 7365 6c66  nceType'] = self
+00012ab0: 2e69 6e73 7461 6e63 655f 7479 7065 0a20  .instance_type. 
+00012ac0: 2020 2020 2020 2069 6620 7365 6c66 2e6a         if self.j
+00012ad0: 7570 7974 6572 5f75 726c 2069 7320 6e6f  upyter_url is no
+00012ae0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00012af0: 2020 2020 7265 7375 6c74 5b27 4a75 7079      result['Jupy
+00012b00: 7465 7255 726c 275d 203d 2073 656c 662e  terUrl'] = self.
+00012b10: 6a75 7079 7465 725f 7572 6c0a 2020 2020  jupyter_url.    
+00012b20: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
+00012b30: 6f6e 5f69 6420 6973 206e 6f74 204e 6f6e  on_id is not Non
+00012b40: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00012b50: 6573 756c 745b 2752 6567 696f 6e49 6427  esult['RegionId'
+00012b60: 5d20 3d20 7365 6c66 2e72 6567 696f 6e5f  ] = self.region_
+00012b70: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+00012b80: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
+00012b90: 705f 6964 2069 7320 6e6f 7420 4e6f 6e65  p_id is not None
+00012ba0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00012bb0: 7375 6c74 5b27 5265 736f 7572 6365 4772  sult['ResourceGr
+00012bc0: 6f75 7049 6427 5d20 3d20 7365 6c66 2e72  oupId'] = self.r
+00012bd0: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
+00012be0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00012bf0: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
+00012c00: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00012c10: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00012c20: 6c74 5b27 5365 6375 7269 7479 4772 6f75  lt['SecurityGrou
+00012c30: 7049 6427 5d20 3d20 7365 6c66 2e73 6563  pId'] = self.sec
+00012c40: 7572 6974 795f 6772 6f75 705f 6964 0a20  urity_group_id. 
+00012c50: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00012c60: 7461 7274 5f74 696d 6520 6973 206e 6f74  tart_time is not
+00012c70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00012c80: 2020 2072 6573 756c 745b 2753 7461 7274     result['Start
+00012c90: 5469 6d65 275d 203d 2073 656c 662e 7374  Time'] = self.st
+00012ca0: 6172 745f 7469 6d65 0a20 2020 2020 2020  art_time.       
+00012cb0: 2069 6620 7365 6c66 2e73 7461 7475 7320   if self.status 
+00012cc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00012cd0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00012ce0: 2753 7461 7475 7327 5d20 3d20 7365 6c66  'Status'] = self
+00012cf0: 2e73 7461 7475 730a 2020 2020 2020 2020  .status.        
+00012d00: 6966 2073 656c 662e 7461 6773 2069 7320  if self.tags is 
+00012d10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00012d20: 2020 2020 2020 7265 7375 6c74 5b27 5461        result['Ta
+00012d30: 6773 275d 203d 2073 656c 662e 7461 6773  gs'] = self.tags
+00012d40: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00012d50: 2020 6966 2073 656c 662e 765f 7377 6974    if self.v_swit
+00012d60: 6368 5f69 6420 6973 206e 6f74 204e 6f6e  ch_id is not Non
+00012d70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00012d80: 6573 756c 745b 2756 5377 6974 6368 4964  esult['VSwitchId
+00012d90: 275d 203d 2073 656c 662e 765f 7377 6974  '] = self.v_swit
+00012da0: 6368 5f69 640a 2020 2020 2020 2020 6966  ch_id.        if
+00012db0: 2073 656c 662e 7a6f 6e65 5f69 6420 6973   self.zone_id is
+00012dc0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00012dd0: 2020 2020 2020 2072 6573 756c 745b 275a         result['Z
+00012de0: 6f6e 6549 6427 5d20 3d20 7365 6c66 2e7a  oneId'] = self.z
+00012df0: 6f6e 655f 6964 0a20 2020 2020 2020 2072  one_id.        r
+00012e00: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00012e10: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00012e20: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
+00012e30: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00012e40: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00012e50: 206d 2e67 6574 2827 4361 7465 676f 7279   m.get('Category
+00012e60: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00012e70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012e80: 2e63 6174 6567 6f72 7920 3d20 6d2e 6765  .category = m.ge
+00012e90: 7428 2743 6174 6567 6f72 7927 290a 2020  t('Category').  
+00012ea0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00012eb0: 436c 6965 6e74 496e 7374 616e 6365 4964  ClientInstanceId
+00012ec0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00012ed0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012ee0: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
+00012ef0: 5f69 6420 3d20 6d2e 6765 7428 2743 6c69  _id = m.get('Cli
+00012f00: 656e 7449 6e73 7461 6e63 6549 6427 290a  entInstanceId').
+00012f10: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00012f20: 2827 436c 6965 6e74 496e 7374 616e 6365  ('ClientInstance
+00012f30: 4e61 6d65 2729 2069 7320 6e6f 7420 4e6f  Name') is not No
+00012f40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00012f50: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
+00012f60: 616e 6365 5f6e 616d 6520 3d20 6d2e 6765  ance_name = m.ge
+00012f70: 7428 2743 6c69 656e 7449 6e73 7461 6e63  t('ClientInstanc
+00012f80: 654e 616d 6527 290a 2020 2020 2020 2020  eName').        
+00012f90: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
+00012fa0: 496e 7374 616e 6365 5479 7065 2729 2069  InstanceType') i
+00012fb0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00012fc0: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
+00012fd0: 656e 745f 696e 7374 616e 6365 5f74 7970  ent_instance_typ
+00012fe0: 6520 3d20 6d2e 6765 7428 2743 6c69 656e  e = m.get('Clien
+00012ff0: 7449 6e73 7461 6e63 6554 7970 6527 290a  tInstanceType').
+00013000: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00013010: 2827 4372 6561 7469 6f6e 5469 6d65 2729  ('CreationTime')
+00013020: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00013030: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00013040: 7265 6174 696f 6e5f 7469 6d65 203d 206d  reation_time = m
+00013050: 2e67 6574 2827 4372 6561 7469 6f6e 5469  .get('CreationTi
+00013060: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
+00013070: 6d2e 6765 7428 2744 6573 6372 6970 7469  m.get('Descripti
+00013080: 6f6e 2729 2069 7320 6e6f 7420 4e6f 6e65  on') is not None
+00013090: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000130a0: 6c66 2e64 6573 6372 6970 7469 6f6e 203d  lf.description =
+000130b0: 206d 2e67 6574 2827 4465 7363 7269 7074   m.get('Descript
+000130c0: 696f 6e27 290a 2020 2020 2020 2020 6966  ion').        if
+000130d0: 206d 2e67 6574 2827 456c 6173 7469 6341   m.get('ElasticA
+000130e0: 6363 656c 6572 6174 6564 496e 7374 616e  cceleratedInstan
+000130f0: 6365 4964 2729 2069 7320 6e6f 7420 4e6f  ceId') is not No
+00013100: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00013110: 7365 6c66 2e65 6c61 7374 6963 5f61 6363  self.elastic_acc
+00013120: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
+00013130: 655f 6964 203d 206d 2e67 6574 2827 456c  e_id = m.get('El
+00013140: 6173 7469 6341 6363 656c 6572 6174 6564  asticAccelerated
+00013150: 496e 7374 616e 6365 4964 2729 0a20 2020  InstanceId').   
+00013160: 2020 2020 2069 6620 6d2e 6765 7428 2749       if m.get('I
+00013170: 6e73 7461 6e63 654e 616d 6527 2920 6973  nstanceName') is
+00013180: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00013190: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
+000131a0: 616e 6365 5f6e 616d 6520 3d20 6d2e 6765  ance_name = m.ge
+000131b0: 7428 2749 6e73 7461 6e63 654e 616d 6527  t('InstanceName'
+000131c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000131d0: 6574 2827 496e 7374 616e 6365 5479 7065  et('InstanceType
+000131e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000131f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013200: 2e69 6e73 7461 6e63 655f 7479 7065 203d  .instance_type =
+00013210: 206d 2e67 6574 2827 496e 7374 616e 6365   m.get('Instance
+00013220: 5479 7065 2729 0a20 2020 2020 2020 2069  Type').        i
+00013230: 6620 6d2e 6765 7428 274a 7570 7974 6572  f m.get('Jupyter
+00013240: 5572 6c27 2920 6973 206e 6f74 204e 6f6e  Url') is not Non
+00013250: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00013260: 656c 662e 6a75 7079 7465 725f 7572 6c20  elf.jupyter_url 
+00013270: 3d20 6d2e 6765 7428 274a 7570 7974 6572  = m.get('Jupyter
+00013280: 5572 6c27 290a 2020 2020 2020 2020 6966  Url').        if
+00013290: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
+000132a0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000132b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000132c0: 2e72 6567 696f 6e5f 6964 203d 206d 2e67  .region_id = m.g
+000132d0: 6574 2827 5265 6769 6f6e 4964 2729 0a20  et('RegionId'). 
+000132e0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000132f0: 2752 6573 6f75 7263 6547 726f 7570 4964  'ResourceGroupId
+00013300: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00013310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013320: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
+00013330: 6964 203d 206d 2e67 6574 2827 5265 736f  id = m.get('Reso
+00013340: 7572 6365 4772 6f75 7049 6427 290a 2020  urceGroupId').  
+00013350: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00013360: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
+00013370: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00013380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013390: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
+000133a0: 6420 3d20 6d2e 6765 7428 2753 6563 7572  d = m.get('Secur
+000133b0: 6974 7947 726f 7570 4964 2729 0a20 2020  ityGroupId').   
+000133c0: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
+000133d0: 7461 7274 5469 6d65 2729 2069 7320 6e6f  tartTime') is no
+000133e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000133f0: 2020 2020 7365 6c66 2e73 7461 7274 5f74      self.start_t
+00013400: 696d 6520 3d20 6d2e 6765 7428 2753 7461  ime = m.get('Sta
+00013410: 7274 5469 6d65 2729 0a20 2020 2020 2020  rtTime').       
+00013420: 2069 6620 6d2e 6765 7428 2753 7461 7475   if m.get('Statu
+00013430: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00013440: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013450: 662e 7374 6174 7573 203d 206d 2e67 6574  f.status = m.get
+00013460: 2827 5374 6174 7573 2729 0a20 2020 2020  ('Status').     
+00013470: 2020 2069 6620 6d2e 6765 7428 2754 6167     if m.get('Tag
+00013480: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00013490: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+000134a0: 705f 6d6f 6465 6c20 3d20 4465 7363 7269  p_model = Descri
+000134b0: 6265 4561 6973 5265 7370 6f6e 7365 426f  beEaisResponseBo
+000134c0: 6479 496e 7374 616e 6365 7349 6e73 7461  dyInstancesInsta
+000134d0: 6e63 6554 6167 7328 290a 2020 2020 2020  nceTags().      
+000134e0: 2020 2020 2020 7365 6c66 2e74 6167 7320        self.tags 
+000134f0: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+00013500: 6d5f 6d61 7028 6d5b 2754 6167 7327 5d29  m_map(m['Tags'])
+00013510: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00013520: 7428 2756 5377 6974 6368 4964 2729 2069  t('VSwitchId') i
+00013530: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00013540: 2020 2020 2020 2020 7365 6c66 2e76 5f73          self.v_s
+00013550: 7769 7463 685f 6964 203d 206d 2e67 6574  witch_id = m.get
+00013560: 2827 5653 7769 7463 6849 6427 290a 2020  ('VSwitchId').  
+00013570: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00013580: 5a6f 6e65 4964 2729 2069 7320 6e6f 7420  ZoneId') is not 
+00013590: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000135a0: 2020 7365 6c66 2e7a 6f6e 655f 6964 203d    self.zone_id =
+000135b0: 206d 2e67 6574 2827 5a6f 6e65 4964 2729   m.get('ZoneId')
+000135c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000135d0: 7365 6c66 0a0a 0a63 6c61 7373 2044 6573  self...class Des
+000135e0: 6372 6962 6545 6169 7352 6573 706f 6e73  cribeEaisRespons
+000135f0: 6542 6f64 7949 6e73 7461 6e63 6573 2854  eBodyInstances(T
+00013600: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00013610: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00013620: 2069 6e73 7461 6e63 653d 4e6f 6e65 293a   instance=None):
+00013630: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00013640: 7374 616e 6365 203d 2069 6e73 7461 6e63  stance = instanc
+00013650: 6520 2023 2074 7970 653a 206c 6973 745b  e  # type: list[
+00013660: 4465 7363 7269 6265 4561 6973 5265 7370  DescribeEaisResp
+00013670: 6f6e 7365 426f 6479 496e 7374 616e 6365  onseBodyInstance
+00013680: 7349 6e73 7461 6e63 655d 0a0a 2020 2020  sInstance]..    
+00013690: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+000136a0: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+000136b0: 656c 662e 696e 7374 616e 6365 3a0a 2020  elf.instance:.  
+000136c0: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+000136d0: 696e 2073 656c 662e 696e 7374 616e 6365  in self.instance
+000136e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000136f0: 2020 6966 206b 3a0a 2020 2020 2020 2020    if k:.        
+00013700: 2020 2020 2020 2020 2020 2020 6b2e 7661              k.va
+00013710: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+00013720: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00013730: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00013740: 7570 6572 2844 6573 6372 6962 6545 6169  uper(DescribeEai
+00013750: 7352 6573 706f 6e73 6542 6f64 7949 6e73  sResponseBodyIns
+00013760: 7461 6e63 6573 2c20 7365 6c66 292e 746f  tances, self).to
+00013770: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00013780: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00013790: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000137a0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000137b0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000137c0: 6374 2829 0a20 2020 2020 2020 2072 6573  ct().        res
+000137d0: 756c 745b 2749 6e73 7461 6e63 6527 5d20  ult['Instance'] 
+000137e0: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
+000137f0: 7365 6c66 2e69 6e73 7461 6e63 6520 6973  self.instance is
+00013800: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00013810: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00013820: 7365 6c66 2e69 6e73 7461 6e63 653a 0a20  self.instance:. 
+00013830: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00013840: 6573 756c 745b 2749 6e73 7461 6e63 6527  esult['Instance'
+00013850: 5d2e 6170 7065 6e64 286b 2e74 6f5f 6d61  ].append(k.to_ma
+00013860: 7028 2920 6966 206b 2065 6c73 6520 4e6f  p() if k else No
+00013870: 6e65 290a 2020 2020 2020 2020 7265 7475  ne).        retu
+00013880: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00013890: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+000138a0: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+000138b0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+000138c0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000138d0: 696e 7374 616e 6365 203d 205b 5d0a 2020  instance = [].  
+000138e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000138f0: 496e 7374 616e 6365 2729 2069 7320 6e6f  Instance') is no
+00013900: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00013910: 2020 2020 666f 7220 6b20 696e 206d 2e67      for k in m.g
+00013920: 6574 2827 496e 7374 616e 6365 2729 3a0a  et('Instance'):.
+00013930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013940: 7465 6d70 5f6d 6f64 656c 203d 2044 6573  temp_model = Des
+00013950: 6372 6962 6545 6169 7352 6573 706f 6e73  cribeEaisRespons
+00013960: 6542 6f64 7949 6e73 7461 6e63 6573 496e  eBodyInstancesIn
+00013970: 7374 616e 6365 2829 0a20 2020 2020 2020  stance().       
+00013980: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
+00013990: 7374 616e 6365 2e61 7070 656e 6428 7465  stance.append(te
+000139a0: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
+000139b0: 7028 6b29 290a 2020 2020 2020 2020 7265  p(k)).        re
+000139c0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+000139d0: 7320 4465 7363 7269 6265 4561 6973 5265  s DescribeEaisRe
+000139e0: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
+000139f0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00013a00: 696e 6974 5f5f 2873 656c 662c 2069 6e73  init__(self, ins
+00013a10: 7461 6e63 6573 3d4e 6f6e 652c 2070 6167  tances=None, pag
+00013a20: 655f 6e75 6d62 6572 3d4e 6f6e 652c 2070  e_number=None, p
+00013a30: 6167 655f 7369 7a65 3d4e 6f6e 652c 2072  age_size=None, r
+00013a40: 6571 7565 7374 5f69 643d 4e6f 6e65 2c20  equest_id=None, 
+00013a50: 746f 7461 6c5f 636f 756e 743d 4e6f 6e65  total_count=None
+00013a60: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00013a70: 696e 7374 616e 6365 7320 3d20 696e 7374  instances = inst
+00013a80: 616e 6365 7320 2023 2074 7970 653a 2044  ances  # type: D
+00013a90: 6573 6372 6962 6545 6169 7352 6573 706f  escribeEaisRespo
+00013aa0: 6e73 6542 6f64 7949 6e73 7461 6e63 6573  nseBodyInstances
+00013ab0: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
+00013ac0: 6765 5f6e 756d 6265 7220 3d20 7061 6765  ge_number = page
+00013ad0: 5f6e 756d 6265 7220 2023 2074 7970 653a  _number  # type:
+00013ae0: 2069 6e74 0a20 2020 2020 2020 2073 656c   int.        sel
+00013af0: 662e 7061 6765 5f73 697a 6520 3d20 7061  f.page_size = pa
+00013b00: 6765 5f73 697a 6520 2023 2074 7970 653a  ge_size  # type:
+00013b10: 2069 6e74 0a20 2020 2020 2020 2073 656c   int.        sel
+00013b20: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
+00013b30: 6571 7565 7374 5f69 6420 2023 2074 7970  equest_id  # typ
+00013b40: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+00013b50: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
+00013b60: 3d20 746f 7461 6c5f 636f 756e 7420 2023  = total_count  #
+00013b70: 2074 7970 653a 2069 6e74 0a0a 2020 2020   type: int..    
+00013b80: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00013b90: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+00013ba0: 656c 662e 696e 7374 616e 6365 733a 0a20  elf.instances:. 
+00013bb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013bc0: 696e 7374 616e 6365 732e 7661 6c69 6461  instances.valida
+00013bd0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+00013be0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00013bf0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00013c00: 2844 6573 6372 6962 6545 6169 7352 6573  (DescribeEaisRes
+00013c10: 706f 6e73 6542 6f64 792c 2073 656c 6629  ponseBody, self)
+00013c20: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00013c30: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00013c40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00013c50: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00013c60: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00013c70: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00013c80: 6966 2073 656c 662e 696e 7374 616e 6365  if self.instance
+00013c90: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00013ca0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00013cb0: 745b 2749 6e73 7461 6e63 6573 275d 203d  t['Instances'] =
+00013cc0: 2073 656c 662e 696e 7374 616e 6365 732e   self.instances.
+00013cd0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00013ce0: 2069 6620 7365 6c66 2e70 6167 655f 6e75   if self.page_nu
+00013cf0: 6d62 6572 2069 7320 6e6f 7420 4e6f 6e65  mber is not None
+00013d00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00013d10: 7375 6c74 5b27 5061 6765 4e75 6d62 6572  sult['PageNumber
+00013d20: 275d 203d 2073 656c 662e 7061 6765 5f6e  '] = self.page_n
+00013d30: 756d 6265 720a 2020 2020 2020 2020 6966  umber.        if
+00013d40: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
+00013d50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00013d60: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00013d70: 2750 6167 6553 697a 6527 5d20 3d20 7365  'PageSize'] = se
+00013d80: 6c66 2e70 6167 655f 7369 7a65 0a20 2020  lf.page_size.   
+00013d90: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
+00013da0: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
+00013db0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013dc0: 2072 6573 756c 745b 2752 6571 7565 7374   result['Request
+00013dd0: 4964 275d 203d 2073 656c 662e 7265 7175  Id'] = self.requ
+00013de0: 6573 745f 6964 0a20 2020 2020 2020 2069  est_id.        i
+00013df0: 6620 7365 6c66 2e74 6f74 616c 5f63 6f75  f self.total_cou
+00013e00: 6e74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  nt is not None:.
+00013e10: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00013e20: 6c74 5b27 546f 7461 6c43 6f75 6e74 275d  lt['TotalCount']
+00013e30: 203d 2073 656c 662e 746f 7461 6c5f 636f   = self.total_co
+00013e40: 756e 740a 2020 2020 2020 2020 7265 7475  unt.        retu
+00013e50: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00013e60: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00013e70: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+00013e80: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00013e90: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00013ea0: 6765 7428 2749 6e73 7461 6e63 6573 2729  get('Instances')
+00013eb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00013ec0: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+00013ed0: 6f64 656c 203d 2044 6573 6372 6962 6545  odel = DescribeE
+00013ee0: 6169 7352 6573 706f 6e73 6542 6f64 7949  aisResponseBodyI
+00013ef0: 6e73 7461 6e63 6573 2829 0a20 2020 2020  nstances().     
+00013f00: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
+00013f10: 616e 6365 7320 3d20 7465 6d70 5f6d 6f64  ances = temp_mod
+00013f20: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2749  el.from_map(m['I
+00013f30: 6e73 7461 6e63 6573 275d 290a 2020 2020  nstances']).    
+00013f40: 2020 2020 6966 206d 2e67 6574 2827 5061      if m.get('Pa
+00013f50: 6765 4e75 6d62 6572 2729 2069 7320 6e6f  geNumber') is no
+00013f60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00013f70: 2020 2020 7365 6c66 2e70 6167 655f 6e75      self.page_nu
+00013f80: 6d62 6572 203d 206d 2e67 6574 2827 5061  mber = m.get('Pa
+00013f90: 6765 4e75 6d62 6572 2729 0a20 2020 2020  geNumber').     
+00013fa0: 2020 2069 6620 6d2e 6765 7428 2750 6167     if m.get('Pag
+00013fb0: 6553 697a 6527 2920 6973 206e 6f74 204e  eSize') is not N
+00013fc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013fd0: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
+00013fe0: 3d20 6d2e 6765 7428 2750 6167 6553 697a  = m.get('PageSiz
+00013ff0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00014000: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+00014010: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00014020: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014030: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
+00014040: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
+00014050: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00014060: 2827 546f 7461 6c43 6f75 6e74 2729 2069  ('TotalCount') i
+00014070: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00014080: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
+00014090: 616c 5f63 6f75 6e74 203d 206d 2e67 6574  al_count = m.get
+000140a0: 2827 546f 7461 6c43 6f75 6e74 2729 0a20  ('TotalCount'). 
+000140b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000140c0: 6c66 0a0a 0a63 6c61 7373 2044 6573 6372  lf...class Descr
+000140d0: 6962 6545 6169 7352 6573 706f 6e73 6528  ibeEaisResponse(
+000140e0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+000140f0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00014100: 2c20 6865 6164 6572 733d 4e6f 6e65 2c20  , headers=None, 
+00014110: 7374 6174 7573 5f63 6f64 653d 4e6f 6e65  status_code=None
+00014120: 2c20 626f 6479 3d4e 6f6e 6529 3a0a 2020  , body=None):.  
+00014130: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00014140: 7273 203d 2068 6561 6465 7273 2020 2320  rs = headers  # 
+00014150: 7479 7065 3a20 6469 6374 5b73 7472 2c20  type: dict[str, 
+00014160: 7374 725d 0a20 2020 2020 2020 2073 656c  str].        sel
+00014170: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00014180: 7374 6174 7573 5f63 6f64 6520 2023 2074  status_code  # t
+00014190: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+000141a0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+000141b0: 7920 2023 2074 7970 653a 2044 6573 6372  y  # type: Descr
+000141c0: 6962 6545 6169 7352 6573 706f 6e73 6542  ibeEaisResponseB
+000141d0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+000141e0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000141f0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+00014200: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+00014210: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
+00014220: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
+00014230: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00014240: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
+00014250: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
+00014260: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
+00014270: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00014280: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
+00014290: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
+000142a0: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
+000142b0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000142c0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
+000142d0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+000142e0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+000142f0: 7020 3d20 7375 7065 7228 4465 7363 7269  p = super(Descri
+00014300: 6265 4561 6973 5265 7370 6f6e 7365 2c20  beEaisResponse, 
+00014310: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+00014320: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00014330: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00014340: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00014350: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00014360: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00014370: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+00014380: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+00014390: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000143a0: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+000143b0: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+000143c0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+000143d0: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+000143e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000143f0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+00014400: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+00014410: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+00014420: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00014430: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00014440: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00014450: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+00014460: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+00014470: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00014480: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00014490: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+000144a0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000144b0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000144c0: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+000144d0: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+000144e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000144f0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00014500: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+00014510: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00014520: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00014530: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00014540: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00014550: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+00014560: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00014570: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00014580: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+00014590: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000145a0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+000145b0: 4465 7363 7269 6265 4561 6973 5265 7370  DescribeEaisResp
+000145c0: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+000145d0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000145e0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+000145f0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00014600: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00014610: 2073 656c 660a 0a0a 636c 6173 7320 4465   self...class De
+00014620: 7363 7269 6265 5265 6769 6f6e 7352 6573  scribeRegionsRes
+00014630: 706f 6e73 6542 6f64 7952 6567 696f 6e73  ponseBodyRegions
+00014640: 5265 6769 6f6e 2854 6561 4d6f 6465 6c29  Region(TeaModel)
+00014650: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00014660: 5f5f 2873 656c 662c 206c 6f63 616c 5f6e  __(self, local_n
+00014670: 616d 653d 4e6f 6e65 2c20 7265 6769 6f6e  ame=None, region
+00014680: 5f65 6e64 706f 696e 743d 4e6f 6e65 2c20  _endpoint=None, 
+00014690: 7265 6769 6f6e 5f69 643d 4e6f 6e65 293a  region_id=None):
+000146a0: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+000146b0: 6361 6c5f 6e61 6d65 203d 206c 6f63 616c  cal_name = local
+000146c0: 5f6e 616d 6520 2023 2074 7970 653a 2073  _name  # type: s
+000146d0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+000146e0: 7265 6769 6f6e 5f65 6e64 706f 696e 7420  region_endpoint 
+000146f0: 3d20 7265 6769 6f6e 5f65 6e64 706f 696e  = region_endpoin
+00014700: 7420 2023 2074 7970 653a 2073 7472 0a20  t  # type: str. 
+00014710: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
+00014720: 6f6e 5f69 6420 3d20 7265 6769 6f6e 5f69  on_id = region_i
+00014730: 6420 2023 2074 7970 653a 2073 7472 0a0a  d  # type: str..
+00014740: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00014750: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00014760: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+00014770: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00014780: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00014790: 2844 6573 6372 6962 6552 6567 696f 6e73  (DescribeRegions
+000147a0: 5265 7370 6f6e 7365 426f 6479 5265 6769  ResponseBodyRegi
+000147b0: 6f6e 7352 6567 696f 6e2c 2073 656c 6629  onsRegion, self)
+000147c0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000147d0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+000147e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000147f0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00014800: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00014810: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00014820: 6966 2073 656c 662e 6c6f 6361 6c5f 6e61  if self.local_na
+00014830: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+00014840: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00014850: 6c74 5b27 4c6f 6361 6c4e 616d 6527 5d20  lt['LocalName'] 
+00014860: 3d20 7365 6c66 2e6c 6f63 616c 5f6e 616d  = self.local_nam
+00014870: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00014880: 662e 7265 6769 6f6e 5f65 6e64 706f 696e  f.region_endpoin
+00014890: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+000148a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000148b0: 745b 2752 6567 696f 6e45 6e64 706f 696e  t['RegionEndpoin
+000148c0: 7427 5d20 3d20 7365 6c66 2e72 6567 696f  t'] = self.regio
+000148d0: 6e5f 656e 6470 6f69 6e74 0a20 2020 2020  n_endpoint.     
+000148e0: 2020 2069 6620 7365 6c66 2e72 6567 696f     if self.regio
+000148f0: 6e5f 6964 2069 7320 6e6f 7420 4e6f 6e65  n_id is not None
+00014900: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00014910: 7375 6c74 5b27 5265 6769 6f6e 4964 275d  sult['RegionId']
+00014920: 203d 2073 656c 662e 7265 6769 6f6e 5f69   = self.region_i
+00014930: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+00014940: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00014950: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00014960: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+00014970: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00014980: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00014990: 7428 274c 6f63 616c 4e61 6d65 2729 2069  t('LocalName') i
+000149a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000149b0: 2020 2020 2020 2020 7365 6c66 2e6c 6f63          self.loc
+000149c0: 616c 5f6e 616d 6520 3d20 6d2e 6765 7428  al_name = m.get(
+000149d0: 274c 6f63 616c 4e61 6d65 2729 0a20 2020  'LocalName').   
+000149e0: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+000149f0: 6567 696f 6e45 6e64 706f 696e 7427 2920  egionEndpoint') 
+00014a00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00014a10: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00014a20: 6769 6f6e 5f65 6e64 706f 696e 7420 3d20  gion_endpoint = 
+00014a30: 6d2e 6765 7428 2752 6567 696f 6e45 6e64  m.get('RegionEnd
+00014a40: 706f 696e 7427 290a 2020 2020 2020 2020  point').        
+00014a50: 6966 206d 2e67 6574 2827 5265 6769 6f6e  if m.get('Region
+00014a60: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00014a70: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00014a80: 6c66 2e72 6567 696f 6e5f 6964 203d 206d  lf.region_id = m
+00014a90: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
+00014aa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00014ab0: 7365 6c66 0a0a 0a63 6c61 7373 2044 6573  self...class Des
+00014ac0: 6372 6962 6552 6567 696f 6e73 5265 7370  cribeRegionsResp
+00014ad0: 6f6e 7365 426f 6479 5265 6769 6f6e 7328  onseBodyRegions(
+00014ae0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00014af0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00014b00: 2c20 7265 6769 6f6e 3d4e 6f6e 6529 3a0a  , region=None):.
+00014b10: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
+00014b20: 696f 6e20 3d20 7265 6769 6f6e 2020 2320  ion = region  # 
+00014b30: 7479 7065 3a20 6c69 7374 5b44 6573 6372  type: list[Descr
+00014b40: 6962 6552 6567 696f 6e73 5265 7370 6f6e  ibeRegionsRespon
+00014b50: 7365 426f 6479 5265 6769 6f6e 7352 6567  seBodyRegionsReg
+00014b60: 696f 6e5d 0a0a 2020 2020 6465 6620 7661  ion]..    def va
+00014b70: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00014b80: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+00014b90: 6769 6f6e 3a0a 2020 2020 2020 2020 2020  gion:.          
+00014ba0: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
+00014bb0: 7265 6769 6f6e 3a0a 2020 2020 2020 2020  region:.        
+00014bc0: 2020 2020 2020 2020 6966 206b 3a0a 2020          if k:.  
+00014bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014be0: 2020 6b2e 7661 6c69 6461 7465 2829 0a0a    k.validate()..
+00014bf0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00014c00: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00014c10: 6170 203d 2073 7570 6572 2844 6573 6372  ap = super(Descr
+00014c20: 6962 6552 6567 696f 6e73 5265 7370 6f6e  ibeRegionsRespon
+00014c30: 7365 426f 6479 5265 6769 6f6e 732c 2073  seBodyRegions, s
+00014c40: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
+00014c50: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00014c60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00014c70: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00014c80: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00014c90: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00014ca0: 2020 2020 7265 7375 6c74 5b27 5265 6769      result['Regi
+00014cb0: 6f6e 275d 203d 205b 5d0a 2020 2020 2020  on'] = [].      
+00014cc0: 2020 6966 2073 656c 662e 7265 6769 6f6e    if self.region
+00014cd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00014ce0: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+00014cf0: 696e 2073 656c 662e 7265 6769 6f6e 3a0a  in self.region:.
+00014d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d10: 7265 7375 6c74 5b27 5265 6769 6f6e 275d  result['Region']
+00014d20: 2e61 7070 656e 6428 6b2e 746f 5f6d 6170  .append(k.to_map
+00014d30: 2829 2069 6620 6b20 656c 7365 204e 6f6e  () if k else Non
+00014d40: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+00014d50: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00014d60: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00014d70: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+00014d80: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+00014d90: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+00014da0: 6567 696f 6e20 3d20 5b5d 0a20 2020 2020  egion = [].     
+00014db0: 2020 2069 6620 6d2e 6765 7428 2752 6567     if m.get('Reg
+00014dc0: 696f 6e27 2920 6973 206e 6f74 204e 6f6e  ion') is not Non
+00014dd0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+00014de0: 6f72 206b 2069 6e20 6d2e 6765 7428 2752  or k in m.get('R
+00014df0: 6567 696f 6e27 293a 0a20 2020 2020 2020  egion'):.       
+00014e00: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+00014e10: 6465 6c20 3d20 4465 7363 7269 6265 5265  del = DescribeRe
+00014e20: 6769 6f6e 7352 6573 706f 6e73 6542 6f64  gionsResponseBod
+00014e30: 7952 6567 696f 6e73 5265 6769 6f6e 2829  yRegionsRegion()
+00014e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014e50: 2073 656c 662e 7265 6769 6f6e 2e61 7070   self.region.app
+00014e60: 656e 6428 7465 6d70 5f6d 6f64 656c 2e66  end(temp_model.f
+00014e70: 726f 6d5f 6d61 7028 6b29 290a 2020 2020  rom_map(k)).    
+00014e80: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00014e90: 0a0a 636c 6173 7320 4465 7363 7269 6265  ..class Describe
+00014ea0: 5265 6769 6f6e 7352 6573 706f 6e73 6542  RegionsResponseB
+00014eb0: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
+00014ec0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00014ed0: 7365 6c66 2c20 7265 6769 6f6e 733d 4e6f  self, regions=No
+00014ee0: 6e65 2c20 7265 7175 6573 745f 6964 3d4e  ne, request_id=N
+00014ef0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+00014f00: 6c66 2e72 6567 696f 6e73 203d 2072 6567  lf.regions = reg
+00014f10: 696f 6e73 2020 2320 7479 7065 3a20 4465  ions  # type: De
+00014f20: 7363 7269 6265 5265 6769 6f6e 7352 6573  scribeRegionsRes
+00014f30: 706f 6e73 6542 6f64 7952 6567 696f 6e73  ponseBodyRegions
+00014f40: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00014f50: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
+00014f60: 7374 5f69 6420 2023 2074 7970 653a 2073  st_id  # type: s
+00014f70: 7472 0a0a 2020 2020 6465 6620 7661 6c69  tr..    def vali
+00014f80: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00014f90: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
+00014fa0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
+00014fb0: 2073 656c 662e 7265 6769 6f6e 732e 7661   self.regions.va
+00014fc0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+00014fd0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00014fe0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00014ff0: 7570 6572 2844 6573 6372 6962 6552 6567  uper(DescribeReg
+00015000: 696f 6e73 5265 7370 6f6e 7365 426f 6479  ionsResponseBody
+00015010: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+00015020: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00015030: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00015040: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00015050: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00015060: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00015070: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00015080: 6567 696f 6e73 2069 7320 6e6f 7420 4e6f  egions is not No
+00015090: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000150a0: 7265 7375 6c74 5b27 5265 6769 6f6e 7327  result['Regions'
+000150b0: 5d20 3d20 7365 6c66 2e72 6567 696f 6e73  ] = self.regions
+000150c0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000150d0: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
+000150e0: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
+000150f0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00015100: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
+00015110: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
+00015120: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+00015130: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00015140: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00015150: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+00015160: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00015170: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00015180: 6765 7428 2752 6567 696f 6e73 2729 2069  get('Regions') i
+00015190: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000151a0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+000151b0: 656c 203d 2044 6573 6372 6962 6552 6567  el = DescribeReg
+000151c0: 696f 6e73 5265 7370 6f6e 7365 426f 6479  ionsResponseBody
+000151d0: 5265 6769 6f6e 7328 290a 2020 2020 2020  Regions().      
+000151e0: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
+000151f0: 6e73 203d 2074 656d 705f 6d6f 6465 6c2e  ns = temp_model.
+00015200: 6672 6f6d 5f6d 6170 286d 5b27 5265 6769  from_map(m['Regi
+00015210: 6f6e 7327 5d29 0a20 2020 2020 2020 2069  ons']).        i
+00015220: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
+00015230: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00015240: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00015250: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+00015260: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+00015270: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+00015280: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2044  n self...class D
+00015290: 6573 6372 6962 6552 6567 696f 6e73 5265  escribeRegionsRe
+000152a0: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+000152b0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+000152c0: 5f5f 2873 656c 662c 2068 6561 6465 7273  __(self, headers
+000152d0: 3d4e 6f6e 652c 2073 7461 7475 735f 636f  =None, status_co
+000152e0: 6465 3d4e 6f6e 652c 2062 6f64 793d 4e6f  de=None, body=No
+000152f0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+00015300: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00015310: 6572 7320 2023 2074 7970 653a 2064 6963  ers  # type: dic
+00015320: 745b 7374 722c 2073 7472 5d0a 2020 2020  t[str, str].    
+00015330: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00015340: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00015350: 6465 2020 2320 7479 7065 3a20 696e 740a  de  # type: int.
+00015360: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00015370: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
+00015380: 3a20 4465 7363 7269 6265 5265 6769 6f6e  : DescribeRegion
+00015390: 7352 6573 706f 6e73 6542 6f64 790a 0a20  sResponseBody.. 
+000153a0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+000153b0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+000153c0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+000153d0: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
+000153e0: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
+000153f0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+00015400: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+00015410: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
+00015420: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
+00015430: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+00015440: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+00015450: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
+00015460: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00015470: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+00015480: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+00015490: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+000154a0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000154b0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000154c0: 7065 7228 4465 7363 7269 6265 5265 6769  per(DescribeRegi
+000154d0: 6f6e 7352 6573 706f 6e73 652c 2073 656c  onsResponse, sel
+000154e0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
+000154f0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00015500: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00015510: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00015520: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00015530: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00015540: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+00015550: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00015560: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00015570: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+00015580: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+00015590: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+000155a0: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+000155b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000155c0: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+000155d0: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+000155e0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+000155f0: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+00015600: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00015610: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+00015620: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+00015630: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+00015640: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00015650: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00015660: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+00015670: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00015680: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00015690: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+000156a0: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+000156b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000156c0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+000156d0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+000156e0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000156f0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+00015700: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00015710: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00015720: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+00015730: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+00015740: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00015750: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+00015760: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00015770: 7465 6d70 5f6d 6f64 656c 203d 2044 6573  temp_model = Des
+00015780: 6372 6962 6552 6567 696f 6e73 5265 7370  cribeRegionsResp
+00015790: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+000157a0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000157b0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+000157c0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+000157d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000157e0: 2073 656c 660a 0a0a 636c 6173 7320 4465   self...class De
+000157f0: 7461 6368 4561 6952 6571 7565 7374 2854  tachEaiRequest(T
+00015800: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00015810: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00015820: 2065 6c61 7374 6963 5f61 6363 656c 6572   elastic_acceler
+00015830: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
+00015840: 3d4e 6f6e 652c 2072 6567 696f 6e5f 6964  =None, region_id
+00015850: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00015860: 7365 6c66 2e65 6c61 7374 6963 5f61 6363  self.elastic_acc
+00015870: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
+00015880: 655f 6964 203d 2065 6c61 7374 6963 5f61  e_id = elastic_a
+00015890: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
+000158a0: 6e63 655f 6964 2020 2320 7479 7065 3a20  nce_id  # type: 
+000158b0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+000158c0: 2e72 6567 696f 6e5f 6964 203d 2072 6567  .region_id = reg
+000158d0: 696f 6e5f 6964 2020 2320 7479 7065 3a20  ion_id  # type: 
+000158e0: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
+000158f0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00015900: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00015910: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00015920: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00015930: 7375 7065 7228 4465 7461 6368 4561 6952  super(DetachEaiR
+00015940: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
+00015950: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00015960: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00015970: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00015980: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00015990: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000159a0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000159b0: 7365 6c66 2e65 6c61 7374 6963 5f61 6363  self.elastic_acc
+000159c0: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
+000159d0: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+000159e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000159f0: 7375 6c74 5b27 456c 6173 7469 6341 6363  sult['ElasticAcc
+00015a00: 656c 6572 6174 6564 496e 7374 616e 6365  eleratedInstance
+00015a10: 4964 275d 203d 2073 656c 662e 656c 6173  Id'] = self.elas
+00015a20: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
+00015a30: 696e 7374 616e 6365 5f69 640a 2020 2020  instance_id.    
+00015a40: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
+00015a50: 6f6e 5f69 6420 6973 206e 6f74 204e 6f6e  on_id is not Non
+00015a60: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00015a70: 6573 756c 745b 2752 6567 696f 6e49 6427  esult['RegionId'
+00015a80: 5d20 3d20 7365 6c66 2e72 6567 696f 6e5f  ] = self.region_
+00015a90: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+00015aa0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00015ab0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00015ac0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+00015ad0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+00015ae0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00015af0: 6574 2827 456c 6173 7469 6341 6363 656c  et('ElasticAccel
+00015b00: 6572 6174 6564 496e 7374 616e 6365 4964  eratedInstanceId
+00015b10: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00015b20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015b30: 2e65 6c61 7374 6963 5f61 6363 656c 6572  .elastic_acceler
+00015b40: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
+00015b50: 203d 206d 2e67 6574 2827 456c 6173 7469   = m.get('Elasti
+00015b60: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
+00015b70: 616e 6365 4964 2729 0a20 2020 2020 2020  anceId').       
+00015b80: 2069 6620 6d2e 6765 7428 2752 6567 696f   if m.get('Regio
+00015b90: 6e49 6427 2920 6973 206e 6f74 204e 6f6e  nId') is not Non
+00015ba0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00015bb0: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
+00015bc0: 6d2e 6765 7428 2752 6567 696f 6e49 6427  m.get('RegionId'
+00015bd0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00015be0: 2073 656c 660a 0a0a 636c 6173 7320 4465   self...class De
+00015bf0: 7461 6368 4561 6952 6573 706f 6e73 6542  tachEaiResponseB
+00015c00: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
+00015c10: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00015c20: 7365 6c66 2c20 7265 7175 6573 745f 6964  self, request_id
+00015c30: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00015c40: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00015c50: 3d20 7265 7175 6573 745f 6964 2020 2320  = request_id  # 
+00015c60: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
+00015c70: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00015c80: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+00015c90: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00015ca0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00015cb0: 6d61 7020 3d20 7375 7065 7228 4465 7461  map = super(Deta
+00015cc0: 6368 4561 6952 6573 706f 6e73 6542 6f64  chEaiResponseBod
+00015cd0: 792c 2073 656c 6629 2e74 6f5f 6d61 7028  y, self).to_map(
+00015ce0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00015cf0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00015d00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00015d10: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00015d20: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00015d30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00015d40: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
+00015d50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00015d60: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
+00015d70: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
+00015d80: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
+00015d90: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00015da0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00015db0: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+00015dc0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00015dd0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00015de0: 2069 6620 6d2e 6765 7428 2752 6571 7565   if m.get('Reque
+00015df0: 7374 4964 2729 2069 7320 6e6f 7420 4e6f  stId') is not No
+00015e00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00015e10: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00015e20: 3d20 6d2e 6765 7428 2752 6571 7565 7374  = m.get('Request
+00015e30: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
+00015e40: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00015e50: 2044 6574 6163 6845 6169 5265 7370 6f6e   DetachEaiRespon
+00015e60: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+00015e70: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00015e80: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
+00015e90: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
+00015ea0: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
+00015eb0: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+00015ec0: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
+00015ed0: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
+00015ee0: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
+00015ef0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00015f00: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
+00015f10: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
+00015f20: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00015f30: 626f 6479 2020 2320 7479 7065 3a20 4465  body  # type: De
+00015f40: 7461 6368 4561 6952 6573 706f 6e73 6542  tachEaiResponseB
+00015f50: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+00015f60: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00015f70: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+00015f80: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+00015f90: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
+00015fa0: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
+00015fb0: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00015fc0: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
+00015fd0: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
+00015fe0: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
+00015ff0: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00016000: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
+00016010: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
+00016020: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
+00016030: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+00016040: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
+00016050: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00016060: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00016070: 7020 3d20 7375 7065 7228 4465 7461 6368  p = super(Detach
+00016080: 4561 6952 6573 706f 6e73 652c 2073 656c  EaiResponse, sel
+00016090: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
+000160a0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+000160b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000160c0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+000160d0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+000160e0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+000160f0: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+00016100: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00016110: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00016120: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+00016130: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+00016140: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00016150: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+00016160: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00016170: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+00016180: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+00016190: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+000161a0: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+000161b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000161c0: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+000161d0: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+000161e0: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+000161f0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00016200: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00016210: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+00016220: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00016230: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00016240: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+00016250: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+00016260: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00016270: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+00016280: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+00016290: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000162a0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+000162b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000162c0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000162d0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+000162e0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+000162f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00016300: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+00016310: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00016320: 7465 6d70 5f6d 6f64 656c 203d 2044 6574  temp_model = Det
+00016330: 6163 6845 6169 5265 7370 6f6e 7365 426f  achEaiResponseBo
+00016340: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+00016350: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+00016360: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00016370: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+00016380: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00016390: 0a0a 636c 6173 7320 4465 7461 6368 4561  ..class DetachEa
+000163a0: 6973 4569 5265 7175 6573 7428 5465 614d  isEiRequest(TeaM
+000163b0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+000163c0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6569  _init__(self, ei
+000163d0: 5f69 6e73 7461 6e63 655f 6964 3d4e 6f6e  _instance_id=Non
+000163e0: 652c 2072 6567 696f 6e5f 6964 3d4e 6f6e  e, region_id=Non
+000163f0: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00016400: 2e65 695f 696e 7374 616e 6365 5f69 6420  .ei_instance_id 
+00016410: 3d20 6569 5f69 6e73 7461 6e63 655f 6964  = ei_instance_id
+00016420: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+00016430: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
+00016440: 6e5f 6964 203d 2072 6567 696f 6e5f 6964  n_id = region_id
+00016450: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
+00016460: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+00016470: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00016480: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+00016490: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+000164a0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+000164b0: 4465 7461 6368 4561 6973 4569 5265 7175  DetachEaisEiRequ
+000164c0: 6573 742c 2073 656c 6629 2e74 6f5f 6d61  est, self).to_ma
+000164d0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+000164e0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+000164f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00016500: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+00016510: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00016520: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00016530: 662e 6569 5f69 6e73 7461 6e63 655f 6964  f.ei_instance_id
+00016540: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00016550: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00016560: 5b27 4569 496e 7374 616e 6365 4964 275d  ['EiInstanceId']
+00016570: 203d 2073 656c 662e 6569 5f69 6e73 7461   = self.ei_insta
+00016580: 6e63 655f 6964 0a20 2020 2020 2020 2069  nce_id.        i
+00016590: 6620 7365 6c66 2e72 6567 696f 6e5f 6964  f self.region_id
+000165a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000165b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000165c0: 5b27 5265 6769 6f6e 4964 275d 203d 2073  ['RegionId'] = s
+000165d0: 656c 662e 7265 6769 6f6e 5f69 640a 2020  elf.region_id.  
+000165e0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000165f0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00016600: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+00016610: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00016620: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00016630: 2020 2020 2069 6620 6d2e 6765 7428 2745       if m.get('E
+00016640: 6949 6e73 7461 6e63 6549 6427 2920 6973  iInstanceId') is
+00016650: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00016660: 2020 2020 2020 2073 656c 662e 6569 5f69         self.ei_i
+00016670: 6e73 7461 6e63 655f 6964 203d 206d 2e67  nstance_id = m.g
+00016680: 6574 2827 4569 496e 7374 616e 6365 4964  et('EiInstanceId
+00016690: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000166a0: 6765 7428 2752 6567 696f 6e49 6427 2920  get('RegionId') 
+000166b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000166c0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+000166d0: 6769 6f6e 5f69 6420 3d20 6d2e 6765 7428  gion_id = m.get(
+000166e0: 2752 6567 696f 6e49 6427 290a 2020 2020  'RegionId').    
+000166f0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00016700: 0a0a 636c 6173 7320 4465 7461 6368 4561  ..class DetachEa
+00016710: 6973 4569 5265 7370 6f6e 7365 426f 6479  isEiResponseBody
+00016720: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00016730: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00016740: 662c 2072 6571 7565 7374 5f69 643d 4e6f  f, request_id=No
+00016750: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+00016760: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
+00016770: 6571 7565 7374 5f69 6420 2023 2074 7970  equest_id  # typ
+00016780: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
+00016790: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000167a0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000167b0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000167c0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000167d0: 203d 2073 7570 6572 2844 6574 6163 6845   = super(DetachE
+000167e0: 6169 7345 6952 6573 706f 6e73 6542 6f64  aisEiResponseBod
+000167f0: 792c 2073 656c 6629 2e74 6f5f 6d61 7028  y, self).to_map(
+00016800: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00016810: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00016820: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00016830: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00016840: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00016850: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00016860: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
+00016870: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00016880: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
+00016890: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
+000168a0: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
+000168b0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+000168c0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+000168d0: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+000168e0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+000168f0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00016900: 2069 6620 6d2e 6765 7428 2752 6571 7565   if m.get('Reque
+00016910: 7374 4964 2729 2069 7320 6e6f 7420 4e6f  stId') is not No
+00016920: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00016930: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00016940: 3d20 6d2e 6765 7428 2752 6571 7565 7374  = m.get('Request
+00016950: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
+00016960: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00016970: 2044 6574 6163 6845 6169 7345 6952 6573   DetachEaisEiRes
+00016980: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
+00016990: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000169a0: 5f28 7365 6c66 2c20 6865 6164 6572 733d  _(self, headers=
+000169b0: 4e6f 6e65 2c20 7374 6174 7573 5f63 6f64  None, status_cod
+000169c0: 653d 4e6f 6e65 2c20 626f 6479 3d4e 6f6e  e=None, body=Non
+000169d0: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+000169e0: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
+000169f0: 7273 2020 2320 7479 7065 3a20 6469 6374  rs  # type: dict
+00016a00: 5b73 7472 2c20 7374 725d 0a20 2020 2020  [str, str].     
+00016a10: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+00016a20: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+00016a30: 6520 2023 2074 7970 653a 2069 6e74 0a20  e  # type: int. 
+00016a40: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00016a50: 203d 2062 6f64 7920 2023 2074 7970 653a   = body  # type:
+00016a60: 2044 6574 6163 6845 6169 7345 6952 6573   DetachEaisEiRes
+00016a70: 706f 6e73 6542 6f64 790a 0a20 2020 2064  ponseBody..    d
+00016a80: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00016a90: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00016aa0: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+00016ab0: 6428 7365 6c66 2e68 6561 6465 7273 2c20  d(self.headers, 
+00016ac0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+00016ad0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+00016ae0: 5f72 6571 7569 7265 6428 7365 6c66 2e73  _required(self.s
+00016af0: 7461 7475 735f 636f 6465 2c20 2773 7461  tatus_code, 'sta
+00016b00: 7475 735f 636f 6465 2729 0a20 2020 2020  tus_code').     
+00016b10: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+00016b20: 5f72 6571 7569 7265 6428 7365 6c66 2e62  _required(self.b
+00016b30: 6f64 792c 2027 626f 6479 2729 0a20 2020  ody, 'body').   
+00016b40: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00016b50: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00016b60: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00016b70: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00016b80: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00016b90: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00016ba0: 4465 7461 6368 4561 6973 4569 5265 7370  DetachEaisEiResp
+00016bb0: 6f6e 7365 2c20 7365 6c66 292e 746f 5f6d  onse, self).to_m
+00016bc0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00016bd0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00016be0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00016bf0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00016c00: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00016c10: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00016c20: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+00016c30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00016c40: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+00016c50: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+00016c60: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+00016c70: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00016c80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00016c90: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00016ca0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+00016cb0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00016cc0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00016cd0: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+00016ce0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00016cf0: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+00016d00: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+00016d10: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+00016d20: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00016d30: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00016d40: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+00016d50: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00016d60: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00016d70: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
+00016d80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00016d90: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+00016da0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
+00016db0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+00016dc0: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
+00016dd0: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
+00016de0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00016df0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00016e00: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
+00016e10: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
+00016e20: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
+00016e30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00016e40: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+00016e50: 6465 6c20 3d20 4465 7461 6368 4561 6973  del = DetachEais
+00016e60: 4569 5265 7370 6f6e 7365 426f 6479 2829  EiResponseBody()
+00016e70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00016e80: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+00016e90: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+00016ea0: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+00016eb0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00016ec0: 6173 7320 4765 7449 6e73 7461 6e63 654d  ass GetInstanceM
+00016ed0: 6574 7269 6373 5265 7175 6573 7428 5465  etricsRequest(Te
+00016ee0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00016ef0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00016f00: 656e 645f 7469 6d65 3d4e 6f6e 652c 2069  end_time=None, i
+00016f10: 6e73 7461 6e63 655f 6964 3d4e 6f6e 652c  nstance_id=None,
+00016f20: 206d 6574 7269 635f 7479 7065 3d4e 6f6e   metric_type=Non
+00016f30: 652c 2072 6567 696f 6e5f 6964 3d4e 6f6e  e, region_id=Non
+00016f40: 652c 2073 7461 7274 5f74 696d 653d 4e6f  e, start_time=No
+00016f50: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00016f60: 2020 2020 2074 696d 655f 7374 6570 3d4e       time_step=N
+00016f70: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+00016f80: 6c66 2e65 6e64 5f74 696d 6520 3d20 656e  lf.end_time = en
+00016f90: 645f 7469 6d65 2020 2320 7479 7065 3a20  d_time  # type: 
+00016fa0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+00016fb0: 2e69 6e73 7461 6e63 655f 6964 203d 2069  .instance_id = i
+00016fc0: 6e73 7461 6e63 655f 6964 2020 2320 7479  nstance_id  # ty
+00016fd0: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
+00016fe0: 7365 6c66 2e6d 6574 7269 635f 7479 7065  self.metric_type
+00016ff0: 203d 206d 6574 7269 635f 7479 7065 2020   = metric_type  
+00017000: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+00017010: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
+00017020: 6964 203d 2072 6567 696f 6e5f 6964 2020  id = region_id  
+00017030: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+00017040: 2020 2020 7365 6c66 2e73 7461 7274 5f74      self.start_t
+00017050: 696d 6520 3d20 7374 6172 745f 7469 6d65  ime = start_time
+00017060: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+00017070: 2020 2020 2020 7365 6c66 2e74 696d 655f        self.time_
+00017080: 7374 6570 203d 2074 696d 655f 7374 6570  step = time_step
+00017090: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
+000170a0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+000170b0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+000170c0: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+000170d0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+000170e0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+000170f0: 4765 7449 6e73 7461 6e63 654d 6574 7269  GetInstanceMetri
+00017100: 6373 5265 7175 6573 742c 2073 656c 6629  csRequest, self)
+00017110: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00017120: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00017130: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00017140: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00017150: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00017160: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00017170: 6966 2073 656c 662e 656e 645f 7469 6d65  if self.end_time
+00017180: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00017190: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000171a0: 5b27 456e 6454 696d 6527 5d20 3d20 7365  ['EndTime'] = se
+000171b0: 6c66 2e65 6e64 5f74 696d 650a 2020 2020  lf.end_time.    
+000171c0: 2020 2020 6966 2073 656c 662e 696e 7374      if self.inst
+000171d0: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
+000171e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000171f0: 2072 6573 756c 745b 2749 6e73 7461 6e63   result['Instanc
+00017200: 6549 6427 5d20 3d20 7365 6c66 2e69 6e73  eId'] = self.ins
+00017210: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+00017220: 2069 6620 7365 6c66 2e6d 6574 7269 635f   if self.metric_
+00017230: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
+00017240: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00017250: 7375 6c74 5b27 4d65 7472 6963 5479 7065  sult['MetricType
+00017260: 275d 203d 2073 656c 662e 6d65 7472 6963  '] = self.metric
+00017270: 5f74 7970 650a 2020 2020 2020 2020 6966  _type.        if
+00017280: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+00017290: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000172a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000172b0: 2752 6567 696f 6e49 6427 5d20 3d20 7365  'RegionId'] = se
+000172c0: 6c66 2e72 6567 696f 6e5f 6964 0a20 2020  lf.region_id.   
+000172d0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+000172e0: 7274 5f74 696d 6520 6973 206e 6f74 204e  rt_time is not N
+000172f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00017300: 2072 6573 756c 745b 2753 7461 7274 5469   result['StartTi
+00017310: 6d65 275d 203d 2073 656c 662e 7374 6172  me'] = self.star
+00017320: 745f 7469 6d65 0a20 2020 2020 2020 2069  t_time.        i
+00017330: 6620 7365 6c66 2e74 696d 655f 7374 6570  f self.time_step
+00017340: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00017350: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00017360: 5b27 5469 6d65 5374 6570 275d 203d 2073  ['TimeStep'] = s
+00017370: 656c 662e 7469 6d65 5f73 7465 700a 2020  elf.time_step.  
+00017380: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00017390: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+000173a0: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+000173b0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000173c0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000173d0: 2020 2020 2069 6620 6d2e 6765 7428 2745       if m.get('E
+000173e0: 6e64 5469 6d65 2729 2069 7320 6e6f 7420  ndTime') is not 
+000173f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00017400: 2020 7365 6c66 2e65 6e64 5f74 696d 6520    self.end_time 
+00017410: 3d20 6d2e 6765 7428 2745 6e64 5469 6d65  = m.get('EndTime
+00017420: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00017430: 6765 7428 2749 6e73 7461 6e63 6549 6427  get('InstanceId'
+00017440: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00017450: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017460: 696e 7374 616e 6365 5f69 6420 3d20 6d2e  instance_id = m.
+00017470: 6765 7428 2749 6e73 7461 6e63 6549 6427  get('InstanceId'
+00017480: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00017490: 6574 2827 4d65 7472 6963 5479 7065 2729  et('MetricType')
+000174a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000174b0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000174c0: 6574 7269 635f 7479 7065 203d 206d 2e67  etric_type = m.g
+000174d0: 6574 2827 4d65 7472 6963 5479 7065 2729  et('MetricType')
+000174e0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000174f0: 7428 2752 6567 696f 6e49 6427 2920 6973  t('RegionId') is
+00017500: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00017510: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
+00017520: 6f6e 5f69 6420 3d20 6d2e 6765 7428 2752  on_id = m.get('R
+00017530: 6567 696f 6e49 6427 290a 2020 2020 2020  egionId').      
+00017540: 2020 6966 206d 2e67 6574 2827 5374 6172    if m.get('Star
+00017550: 7454 696d 6527 2920 6973 206e 6f74 204e  tTime') is not N
+00017560: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00017570: 2073 656c 662e 7374 6172 745f 7469 6d65   self.start_time
+00017580: 203d 206d 2e67 6574 2827 5374 6172 7454   = m.get('StartT
+00017590: 696d 6527 290a 2020 2020 2020 2020 6966  ime').        if
+000175a0: 206d 2e67 6574 2827 5469 6d65 5374 6570   m.get('TimeStep
+000175b0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000175c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000175d0: 2e74 696d 655f 7374 6570 203d 206d 2e67  .time_step = m.g
+000175e0: 6574 2827 5469 6d65 5374 6570 2729 0a20  et('TimeStep'). 
+000175f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00017600: 6c66 0a0a 0a63 6c61 7373 2047 6574 496e  lf...class GetIn
+00017610: 7374 616e 6365 4d65 7472 6963 7352 6573  stanceMetricsRes
+00017620: 706f 6e73 6542 6f64 7950 6f64 4d65 7472  ponseBodyPodMetr
+00017630: 6963 734d 6574 7269 6373 2854 6561 4d6f  icsMetrics(TeaMo
+00017640: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00017650: 696e 6974 5f5f 2873 656c 662c 2074 696d  init__(self, tim
+00017660: 653d 4e6f 6e65 2c20 7661 6c75 653d 4e6f  e=None, value=No
+00017670: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+00017680: 662e 7469 6d65 203d 2074 696d 6520 2023  f.time = time  #
+00017690: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
+000176a0: 2020 2073 656c 662e 7661 6c75 6520 3d20     self.value = 
+000176b0: 7661 6c75 6520 2023 2074 7970 653a 2073  value  # type: s
+000176c0: 7472 0a0a 2020 2020 6465 6620 7661 6c69  tr..    def vali
+000176d0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+000176e0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000176f0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00017700: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00017710: 7570 6572 2847 6574 496e 7374 616e 6365  uper(GetInstance
+00017720: 4d65 7472 6963 7352 6573 706f 6e73 6542  MetricsResponseB
+00017730: 6f64 7950 6f64 4d65 7472 6963 734d 6574  odyPodMetricsMet
+00017740: 7269 6373 2c20 7365 6c66 292e 746f 5f6d  rics, self).to_m
+00017750: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00017760: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00017770: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00017780: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00017790: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+000177a0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+000177b0: 6c66 2e74 696d 6520 6973 206e 6f74 204e  lf.time is not N
+000177c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000177d0: 2072 6573 756c 745b 2754 696d 6527 5d20   result['Time'] 
+000177e0: 3d20 7365 6c66 2e74 696d 650a 2020 2020  = self.time.    
+000177f0: 2020 2020 6966 2073 656c 662e 7661 6c75      if self.valu
+00017800: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00017810: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00017820: 745b 2756 616c 7565 275d 203d 2073 656c  t['Value'] = sel
+00017830: 662e 7661 6c75 650a 2020 2020 2020 2020  f.value.        
+00017840: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00017850: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00017860: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
+00017870: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00017880: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00017890: 6620 6d2e 6765 7428 2754 696d 6527 2920  f m.get('Time') 
+000178a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000178b0: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
+000178c0: 6d65 203d 206d 2e67 6574 2827 5469 6d65  me = m.get('Time
+000178d0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000178e0: 6765 7428 2756 616c 7565 2729 2069 7320  get('Value') is 
+000178f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00017900: 2020 2020 2020 7365 6c66 2e76 616c 7565        self.value
+00017910: 203d 206d 2e67 6574 2827 5661 6c75 6527   = m.get('Value'
+00017920: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00017930: 2073 656c 660a 0a0a 636c 6173 7320 4765   self...class Ge
+00017940: 7449 6e73 7461 6e63 654d 6574 7269 6373  tInstanceMetrics
+00017950: 5265 7370 6f6e 7365 426f 6479 506f 644d  ResponseBodyPodM
+00017960: 6574 7269 6373 2854 6561 4d6f 6465 6c29  etrics(TeaModel)
+00017970: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00017980: 5f5f 2873 656c 662c 206d 6574 7269 6373  __(self, metrics
+00017990: 3d4e 6f6e 652c 2070 6f64 5f69 643d 4e6f  =None, pod_id=No
+000179a0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+000179b0: 662e 6d65 7472 6963 7320 3d20 6d65 7472  f.metrics = metr
+000179c0: 6963 7320 2023 2074 7970 653a 206c 6973  ics  # type: lis
+000179d0: 745b 4765 7449 6e73 7461 6e63 654d 6574  t[GetInstanceMet
+000179e0: 7269 6373 5265 7370 6f6e 7365 426f 6479  ricsResponseBody
+000179f0: 506f 644d 6574 7269 6373 4d65 7472 6963  PodMetricsMetric
+00017a00: 735d 0a20 2020 2020 2020 2023 2050 6f64  s].        # Pod
+00017a10: 2049 44e3 8082 0a20 2020 2020 2020 2073   ID....        s
+00017a20: 656c 662e 706f 645f 6964 203d 2070 6f64  elf.pod_id = pod
+00017a30: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
+00017a40: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00017a50: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00017a60: 2020 6966 2073 656c 662e 6d65 7472 6963    if self.metric
+00017a70: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+00017a80: 6f72 206b 2069 6e20 7365 6c66 2e6d 6574  or k in self.met
+00017a90: 7269 6373 3a0a 2020 2020 2020 2020 2020  rics:.          
+00017aa0: 2020 2020 2020 6966 206b 3a0a 2020 2020        if k:.    
+00017ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ac0: 6b2e 7661 6c69 6461 7465 2829 0a0a 2020  k.validate()..  
+00017ad0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00017ae0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00017af0: 203d 2073 7570 6572 2847 6574 496e 7374   = super(GetInst
+00017b00: 616e 6365 4d65 7472 6963 7352 6573 706f  anceMetricsRespo
+00017b10: 6e73 6542 6f64 7950 6f64 4d65 7472 6963  nseBodyPodMetric
+00017b20: 732c 2073 656c 6629 2e74 6f5f 6d61 7028  s, self).to_map(
+00017b30: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00017b40: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00017b50: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00017b60: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00017b70: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00017b80: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00017b90: 4d65 7472 6963 7327 5d20 3d20 5b5d 0a20  Metrics'] = []. 
+00017ba0: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00017bb0: 6574 7269 6373 2069 7320 6e6f 7420 4e6f  etrics is not No
+00017bc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00017bd0: 666f 7220 6b20 696e 2073 656c 662e 6d65  for k in self.me
+00017be0: 7472 6963 733a 0a20 2020 2020 2020 2020  trics:.         
+00017bf0: 2020 2020 2020 2072 6573 756c 745b 274d         result['M
+00017c00: 6574 7269 6373 275d 2e61 7070 656e 6428  etrics'].append(
+00017c10: 6b2e 746f 5f6d 6170 2829 2069 6620 6b20  k.to_map() if k 
+00017c20: 656c 7365 204e 6f6e 6529 0a20 2020 2020  else None).     
+00017c30: 2020 2069 6620 7365 6c66 2e70 6f64 5f69     if self.pod_i
+00017c40: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00017c50: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00017c60: 745b 2750 6f64 4964 275d 203d 2073 656c  t['PodId'] = sel
+00017c70: 662e 706f 645f 6964 0a20 2020 2020 2020  f.pod_id.       
+00017c80: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00017c90: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00017ca0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+00017cb0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00017cc0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00017cd0: 7365 6c66 2e6d 6574 7269 6373 203d 205b  self.metrics = [
+00017ce0: 5d0a 2020 2020 2020 2020 6966 206d 2e67  ].        if m.g
+00017cf0: 6574 2827 4d65 7472 6963 7327 2920 6973  et('Metrics') is
+00017d00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00017d10: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00017d20: 6d2e 6765 7428 274d 6574 7269 6373 2729  m.get('Metrics')
+00017d30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017d40: 2020 7465 6d70 5f6d 6f64 656c 203d 2047    temp_model = G
+00017d50: 6574 496e 7374 616e 6365 4d65 7472 6963  etInstanceMetric
+00017d60: 7352 6573 706f 6e73 6542 6f64 7950 6f64  sResponseBodyPod
+00017d70: 4d65 7472 6963 734d 6574 7269 6373 2829  MetricsMetrics()
+00017d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017d90: 2073 656c 662e 6d65 7472 6963 732e 6170   self.metrics.ap
+00017da0: 7065 6e64 2874 656d 705f 6d6f 6465 6c2e  pend(temp_model.
+00017db0: 6672 6f6d 5f6d 6170 286b 2929 0a20 2020  from_map(k)).   
+00017dc0: 2020 2020 2069 6620 6d2e 6765 7428 2750       if m.get('P
+00017dd0: 6f64 4964 2729 2069 7320 6e6f 7420 4e6f  odId') is not No
+00017de0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00017df0: 7365 6c66 2e70 6f64 5f69 6420 3d20 6d2e  self.pod_id = m.
+00017e00: 6765 7428 2750 6f64 4964 2729 0a20 2020  get('PodId').   
+00017e10: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00017e20: 0a0a 0a63 6c61 7373 2047 6574 496e 7374  ...class GetInst
+00017e30: 616e 6365 4d65 7472 6963 7352 6573 706f  anceMetricsRespo
+00017e40: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
+00017e50: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00017e60: 745f 5f28 7365 6c66 2c20 696e 7374 616e  t__(self, instan
+00017e70: 6365 5f69 643d 4e6f 6e65 2c20 706f 645f  ce_id=None, pod_
+00017e80: 6d65 7472 6963 733d 4e6f 6e65 2c20 7265  metrics=None, re
+00017e90: 7175 6573 745f 6964 3d4e 6f6e 6529 3a0a  quest_id=None):.
+00017ea0: 2020 2020 2020 2020 7365 6c66 2e69 6e73          self.ins
+00017eb0: 7461 6e63 655f 6964 203d 2069 6e73 7461  tance_id = insta
+00017ec0: 6e63 655f 6964 2020 2320 7479 7065 3a20  nce_id  # type: 
+00017ed0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+00017ee0: 2e70 6f64 5f6d 6574 7269 6373 203d 2070  .pod_metrics = p
+00017ef0: 6f64 5f6d 6574 7269 6373 2020 2320 7479  od_metrics  # ty
+00017f00: 7065 3a20 6c69 7374 5b47 6574 496e 7374  pe: list[GetInst
+00017f10: 616e 6365 4d65 7472 6963 7352 6573 706f  anceMetricsRespo
+00017f20: 6e73 6542 6f64 7950 6f64 4d65 7472 6963  nseBodyPodMetric
+00017f30: 735d 0a20 2020 2020 2020 2073 656c 662e  s].        self.
+00017f40: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
+00017f50: 7565 7374 5f69 6420 2023 2074 7970 653a  uest_id  # type:
+00017f60: 2073 7472 0a0a 2020 2020 6465 6620 7661   str..    def va
+00017f70: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00017f80: 2020 2020 2020 6966 2073 656c 662e 706f        if self.po
+00017f90: 645f 6d65 7472 6963 733a 0a20 2020 2020  d_metrics:.     
+00017fa0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00017fb0: 7365 6c66 2e70 6f64 5f6d 6574 7269 6373  self.pod_metrics
+00017fc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017fd0: 2020 6966 206b 3a0a 2020 2020 2020 2020    if k:.        
+00017fe0: 2020 2020 2020 2020 2020 2020 6b2e 7661              k.va
+00017ff0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+00018000: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00018010: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00018020: 7570 6572 2847 6574 496e 7374 616e 6365  uper(GetInstance
+00018030: 4d65 7472 6963 7352 6573 706f 6e73 6542  MetricsResponseB
+00018040: 6f64 792c 2073 656c 6629 2e74 6f5f 6d61  ody, self).to_ma
+00018050: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00018060: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00018070: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00018080: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+00018090: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000180a0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000180b0: 662e 696e 7374 616e 6365 5f69 6420 6973  f.instance_id is
+000180c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000180d0: 2020 2020 2020 2072 6573 756c 745b 2749         result['I
+000180e0: 6e73 7461 6e63 6549 6427 5d20 3d20 7365  nstanceId'] = se
+000180f0: 6c66 2e69 6e73 7461 6e63 655f 6964 0a20  lf.instance_id. 
+00018100: 2020 2020 2020 2072 6573 756c 745b 2750         result['P
+00018110: 6f64 4d65 7472 6963 7327 5d20 3d20 5b5d  odMetrics'] = []
+00018120: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00018130: 2e70 6f64 5f6d 6574 7269 6373 2069 7320  .pod_metrics is 
+00018140: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00018150: 2020 2020 2020 666f 7220 6b20 696e 2073        for k in s
+00018160: 656c 662e 706f 645f 6d65 7472 6963 733a  elf.pod_metrics:
+00018170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018180: 2072 6573 756c 745b 2750 6f64 4d65 7472   result['PodMetr
+00018190: 6963 7327 5d2e 6170 7065 6e64 286b 2e74  ics'].append(k.t
+000181a0: 6f5f 6d61 7028 2920 6966 206b 2065 6c73  o_map() if k els
+000181b0: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
+000181c0: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+000181d0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000181e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000181f0: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
+00018200: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
+00018210: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+00018220: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00018230: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00018240: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+00018250: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00018260: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00018270: 7428 2749 6e73 7461 6e63 6549 6427 2920  t('InstanceId') 
+00018280: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00018290: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
+000182a0: 7374 616e 6365 5f69 6420 3d20 6d2e 6765  stance_id = m.ge
+000182b0: 7428 2749 6e73 7461 6e63 6549 6427 290a  t('InstanceId').
+000182c0: 2020 2020 2020 2020 7365 6c66 2e70 6f64          self.pod
+000182d0: 5f6d 6574 7269 6373 203d 205b 5d0a 2020  _metrics = [].  
+000182e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000182f0: 506f 644d 6574 7269 6373 2729 2069 7320  PodMetrics') is 
+00018300: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00018310: 2020 2020 2020 666f 7220 6b20 696e 206d        for k in m
+00018320: 2e67 6574 2827 506f 644d 6574 7269 6373  .get('PodMetrics
+00018330: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
+00018340: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+00018350: 2047 6574 496e 7374 616e 6365 4d65 7472   GetInstanceMetr
+00018360: 6963 7352 6573 706f 6e73 6542 6f64 7950  icsResponseBodyP
+00018370: 6f64 4d65 7472 6963 7328 290a 2020 2020  odMetrics().    
+00018380: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018390: 2e70 6f64 5f6d 6574 7269 6373 2e61 7070  .pod_metrics.app
+000183a0: 656e 6428 7465 6d70 5f6d 6f64 656c 2e66  end(temp_model.f
+000183b0: 726f 6d5f 6d61 7028 6b29 290a 2020 2020  rom_map(k)).    
+000183c0: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+000183d0: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
+000183e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000183f0: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+00018400: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
+00018410: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
+00018420: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00018430: 6173 7320 4765 7449 6e73 7461 6e63 654d  ass GetInstanceM
+00018440: 6574 7269 6373 5265 7370 6f6e 7365 2854  etricsResponse(T
+00018450: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00018460: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00018470: 2068 6561 6465 7273 3d4e 6f6e 652c 2073   headers=None, s
+00018480: 7461 7475 735f 636f 6465 3d4e 6f6e 652c  tatus_code=None,
+00018490: 2062 6f64 793d 4e6f 6e65 293a 0a20 2020   body=None):.   
+000184a0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+000184b0: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
+000184c0: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
+000184d0: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
+000184e0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+000184f0: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
+00018500: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
+00018510: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+00018520: 2020 2320 7479 7065 3a20 4765 7449 6e73    # type: GetIns
+00018530: 7461 6e63 654d 6574 7269 6373 5265 7370  tanceMetricsResp
+00018540: 6f6e 7365 426f 6479 0a0a 2020 2020 6465  onseBody..    de
+00018550: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00018560: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
+00018570: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00018580: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
+00018590: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+000185a0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+000185b0: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
+000185c0: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
+000185d0: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
+000185e0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+000185f0: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
+00018600: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
+00018610: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00018620: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00018630: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00018640: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00018650: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00018660: 2020 5f6d 6170 203d 2073 7570 6572 2847    _map = super(G
+00018670: 6574 496e 7374 616e 6365 4d65 7472 6963  etInstanceMetric
+00018680: 7352 6573 706f 6e73 652c 2073 656c 6629  sResponse, self)
+00018690: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000186a0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+000186b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000186c0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+000186d0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000186e0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000186f0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+00018700: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00018710: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00018720: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+00018730: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+00018740: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00018750: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00018760: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00018770: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00018780: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00018790: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+000187a0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+000187b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000187c0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+000187d0: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+000187e0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000187f0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00018800: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00018810: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+00018820: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00018830: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00018840: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+00018850: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00018860: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00018870: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+00018880: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+00018890: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+000188a0: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+000188b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000188c0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+000188d0: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+000188e0: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+000188f0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+00018900: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+00018910: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00018920: 6d70 5f6d 6f64 656c 203d 2047 6574 496e  mp_model = GetIn
+00018930: 7374 616e 6365 4d65 7472 6963 7352 6573  stanceMetricsRes
+00018940: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
+00018950: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00018960: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
+00018970: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
+00018980: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+00018990: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
+000189a0: 7461 7274 4561 6973 4569 5265 7175 6573  tartEaisEiReques
+000189b0: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+000189c0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+000189d0: 6c66 2c20 6569 5f69 6e73 7461 6e63 655f  lf, ei_instance_
+000189e0: 6964 3d4e 6f6e 652c 2072 6567 696f 6e5f  id=None, region_
+000189f0: 6964 3d4e 6f6e 6529 3a0a 2020 2020 2020  id=None):.      
+00018a00: 2020 7365 6c66 2e65 695f 696e 7374 616e    self.ei_instan
+00018a10: 6365 5f69 6420 3d20 6569 5f69 6e73 7461  ce_id = ei_insta
+00018a20: 6e63 655f 6964 2020 2320 7479 7065 3a20  nce_id  # type: 
+00018a30: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+00018a40: 2e72 6567 696f 6e5f 6964 203d 2072 6567  .region_id = reg
+00018a50: 696f 6e5f 6964 2020 2320 7479 7065 3a20  ion_id  # type: 
+00018a60: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
+00018a70: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00018a80: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00018a90: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00018aa0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00018ab0: 7375 7065 7228 5374 6172 7445 6169 7345  super(StartEaisE
+00018ac0: 6952 6571 7565 7374 2c20 7365 6c66 292e  iRequest, self).
+00018ad0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00018ae0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00018af0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00018b00: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00018b10: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00018b20: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00018b30: 6620 7365 6c66 2e65 695f 696e 7374 616e  f self.ei_instan
+00018b40: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
+00018b50: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00018b60: 6573 756c 745b 2745 6949 6e73 7461 6e63  esult['EiInstanc
+00018b70: 6549 6427 5d20 3d20 7365 6c66 2e65 695f  eId'] = self.ei_
+00018b80: 696e 7374 616e 6365 5f69 640a 2020 2020  instance_id.    
+00018b90: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
+00018ba0: 6f6e 5f69 6420 6973 206e 6f74 204e 6f6e  on_id is not Non
+00018bb0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00018bc0: 6573 756c 745b 2752 6567 696f 6e49 6427  esult['RegionId'
+00018bd0: 5d20 3d20 7365 6c66 2e72 6567 696f 6e5f  ] = self.region_
+00018be0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+00018bf0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00018c00: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00018c10: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+00018c20: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+00018c30: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00018c40: 6574 2827 4569 496e 7374 616e 6365 4964  et('EiInstanceId
+00018c50: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00018c60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018c70: 2e65 695f 696e 7374 616e 6365 5f69 6420  .ei_instance_id 
+00018c80: 3d20 6d2e 6765 7428 2745 6949 6e73 7461  = m.get('EiInsta
+00018c90: 6e63 6549 6427 290a 2020 2020 2020 2020  nceId').        
+00018ca0: 6966 206d 2e67 6574 2827 5265 6769 6f6e  if m.get('Region
+00018cb0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00018cc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00018cd0: 6c66 2e72 6567 696f 6e5f 6964 203d 206d  lf.region_id = m
+00018ce0: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
+00018cf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00018d00: 7365 6c66 0a0a 0a63 6c61 7373 2053 7461  self...class Sta
+00018d10: 7274 4561 6973 4569 5265 7370 6f6e 7365  rtEaisEiResponse
+00018d20: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
+00018d30: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00018d40: 2873 656c 662c 2072 6571 7565 7374 5f69  (self, request_i
+00018d50: 643d 4e6f 6e65 293a 0a20 2020 2020 2020  d=None):.       
+00018d60: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+00018d70: 203d 2072 6571 7565 7374 5f69 6420 2023   = request_id  #
+00018d80: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
+00018d90: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00018da0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00018db0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00018dc0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00018dd0: 5f6d 6170 203d 2073 7570 6572 2853 7461  _map = super(Sta
+00018de0: 7274 4561 6973 4569 5265 7370 6f6e 7365  rtEaisEiResponse
+00018df0: 426f 6479 2c20 7365 6c66 292e 746f 5f6d  Body, self).to_m
+00018e00: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00018e10: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00018e20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00018e30: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00018e40: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00018e50: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00018e60: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
+00018e70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00018e80: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
+00018e90: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
+00018ea0: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
+00018eb0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00018ec0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00018ed0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+00018ee0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00018ef0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00018f00: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+00018f10: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
+00018f20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00018f30: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+00018f40: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
+00018f50: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
+00018f60: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00018f70: 6173 7320 5374 6172 7445 6169 7345 6952  ass StartEaisEiR
+00018f80: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
+00018f90: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00018fa0: 745f 5f28 7365 6c66 2c20 6865 6164 6572  t__(self, header
+00018fb0: 733d 4e6f 6e65 2c20 7374 6174 7573 5f63  s=None, status_c
+00018fc0: 6f64 653d 4e6f 6e65 2c20 626f 6479 3d4e  ode=None, body=N
+00018fd0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+00018fe0: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+00018ff0: 6465 7273 2020 2320 7479 7065 3a20 6469  ders  # type: di
+00019000: 6374 5b73 7472 2c20 7374 725d 0a20 2020  ct[str, str].   
+00019010: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00019020: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+00019030: 6f64 6520 2023 2074 7970 653a 2069 6e74  ode  # type: int
+00019040: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+00019050: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
+00019060: 653a 2053 7461 7274 4561 6973 4569 5265  e: StartEaisEiRe
+00019070: 7370 6f6e 7365 426f 6479 0a0a 2020 2020  sponseBody..    
+00019080: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00019090: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+000190a0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+000190b0: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
+000190c0: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
+000190d0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+000190e0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+000190f0: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
+00019100: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
+00019110: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+00019120: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+00019130: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
+00019140: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00019150: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
+00019160: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
+00019170: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+00019180: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00019190: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+000191a0: 2853 7461 7274 4561 6973 4569 5265 7370  (StartEaisEiResp
+000191b0: 6f6e 7365 2c20 7365 6c66 292e 746f 5f6d  onse, self).to_m
+000191c0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+000191d0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+000191e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000191f0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00019200: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00019210: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00019220: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+00019230: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00019240: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+00019250: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+00019260: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+00019270: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00019280: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00019290: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000192a0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+000192b0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000192c0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+000192d0: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+000192e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000192f0: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+00019300: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+00019310: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+00019320: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00019330: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00019340: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+00019350: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00019360: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00019370: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
+00019380: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00019390: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+000193a0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
+000193b0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+000193c0: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
+000193d0: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
+000193e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000193f0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00019400: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
+00019410: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
+00019420: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
+00019430: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00019440: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+00019450: 6465 6c20 3d20 5374 6172 7445 6169 7345  del = StartEaisE
+00019460: 6952 6573 706f 6e73 6542 6f64 7928 290a  iResponseBody().
+00019470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019480: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+00019490: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+000194a0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+000194b0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000194c0: 7373 2053 746f 7045 6169 7345 6952 6571  ss StopEaisEiReq
+000194d0: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+000194e0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000194f0: 2873 656c 662c 2065 695f 696e 7374 616e  (self, ei_instan
+00019500: 6365 5f69 643d 4e6f 6e65 2c20 7265 6769  ce_id=None, regi
+00019510: 6f6e 5f69 643d 4e6f 6e65 293a 0a20 2020  on_id=None):.   
+00019520: 2020 2020 2073 656c 662e 6569 5f69 6e73       self.ei_ins
+00019530: 7461 6e63 655f 6964 203d 2065 695f 696e  tance_id = ei_in
+00019540: 7374 616e 6365 5f69 6420 2023 2074 7970  stance_id  # typ
+00019550: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+00019560: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
+00019570: 7265 6769 6f6e 5f69 6420 2023 2074 7970  region_id  # typ
+00019580: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
+00019590: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000195a0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000195b0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000195c0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+000195d0: 203d 2073 7570 6572 2853 746f 7045 6169   = super(StopEai
+000195e0: 7345 6952 6571 7565 7374 2c20 7365 6c66  sEiRequest, self
+000195f0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00019600: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00019610: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00019620: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00019630: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00019640: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00019650: 2069 6620 7365 6c66 2e65 695f 696e 7374   if self.ei_inst
+00019660: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
+00019670: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00019680: 2072 6573 756c 745b 2745 6949 6e73 7461   result['EiInsta
+00019690: 6e63 6549 6427 5d20 3d20 7365 6c66 2e65  nceId'] = self.e
+000196a0: 695f 696e 7374 616e 6365 5f69 640a 2020  i_instance_id.  
+000196b0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+000196c0: 6769 6f6e 5f69 6420 6973 206e 6f74 204e  gion_id is not N
+000196d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000196e0: 2072 6573 756c 745b 2752 6567 696f 6e49   result['RegionI
+000196f0: 6427 5d20 3d20 7365 6c66 2e72 6567 696f  d'] = self.regio
+00019700: 6e5f 6964 0a20 2020 2020 2020 2072 6574  n_id.        ret
+00019710: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00019720: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00019730: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+00019740: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00019750: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00019760: 2e67 6574 2827 4569 496e 7374 616e 6365  .get('EiInstance
+00019770: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00019780: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00019790: 6c66 2e65 695f 696e 7374 616e 6365 5f69  lf.ei_instance_i
+000197a0: 6420 3d20 6d2e 6765 7428 2745 6949 6e73  d = m.get('EiIns
+000197b0: 7461 6e63 6549 6427 290a 2020 2020 2020  tanceId').      
+000197c0: 2020 6966 206d 2e67 6574 2827 5265 6769    if m.get('Regi
+000197d0: 6f6e 4964 2729 2069 7320 6e6f 7420 4e6f  onId') is not No
+000197e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000197f0: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
+00019800: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
+00019810: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+00019820: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
+00019830: 746f 7045 6169 7345 6952 6573 706f 6e73  topEaisEiRespons
+00019840: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
+00019850: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00019860: 5f28 7365 6c66 2c20 7265 7175 6573 745f  _(self, request_
+00019870: 6964 3d4e 6f6e 6529 3a0a 2020 2020 2020  id=None):.      
+00019880: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+00019890: 6420 3d20 7265 7175 6573 745f 6964 2020  d = request_id  
+000198a0: 2320 7479 7065 3a20 7374 720a 0a20 2020  # type: str..   
+000198b0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+000198c0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+000198d0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+000198e0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+000198f0: 205f 6d61 7020 3d20 7375 7065 7228 5374   _map = super(St
+00019900: 6f70 4561 6973 4569 5265 7370 6f6e 7365  opEaisEiResponse
+00019910: 426f 6479 2c20 7365 6c66 292e 746f 5f6d  Body, self).to_m
+00019920: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00019930: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00019940: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00019950: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00019960: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00019970: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00019980: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
+00019990: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000199a0: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
+000199b0: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
+000199c0: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
+000199d0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000199e0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+000199f0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+00019a00: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00019a10: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00019a20: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+00019a30: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
+00019a40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00019a50: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+00019a60: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
+00019a70: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
+00019a80: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00019a90: 6173 7320 5374 6f70 4561 6973 4569 5265  ass StopEaisEiRe
+00019aa0: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+00019ab0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00019ac0: 5f5f 2873 656c 662c 2068 6561 6465 7273  __(self, headers
+00019ad0: 3d4e 6f6e 652c 2073 7461 7475 735f 636f  =None, status_co
+00019ae0: 6465 3d4e 6f6e 652c 2062 6f64 793d 4e6f  de=None, body=No
+00019af0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+00019b00: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00019b10: 6572 7320 2023 2074 7970 653a 2064 6963  ers  # type: dic
+00019b20: 745b 7374 722c 2073 7472 5d0a 2020 2020  t[str, str].    
+00019b30: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00019b40: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00019b50: 6465 2020 2320 7479 7065 3a20 696e 740a  de  # type: int.
+00019b60: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00019b70: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
+00019b80: 3a20 5374 6f70 4561 6973 4569 5265 7370  : StopEaisEiResp
+00019b90: 6f6e 7365 426f 6479 0a0a 2020 2020 6465  onseBody..    de
+00019ba0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00019bb0: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
+00019bc0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00019bd0: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
+00019be0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+00019bf0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00019c00: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
+00019c10: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
+00019c20: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
+00019c30: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00019c40: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
+00019c50: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
+00019c60: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00019c70: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00019c80: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00019c90: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00019ca0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00019cb0: 2020 5f6d 6170 203d 2073 7570 6572 2853    _map = super(S
+00019cc0: 746f 7045 6169 7345 6952 6573 706f 6e73  topEaisEiRespons
+00019cd0: 652c 2073 656c 6629 2e74 6f5f 6d61 7028  e, self).to_map(
+00019ce0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00019cf0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00019d00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00019d10: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00019d20: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00019d30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00019d40: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+00019d50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00019d60: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
+00019d70: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
+00019d80: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00019d90: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
+00019da0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00019db0: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+00019dc0: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
+00019dd0: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
+00019de0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00019df0: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+00019e00: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00019e10: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
+00019e20: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
+00019e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019e40: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00019e50: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00019e60: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00019e70: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00019e80: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00019e90: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+00019ea0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00019eb0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00019ec0: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+00019ed0: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+00019ee0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00019ef0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00019f00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00019f10: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00019f20: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00019f30: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00019f40: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+00019f50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00019f60: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00019f70: 203d 2053 746f 7045 6169 7345 6952 6573   = StopEaisEiRes
+00019f80: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
+00019f90: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00019fa0: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
+00019fb0: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
+00019fc0: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+00019fd0: 6e20 7365 6c66 0a0a 0a                   n self...
```

### Comparing `alibabacloud_eais20190624_py2-2.1.2/alibabacloud_eais20190624_py2.egg-info/PKG-INFO` & `alibabacloud_eais20190624_py2-2.1.3/alibabacloud_eais20190624_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eais20190624-py2
-Version: 2.1.2
+Version: 2.1.3
 Summary: Alibaba Cloud eais (20190624) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eais20190624_py2-2.1.2/setup.py` & `alibabacloud_eais20190624_py2-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eais20190624_py2.
 
-Created on 10/01/2023
+Created on 12/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eais20190624"
 NAME = "alibabacloud_eais20190624_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eais (20190624) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.0, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

