# Comparing `tmp/alibabacloud_eais20190624-2.1.2.tar.gz` & `tmp/alibabacloud_eais20190624-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eais20190624-2.1.2.tar", last modified: Tue Jan 10 06:16:02 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eais20190624-2.1.3.tar", last modified: Wed Jul 12 03:15:16 2023, max compression
```

## Comparing `alibabacloud_eais20190624-2.1.2.tar` & `alibabacloud_eais20190624-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:16:02.000000 alibabacloud_eais20190624-2.1.2/
--rw-r--r--   0 root         (0) root         (0)      638 2023-01-10 06:16:01.000000 alibabacloud_eais20190624-2.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-01-10 06:16:01.000000 alibabacloud_eais20190624-2.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-10 06:16:01.000000 alibabacloud_eais20190624-2.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2334 2023-01-10 06:16:02.000000 alibabacloud_eais20190624-2.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-01-10 06:16:01.000000 alibabacloud_eais20190624-2.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-01-10 06:16:01.000000 alibabacloud_eais20190624-2.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:16:02.000000 alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-10 06:16:01.000000 alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53744 2023-01-10 06:16:01.000000 alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624/client.py
--rw-r--r--   0 root         (0) root         (0)    84992 2023-01-10 06:16:01.000000 alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-10 06:16:02.000000 alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-01-10 06:16:02.000000 alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-01-10 06:16:02.000000 alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-10 06:16:02.000000 alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-01-10 06:16:02.000000 alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-01-10 06:16:02.000000 alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-10 06:16:02.000000 alibabacloud_eais20190624-2.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2615 2023-01-10 06:16:01.000000 alibabacloud_eais20190624-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:15:16.000000 alibabacloud_eais20190624-2.1.3/
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-12 03:15:15.000000 alibabacloud_eais20190624-2.1.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-12 03:15:15.000000 alibabacloud_eais20190624-2.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 03:15:15.000000 alibabacloud_eais20190624-2.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-12 03:15:16.000000 alibabacloud_eais20190624-2.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-07-12 03:15:15.000000 alibabacloud_eais20190624-2.1.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-07-12 03:15:15.000000 alibabacloud_eais20190624-2.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:15:16.000000 alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 03:15:15.000000 alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72472 2023-07-12 03:15:15.000000 alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624/client.py
+-rw-r--r--   0 root         (0) root         (0)   106212 2023-07-12 03:15:15.000000 alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:15:16.000000 alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-12 03:15:16.000000 alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-07-12 03:15:16.000000 alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 03:15:16.000000 alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-12 03:15:16.000000 alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-12 03:15:16.000000 alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 03:15:16.000000 alibabacloud_eais20190624-2.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-07-12 03:15:15.000000 alibabacloud_eais20190624-2.1.3/setup.py
```

### Comparing `alibabacloud_eais20190624-2.1.2/ChangeLog.md` & `alibabacloud_eais20190624-2.1.3/ChangeLog.md`

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

### Comparing `alibabacloud_eais20190624-2.1.2/LICENSE` & `alibabacloud_eais20190624-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eais20190624-2.1.2/PKG-INFO` & `alibabacloud_eais20190624-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eais20190624
-Version: 2.1.2
+Version: 2.1.3
 Summary: Alibaba Cloud eais (20190624) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eais20190624-2.1.2/README-CN.md` & `alibabacloud_eais20190624-2.1.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eais20190624-2.1.2/README.md` & `alibabacloud_eais20190624-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624/client.py` & `alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -168,14 +168,96 @@
     async def attach_eai_async(
         self,
         request: eais_20190624_models.AttachEaiRequest,
     ) -> eais_20190624_models.AttachEaiResponse:
         runtime = util_models.RuntimeOptions()
         return await self.attach_eai_with_options_async(request, runtime)
 
+    def attach_eais_ei_with_options(
+        self,
+        request: eais_20190624_models.AttachEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.AttachEaisEiResponse:
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
+    async def attach_eais_ei_with_options_async(
+        self,
+        request: eais_20190624_models.AttachEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.AttachEaisEiResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def attach_eais_ei(
+        self,
+        request: eais_20190624_models.AttachEaisEiRequest,
+    ) -> eais_20190624_models.AttachEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.attach_eais_ei_with_options(request, runtime)
+
+    async def attach_eais_ei_async(
+        self,
+        request: eais_20190624_models.AttachEaisEiRequest,
+    ) -> eais_20190624_models.AttachEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.attach_eais_ei_with_options_async(request, runtime)
+
     def change_resource_group_with_options(
         self,
         request: eais_20190624_models.ChangeResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> eais_20190624_models.ChangeResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -255,14 +337,16 @@
         request: eais_20190624_models.CreateEaiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> eais_20190624_models.CreateEaiResponse:
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
@@ -295,14 +379,16 @@
         request: eais_20190624_models.CreateEaiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> eais_20190624_models.CreateEaiResponse:
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
@@ -725,14 +811,16 @@
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
@@ -769,14 +857,16 @@
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
@@ -814,14 +904,108 @@
     async def create_eai_jupyter_async(
         self,
         request: eais_20190624_models.CreateEaiJupyterRequest,
     ) -> eais_20190624_models.CreateEaiJupyterResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_eai_jupyter_with_options_async(request, runtime)
 
+    def create_eais_ei_with_options(
+        self,
+        request: eais_20190624_models.CreateEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.CreateEaisEiResponse:
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
+    async def create_eais_ei_with_options_async(
+        self,
+        request: eais_20190624_models.CreateEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.CreateEaisEiResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_eais_ei(
+        self,
+        request: eais_20190624_models.CreateEaisEiRequest,
+    ) -> eais_20190624_models.CreateEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_eais_ei_with_options(request, runtime)
+
+    async def create_eais_ei_async(
+        self,
+        request: eais_20190624_models.CreateEaisEiRequest,
+    ) -> eais_20190624_models.CreateEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_eais_ei_with_options_async(request, runtime)
+
     def delete_eai_with_options(
         self,
         request: eais_20190624_models.DeleteEaiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> eais_20190624_models.DeleteEaiResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -970,14 +1154,92 @@
     async def delete_eai_all_async(
         self,
         request: eais_20190624_models.DeleteEaiAllRequest,
     ) -> eais_20190624_models.DeleteEaiAllResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_eai_all_with_options_async(request, runtime)
 
+    def delete_eais_ei_with_options(
+        self,
+        request: eais_20190624_models.DeleteEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.DeleteEaisEiResponse:
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
+    async def delete_eais_ei_with_options_async(
+        self,
+        request: eais_20190624_models.DeleteEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.DeleteEaisEiResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_eais_ei(
+        self,
+        request: eais_20190624_models.DeleteEaisEiRequest,
+    ) -> eais_20190624_models.DeleteEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_eais_ei_with_options(request, runtime)
+
+    async def delete_eais_ei_async(
+        self,
+        request: eais_20190624_models.DeleteEaisEiRequest,
+    ) -> eais_20190624_models.DeleteEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_eais_ei_with_options_async(request, runtime)
+
     def describe_eais_with_options(
         self,
         request: eais_20190624_models.DescribeEaisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> eais_20190624_models.DescribeEaisResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1192,27 +1454,103 @@
     async def detach_eai_async(
         self,
         request: eais_20190624_models.DetachEaiRequest,
     ) -> eais_20190624_models.DetachEaiResponse:
         runtime = util_models.RuntimeOptions()
         return await self.detach_eai_with_options_async(request, runtime)
 
+    def detach_eais_ei_with_options(
+        self,
+        request: eais_20190624_models.DetachEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.DetachEaisEiResponse:
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
+    async def detach_eais_ei_with_options_async(
+        self,
+        request: eais_20190624_models.DetachEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.DetachEaisEiResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def detach_eais_ei(
+        self,
+        request: eais_20190624_models.DetachEaisEiRequest,
+    ) -> eais_20190624_models.DetachEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.detach_eais_ei_with_options(request, runtime)
+
+    async def detach_eais_ei_async(
+        self,
+        request: eais_20190624_models.DetachEaisEiRequest,
+    ) -> eais_20190624_models.DetachEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.detach_eais_ei_with_options_async(request, runtime)
+
     def get_instance_metrics_with_options(
         self,
         request: eais_20190624_models.GetInstanceMetricsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> eais_20190624_models.GetInstanceMetricsResponse:
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
@@ -1241,14 +1579,16 @@
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
@@ -1277,7 +1617,155 @@
 
     async def get_instance_metrics_async(
         self,
         request: eais_20190624_models.GetInstanceMetricsRequest,
     ) -> eais_20190624_models.GetInstanceMetricsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_instance_metrics_with_options_async(request, runtime)
+
+    def start_eais_ei_with_options(
+        self,
+        request: eais_20190624_models.StartEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.StartEaisEiResponse:
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
+    async def start_eais_ei_with_options_async(
+        self,
+        request: eais_20190624_models.StartEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.StartEaisEiResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def start_eais_ei(
+        self,
+        request: eais_20190624_models.StartEaisEiRequest,
+    ) -> eais_20190624_models.StartEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.start_eais_ei_with_options(request, runtime)
+
+    async def start_eais_ei_async(
+        self,
+        request: eais_20190624_models.StartEaisEiRequest,
+    ) -> eais_20190624_models.StartEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.start_eais_ei_with_options_async(request, runtime)
+
+    def stop_eais_ei_with_options(
+        self,
+        request: eais_20190624_models.StopEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.StopEaisEiResponse:
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
+    async def stop_eais_ei_with_options_async(
+        self,
+        request: eais_20190624_models.StopEaisEiRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> eais_20190624_models.StopEaisEiResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def stop_eais_ei(
+        self,
+        request: eais_20190624_models.StopEaisEiRequest,
+    ) -> eais_20190624_models.StopEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.stop_eais_ei_with_options(request, runtime)
+
+    async def stop_eais_ei_async(
+        self,
+        request: eais_20190624_models.StopEaisEiRequest,
+    ) -> eais_20190624_models.StopEaisEiResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.stop_eais_ei_with_options_async(request, runtime)
```

### Comparing `alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624/models.py` & `alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -257,5056 +257,6383 @@
 00001000: 7465 6d70 5f6d 6f64 656c 203d 2041 7474  temp_model = Att
 00001010: 6163 6845 6169 5265 7370 6f6e 7365 426f  achEaiResponseBo
 00001020: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
 00001030: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
 00001040: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
 00001050: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
 00001060: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00001070: 0a0a 636c 6173 7320 4368 616e 6765 5265  ..class ChangeRe
-00001080: 736f 7572 6365 4772 6f75 7052 6571 7565  sourceGroupReque
-00001090: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
-000010a0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-000010b0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000010c0: 2020 2020 2020 7265 736f 7572 6365 5f67        resource_g
-000010d0: 726f 7570 5f69 643a 2073 7472 203d 204e  roup_id: str = N
-000010e0: 6f6e 652c 0a20 2020 2020 2020 2072 6573  one,.        res
-000010f0: 6f75 7263 655f 6964 3a20 7374 7220 3d20  ource_id: str = 
-00001100: 4e6f 6e65 2c0a 2020 2020 2020 2020 7265  None,.        re
-00001110: 736f 7572 6365 5f72 6567 696f 6e5f 6964  source_region_id
-00001120: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00001130: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-00001140: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
-00001150: 5f69 6420 3d20 7265 736f 7572 6365 5f67  _id = resource_g
-00001160: 726f 7570 5f69 640a 2020 2020 2020 2020  roup_id.        
-00001170: 7365 6c66 2e72 6573 6f75 7263 655f 6964  self.resource_id
-00001180: 203d 2072 6573 6f75 7263 655f 6964 0a20   = resource_id. 
-00001190: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
-000011a0: 7572 6365 5f72 6567 696f 6e5f 6964 203d  urce_region_id =
-000011b0: 2072 6573 6f75 7263 655f 7265 6769 6f6e   resource_region
-000011c0: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
-000011d0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-000011e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000011f0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00001200: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00001210: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-00001220: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00001230: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00001240: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001250: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00001260: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00001270: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-00001280: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-00001290: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000012a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000012b0: 5b27 5265 736f 7572 6365 4772 6f75 7049  ['ResourceGroupI
-000012c0: 6427 5d20 3d20 7365 6c66 2e72 6573 6f75  d'] = self.resou
-000012d0: 7263 655f 6772 6f75 705f 6964 0a20 2020  rce_group_id.   
-000012e0: 2020 2020 2069 6620 7365 6c66 2e72 6573       if self.res
-000012f0: 6f75 7263 655f 6964 2069 7320 6e6f 7420  ource_id is not 
-00001300: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00001310: 2020 7265 7375 6c74 5b27 5265 736f 7572    result['Resour
-00001320: 6365 4964 275d 203d 2073 656c 662e 7265  ceId'] = self.re
-00001330: 736f 7572 6365 5f69 640a 2020 2020 2020  source_id.      
-00001340: 2020 6966 2073 656c 662e 7265 736f 7572    if self.resour
-00001350: 6365 5f72 6567 696f 6e5f 6964 2069 7320  ce_region_id is 
-00001360: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00001370: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-00001380: 736f 7572 6365 5265 6769 6f6e 4964 275d  sourceRegionId']
-00001390: 203d 2073 656c 662e 7265 736f 7572 6365   = self.resource
-000013a0: 5f72 6567 696f 6e5f 6964 0a20 2020 2020  _region_id.     
-000013b0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-000013c0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-000013d0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-000013e0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-000013f0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-00001400: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00001410: 6574 2827 5265 736f 7572 6365 4772 6f75  et('ResourceGrou
-00001420: 7049 6427 2920 6973 206e 6f74 204e 6f6e  pId') is not Non
-00001430: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00001440: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
-00001450: 7570 5f69 6420 3d20 6d2e 6765 7428 2752  up_id = m.get('R
-00001460: 6573 6f75 7263 6547 726f 7570 4964 2729  esourceGroupId')
-00001470: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00001480: 7428 2752 6573 6f75 7263 6549 6427 2920  t('ResourceId') 
-00001490: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000014a0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-000014b0: 736f 7572 6365 5f69 6420 3d20 6d2e 6765  source_id = m.ge
-000014c0: 7428 2752 6573 6f75 7263 6549 6427 290a  t('ResourceId').
-000014d0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000014e0: 2827 5265 736f 7572 6365 5265 6769 6f6e  ('ResourceRegion
-000014f0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00001500: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00001510: 6c66 2e72 6573 6f75 7263 655f 7265 6769  lf.resource_regi
-00001520: 6f6e 5f69 6420 3d20 6d2e 6765 7428 2752  on_id = m.get('R
-00001530: 6573 6f75 7263 6552 6567 696f 6e49 6427  esourceRegionId'
-00001540: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00001550: 2073 656c 660a 0a0a 636c 6173 7320 4368   self...class Ch
-00001560: 616e 6765 5265 736f 7572 6365 4772 6f75  angeResourceGrou
-00001570: 7052 6573 706f 6e73 6542 6f64 7928 5465  pResponseBody(Te
-00001580: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00001590: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-000015a0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000015b0: 2072 6571 7565 7374 5f69 643a 2073 7472   request_id: str
-000015c0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000015d0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
-000015e0: 7565 7374 5f69 6420 3d20 7265 7175 6573  uest_id = reques
-000015f0: 745f 6964 0a0a 2020 2020 6465 6620 7661  t_id..    def va
-00001600: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-00001610: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00001620: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-00001630: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-00001640: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-00001650: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-00001660: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-00001670: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001680: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-00001690: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-000016a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000016b0: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
-000016c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000016d0: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
-000016e0: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
-000016f0: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
-00001700: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00001710: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00001720: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-00001730: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-00001740: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00001750: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00001760: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
-00001770: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00001780: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
-00001790: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
-000017a0: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
-000017b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000017c0: 0a0a 0a63 6c61 7373 2043 6861 6e67 6552  ...class ChangeR
-000017d0: 6573 6f75 7263 6547 726f 7570 5265 7370  esourceGroupResp
-000017e0: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-000017f0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00001800: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00001810: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-00001820: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
-00001830: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00001840: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
-00001850: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00001860: 2062 6f64 793a 2043 6861 6e67 6552 6573   body: ChangeRes
-00001870: 6f75 7263 6547 726f 7570 5265 7370 6f6e  ourceGroupRespon
-00001880: 7365 426f 6479 203d 204e 6f6e 652c 0a20  seBody = None,. 
-00001890: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-000018a0: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
-000018b0: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
-000018c0: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-000018d0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-000018e0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-000018f0: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
-00001900: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-00001910: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-00001920: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-00001930: 662e 6865 6164 6572 732c 2027 6865 6164  f.headers, 'head
-00001940: 6572 7327 290a 2020 2020 2020 2020 7365  ers').        se
-00001950: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-00001960: 6972 6564 2873 656c 662e 7374 6174 7573  ired(self.status
-00001970: 5f63 6f64 652c 2027 7374 6174 7573 5f63  _code, 'status_c
-00001980: 6f64 6527 290a 2020 2020 2020 2020 7365  ode').        se
-00001990: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-000019a0: 6972 6564 2873 656c 662e 626f 6479 2c20  ired(self.body, 
-000019b0: 2762 6f64 7927 290a 2020 2020 2020 2020  'body').        
-000019c0: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-000019d0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-000019e0: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-000019f0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-00001a00: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-00001a10: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-00001a20: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00001a30: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00001a40: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00001a50: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00001a60: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00001a70: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00001a80: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-00001a90: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00001aa0: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-00001ab0: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-00001ac0: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-00001ad0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00001ae0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00001af0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00001b00: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
-00001b10: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
-00001b20: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
-00001b30: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
-00001b40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00001b50: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
-00001b60: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
-00001b70: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
-00001b80: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00001b90: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00001ba0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-00001bb0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00001bc0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-00001bd0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
-00001be0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
-00001bf0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00001c00: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-00001c10: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-00001c20: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00001c30: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
-00001c40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00001c50: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00001c60: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
-00001c70: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
-00001c80: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00001c90: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
-00001ca0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00001cb0: 2020 7465 6d70 5f6d 6f64 656c 203d 2043    temp_model = C
-00001cc0: 6861 6e67 6552 6573 6f75 7263 6547 726f  hangeResourceGro
-00001cd0: 7570 5265 7370 6f6e 7365 426f 6479 2829  upResponseBody()
-00001ce0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00001cf0: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
-00001d00: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
-00001d10: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
-00001d20: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00001d30: 6173 7320 4372 6561 7465 4561 6952 6571  ass CreateEaiReq
-00001d40: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
-00001d50: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00001d60: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00001d70: 2020 2020 2020 2020 636c 6965 6e74 5f74          client_t
-00001d80: 6f6b 656e 3a20 7374 7220 3d20 4e6f 6e65  oken: str = None
-00001d90: 2c0a 2020 2020 2020 2020 696e 7374 616e  ,.        instan
-00001da0: 6365 5f6e 616d 653a 2073 7472 203d 204e  ce_name: str = N
-00001db0: 6f6e 652c 0a20 2020 2020 2020 2069 6e73  one,.        ins
-00001dc0: 7461 6e63 655f 7479 7065 3a20 7374 7220  tance_type: str 
-00001dd0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00001de0: 7265 6769 6f6e 5f69 643a 2073 7472 203d  region_id: str =
-00001df0: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
-00001e00: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-00001e10: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00001e20: 2020 2020 2020 7365 6375 7269 7479 5f67        security_g
-00001e30: 726f 7570 5f69 643a 2073 7472 203d 204e  roup_id: str = N
-00001e40: 6f6e 652c 0a20 2020 2020 2020 2076 5f73  one,.        v_s
-00001e50: 7769 7463 685f 6964 3a20 7374 7220 3d20  witch_id: str = 
-00001e60: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00001e70: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-00001e80: 5f74 6f6b 656e 203d 2063 6c69 656e 745f  _token = client_
-00001e90: 746f 6b65 6e0a 2020 2020 2020 2020 7365  token.        se
-00001ea0: 6c66 2e69 6e73 7461 6e63 655f 6e61 6d65  lf.instance_name
-00001eb0: 203d 2069 6e73 7461 6e63 655f 6e61 6d65   = instance_name
-00001ec0: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00001ed0: 7374 616e 6365 5f74 7970 6520 3d20 696e  stance_type = in
-00001ee0: 7374 616e 6365 5f74 7970 650a 2020 2020  stance_type.    
-00001ef0: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
-00001f00: 6964 203d 2072 6567 696f 6e5f 6964 0a20  id = region_id. 
-00001f10: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
-00001f20: 7572 6365 5f67 726f 7570 5f69 6420 3d20  urce_group_id = 
-00001f30: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-00001f40: 640a 2020 2020 2020 2020 7365 6c66 2e73  d.        self.s
-00001f50: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
-00001f60: 203d 2073 6563 7572 6974 795f 6772 6f75   = security_grou
-00001f70: 705f 6964 0a20 2020 2020 2020 2073 656c  p_id.        sel
-00001f80: 662e 765f 7377 6974 6368 5f69 6420 3d20  f.v_switch_id = 
-00001f90: 765f 7377 6974 6368 5f69 640a 0a20 2020  v_switch_id..   
-00001fa0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00001fb0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-00001fc0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-00001fd0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00001fe0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-00001ff0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00002000: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00002010: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00002020: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00002030: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00002040: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00002050: 6620 7365 6c66 2e63 6c69 656e 745f 746f  f self.client_to
-00002060: 6b65 6e20 6973 206e 6f74 204e 6f6e 653a  ken is not None:
-00002070: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00002080: 756c 745b 2743 6c69 656e 7454 6f6b 656e  ult['ClientToken
-00002090: 275d 203d 2073 656c 662e 636c 6965 6e74  '] = self.client
-000020a0: 5f74 6f6b 656e 0a20 2020 2020 2020 2069  _token.        i
-000020b0: 6620 7365 6c66 2e69 6e73 7461 6e63 655f  f self.instance_
-000020c0: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-000020d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000020e0: 7375 6c74 5b27 496e 7374 616e 6365 4e61  sult['InstanceNa
-000020f0: 6d65 275d 203d 2073 656c 662e 696e 7374  me'] = self.inst
-00002100: 616e 6365 5f6e 616d 650a 2020 2020 2020  ance_name.      
-00002110: 2020 6966 2073 656c 662e 696e 7374 616e    if self.instan
-00002120: 6365 5f74 7970 6520 6973 206e 6f74 204e  ce_type is not N
-00002130: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002140: 2072 6573 756c 745b 2749 6e73 7461 6e63   result['Instanc
-00002150: 6554 7970 6527 5d20 3d20 7365 6c66 2e69  eType'] = self.i
-00002160: 6e73 7461 6e63 655f 7479 7065 0a20 2020  nstance_type.   
-00002170: 2020 2020 2069 6620 7365 6c66 2e72 6567       if self.reg
-00002180: 696f 6e5f 6964 2069 7320 6e6f 7420 4e6f  ion_id is not No
-00002190: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000021a0: 7265 7375 6c74 5b27 5265 6769 6f6e 4964  result['RegionId
-000021b0: 275d 203d 2073 656c 662e 7265 6769 6f6e  '] = self.region
-000021c0: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-000021d0: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
-000021e0: 7570 5f69 6420 6973 206e 6f74 204e 6f6e  up_id is not Non
-000021f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00002200: 6573 756c 745b 2752 6573 6f75 7263 6547  esult['ResourceG
-00002210: 726f 7570 4964 275d 203d 2073 656c 662e  roupId'] = self.
-00002220: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-00002230: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00002240: 662e 7365 6375 7269 7479 5f67 726f 7570  f.security_group
-00002250: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00002260: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00002270: 756c 745b 2753 6563 7572 6974 7947 726f  ult['SecurityGro
-00002280: 7570 4964 275d 203d 2073 656c 662e 7365  upId'] = self.se
-00002290: 6375 7269 7479 5f67 726f 7570 5f69 640a  curity_group_id.
-000022a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000022b0: 765f 7377 6974 6368 5f69 6420 6973 206e  v_switch_id is n
-000022c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000022d0: 2020 2020 2072 6573 756c 745b 2756 5377       result['VSw
-000022e0: 6974 6368 4964 275d 203d 2073 656c 662e  itchId'] = self.
-000022f0: 765f 7377 6974 6368 5f69 640a 2020 2020  v_switch_id.    
-00002300: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00002310: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00002320: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00002330: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00002340: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00002350: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00002360: 6765 7428 2743 6c69 656e 7454 6f6b 656e  get('ClientToken
-00002370: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00002380: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002390: 2e63 6c69 656e 745f 746f 6b65 6e20 3d20  .client_token = 
-000023a0: 6d2e 6765 7428 2743 6c69 656e 7454 6f6b  m.get('ClientTok
-000023b0: 656e 2729 0a20 2020 2020 2020 2069 6620  en').        if 
-000023c0: 6d2e 6765 7428 2749 6e73 7461 6e63 654e  m.get('InstanceN
-000023d0: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
-000023e0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-000023f0: 656c 662e 696e 7374 616e 6365 5f6e 616d  elf.instance_nam
-00002400: 6520 3d20 6d2e 6765 7428 2749 6e73 7461  e = m.get('Insta
-00002410: 6e63 654e 616d 6527 290a 2020 2020 2020  nceName').      
-00002420: 2020 6966 206d 2e67 6574 2827 496e 7374    if m.get('Inst
-00002430: 616e 6365 5479 7065 2729 2069 7320 6e6f  anceType') is no
-00002440: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002450: 2020 2020 7365 6c66 2e69 6e73 7461 6e63      self.instanc
-00002460: 655f 7479 7065 203d 206d 2e67 6574 2827  e_type = m.get('
-00002470: 496e 7374 616e 6365 5479 7065 2729 0a20  InstanceType'). 
-00002480: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00002490: 2752 6567 696f 6e49 6427 2920 6973 206e  'RegionId') is n
-000024a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000024b0: 2020 2020 2073 656c 662e 7265 6769 6f6e       self.region
-000024c0: 5f69 6420 3d20 6d2e 6765 7428 2752 6567  _id = m.get('Reg
-000024d0: 696f 6e49 6427 290a 2020 2020 2020 2020  ionId').        
-000024e0: 6966 206d 2e67 6574 2827 5265 736f 7572  if m.get('Resour
-000024f0: 6365 4772 6f75 7049 6427 2920 6973 206e  ceGroupId') is n
-00002500: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00002510: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
-00002520: 6365 5f67 726f 7570 5f69 6420 3d20 6d2e  ce_group_id = m.
-00002530: 6765 7428 2752 6573 6f75 7263 6547 726f  get('ResourceGro
-00002540: 7570 4964 2729 0a20 2020 2020 2020 2069  upId').        i
-00002550: 6620 6d2e 6765 7428 2753 6563 7572 6974  f m.get('Securit
-00002560: 7947 726f 7570 4964 2729 2069 7320 6e6f  yGroupId') is no
-00002570: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002580: 2020 2020 7365 6c66 2e73 6563 7572 6974      self.securit
-00002590: 795f 6772 6f75 705f 6964 203d 206d 2e67  y_group_id = m.g
-000025a0: 6574 2827 5365 6375 7269 7479 4772 6f75  et('SecurityGrou
-000025b0: 7049 6427 290a 2020 2020 2020 2020 6966  pId').        if
-000025c0: 206d 2e67 6574 2827 5653 7769 7463 6849   m.get('VSwitchI
-000025d0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-000025e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000025f0: 662e 765f 7377 6974 6368 5f69 6420 3d20  f.v_switch_id = 
-00002600: 6d2e 6765 7428 2756 5377 6974 6368 4964  m.get('VSwitchId
-00002610: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00002620: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2043  n self...class C
-00002630: 7265 6174 6545 6169 5265 7370 6f6e 7365  reateEaiResponse
-00002640: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
-00002650: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00002660: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00002670: 2020 2020 2020 2020 656c 6173 7469 635f          elastic_
-00002680: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
-00002690: 616e 6365 5f69 643a 2073 7472 203d 204e  ance_id: str = N
-000026a0: 6f6e 652c 0a20 2020 2020 2020 2072 6571  one,.        req
-000026b0: 7565 7374 5f69 643a 2073 7472 203d 204e  uest_id: str = N
-000026c0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-000026d0: 2020 2020 7365 6c66 2e65 6c61 7374 6963      self.elastic
-000026e0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
-000026f0: 7461 6e63 655f 6964 203d 2065 6c61 7374  tance_id = elast
-00002700: 6963 5f61 6363 656c 6572 6174 6564 5f69  ic_accelerated_i
-00002710: 6e73 7461 6e63 655f 6964 0a20 2020 2020  nstance_id.     
-00002720: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-00002730: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
-00002740: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00002750: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00002760: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00002770: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00002780: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00002790: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-000027a0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-000027b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000027c0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-000027d0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-000027e0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-000027f0: 2020 2069 6620 7365 6c66 2e65 6c61 7374     if self.elast
-00002800: 6963 5f61 6363 656c 6572 6174 6564 5f69  ic_accelerated_i
-00002810: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
-00002820: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002830: 2020 2020 7265 7375 6c74 5b27 456c 6173      result['Elas
-00002840: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
-00002850: 7374 616e 6365 4964 275d 203d 2073 656c  stanceId'] = sel
-00002860: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-00002870: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-00002880: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00002890: 662e 7265 7175 6573 745f 6964 2069 7320  f.request_id is 
-000028a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000028b0: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-000028c0: 7175 6573 7449 6427 5d20 3d20 7365 6c66  questId'] = self
-000028d0: 2e72 6571 7565 7374 5f69 640a 2020 2020  .request_id.    
-000028e0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-000028f0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00002900: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00002910: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00002920: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00002930: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00002940: 6765 7428 2745 6c61 7374 6963 4163 6365  get('ElasticAcce
-00002950: 6c65 7261 7465 6449 6e73 7461 6e63 6549  leratedInstanceI
-00002960: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00002970: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002980: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-00002990: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-000029a0: 6420 3d20 6d2e 6765 7428 2745 6c61 7374  d = m.get('Elast
-000029b0: 6963 4163 6365 6c65 7261 7465 6449 6e73  icAcceleratedIns
-000029c0: 7461 6e63 6549 6427 290a 2020 2020 2020  tanceId').      
-000029d0: 2020 6966 206d 2e67 6574 2827 5265 7175    if m.get('Requ
-000029e0: 6573 7449 6427 2920 6973 206e 6f74 204e  estId') is not N
-000029f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00002a00: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-00002a10: 203d 206d 2e67 6574 2827 5265 7175 6573   = m.get('Reques
-00002a20: 7449 6427 290a 2020 2020 2020 2020 7265  tId').        re
-00002a30: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-00002a40: 7320 4372 6561 7465 4561 6952 6573 706f  s CreateEaiRespo
-00002a50: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
-00002a60: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00002a70: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00002a80: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
-00002a90: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
-00002aa0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-00002ab0: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
-00002ac0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00002ad0: 626f 6479 3a20 4372 6561 7465 4561 6952  body: CreateEaiR
-00002ae0: 6573 706f 6e73 6542 6f64 7920 3d20 4e6f  esponseBody = No
-00002af0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00002b00: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-00002b10: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
-00002b20: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-00002b30: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-00002b40: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-00002b50: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
-00002b60: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-00002b70: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00002b80: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-00002b90: 6428 7365 6c66 2e68 6561 6465 7273 2c20  d(self.headers, 
-00002ba0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00002bb0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-00002bc0: 5f72 6571 7569 7265 6428 7365 6c66 2e73  _required(self.s
-00002bd0: 7461 7475 735f 636f 6465 2c20 2773 7461  tatus_code, 'sta
-00002be0: 7475 735f 636f 6465 2729 0a20 2020 2020  tus_code').     
-00002bf0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-00002c00: 5f72 6571 7569 7265 6428 7365 6c66 2e62  _required(self.b
-00002c10: 6f64 792c 2027 626f 6479 2729 0a20 2020  ody, 'body').   
-00002c20: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00002c30: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-00002c40: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-00002c50: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-00002c60: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00002c70: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00002c80: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00002c90: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00002ca0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00002cb0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00002cc0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00002cd0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00002ce0: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-00002cf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00002d00: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00002d10: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-00002d20: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-00002d30: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-00002d40: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-00002d50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002d60: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-00002d70: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-00002d80: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-00002d90: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-00002da0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00002db0: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00002dc0: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00002dd0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00002de0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00002df0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00002e00: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-00002e10: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-00002e20: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00002e30: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00002e40: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
-00002e50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00002e60: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-00002e70: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
-00002e80: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
-00002e90: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-00002ea0: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
-00002eb0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00002ec0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-00002ed0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
-00002ee0: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
-00002ef0: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
-00002f00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00002f10: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-00002f20: 6c20 3d20 4372 6561 7465 4561 6952 6573  l = CreateEaiRes
-00002f30: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
-00002f40: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00002f50: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-00002f60: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-00002f70: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-00002f80: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2043  n self...class C
-00002f90: 7265 6174 6545 6169 416c 6c52 6571 7565  reateEaiAllReque
-00002fa0: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
-00002fb0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00002fc0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00002fd0: 2020 2020 2020 636c 6965 6e74 5f69 6d61        client_ima
-00002fe0: 6765 5f69 643a 2073 7472 203d 204e 6f6e  ge_id: str = Non
-00002ff0: 652c 0a20 2020 2020 2020 2063 6c69 656e  e,.        clien
-00003000: 745f 696e 7374 616e 6365 5f6e 616d 653a  t_instance_name:
-00003010: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00003020: 2020 2020 2063 6c69 656e 745f 696e 7374       client_inst
-00003030: 616e 6365 5f74 7970 653a 2073 7472 203d  ance_type: str =
-00003040: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-00003050: 6c69 656e 745f 696e 7465 726e 6574 5f6d  lient_internet_m
-00003060: 6178 5f62 616e 6477 6964 7468 5f69 6e3a  ax_bandwidth_in:
-00003070: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-00003080: 2020 2020 2063 6c69 656e 745f 696e 7465       client_inte
-00003090: 726e 6574 5f6d 6178 5f62 616e 6477 6964  rnet_max_bandwid
-000030a0: 7468 5f6f 7574 3a20 696e 7420 3d20 4e6f  th_out: int = No
-000030b0: 6e65 2c0a 2020 2020 2020 2020 636c 6965  ne,.        clie
-000030c0: 6e74 5f70 6173 7377 6f72 643a 2073 7472  nt_password: str
-000030d0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000030e0: 2063 6c69 656e 745f 7365 6375 7269 7479   client_security
-000030f0: 5f67 726f 7570 5f69 643a 2073 7472 203d  _group_id: str =
-00003100: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-00003110: 6c69 656e 745f 7379 7374 656d 5f64 6973  lient_system_dis
-00003120: 6b5f 6361 7465 676f 7279 3a20 7374 7220  k_category: str 
-00003130: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00003140: 636c 6965 6e74 5f73 7973 7465 6d5f 6469  client_system_di
-00003150: 736b 5f73 697a 653a 2069 6e74 203d 204e  sk_size: int = N
-00003160: 6f6e 652c 0a20 2020 2020 2020 2063 6c69  one,.        cli
-00003170: 656e 745f 746f 6b65 6e3a 2073 7472 203d  ent_token: str =
-00003180: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-00003190: 6c69 656e 745f 7673 7769 7463 685f 6964  lient_vswitch_id
-000031a0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000031b0: 2020 2020 2020 636c 6965 6e74 5f7a 6f6e        client_zon
-000031c0: 655f 6964 3a20 7374 7220 3d20 4e6f 6e65  e_id: str = None
-000031d0: 2c0a 2020 2020 2020 2020 6561 695f 696e  ,.        eai_in
-000031e0: 7374 616e 6365 5f74 7970 653a 2073 7472  stance_type: str
-000031f0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00003200: 2069 6e73 7461 6e63 655f 6e61 6d65 3a20   instance_name: 
-00003210: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00003220: 2020 2020 7265 6769 6f6e 5f69 643a 2073      region_id: s
-00003230: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-00003240: 2020 2072 6573 6f75 7263 655f 6772 6f75     resource_grou
-00003250: 705f 6964 3a20 7374 7220 3d20 4e6f 6e65  p_id: str = None
-00003260: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00003270: 2073 656c 662e 636c 6965 6e74 5f69 6d61   self.client_ima
-00003280: 6765 5f69 6420 3d20 636c 6965 6e74 5f69  ge_id = client_i
-00003290: 6d61 6765 5f69 640a 2020 2020 2020 2020  mage_id.        
-000032a0: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
-000032b0: 616e 6365 5f6e 616d 6520 3d20 636c 6965  ance_name = clie
-000032c0: 6e74 5f69 6e73 7461 6e63 655f 6e61 6d65  nt_instance_name
-000032d0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
-000032e0: 6965 6e74 5f69 6e73 7461 6e63 655f 7479  ient_instance_ty
-000032f0: 7065 203d 2063 6c69 656e 745f 696e 7374  pe = client_inst
-00003300: 616e 6365 5f74 7970 650a 2020 2020 2020  ance_type.      
-00003310: 2020 7365 6c66 2e63 6c69 656e 745f 696e    self.client_in
-00003320: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
-00003330: 6964 7468 5f69 6e20 3d20 636c 6965 6e74  idth_in = client
-00003340: 5f69 6e74 6572 6e65 745f 6d61 785f 6261  _internet_max_ba
-00003350: 6e64 7769 6474 685f 696e 0a20 2020 2020  ndwidth_in.     
-00003360: 2020 2073 656c 662e 636c 6965 6e74 5f69     self.client_i
-00003370: 6e74 6572 6e65 745f 6d61 785f 6261 6e64  nternet_max_band
-00003380: 7769 6474 685f 6f75 7420 3d20 636c 6965  width_out = clie
-00003390: 6e74 5f69 6e74 6572 6e65 745f 6d61 785f  nt_internet_max_
-000033a0: 6261 6e64 7769 6474 685f 6f75 740a 2020  bandwidth_out.  
-000033b0: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-000033c0: 745f 7061 7373 776f 7264 203d 2063 6c69  t_password = cli
-000033d0: 656e 745f 7061 7373 776f 7264 0a20 2020  ent_password.   
-000033e0: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-000033f0: 5f73 6563 7572 6974 795f 6772 6f75 705f  _security_group_
-00003400: 6964 203d 2063 6c69 656e 745f 7365 6375  id = client_secu
-00003410: 7269 7479 5f67 726f 7570 5f69 640a 2020  rity_group_id.  
-00003420: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-00003430: 745f 7379 7374 656d 5f64 6973 6b5f 6361  t_system_disk_ca
-00003440: 7465 676f 7279 203d 2063 6c69 656e 745f  tegory = client_
-00003450: 7379 7374 656d 5f64 6973 6b5f 6361 7465  system_disk_cate
-00003460: 676f 7279 0a20 2020 2020 2020 2073 656c  gory.        sel
-00003470: 662e 636c 6965 6e74 5f73 7973 7465 6d5f  f.client_system_
-00003480: 6469 736b 5f73 697a 6520 3d20 636c 6965  disk_size = clie
-00003490: 6e74 5f73 7973 7465 6d5f 6469 736b 5f73  nt_system_disk_s
-000034a0: 697a 650a 2020 2020 2020 2020 7365 6c66  ize.        self
-000034b0: 2e63 6c69 656e 745f 746f 6b65 6e20 3d20  .client_token = 
-000034c0: 636c 6965 6e74 5f74 6f6b 656e 0a20 2020  client_token.   
-000034d0: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-000034e0: 5f76 7377 6974 6368 5f69 6420 3d20 636c  _vswitch_id = cl
-000034f0: 6965 6e74 5f76 7377 6974 6368 5f69 640a  ient_vswitch_id.
-00003500: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-00003510: 656e 745f 7a6f 6e65 5f69 6420 3d20 636c  ent_zone_id = cl
-00003520: 6965 6e74 5f7a 6f6e 655f 6964 0a20 2020  ient_zone_id.   
-00003530: 2020 2020 2073 656c 662e 6561 695f 696e       self.eai_in
-00003540: 7374 616e 6365 5f74 7970 6520 3d20 6561  stance_type = ea
-00003550: 695f 696e 7374 616e 6365 5f74 7970 650a  i_instance_type.
-00003560: 2020 2020 2020 2020 7365 6c66 2e69 6e73          self.ins
-00003570: 7461 6e63 655f 6e61 6d65 203d 2069 6e73  tance_name = ins
-00003580: 7461 6e63 655f 6e61 6d65 0a20 2020 2020  tance_name.     
-00003590: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
-000035a0: 6420 3d20 7265 6769 6f6e 5f69 640a 2020  d = region_id.  
-000035b0: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
-000035c0: 7263 655f 6772 6f75 705f 6964 203d 2072  rce_group_id = r
-000035d0: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-000035e0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-000035f0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00003600: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00003610: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00003620: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00003630: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-00003640: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-00003650: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00003660: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-00003670: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-00003680: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-00003690: 2020 2020 6966 2073 656c 662e 636c 6965      if self.clie
-000036a0: 6e74 5f69 6d61 6765 5f69 6420 6973 206e  nt_image_id is n
-000036b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000036c0: 2020 2020 2072 6573 756c 745b 2743 6c69       result['Cli
-000036d0: 656e 7449 6d61 6765 4964 275d 203d 2073  entImageId'] = s
-000036e0: 656c 662e 636c 6965 6e74 5f69 6d61 6765  elf.client_image
-000036f0: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-00003700: 656c 662e 636c 6965 6e74 5f69 6e73 7461  elf.client_insta
-00003710: 6e63 655f 6e61 6d65 2069 7320 6e6f 7420  nce_name is not 
-00003720: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003730: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-00003740: 496e 7374 616e 6365 4e61 6d65 275d 203d  InstanceName'] =
-00003750: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
-00003760: 7461 6e63 655f 6e61 6d65 0a20 2020 2020  tance_name.     
-00003770: 2020 2069 6620 7365 6c66 2e63 6c69 656e     if self.clien
-00003780: 745f 696e 7374 616e 6365 5f74 7970 6520  t_instance_type 
-00003790: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000037a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000037b0: 2743 6c69 656e 7449 6e73 7461 6e63 6554  'ClientInstanceT
-000037c0: 7970 6527 5d20 3d20 7365 6c66 2e63 6c69  ype'] = self.cli
-000037d0: 656e 745f 696e 7374 616e 6365 5f74 7970  ent_instance_typ
-000037e0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-000037f0: 662e 636c 6965 6e74 5f69 6e74 6572 6e65  f.client_interne
-00003800: 745f 6d61 785f 6261 6e64 7769 6474 685f  t_max_bandwidth_
-00003810: 696e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  in is not None:.
-00003820: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00003830: 6c74 5b27 436c 6965 6e74 496e 7465 726e  lt['ClientIntern
-00003840: 6574 4d61 7842 616e 6477 6964 7468 496e  etMaxBandwidthIn
-00003850: 275d 203d 2073 656c 662e 636c 6965 6e74  '] = self.client
-00003860: 5f69 6e74 6572 6e65 745f 6d61 785f 6261  _internet_max_ba
-00003870: 6e64 7769 6474 685f 696e 0a20 2020 2020  ndwidth_in.     
-00003880: 2020 2069 6620 7365 6c66 2e63 6c69 656e     if self.clien
-00003890: 745f 696e 7465 726e 6574 5f6d 6178 5f62  t_internet_max_b
-000038a0: 616e 6477 6964 7468 5f6f 7574 2069 7320  andwidth_out is 
-000038b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000038c0: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
-000038d0: 6965 6e74 496e 7465 726e 6574 4d61 7842  ientInternetMaxB
-000038e0: 616e 6477 6964 7468 4f75 7427 5d20 3d20  andwidthOut'] = 
-000038f0: 7365 6c66 2e63 6c69 656e 745f 696e 7465  self.client_inte
-00003900: 726e 6574 5f6d 6178 5f62 616e 6477 6964  rnet_max_bandwid
-00003910: 7468 5f6f 7574 0a20 2020 2020 2020 2069  th_out.        i
-00003920: 6620 7365 6c66 2e63 6c69 656e 745f 7061  f self.client_pa
-00003930: 7373 776f 7264 2069 7320 6e6f 7420 4e6f  ssword is not No
-00003940: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00003950: 7265 7375 6c74 5b27 436c 6965 6e74 5061  result['ClientPa
-00003960: 7373 776f 7264 275d 203d 2073 656c 662e  ssword'] = self.
-00003970: 636c 6965 6e74 5f70 6173 7377 6f72 640a  client_password.
-00003980: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003990: 636c 6965 6e74 5f73 6563 7572 6974 795f  client_security_
-000039a0: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
-000039b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000039c0: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-000039d0: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
-000039e0: 5d20 3d20 7365 6c66 2e63 6c69 656e 745f  ] = self.client_
-000039f0: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
-00003a00: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00003a10: 662e 636c 6965 6e74 5f73 7973 7465 6d5f  f.client_system_
-00003a20: 6469 736b 5f63 6174 6567 6f72 7920 6973  disk_category is
-00003a30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00003a40: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
-00003a50: 6c69 656e 7453 7973 7465 6d44 6973 6b43  lientSystemDiskC
-00003a60: 6174 6567 6f72 7927 5d20 3d20 7365 6c66  ategory'] = self
-00003a70: 2e63 6c69 656e 745f 7379 7374 656d 5f64  .client_system_d
-00003a80: 6973 6b5f 6361 7465 676f 7279 0a20 2020  isk_category.   
-00003a90: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
-00003aa0: 656e 745f 7379 7374 656d 5f64 6973 6b5f  ent_system_disk_
-00003ab0: 7369 7a65 2069 7320 6e6f 7420 4e6f 6e65  size is not None
-00003ac0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00003ad0: 7375 6c74 5b27 436c 6965 6e74 5379 7374  sult['ClientSyst
-00003ae0: 656d 4469 736b 5369 7a65 275d 203d 2073  emDiskSize'] = s
-00003af0: 656c 662e 636c 6965 6e74 5f73 7973 7465  elf.client_syste
-00003b00: 6d5f 6469 736b 5f73 697a 650a 2020 2020  m_disk_size.    
-00003b10: 2020 2020 6966 2073 656c 662e 636c 6965      if self.clie
-00003b20: 6e74 5f74 6f6b 656e 2069 7320 6e6f 7420  nt_token is not 
-00003b30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003b40: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-00003b50: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e63  Token'] = self.c
-00003b60: 6c69 656e 745f 746f 6b65 6e0a 2020 2020  lient_token.    
-00003b70: 2020 2020 6966 2073 656c 662e 636c 6965      if self.clie
-00003b80: 6e74 5f76 7377 6974 6368 5f69 6420 6973  nt_vswitch_id is
-00003b90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00003ba0: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
-00003bb0: 6c69 656e 7456 5377 6974 6368 4964 275d  lientVSwitchId']
-00003bc0: 203d 2073 656c 662e 636c 6965 6e74 5f76   = self.client_v
-00003bd0: 7377 6974 6368 5f69 640a 2020 2020 2020  switch_id.      
-00003be0: 2020 6966 2073 656c 662e 636c 6965 6e74    if self.client
-00003bf0: 5f7a 6f6e 655f 6964 2069 7320 6e6f 7420  _zone_id is not 
-00003c00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003c10: 2020 7265 7375 6c74 5b27 436c 6965 6e74    result['Client
-00003c20: 5a6f 6e65 4964 275d 203d 2073 656c 662e  ZoneId'] = self.
-00003c30: 636c 6965 6e74 5f7a 6f6e 655f 6964 0a20  client_zone_id. 
-00003c40: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-00003c50: 6169 5f69 6e73 7461 6e63 655f 7479 7065  ai_instance_type
-00003c60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00003c70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00003c80: 5b27 4561 6949 6e73 7461 6e63 6554 7970  ['EaiInstanceTyp
-00003c90: 6527 5d20 3d20 7365 6c66 2e65 6169 5f69  e'] = self.eai_i
-00003ca0: 6e73 7461 6e63 655f 7479 7065 0a20 2020  nstance_type.   
-00003cb0: 2020 2020 2069 6620 7365 6c66 2e69 6e73       if self.ins
-00003cc0: 7461 6e63 655f 6e61 6d65 2069 7320 6e6f  tance_name is no
-00003cd0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00003ce0: 2020 2020 7265 7375 6c74 5b27 496e 7374      result['Inst
-00003cf0: 616e 6365 4e61 6d65 275d 203d 2073 656c  anceName'] = sel
-00003d00: 662e 696e 7374 616e 6365 5f6e 616d 650a  f.instance_name.
-00003d10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003d20: 7265 6769 6f6e 5f69 6420 6973 206e 6f74  region_id is not
-00003d30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00003d40: 2020 2072 6573 756c 745b 2752 6567 696f     result['Regio
-00003d50: 6e49 6427 5d20 3d20 7365 6c66 2e72 6567  nId'] = self.reg
-00003d60: 696f 6e5f 6964 0a20 2020 2020 2020 2069  ion_id.        i
-00003d70: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
-00003d80: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
-00003d90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003da0: 2020 7265 7375 6c74 5b27 5265 736f 7572    result['Resour
-00003db0: 6365 4772 6f75 7049 6427 5d20 3d20 7365  ceGroupId'] = se
-00003dc0: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
-00003dd0: 705f 6964 0a20 2020 2020 2020 2072 6574  p_id.        ret
-00003de0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00003df0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00003e00: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-00003e10: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00003e20: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-00003e30: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
-00003e40: 6965 6e74 496d 6167 6549 6427 2920 6973  ientImageId') is
-00003e50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00003e60: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
-00003e70: 6e74 5f69 6d61 6765 5f69 6420 3d20 6d2e  nt_image_id = m.
-00003e80: 6765 7428 2743 6c69 656e 7449 6d61 6765  get('ClientImage
-00003e90: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-00003ea0: 6d2e 6765 7428 2743 6c69 656e 7449 6e73  m.get('ClientIns
-00003eb0: 7461 6e63 654e 616d 6527 2920 6973 206e  tanceName') is n
-00003ec0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00003ed0: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-00003ee0: 5f69 6e73 7461 6e63 655f 6e61 6d65 203d  _instance_name =
-00003ef0: 206d 2e67 6574 2827 436c 6965 6e74 496e   m.get('ClientIn
-00003f00: 7374 616e 6365 4e61 6d65 2729 0a20 2020  stanceName').   
-00003f10: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
-00003f20: 6c69 656e 7449 6e73 7461 6e63 6554 7970  lientInstanceTyp
-00003f30: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00003f40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003f50: 662e 636c 6965 6e74 5f69 6e73 7461 6e63  f.client_instanc
-00003f60: 655f 7479 7065 203d 206d 2e67 6574 2827  e_type = m.get('
-00003f70: 436c 6965 6e74 496e 7374 616e 6365 5479  ClientInstanceTy
-00003f80: 7065 2729 0a20 2020 2020 2020 2069 6620  pe').        if 
-00003f90: 6d2e 6765 7428 2743 6c69 656e 7449 6e74  m.get('ClientInt
-00003fa0: 6572 6e65 744d 6178 4261 6e64 7769 6474  ernetMaxBandwidt
-00003fb0: 6849 6e27 2920 6973 206e 6f74 204e 6f6e  hIn') is not Non
-00003fc0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00003fd0: 656c 662e 636c 6965 6e74 5f69 6e74 6572  elf.client_inter
-00003fe0: 6e65 745f 6d61 785f 6261 6e64 7769 6474  net_max_bandwidt
-00003ff0: 685f 696e 203d 206d 2e67 6574 2827 436c  h_in = m.get('Cl
-00004000: 6965 6e74 496e 7465 726e 6574 4d61 7842  ientInternetMaxB
-00004010: 616e 6477 6964 7468 496e 2729 0a20 2020  andwidthIn').   
-00004020: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
-00004030: 6c69 656e 7449 6e74 6572 6e65 744d 6178  lientInternetMax
-00004040: 4261 6e64 7769 6474 684f 7574 2729 2069  BandwidthOut') i
-00004050: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00004060: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-00004070: 656e 745f 696e 7465 726e 6574 5f6d 6178  ent_internet_max
-00004080: 5f62 616e 6477 6964 7468 5f6f 7574 203d  _bandwidth_out =
-00004090: 206d 2e67 6574 2827 436c 6965 6e74 496e   m.get('ClientIn
-000040a0: 7465 726e 6574 4d61 7842 616e 6477 6964  ternetMaxBandwid
-000040b0: 7468 4f75 7427 290a 2020 2020 2020 2020  thOut').        
-000040c0: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
-000040d0: 5061 7373 776f 7264 2729 2069 7320 6e6f  Password') is no
-000040e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000040f0: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
-00004100: 7061 7373 776f 7264 203d 206d 2e67 6574  password = m.get
-00004110: 2827 436c 6965 6e74 5061 7373 776f 7264  ('ClientPassword
-00004120: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00004130: 6765 7428 2743 6c69 656e 7453 6563 7572  get('ClientSecur
-00004140: 6974 7947 726f 7570 4964 2729 2069 7320  ityGroupId') is 
-00004150: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00004160: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-00004170: 745f 7365 6375 7269 7479 5f67 726f 7570  t_security_group
-00004180: 5f69 6420 3d20 6d2e 6765 7428 2743 6c69  _id = m.get('Cli
-00004190: 656e 7453 6563 7572 6974 7947 726f 7570  entSecurityGroup
-000041a0: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-000041b0: 6d2e 6765 7428 2743 6c69 656e 7453 7973  m.get('ClientSys
-000041c0: 7465 6d44 6973 6b43 6174 6567 6f72 7927  temDiskCategory'
-000041d0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000041e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000041f0: 636c 6965 6e74 5f73 7973 7465 6d5f 6469  client_system_di
-00004200: 736b 5f63 6174 6567 6f72 7920 3d20 6d2e  sk_category = m.
-00004210: 6765 7428 2743 6c69 656e 7453 7973 7465  get('ClientSyste
-00004220: 6d44 6973 6b43 6174 6567 6f72 7927 290a  mDiskCategory').
-00004230: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00004240: 2827 436c 6965 6e74 5379 7374 656d 4469  ('ClientSystemDi
-00004250: 736b 5369 7a65 2729 2069 7320 6e6f 7420  skSize') is not 
-00004260: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00004270: 2020 7365 6c66 2e63 6c69 656e 745f 7379    self.client_sy
-00004280: 7374 656d 5f64 6973 6b5f 7369 7a65 203d  stem_disk_size =
-00004290: 206d 2e67 6574 2827 436c 6965 6e74 5379   m.get('ClientSy
-000042a0: 7374 656d 4469 736b 5369 7a65 2729 0a20  stemDiskSize'). 
-000042b0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000042c0: 2743 6c69 656e 7454 6f6b 656e 2729 2069  'ClientToken') i
-000042d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000042e0: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-000042f0: 656e 745f 746f 6b65 6e20 3d20 6d2e 6765  ent_token = m.ge
-00004300: 7428 2743 6c69 656e 7454 6f6b 656e 2729  t('ClientToken')
-00004310: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00004320: 7428 2743 6c69 656e 7456 5377 6974 6368  t('ClientVSwitch
-00004330: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00004340: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00004350: 6c66 2e63 6c69 656e 745f 7673 7769 7463  lf.client_vswitc
-00004360: 685f 6964 203d 206d 2e67 6574 2827 436c  h_id = m.get('Cl
-00004370: 6965 6e74 5653 7769 7463 6849 6427 290a  ientVSwitchId').
-00004380: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00004390: 2827 436c 6965 6e74 5a6f 6e65 4964 2729  ('ClientZoneId')
-000043a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000043b0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000043c0: 6c69 656e 745f 7a6f 6e65 5f69 6420 3d20  lient_zone_id = 
-000043d0: 6d2e 6765 7428 2743 6c69 656e 745a 6f6e  m.get('ClientZon
-000043e0: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
-000043f0: 206d 2e67 6574 2827 4561 6949 6e73 7461   m.get('EaiInsta
-00004400: 6e63 6554 7970 6527 2920 6973 206e 6f74  nceType') is not
-00004410: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00004420: 2020 2073 656c 662e 6561 695f 696e 7374     self.eai_inst
-00004430: 616e 6365 5f74 7970 6520 3d20 6d2e 6765  ance_type = m.ge
-00004440: 7428 2745 6169 496e 7374 616e 6365 5479  t('EaiInstanceTy
-00004450: 7065 2729 0a20 2020 2020 2020 2069 6620  pe').        if 
-00004460: 6d2e 6765 7428 2749 6e73 7461 6e63 654e  m.get('InstanceN
-00004470: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
-00004480: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00004490: 656c 662e 696e 7374 616e 6365 5f6e 616d  elf.instance_nam
-000044a0: 6520 3d20 6d2e 6765 7428 2749 6e73 7461  e = m.get('Insta
-000044b0: 6e63 654e 616d 6527 290a 2020 2020 2020  nceName').      
-000044c0: 2020 6966 206d 2e67 6574 2827 5265 6769    if m.get('Regi
-000044d0: 6f6e 4964 2729 2069 7320 6e6f 7420 4e6f  onId') is not No
-000044e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000044f0: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
-00004500: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
-00004510: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00004520: 6765 7428 2752 6573 6f75 7263 6547 726f  get('ResourceGro
-00004530: 7570 4964 2729 2069 7320 6e6f 7420 4e6f  upId') is not No
-00004540: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00004550: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
-00004560: 6f75 705f 6964 203d 206d 2e67 6574 2827  oup_id = m.get('
-00004570: 5265 736f 7572 6365 4772 6f75 7049 6427  ResourceGroupId'
-00004580: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00004590: 2073 656c 660a 0a0a 636c 6173 7320 4372   self...class Cr
-000045a0: 6561 7465 4561 6941 6c6c 5265 7370 6f6e  eateEaiAllRespon
-000045b0: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
-000045c0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000045d0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-000045e0: 2c0a 2020 2020 2020 2020 636c 6965 6e74  ,.        client
-000045f0: 5f69 6e73 7461 6e63 655f 6964 3a20 7374  _instance_id: st
-00004600: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00004610: 2020 656c 6173 7469 635f 6163 6365 6c65    elastic_accele
-00004620: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-00004630: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00004640: 2020 2020 2020 2072 6571 7565 7374 5f69         request_i
-00004650: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00004660: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-00004670: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
-00004680: 6365 5f69 6420 3d20 636c 6965 6e74 5f69  ce_id = client_i
-00004690: 6e73 7461 6e63 655f 6964 0a20 2020 2020  nstance_id.     
-000046a0: 2020 2073 656c 662e 656c 6173 7469 635f     self.elastic_
-000046b0: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
-000046c0: 616e 6365 5f69 6420 3d20 656c 6173 7469  ance_id = elasti
-000046d0: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
-000046e0: 7374 616e 6365 5f69 640a 2020 2020 2020  stance_id.      
-000046f0: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
-00004700: 6420 3d20 7265 7175 6573 745f 6964 0a0a  d = request_id..
-00004710: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00004720: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00004730: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-00004740: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00004750: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00004760: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-00004770: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00004780: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00004790: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-000047a0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-000047b0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-000047c0: 2020 6966 2073 656c 662e 636c 6965 6e74    if self.client
-000047d0: 5f69 6e73 7461 6e63 655f 6964 2069 7320  _instance_id is 
-000047e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000047f0: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
-00004800: 6965 6e74 496e 7374 616e 6365 4964 275d  ientInstanceId']
-00004810: 203d 2073 656c 662e 636c 6965 6e74 5f69   = self.client_i
-00004820: 6e73 7461 6e63 655f 6964 0a20 2020 2020  nstance_id.     
-00004830: 2020 2069 6620 7365 6c66 2e65 6c61 7374     if self.elast
-00004840: 6963 5f61 6363 656c 6572 6174 6564 5f69  ic_accelerated_i
-00004850: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
-00004860: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00004870: 2020 2020 7265 7375 6c74 5b27 456c 6173      result['Elas
-00004880: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
-00004890: 7374 616e 6365 4964 275d 203d 2073 656c  stanceId'] = sel
-000048a0: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-000048b0: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-000048c0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-000048d0: 662e 7265 7175 6573 745f 6964 2069 7320  f.request_id is 
-000048e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000048f0: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-00004900: 7175 6573 7449 6427 5d20 3d20 7365 6c66  questId'] = self
-00004910: 2e72 6571 7565 7374 5f69 640a 2020 2020  .request_id.    
-00004920: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00004930: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00004940: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00004950: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00004960: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00004970: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00004980: 6765 7428 2743 6c69 656e 7449 6e73 7461  get('ClientInsta
-00004990: 6e63 6549 6427 2920 6973 206e 6f74 204e  nceId') is not N
-000049a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000049b0: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
-000049c0: 7461 6e63 655f 6964 203d 206d 2e67 6574  tance_id = m.get
-000049d0: 2827 436c 6965 6e74 496e 7374 616e 6365  ('ClientInstance
-000049e0: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-000049f0: 6d2e 6765 7428 2745 6c61 7374 6963 4163  m.get('ElasticAc
-00004a00: 6365 6c65 7261 7465 6449 6e73 7461 6e63  celeratedInstanc
-00004a10: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
-00004a20: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00004a30: 656c 662e 656c 6173 7469 635f 6163 6365  elf.elastic_acce
-00004a40: 6c65 7261 7465 645f 696e 7374 616e 6365  lerated_instance
-00004a50: 5f69 6420 3d20 6d2e 6765 7428 2745 6c61  _id = m.get('Ela
-00004a60: 7374 6963 4163 6365 6c65 7261 7465 6449  sticAcceleratedI
-00004a70: 6e73 7461 6e63 6549 6427 290a 2020 2020  nstanceId').    
-00004a80: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-00004a90: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
-00004aa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00004ab0: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-00004ac0: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
-00004ad0: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
-00004ae0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00004af0: 6173 7320 4372 6561 7465 4561 6941 6c6c  ass CreateEaiAll
-00004b00: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-00004b10: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00004b20: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00004b30: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-00004b40: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-00004b50: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00004b60: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-00004b70: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-00004b80: 2020 2020 2062 6f64 793a 2043 7265 6174       body: Creat
-00004b90: 6545 6169 416c 6c52 6573 706f 6e73 6542  eEaiAllResponseB
-00004ba0: 6f64 7920 3d20 4e6f 6e65 2c0a 2020 2020  ody = None,.    
-00004bb0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00004bc0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-00004bd0: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-00004be0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-00004bf0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-00004c00: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-00004c10: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-00004c20: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00004c30: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-00004c40: 5f72 6571 7569 7265 6428 7365 6c66 2e68  _required(self.h
-00004c50: 6561 6465 7273 2c20 2768 6561 6465 7273  eaders, 'headers
-00004c60: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00004c70: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-00004c80: 6428 7365 6c66 2e73 7461 7475 735f 636f  d(self.status_co
-00004c90: 6465 2c20 2773 7461 7475 735f 636f 6465  de, 'status_code
-00004ca0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00004cb0: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-00004cc0: 6428 7365 6c66 2e62 6f64 792c 2027 626f  d(self.body, 'bo
-00004cd0: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
-00004ce0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-00004cf0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00004d00: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-00004d10: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-00004d20: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-00004d30: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-00004d40: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-00004d50: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-00004d60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00004d70: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-00004d80: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-00004d90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00004da0: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
-00004db0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00004dc0: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
-00004dd0: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
-00004de0: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
-00004df0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
-00004e00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00004e10: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00004e20: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
-00004e30: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
-00004e40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00004e50: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
-00004e60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00004e70: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
-00004e80: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
-00004e90: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00004ea0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-00004eb0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-00004ec0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
-00004ed0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00004ee0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-00004ef0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-00004f00: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-00004f10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00004f20: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-00004f30: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-00004f40: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00004f50: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-00004f60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00004f70: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00004f80: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-00004f90: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-00004fa0: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-00004fb0: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-00004fc0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-00004fd0: 656d 705f 6d6f 6465 6c20 3d20 4372 6561  emp_model = Crea
-00004fe0: 7465 4561 6941 6c6c 5265 7370 6f6e 7365  teEaiAllResponse
-00004ff0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
-00005000: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-00005010: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-00005020: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-00005030: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00005040: 660a 0a0a 636c 6173 7320 4372 6561 7465  f...class Create
-00005050: 4561 6945 6369 5265 7175 6573 7445 6369  EaiEciRequestEci
-00005060: 436f 6e74 6169 6e65 7228 5465 614d 6f64  Container(TeaMod
-00005070: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-00005080: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00005090: 656c 662c 0a20 2020 2020 2020 2061 7267  elf,.        arg
-000050a0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000050b0: 2020 2020 2020 636f 6d6d 616e 643a 2073        command: s
-000050c0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000050d0: 2020 2069 6d61 6765 3a20 7374 7220 3d20     image: str = 
-000050e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6e61  None,.        na
-000050f0: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
-00005100: 2020 2020 2020 2020 766f 6c75 6d65 733a          volumes:
-00005110: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00005120: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-00005130: 2e61 7267 203d 2061 7267 0a20 2020 2020  .arg = arg.     
-00005140: 2020 2073 656c 662e 636f 6d6d 616e 6420     self.command 
-00005150: 3d20 636f 6d6d 616e 640a 2020 2020 2020  = command.      
-00005160: 2020 7365 6c66 2e69 6d61 6765 203d 2069    self.image = i
-00005170: 6d61 6765 0a20 2020 2020 2020 2073 656c  mage.        sel
-00005180: 662e 6e61 6d65 203d 206e 616d 650a 2020  f.name = name.  
-00005190: 2020 2020 2020 7365 6c66 2e76 6f6c 756d        self.volum
-000051a0: 6573 203d 2076 6f6c 756d 6573 0a0a 2020  es = volumes..  
-000051b0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-000051c0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-000051d0: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-000051e0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-000051f0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-00005200: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00005210: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-00005220: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00005230: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-00005240: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00005250: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00005260: 6966 2073 656c 662e 6172 6720 6973 206e  if self.arg is n
-00005270: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00005280: 2020 2020 2072 6573 756c 745b 2741 7267       result['Arg
-00005290: 275d 203d 2073 656c 662e 6172 670a 2020  '] = self.arg.  
-000052a0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-000052b0: 6d6d 616e 6420 6973 206e 6f74 204e 6f6e  mmand is not Non
-000052c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000052d0: 6573 756c 745b 2743 6f6d 6d61 6e64 275d  esult['Command']
-000052e0: 203d 2073 656c 662e 636f 6d6d 616e 640a   = self.command.
-000052f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00005300: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
-00005310: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00005320: 6573 756c 745b 2749 6d61 6765 275d 203d  esult['Image'] =
-00005330: 2073 656c 662e 696d 6167 650a 2020 2020   self.image.    
-00005340: 2020 2020 6966 2073 656c 662e 6e61 6d65      if self.name
-00005350: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00005360: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00005370: 5b27 4e61 6d65 275d 203d 2073 656c 662e  ['Name'] = self.
-00005380: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
-00005390: 7365 6c66 2e76 6f6c 756d 6573 2069 7320  self.volumes is 
-000053a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000053b0: 2020 2020 2020 7265 7375 6c74 5b27 566f        result['Vo
-000053c0: 6c75 6d65 7327 5d20 3d20 7365 6c66 2e76  lumes'] = self.v
-000053d0: 6f6c 756d 6573 0a20 2020 2020 2020 2072  olumes.        r
-000053e0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-000053f0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-00005400: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-00005410: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-00005420: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-00005430: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00005440: 4172 6727 2920 6973 206e 6f74 204e 6f6e  Arg') is not Non
-00005450: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00005460: 656c 662e 6172 6720 3d20 6d2e 6765 7428  elf.arg = m.get(
-00005470: 2741 7267 2729 0a20 2020 2020 2020 2069  'Arg').        i
-00005480: 6620 6d2e 6765 7428 2743 6f6d 6d61 6e64  f m.get('Command
-00005490: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000054a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000054b0: 2e63 6f6d 6d61 6e64 203d 206d 2e67 6574  .command = m.get
-000054c0: 2827 436f 6d6d 616e 6427 290a 2020 2020  ('Command').    
-000054d0: 2020 2020 6966 206d 2e67 6574 2827 496d      if m.get('Im
-000054e0: 6167 6527 2920 6973 206e 6f74 204e 6f6e  age') is not Non
-000054f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00005500: 656c 662e 696d 6167 6520 3d20 6d2e 6765  elf.image = m.ge
-00005510: 7428 2749 6d61 6765 2729 0a20 2020 2020  t('Image').     
-00005520: 2020 2069 6620 6d2e 6765 7428 274e 616d     if m.get('Nam
-00005530: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00005540: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005550: 662e 6e61 6d65 203d 206d 2e67 6574 2827  f.name = m.get('
-00005560: 4e61 6d65 2729 0a20 2020 2020 2020 2069  Name').        i
-00005570: 6620 6d2e 6765 7428 2756 6f6c 756d 6573  f m.get('Volumes
-00005580: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00005590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000055a0: 2e76 6f6c 756d 6573 203d 206d 2e67 6574  .volumes = m.get
-000055b0: 2827 566f 6c75 6d65 7327 290a 2020 2020  ('Volumes').    
-000055c0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-000055d0: 0a0a 636c 6173 7320 4372 6561 7465 4561  ..class CreateEa
-000055e0: 6945 6369 5265 7175 6573 7445 6369 2854  iEciRequestEci(T
-000055f0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-00005600: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-00005610: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00005620: 2020 636f 6e74 6169 6e65 723a 2043 7265    container: Cre
-00005630: 6174 6545 6169 4563 6952 6571 7565 7374  ateEaiEciRequest
-00005640: 4563 6943 6f6e 7461 696e 6572 203d 204e  EciContainer = N
-00005650: 6f6e 652c 0a20 2020 2020 2020 2065 6970  one,.        eip
-00005660: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-00005670: 0a20 2020 2020 2020 206e 616d 653a 2073  .        name: s
-00005680: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-00005690: 2020 2074 7970 653a 2073 7472 203d 204e     type: str = N
-000056a0: 6f6e 652c 0a20 2020 2020 2020 2076 6f6c  one,.        vol
-000056b0: 756d 653a 2073 7472 203d 204e 6f6e 652c  ume: str = None,
-000056c0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-000056d0: 7365 6c66 2e63 6f6e 7461 696e 6572 203d  self.container =
-000056e0: 2063 6f6e 7461 696e 6572 0a20 2020 2020   container.     
-000056f0: 2020 2073 656c 662e 6569 705f 6964 203d     self.eip_id =
-00005700: 2065 6970 5f69 640a 2020 2020 2020 2020   eip_id.        
-00005710: 7365 6c66 2e6e 616d 6520 3d20 6e61 6d65  self.name = name
-00005720: 0a20 2020 2020 2020 2073 656c 662e 7479  .        self.ty
-00005730: 7065 203d 2074 7970 650a 2020 2020 2020  pe = type.      
-00005740: 2020 7365 6c66 2e76 6f6c 756d 6520 3d20    self.volume = 
-00005750: 766f 6c75 6d65 0a0a 2020 2020 6465 6620  volume..    def 
-00005760: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-00005770: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00005780: 636f 6e74 6169 6e65 723a 0a20 2020 2020  container:.     
-00005790: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-000057a0: 6169 6e65 722e 7661 6c69 6461 7465 2829  ainer.validate()
-000057b0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-000057c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000057d0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-000057e0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-000057f0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00005800: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00005810: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-00005820: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-00005830: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00005840: 2073 656c 662e 636f 6e74 6169 6e65 7220   self.container 
-00005850: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00005860: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00005870: 2743 6f6e 7461 696e 6572 275d 203d 2073  'Container'] = s
-00005880: 656c 662e 636f 6e74 6169 6e65 722e 746f  elf.container.to
-00005890: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-000058a0: 6620 7365 6c66 2e65 6970 5f69 6420 6973  f self.eip_id is
-000058b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000058c0: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
-000058d0: 6970 4964 275d 203d 2073 656c 662e 6569  ipId'] = self.ei
-000058e0: 705f 6964 0a20 2020 2020 2020 2069 6620  p_id.        if 
-000058f0: 7365 6c66 2e6e 616d 6520 6973 206e 6f74  self.name is not
-00005900: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00005910: 2020 2072 6573 756c 745b 274e 616d 6527     result['Name'
-00005920: 5d20 3d20 7365 6c66 2e6e 616d 650a 2020  ] = self.name.  
-00005930: 2020 2020 2020 6966 2073 656c 662e 7479        if self.ty
-00005940: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
-00005950: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00005960: 6c74 5b27 5479 7065 275d 203d 2073 656c  lt['Type'] = sel
-00005970: 662e 7479 7065 0a20 2020 2020 2020 2069  f.type.        i
-00005980: 6620 7365 6c66 2e76 6f6c 756d 6520 6973  f self.volume is
-00005990: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000059a0: 2020 2020 2020 2072 6573 756c 745b 2756         result['V
-000059b0: 6f6c 756d 6527 5d20 3d20 7365 6c66 2e76  olume'] = self.v
-000059c0: 6f6c 756d 650a 2020 2020 2020 2020 7265  olume.        re
-000059d0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-000059e0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-000059f0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-00005a00: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-00005a10: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-00005a20: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
-00005a30: 6f6e 7461 696e 6572 2729 2069 7320 6e6f  ontainer') is no
-00005a40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00005a50: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-00005a60: 2043 7265 6174 6545 6169 4563 6952 6571   CreateEaiEciReq
-00005a70: 7565 7374 4563 6943 6f6e 7461 696e 6572  uestEciContainer
-00005a80: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00005a90: 656c 662e 636f 6e74 6169 6e65 7220 3d20  elf.container = 
-00005aa0: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-00005ab0: 6d61 7028 6d5b 2743 6f6e 7461 696e 6572  map(m['Container
-00005ac0: 275d 290a 2020 2020 2020 2020 6966 206d  ']).        if m
-00005ad0: 2e67 6574 2827 4569 7049 6427 2920 6973  .get('EipId') is
-00005ae0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00005af0: 2020 2020 2020 2073 656c 662e 6569 705f         self.eip_
-00005b00: 6964 203d 206d 2e67 6574 2827 4569 7049  id = m.get('EipI
-00005b10: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00005b20: 2e67 6574 2827 4e61 6d65 2729 2069 7320  .get('Name') is 
-00005b30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00005b40: 2020 2020 2020 7365 6c66 2e6e 616d 6520        self.name 
-00005b50: 3d20 6d2e 6765 7428 274e 616d 6527 290a  = m.get('Name').
-00005b60: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00005b70: 2827 5479 7065 2729 2069 7320 6e6f 7420  ('Type') is not 
-00005b80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00005b90: 2020 7365 6c66 2e74 7970 6520 3d20 6d2e    self.type = m.
-00005ba0: 6765 7428 2754 7970 6527 290a 2020 2020  get('Type').    
-00005bb0: 2020 2020 6966 206d 2e67 6574 2827 566f      if m.get('Vo
-00005bc0: 6c75 6d65 2729 2069 7320 6e6f 7420 4e6f  lume') is not No
-00005bd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00005be0: 7365 6c66 2e76 6f6c 756d 6520 3d20 6d2e  self.volume = m.
-00005bf0: 6765 7428 2756 6f6c 756d 6527 290a 2020  get('Volume').  
-00005c00: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00005c10: 660a 0a0a 636c 6173 7320 4372 6561 7465  f...class Create
-00005c20: 4561 6945 6369 5265 7175 6573 7428 5465  EaiEciRequest(Te
-00005c30: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00005c40: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00005c50: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00005c60: 2063 6c69 656e 745f 746f 6b65 6e3a 2073   client_token: s
-00005c70: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-00005c80: 2020 2065 6169 735f 6e61 6d65 3a20 7374     eais_name: st
-00005c90: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00005ca0: 2020 6561 6973 5f74 7970 653a 2073 7472    eais_type: str
-00005cb0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00005cc0: 2065 6369 3a20 4372 6561 7465 4561 6945   eci: CreateEaiE
-00005cd0: 6369 5265 7175 6573 7445 6369 203d 204e  ciRequestEci = N
-00005ce0: 6f6e 652c 0a20 2020 2020 2020 2072 6567  one,.        reg
-00005cf0: 696f 6e5f 6964 3a20 7374 7220 3d20 4e6f  ion_id: str = No
-00005d00: 6e65 2c0a 2020 2020 2020 2020 7265 736f  ne,.        reso
-00005d10: 7572 6365 5f67 726f 7570 5f69 643a 2073  urce_group_id: s
-00005d20: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-00005d30: 2020 2073 6563 7572 6974 795f 6772 6f75     security_grou
-00005d40: 705f 6964 3a20 7374 7220 3d20 4e6f 6e65  p_id: str = None
-00005d50: 2c0a 2020 2020 2020 2020 765f 7377 6974  ,.        v_swit
-00005d60: 6368 5f69 643a 2073 7472 203d 204e 6f6e  ch_id: str = Non
-00005d70: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00005d80: 2020 7365 6c66 2e63 6c69 656e 745f 746f    self.client_to
-00005d90: 6b65 6e20 3d20 636c 6965 6e74 5f74 6f6b  ken = client_tok
-00005da0: 656e 0a20 2020 2020 2020 2073 656c 662e  en.        self.
-00005db0: 6561 6973 5f6e 616d 6520 3d20 6561 6973  eais_name = eais
-00005dc0: 5f6e 616d 650a 2020 2020 2020 2020 7365  _name.        se
-00005dd0: 6c66 2e65 6169 735f 7479 7065 203d 2065  lf.eais_type = e
-00005de0: 6169 735f 7479 7065 0a20 2020 2020 2020  ais_type.       
-00005df0: 2073 656c 662e 6563 6920 3d20 6563 690a   self.eci = eci.
-00005e00: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
-00005e10: 696f 6e5f 6964 203d 2072 6567 696f 6e5f  ion_id = region_
-00005e20: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
-00005e30: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-00005e40: 6420 3d20 7265 736f 7572 6365 5f67 726f  d = resource_gro
-00005e50: 7570 5f69 640a 2020 2020 2020 2020 7365  up_id.        se
-00005e60: 6c66 2e73 6563 7572 6974 795f 6772 6f75  lf.security_grou
-00005e70: 705f 6964 203d 2073 6563 7572 6974 795f  p_id = security_
-00005e80: 6772 6f75 705f 6964 0a20 2020 2020 2020  group_id.       
-00005e90: 2073 656c 662e 765f 7377 6974 6368 5f69   self.v_switch_i
-00005ea0: 6420 3d20 765f 7377 6974 6368 5f69 640a  d = v_switch_id.
-00005eb0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00005ec0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00005ed0: 2069 6620 7365 6c66 2e65 6369 3a0a 2020   if self.eci:.  
-00005ee0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-00005ef0: 6369 2e76 616c 6964 6174 6528 290a 0a20  ci.validate().. 
-00005f00: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00005f10: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00005f20: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-00005f30: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00005f40: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00005f50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00005f60: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00005f70: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00005f80: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00005f90: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
-00005fa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00005fb0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00005fc0: 2743 6c69 656e 7454 6f6b 656e 275d 203d  'ClientToken'] =
-00005fd0: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
-00005fe0: 656e 0a20 2020 2020 2020 2069 6620 7365  en.        if se
-00005ff0: 6c66 2e65 6169 735f 6e61 6d65 2069 7320  lf.eais_name is 
-00006000: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00006010: 2020 2020 2020 7265 7375 6c74 5b27 4561        result['Ea
-00006020: 6973 4e61 6d65 275d 203d 2073 656c 662e  isName'] = self.
-00006030: 6561 6973 5f6e 616d 650a 2020 2020 2020  eais_name.      
-00006040: 2020 6966 2073 656c 662e 6561 6973 5f74    if self.eais_t
-00006050: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
-00006060: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00006070: 756c 745b 2745 6169 7354 7970 6527 5d20  ult['EaisType'] 
-00006080: 3d20 7365 6c66 2e65 6169 735f 7479 7065  = self.eais_type
-00006090: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000060a0: 2e65 6369 2069 7320 6e6f 7420 4e6f 6e65  .eci is not None
-000060b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000060c0: 7375 6c74 5b27 4563 6927 5d20 3d20 7365  sult['Eci'] = se
-000060d0: 6c66 2e65 6369 2e74 6f5f 6d61 7028 290a  lf.eci.to_map().
-000060e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000060f0: 7265 6769 6f6e 5f69 6420 6973 206e 6f74  region_id is not
-00006100: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006110: 2020 2072 6573 756c 745b 2752 6567 696f     result['Regio
-00006120: 6e49 6427 5d20 3d20 7365 6c66 2e72 6567  nId'] = self.reg
-00006130: 696f 6e5f 6964 0a20 2020 2020 2020 2069  ion_id.        i
-00006140: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
-00006150: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
-00006160: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00006170: 2020 7265 7375 6c74 5b27 5265 736f 7572    result['Resour
-00006180: 6365 4772 6f75 7049 6427 5d20 3d20 7365  ceGroupId'] = se
-00006190: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
-000061a0: 705f 6964 0a20 2020 2020 2020 2069 6620  p_id.        if 
-000061b0: 7365 6c66 2e73 6563 7572 6974 795f 6772  self.security_gr
-000061c0: 6f75 705f 6964 2069 7320 6e6f 7420 4e6f  oup_id is not No
-000061d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000061e0: 7265 7375 6c74 5b27 5365 6375 7269 7479  result['Security
-000061f0: 4772 6f75 7049 6427 5d20 3d20 7365 6c66  GroupId'] = self
-00006200: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
-00006210: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-00006220: 6c66 2e76 5f73 7769 7463 685f 6964 2069  lf.v_switch_id i
-00006230: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00006240: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00006250: 5653 7769 7463 6849 6427 5d20 3d20 7365  VSwitchId'] = se
-00006260: 6c66 2e76 5f73 7769 7463 685f 6964 0a20  lf.v_switch_id. 
-00006270: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00006280: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00006290: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-000062a0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-000062b0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-000062c0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000062d0: 206d 2e67 6574 2827 436c 6965 6e74 546f   m.get('ClientTo
-000062e0: 6b65 6e27 2920 6973 206e 6f74 204e 6f6e  ken') is not Non
-000062f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00006300: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
-00006310: 203d 206d 2e67 6574 2827 436c 6965 6e74   = m.get('Client
-00006320: 546f 6b65 6e27 290a 2020 2020 2020 2020  Token').        
-00006330: 6966 206d 2e67 6574 2827 4561 6973 4e61  if m.get('EaisNa
-00006340: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
-00006350: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00006360: 6c66 2e65 6169 735f 6e61 6d65 203d 206d  lf.eais_name = m
-00006370: 2e67 6574 2827 4561 6973 4e61 6d65 2729  .get('EaisName')
-00006380: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00006390: 7428 2745 6169 7354 7970 6527 2920 6973  t('EaisType') is
-000063a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000063b0: 2020 2020 2020 2073 656c 662e 6561 6973         self.eais
-000063c0: 5f74 7970 6520 3d20 6d2e 6765 7428 2745  _type = m.get('E
-000063d0: 6169 7354 7970 6527 290a 2020 2020 2020  aisType').      
-000063e0: 2020 6966 206d 2e67 6574 2827 4563 6927    if m.get('Eci'
-000063f0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00006400: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-00006410: 6d6f 6465 6c20 3d20 4372 6561 7465 4561  model = CreateEa
-00006420: 6945 6369 5265 7175 6573 7445 6369 2829  iEciRequestEci()
-00006430: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006440: 662e 6563 6920 3d20 7465 6d70 5f6d 6f64  f.eci = temp_mod
-00006450: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2745  el.from_map(m['E
-00006460: 6369 275d 290a 2020 2020 2020 2020 6966  ci']).        if
-00006470: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
-00006480: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00006490: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000064a0: 2e72 6567 696f 6e5f 6964 203d 206d 2e67  .region_id = m.g
-000064b0: 6574 2827 5265 6769 6f6e 4964 2729 0a20  et('RegionId'). 
-000064c0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000064d0: 2752 6573 6f75 7263 6547 726f 7570 4964  'ResourceGroupId
-000064e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000064f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006500: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
-00006510: 6964 203d 206d 2e67 6574 2827 5265 736f  id = m.get('Reso
-00006520: 7572 6365 4772 6f75 7049 6427 290a 2020  urceGroupId').  
-00006530: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00006540: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
-00006550: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00006560: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006570: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
-00006580: 6420 3d20 6d2e 6765 7428 2753 6563 7572  d = m.get('Secur
-00006590: 6974 7947 726f 7570 4964 2729 0a20 2020  ityGroupId').   
-000065a0: 2020 2020 2069 6620 6d2e 6765 7428 2756       if m.get('V
-000065b0: 5377 6974 6368 4964 2729 2069 7320 6e6f  SwitchId') is no
-000065c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000065d0: 2020 2020 7365 6c66 2e76 5f73 7769 7463      self.v_switc
-000065e0: 685f 6964 203d 206d 2e67 6574 2827 5653  h_id = m.get('VS
-000065f0: 7769 7463 6849 6427 290a 2020 2020 2020  witchId').      
-00006600: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00006610: 636c 6173 7320 4372 6561 7465 4561 6945  class CreateEaiE
-00006620: 6369 5368 7269 6e6b 5265 7175 6573 7428  ciShrinkRequest(
-00006630: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00006640: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00006650: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00006660: 2020 2063 6c69 656e 745f 746f 6b65 6e3a     client_token:
-00006670: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00006680: 2020 2020 2065 6169 735f 6e61 6d65 3a20       eais_name: 
-00006690: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000066a0: 2020 2020 6561 6973 5f74 7970 653a 2073      eais_type: s
-000066b0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000066c0: 2020 2065 6369 5f73 6872 696e 6b3a 2073     eci_shrink: s
-000066d0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000066e0: 2020 2072 6567 696f 6e5f 6964 3a20 7374     region_id: st
-000066f0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00006700: 2020 7265 736f 7572 6365 5f67 726f 7570    resource_group
-00006710: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-00006720: 0a20 2020 2020 2020 2073 6563 7572 6974  .        securit
-00006730: 795f 6772 6f75 705f 6964 3a20 7374 7220  y_group_id: str 
-00006740: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00006750: 765f 7377 6974 6368 5f69 643a 2073 7472  v_switch_id: str
-00006760: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-00006770: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-00006780: 656e 745f 746f 6b65 6e20 3d20 636c 6965  ent_token = clie
-00006790: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
-000067a0: 2073 656c 662e 6561 6973 5f6e 616d 6520   self.eais_name 
-000067b0: 3d20 6561 6973 5f6e 616d 650a 2020 2020  = eais_name.    
-000067c0: 2020 2020 7365 6c66 2e65 6169 735f 7479      self.eais_ty
-000067d0: 7065 203d 2065 6169 735f 7479 7065 0a20  pe = eais_type. 
-000067e0: 2020 2020 2020 2073 656c 662e 6563 695f         self.eci_
-000067f0: 7368 7269 6e6b 203d 2065 6369 5f73 6872  shrink = eci_shr
-00006800: 696e 6b0a 2020 2020 2020 2020 7365 6c66  ink.        self
-00006810: 2e72 6567 696f 6e5f 6964 203d 2072 6567  .region_id = reg
-00006820: 696f 6e5f 6964 0a20 2020 2020 2020 2073  ion_id.        s
-00006830: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
-00006840: 7570 5f69 6420 3d20 7265 736f 7572 6365  up_id = resource
-00006850: 5f67 726f 7570 5f69 640a 2020 2020 2020  _group_id.      
-00006860: 2020 7365 6c66 2e73 6563 7572 6974 795f    self.security_
-00006870: 6772 6f75 705f 6964 203d 2073 6563 7572  group_id = secur
-00006880: 6974 795f 6772 6f75 705f 6964 0a20 2020  ity_group_id.   
-00006890: 2020 2020 2073 656c 662e 765f 7377 6974       self.v_swit
-000068a0: 6368 5f69 6420 3d20 765f 7377 6974 6368  ch_id = v_switch
-000068b0: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
-000068c0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-000068d0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000068e0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-000068f0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00006900: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-00006910: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00006920: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00006930: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00006940: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00006950: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00006960: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00006970: 6c69 656e 745f 746f 6b65 6e20 6973 206e  lient_token is n
-00006980: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00006990: 2020 2020 2072 6573 756c 745b 2743 6c69       result['Cli
-000069a0: 656e 7454 6f6b 656e 275d 203d 2073 656c  entToken'] = sel
-000069b0: 662e 636c 6965 6e74 5f74 6f6b 656e 0a20  f.client_token. 
-000069c0: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-000069d0: 6169 735f 6e61 6d65 2069 7320 6e6f 7420  ais_name is not 
-000069e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000069f0: 2020 7265 7375 6c74 5b27 4561 6973 4e61    result['EaisNa
-00006a00: 6d65 275d 203d 2073 656c 662e 6561 6973  me'] = self.eais
-00006a10: 5f6e 616d 650a 2020 2020 2020 2020 6966  _name.        if
-00006a20: 2073 656c 662e 6561 6973 5f74 7970 6520   self.eais_type 
-00006a30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00006a40: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00006a50: 2745 6169 7354 7970 6527 5d20 3d20 7365  'EaisType'] = se
-00006a60: 6c66 2e65 6169 735f 7479 7065 0a20 2020  lf.eais_type.   
-00006a70: 2020 2020 2069 6620 7365 6c66 2e65 6369       if self.eci
-00006a80: 5f73 6872 696e 6b20 6973 206e 6f74 204e  _shrink is not N
-00006a90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00006aa0: 2072 6573 756c 745b 2745 6369 275d 203d   result['Eci'] =
-00006ab0: 2073 656c 662e 6563 695f 7368 7269 6e6b   self.eci_shrink
-00006ac0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00006ad0: 2e72 6567 696f 6e5f 6964 2069 7320 6e6f  .region_id is no
-00006ae0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00006af0: 2020 2020 7265 7375 6c74 5b27 5265 6769      result['Regi
-00006b00: 6f6e 4964 275d 203d 2073 656c 662e 7265  onId'] = self.re
-00006b10: 6769 6f6e 5f69 640a 2020 2020 2020 2020  gion_id.        
-00006b20: 6966 2073 656c 662e 7265 736f 7572 6365  if self.resource
-00006b30: 5f67 726f 7570 5f69 6420 6973 206e 6f74  _group_id is not
-00006b40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006b50: 2020 2072 6573 756c 745b 2752 6573 6f75     result['Resou
-00006b60: 7263 6547 726f 7570 4964 275d 203d 2073  rceGroupId'] = s
-00006b70: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
-00006b80: 7570 5f69 640a 2020 2020 2020 2020 6966  up_id.        if
-00006b90: 2073 656c 662e 7365 6375 7269 7479 5f67   self.security_g
-00006ba0: 726f 7570 5f69 6420 6973 206e 6f74 204e  roup_id is not N
-00006bb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00006bc0: 2072 6573 756c 745b 2753 6563 7572 6974   result['Securit
-00006bd0: 7947 726f 7570 4964 275d 203d 2073 656c  yGroupId'] = sel
-00006be0: 662e 7365 6375 7269 7479 5f67 726f 7570  f.security_group
-00006bf0: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-00006c00: 656c 662e 765f 7377 6974 6368 5f69 6420  elf.v_switch_id 
-00006c10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00006c20: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00006c30: 2756 5377 6974 6368 4964 275d 203d 2073  'VSwitchId'] = s
-00006c40: 656c 662e 765f 7377 6974 6368 5f69 640a  elf.v_switch_id.
-00006c50: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00006c60: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00006c70: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-00006c80: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-00006c90: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00006ca0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00006cb0: 6620 6d2e 6765 7428 2743 6c69 656e 7454  f m.get('ClientT
-00006cc0: 6f6b 656e 2729 2069 7320 6e6f 7420 4e6f  oken') is not No
-00006cd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00006ce0: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
-00006cf0: 6e20 3d20 6d2e 6765 7428 2743 6c69 656e  n = m.get('Clien
-00006d00: 7454 6f6b 656e 2729 0a20 2020 2020 2020  tToken').       
-00006d10: 2069 6620 6d2e 6765 7428 2745 6169 734e   if m.get('EaisN
-00006d20: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
-00006d30: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00006d40: 656c 662e 6561 6973 5f6e 616d 6520 3d20  elf.eais_name = 
-00006d50: 6d2e 6765 7428 2745 6169 734e 616d 6527  m.get('EaisName'
-00006d60: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00006d70: 6574 2827 4561 6973 5479 7065 2729 2069  et('EaisType') i
-00006d80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00006d90: 2020 2020 2020 2020 7365 6c66 2e65 6169          self.eai
-00006da0: 735f 7479 7065 203d 206d 2e67 6574 2827  s_type = m.get('
-00006db0: 4561 6973 5479 7065 2729 0a20 2020 2020  EaisType').     
-00006dc0: 2020 2069 6620 6d2e 6765 7428 2745 6369     if m.get('Eci
-00006dd0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00006de0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006df0: 2e65 6369 5f73 6872 696e 6b20 3d20 6d2e  .eci_shrink = m.
-00006e00: 6765 7428 2745 6369 2729 0a20 2020 2020  get('Eci').     
-00006e10: 2020 2069 6620 6d2e 6765 7428 2752 6567     if m.get('Reg
-00006e20: 696f 6e49 6427 2920 6973 206e 6f74 204e  ionId') is not N
-00006e30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00006e40: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
-00006e50: 3d20 6d2e 6765 7428 2752 6567 696f 6e49  = m.get('RegionI
-00006e60: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00006e70: 2e67 6574 2827 5265 736f 7572 6365 4772  .get('ResourceGr
-00006e80: 6f75 7049 6427 2920 6973 206e 6f74 204e  oupId') is not N
-00006e90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00006ea0: 2073 656c 662e 7265 736f 7572 6365 5f67   self.resource_g
-00006eb0: 726f 7570 5f69 6420 3d20 6d2e 6765 7428  roup_id = m.get(
-00006ec0: 2752 6573 6f75 7263 6547 726f 7570 4964  'ResourceGroupId
-00006ed0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00006ee0: 6765 7428 2753 6563 7572 6974 7947 726f  get('SecurityGro
-00006ef0: 7570 4964 2729 2069 7320 6e6f 7420 4e6f  upId') is not No
-00006f00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00006f10: 7365 6c66 2e73 6563 7572 6974 795f 6772  self.security_gr
-00006f20: 6f75 705f 6964 203d 206d 2e67 6574 2827  oup_id = m.get('
-00006f30: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
-00006f40: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00006f50: 6574 2827 5653 7769 7463 6849 6427 2920  et('VSwitchId') 
-00006f60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00006f70: 2020 2020 2020 2020 2073 656c 662e 765f           self.v_
-00006f80: 7377 6974 6368 5f69 6420 3d20 6d2e 6765  switch_id = m.ge
-00006f90: 7428 2756 5377 6974 6368 4964 2729 0a20  t('VSwitchId'). 
-00006fa0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00006fb0: 6c66 0a0a 0a63 6c61 7373 2043 7265 6174  lf...class Creat
-00006fc0: 6545 6169 4563 6952 6573 706f 6e73 6542  eEaiEciResponseB
-00006fd0: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
-00006fe0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00006ff0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-00007000: 2020 2020 2020 2063 6c69 656e 745f 696e         client_in
-00007010: 7374 616e 6365 5f69 643a 2073 7472 203d  stance_id: str =
-00007020: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
-00007030: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
-00007040: 6564 5f69 6e73 7461 6e63 655f 6964 3a20  ed_instance_id: 
-00007050: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00007060: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
-00007070: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00007080: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00007090: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
-000070a0: 6964 203d 2063 6c69 656e 745f 696e 7374  id = client_inst
-000070b0: 616e 6365 5f69 640a 2020 2020 2020 2020  ance_id.        
-000070c0: 7365 6c66 2e65 6c61 7374 6963 5f61 6363  self.elastic_acc
-000070d0: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
-000070e0: 655f 6964 203d 2065 6c61 7374 6963 5f61  e_id = elastic_a
-000070f0: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
-00007100: 6e63 655f 6964 0a20 2020 2020 2020 2073  nce_id.        s
-00007110: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-00007120: 2072 6571 7565 7374 5f69 640a 0a20 2020   request_id..   
-00007130: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00007140: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-00007150: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-00007160: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00007170: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-00007180: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00007190: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-000071a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000071b0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-000071c0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-000071d0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000071e0: 6620 7365 6c66 2e63 6c69 656e 745f 696e  f self.client_in
-000071f0: 7374 616e 6365 5f69 6420 6973 206e 6f74  stance_id is not
-00007200: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007210: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
-00007220: 7449 6e73 7461 6e63 6549 6427 5d20 3d20  tInstanceId'] = 
-00007230: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
-00007240: 616e 6365 5f69 640a 2020 2020 2020 2020  ance_id.        
-00007250: 6966 2073 656c 662e 656c 6173 7469 635f  if self.elastic_
-00007260: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
-00007270: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
-00007280: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00007290: 2072 6573 756c 745b 2745 6c61 7374 6963   result['Elastic
-000072a0: 4163 6365 6c65 7261 7465 6449 6e73 7461  AcceleratedInsta
-000072b0: 6e63 6549 6427 5d20 3d20 7365 6c66 2e65  nceId'] = self.e
-000072c0: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
-000072d0: 6564 5f69 6e73 7461 6e63 655f 6964 0a20  ed_instance_id. 
-000072e0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-000072f0: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
-00007300: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007310: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
-00007320: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
-00007330: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
-00007340: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00007350: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-00007360: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-00007370: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00007380: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00007390: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000073a0: 2827 436c 6965 6e74 496e 7374 616e 6365  ('ClientInstance
-000073b0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-000073c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000073d0: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
-000073e0: 6365 5f69 6420 3d20 6d2e 6765 7428 2743  ce_id = m.get('C
-000073f0: 6c69 656e 7449 6e73 7461 6e63 6549 6427  lientInstanceId'
-00007400: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00007410: 6574 2827 456c 6173 7469 6341 6363 656c  et('ElasticAccel
-00007420: 6572 6174 6564 496e 7374 616e 6365 4964  eratedInstanceId
-00007430: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00007440: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007450: 2e65 6c61 7374 6963 5f61 6363 656c 6572  .elastic_acceler
-00007460: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
-00007470: 203d 206d 2e67 6574 2827 456c 6173 7469   = m.get('Elasti
-00007480: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
-00007490: 616e 6365 4964 2729 0a20 2020 2020 2020  anceId').       
-000074a0: 2069 6620 6d2e 6765 7428 2752 6571 7565   if m.get('Reque
-000074b0: 7374 4964 2729 2069 7320 6e6f 7420 4e6f  stId') is not No
-000074c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000074d0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-000074e0: 3d20 6d2e 6765 7428 2752 6571 7565 7374  = m.get('Request
-000074f0: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
-00007500: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-00007510: 2043 7265 6174 6545 6169 4563 6952 6573   CreateEaiEciRes
-00007520: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-00007530: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00007540: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00007550: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-00007560: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-00007570: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00007580: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-00007590: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-000075a0: 2020 626f 6479 3a20 4372 6561 7465 4561    body: CreateEa
-000075b0: 6945 6369 5265 7370 6f6e 7365 426f 6479  iEciResponseBody
-000075c0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-000075d0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000075e0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-000075f0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00007600: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-00007610: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
-00007620: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
-00007630: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00007640: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00007650: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-00007660: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
-00007670: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
-00007680: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-00007690: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-000076a0: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
-000076b0: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
-000076c0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-000076d0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-000076e0: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
-000076f0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00007700: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-00007710: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-00007720: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-00007730: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00007740: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00007750: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-00007760: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00007770: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00007780: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00007790: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-000077a0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-000077b0: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-000077c0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-000077d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000077e0: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-000077f0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-00007800: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007810: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-00007820: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00007830: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-00007840: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-00007850: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-00007860: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00007870: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-00007880: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00007890: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-000078a0: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-000078b0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000078c0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-000078d0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-000078e0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-000078f0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00007900: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00007910: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-00007920: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00007930: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007940: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-00007950: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00007960: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-00007970: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-00007980: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007990: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-000079a0: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-000079b0: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-000079c0: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-000079d0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000079e0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000079f0: 5f6d 6f64 656c 203d 2043 7265 6174 6545  _model = CreateE
-00007a00: 6169 4563 6952 6573 706f 6e73 6542 6f64  aiEciResponseBod
-00007a10: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-00007a20: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-00007a30: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-00007a40: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-00007a50: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00007a60: 0a63 6c61 7373 2043 7265 6174 6545 6169  .class CreateEai
-00007a70: 4563 7352 6571 7565 7374 4563 7328 5465  EcsRequestEcs(Te
-00007a80: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00007a90: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00007aa0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00007ab0: 2069 6d61 6765 5f69 643a 2073 7472 203d   image_id: str =
-00007ac0: 204e 6f6e 652c 0a20 2020 2020 2020 2069   None,.        i
-00007ad0: 6e74 6572 6e65 745f 6d61 785f 6261 6e64  nternet_max_band
-00007ae0: 7769 6474 685f 696e 3a20 7374 7220 3d20  width_in: str = 
-00007af0: 4e6f 6e65 2c0a 2020 2020 2020 2020 696e  None,.        in
-00007b00: 7465 726e 6574 5f6d 6178 5f62 616e 6477  ternet_max_bandw
-00007b10: 6964 7468 5f6f 7574 3a20 7374 7220 3d20  idth_out: str = 
-00007b20: 4e6f 6e65 2c0a 2020 2020 2020 2020 6e61  None,.        na
-00007b30: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
-00007b40: 2020 2020 2020 2020 7061 7373 776f 7264          password
-00007b50: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00007b60: 2020 2020 2020 7379 7374 656d 5f64 6973        system_dis
-00007b70: 6b5f 6361 7465 676f 7279 3a20 7374 7220  k_category: str 
-00007b80: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00007b90: 7379 7374 656d 5f64 6973 6b5f 7369 7a65  system_disk_size
-00007ba0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-00007bb0: 2020 2020 2020 7479 7065 3a20 7374 7220        type: str 
-00007bc0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00007bd0: 7a6f 6e65 5f69 643a 2073 7472 203d 204e  zone_id: str = N
-00007be0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-00007bf0: 2020 2020 7365 6c66 2e69 6d61 6765 5f69      self.image_i
-00007c00: 6420 3d20 696d 6167 655f 6964 0a20 2020  d = image_id.   
-00007c10: 2020 2020 2073 656c 662e 696e 7465 726e       self.intern
-00007c20: 6574 5f6d 6178 5f62 616e 6477 6964 7468  et_max_bandwidth
-00007c30: 5f69 6e20 3d20 696e 7465 726e 6574 5f6d  _in = internet_m
-00007c40: 6178 5f62 616e 6477 6964 7468 5f69 6e0a  ax_bandwidth_in.
-00007c50: 2020 2020 2020 2020 7365 6c66 2e69 6e74          self.int
-00007c60: 6572 6e65 745f 6d61 785f 6261 6e64 7769  ernet_max_bandwi
-00007c70: 6474 685f 6f75 7420 3d20 696e 7465 726e  dth_out = intern
-00007c80: 6574 5f6d 6178 5f62 616e 6477 6964 7468  et_max_bandwidth
-00007c90: 5f6f 7574 0a20 2020 2020 2020 2073 656c  _out.        sel
-00007ca0: 662e 6e61 6d65 203d 206e 616d 650a 2020  f.name = name.  
-00007cb0: 2020 2020 2020 7365 6c66 2e70 6173 7377        self.passw
-00007cc0: 6f72 6420 3d20 7061 7373 776f 7264 0a20  ord = password. 
-00007cd0: 2020 2020 2020 2073 656c 662e 7379 7374         self.syst
-00007ce0: 656d 5f64 6973 6b5f 6361 7465 676f 7279  em_disk_category
-00007cf0: 203d 2073 7973 7465 6d5f 6469 736b 5f63   = system_disk_c
-00007d00: 6174 6567 6f72 790a 2020 2020 2020 2020  ategory.        
-00007d10: 7365 6c66 2e73 7973 7465 6d5f 6469 736b  self.system_disk
-00007d20: 5f73 697a 6520 3d20 7379 7374 656d 5f64  _size = system_d
-00007d30: 6973 6b5f 7369 7a65 0a20 2020 2020 2020  isk_size.       
-00007d40: 2073 656c 662e 7479 7065 203d 2074 7970   self.type = typ
-00007d50: 650a 2020 2020 2020 2020 7365 6c66 2e7a  e.        self.z
-00007d60: 6f6e 655f 6964 203d 207a 6f6e 655f 6964  one_id = zone_id
-00007d70: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00007d80: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00007d90: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00007da0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00007db0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00007dc0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-00007dd0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-00007de0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00007df0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-00007e00: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-00007e10: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-00007e20: 2020 2020 6966 2073 656c 662e 696d 6167      if self.imag
-00007e30: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
-00007e40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00007e50: 7375 6c74 5b27 496d 6167 6549 6427 5d20  sult['ImageId'] 
-00007e60: 3d20 7365 6c66 2e69 6d61 6765 5f69 640a  = self.image_id.
-00007e70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007e80: 696e 7465 726e 6574 5f6d 6178 5f62 616e  internet_max_ban
-00007e90: 6477 6964 7468 5f69 6e20 6973 206e 6f74  dwidth_in is not
+00001070: 0a0a 636c 6173 7320 4174 7461 6368 4561  ..class AttachEa
+00001080: 6973 4569 5265 7175 6573 7428 5465 614d  isEiRequest(TeaM
+00001090: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+000010a0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+000010b0: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
+000010c0: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
+000010d0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+000010e0: 2020 2020 2020 2065 695f 696e 7374 616e         ei_instan
+000010f0: 6365 5f69 643a 2073 7472 203d 204e 6f6e  ce_id: str = Non
+00001100: 652c 0a20 2020 2020 2020 2065 695f 696e  e,.        ei_in
+00001110: 7374 616e 6365 5f74 7970 653a 2073 7472  stance_type: str
+00001120: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00001130: 2072 6567 696f 6e5f 6964 3a20 7374 7220   region_id: str 
+00001140: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+00001150: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00001160: 6e74 5f69 6e73 7461 6e63 655f 6964 203d  nt_instance_id =
+00001170: 2063 6c69 656e 745f 696e 7374 616e 6365   client_instance
+00001180: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+00001190: 2e65 695f 696e 7374 616e 6365 5f69 6420  .ei_instance_id 
+000011a0: 3d20 6569 5f69 6e73 7461 6e63 655f 6964  = ei_instance_id
+000011b0: 0a20 2020 2020 2020 2073 656c 662e 6569  .        self.ei
+000011c0: 5f69 6e73 7461 6e63 655f 7479 7065 203d  _instance_type =
+000011d0: 2065 695f 696e 7374 616e 6365 5f74 7970   ei_instance_typ
+000011e0: 650a 2020 2020 2020 2020 7365 6c66 2e72  e.        self.r
+000011f0: 6567 696f 6e5f 6964 203d 2072 6567 696f  egion_id = regio
+00001200: 6e5f 6964 0a0a 2020 2020 6465 6620 7661  n_id..    def va
+00001210: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00001220: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00001230: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00001240: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00001250: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00001260: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00001270: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00001280: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001290: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000012a0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+000012b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000012c0: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
+000012d0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+000012e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000012f0: 6c74 5b27 436c 6965 6e74 496e 7374 616e  lt['ClientInstan
+00001300: 6365 4964 275d 203d 2073 656c 662e 636c  ceId'] = self.cl
+00001310: 6965 6e74 5f69 6e73 7461 6e63 655f 6964  ient_instance_id
+00001320: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00001330: 2e65 695f 696e 7374 616e 6365 5f69 6420  .ei_instance_id 
+00001340: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00001350: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00001360: 2745 6949 6e73 7461 6e63 6549 6427 5d20  'EiInstanceId'] 
+00001370: 3d20 7365 6c66 2e65 695f 696e 7374 616e  = self.ei_instan
+00001380: 6365 5f69 640a 2020 2020 2020 2020 6966  ce_id.        if
+00001390: 2073 656c 662e 6569 5f69 6e73 7461 6e63   self.ei_instanc
+000013a0: 655f 7479 7065 2069 7320 6e6f 7420 4e6f  e_type is not No
+000013b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000013c0: 7265 7375 6c74 5b27 4569 496e 7374 616e  result['EiInstan
+000013d0: 6365 5479 7065 275d 203d 2073 656c 662e  ceType'] = self.
+000013e0: 6569 5f69 6e73 7461 6e63 655f 7479 7065  ei_instance_type
+000013f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00001400: 2e72 6567 696f 6e5f 6964 2069 7320 6e6f  .region_id is no
+00001410: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00001420: 2020 2020 7265 7375 6c74 5b27 5265 6769      result['Regi
+00001430: 6f6e 4964 275d 203d 2073 656c 662e 7265  onId'] = self.re
+00001440: 6769 6f6e 5f69 640a 2020 2020 2020 2020  gion_id.        
+00001450: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00001460: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00001470: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00001480: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00001490: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+000014a0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000014b0: 2743 6c69 656e 7449 6e73 7461 6e63 6549  'ClientInstanceI
+000014c0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+000014d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000014e0: 662e 636c 6965 6e74 5f69 6e73 7461 6e63  f.client_instanc
+000014f0: 655f 6964 203d 206d 2e67 6574 2827 436c  e_id = m.get('Cl
+00001500: 6965 6e74 496e 7374 616e 6365 4964 2729  ientInstanceId')
+00001510: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00001520: 7428 2745 6949 6e73 7461 6e63 6549 6427  t('EiInstanceId'
+00001530: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00001540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001550: 6569 5f69 6e73 7461 6e63 655f 6964 203d  ei_instance_id =
+00001560: 206d 2e67 6574 2827 4569 496e 7374 616e   m.get('EiInstan
+00001570: 6365 4964 2729 0a20 2020 2020 2020 2069  ceId').        i
+00001580: 6620 6d2e 6765 7428 2745 6949 6e73 7461  f m.get('EiInsta
+00001590: 6e63 6554 7970 6527 2920 6973 206e 6f74  nceType') is not
+000015a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000015b0: 2020 2073 656c 662e 6569 5f69 6e73 7461     self.ei_insta
+000015c0: 6e63 655f 7479 7065 203d 206d 2e67 6574  nce_type = m.get
+000015d0: 2827 4569 496e 7374 616e 6365 5479 7065  ('EiInstanceType
+000015e0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000015f0: 6765 7428 2752 6567 696f 6e49 6427 2920  get('RegionId') 
+00001600: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00001610: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00001620: 6769 6f6e 5f69 6420 3d20 6d2e 6765 7428  gion_id = m.get(
+00001630: 2752 6567 696f 6e49 6427 290a 2020 2020  'RegionId').    
+00001640: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00001650: 0a0a 636c 6173 7320 4174 7461 6368 4561  ..class AttachEa
+00001660: 6973 4569 5265 7370 6f6e 7365 426f 6479  isEiResponseBody
+00001670: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00001680: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00001690: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000016a0: 2020 2020 636c 6965 6e74 5f69 6e73 7461      client_insta
+000016b0: 6e63 655f 6964 3a20 7374 7220 3d20 4e6f  nce_id: str = No
+000016c0: 6e65 2c0a 2020 2020 2020 2020 6569 5f69  ne,.        ei_i
+000016d0: 6e73 7461 6e63 655f 6964 3a20 7374 7220  nstance_id: str 
+000016e0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000016f0: 7265 7175 6573 745f 6964 3a20 7374 7220  request_id: str 
+00001700: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+00001710: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00001720: 6e74 5f69 6e73 7461 6e63 655f 6964 203d  nt_instance_id =
+00001730: 2063 6c69 656e 745f 696e 7374 616e 6365   client_instance
+00001740: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+00001750: 2e65 695f 696e 7374 616e 6365 5f69 6420  .ei_instance_id 
+00001760: 3d20 6569 5f69 6e73 7461 6e63 655f 6964  = ei_instance_id
+00001770: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00001780: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
+00001790: 7374 5f69 640a 0a20 2020 2064 6566 2076  st_id..    def v
+000017a0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+000017b0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+000017c0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+000017d0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+000017e0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+000017f0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00001800: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00001810: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001820: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00001830: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00001840: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00001850: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
+00001860: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00001870: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00001880: 756c 745b 2743 6c69 656e 7449 6e73 7461  ult['ClientInsta
+00001890: 6e63 6549 6427 5d20 3d20 7365 6c66 2e63  nceId'] = self.c
+000018a0: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
+000018b0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+000018c0: 662e 6569 5f69 6e73 7461 6e63 655f 6964  f.ei_instance_id
+000018d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000018e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000018f0: 5b27 4569 496e 7374 616e 6365 4964 275d  ['EiInstanceId']
+00001900: 203d 2073 656c 662e 6569 5f69 6e73 7461   = self.ei_insta
+00001910: 6e63 655f 6964 0a20 2020 2020 2020 2069  nce_id.        i
+00001920: 6620 7365 6c66 2e72 6571 7565 7374 5f69  f self.request_i
+00001930: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00001940: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00001950: 745b 2752 6571 7565 7374 4964 275d 203d  t['RequestId'] =
+00001960: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+00001970: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001980: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00001990: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000019a0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000019b0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000019c0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000019d0: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
+000019e0: 496e 7374 616e 6365 4964 2729 2069 7320  InstanceId') is 
+000019f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00001a00: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
+00001a10: 745f 696e 7374 616e 6365 5f69 6420 3d20  t_instance_id = 
+00001a20: 6d2e 6765 7428 2743 6c69 656e 7449 6e73  m.get('ClientIns
+00001a30: 7461 6e63 6549 6427 290a 2020 2020 2020  tanceId').      
+00001a40: 2020 6966 206d 2e67 6574 2827 4569 496e    if m.get('EiIn
+00001a50: 7374 616e 6365 4964 2729 2069 7320 6e6f  stanceId') is no
+00001a60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00001a70: 2020 2020 7365 6c66 2e65 695f 696e 7374      self.ei_inst
+00001a80: 616e 6365 5f69 6420 3d20 6d2e 6765 7428  ance_id = m.get(
+00001a90: 2745 6949 6e73 7461 6e63 6549 6427 290a  'EiInstanceId').
+00001aa0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00001ab0: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
+00001ac0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00001ad0: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+00001ae0: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
+00001af0: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
+00001b00: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00001b10: 0a0a 636c 6173 7320 4174 7461 6368 4561  ..class AttachEa
+00001b20: 6973 4569 5265 7370 6f6e 7365 2854 6561  isEiResponse(Tea
+00001b30: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+00001b40: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00001b50: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00001b60: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
+00001b70: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+00001b80: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+00001b90: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
+00001ba0: 0a20 2020 2020 2020 2062 6f64 793a 2041  .        body: A
+00001bb0: 7474 6163 6845 6169 7345 6952 6573 706f  ttachEaisEiRespo
+00001bc0: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
+00001bd0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00001be0: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
+00001bf0: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
+00001c00: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+00001c10: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
+00001c20: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+00001c30: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
+00001c40: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00001c50: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+00001c60: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+00001c70: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
+00001c80: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
+00001c90: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+00001ca0: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
+00001cb0: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
+00001cc0: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
+00001cd0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+00001ce0: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
+00001cf0: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
+00001d00: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
+00001d10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001d20: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
+00001d30: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00001d40: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00001d50: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+00001d60: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00001d70: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00001d80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00001d90: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00001da0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00001db0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00001dc0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+00001dd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00001de0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+00001df0: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+00001e00: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+00001e10: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+00001e20: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+00001e30: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00001e40: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+00001e50: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+00001e60: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+00001e70: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+00001e80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00001e90: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+00001ea0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+00001eb0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+00001ec0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00001ed0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00001ee0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00001ef0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00001f00: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00001f10: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+00001f20: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+00001f30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00001f40: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00001f50: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+00001f60: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00001f70: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00001f80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00001f90: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00001fa0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+00001fb0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00001fc0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00001fd0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+00001fe0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00001ff0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+00002000: 4174 7461 6368 4561 6973 4569 5265 7370  AttachEaisEiResp
+00002010: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+00002020: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00002030: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+00002040: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00002050: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00002060: 2073 656c 660a 0a0a 636c 6173 7320 4368   self...class Ch
+00002070: 616e 6765 5265 736f 7572 6365 4772 6f75  angeResourceGrou
+00002080: 7052 6571 7565 7374 2854 6561 4d6f 6465  pRequest(TeaMode
+00002090: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+000020a0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000020b0: 6c66 2c0a 2020 2020 2020 2020 7265 736f  lf,.        reso
+000020c0: 7572 6365 5f67 726f 7570 5f69 643a 2073  urce_group_id: s
+000020d0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000020e0: 2020 2072 6573 6f75 7263 655f 6964 3a20     resource_id: 
+000020f0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00002100: 2020 2020 7265 736f 7572 6365 5f72 6567      resource_reg
+00002110: 696f 6e5f 6964 3a20 7374 7220 3d20 4e6f  ion_id: str = No
+00002120: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+00002130: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
+00002140: 5f67 726f 7570 5f69 6420 3d20 7265 736f  _group_id = reso
+00002150: 7572 6365 5f67 726f 7570 5f69 640a 2020  urce_group_id.  
+00002160: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
+00002170: 7263 655f 6964 203d 2072 6573 6f75 7263  rce_id = resourc
+00002180: 655f 6964 0a20 2020 2020 2020 2073 656c  e_id.        sel
+00002190: 662e 7265 736f 7572 6365 5f72 6567 696f  f.resource_regio
+000021a0: 6e5f 6964 203d 2072 6573 6f75 7263 655f  n_id = resource_
+000021b0: 7265 6769 6f6e 5f69 640a 0a20 2020 2064  region_id..    d
+000021c0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+000021d0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+000021e0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+000021f0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00002200: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+00002210: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00002220: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00002230: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00002240: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00002250: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00002260: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00002270: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
+00002280: 6f75 705f 6964 2069 7320 6e6f 7420 4e6f  oup_id is not No
+00002290: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000022a0: 7265 7375 6c74 5b27 5265 736f 7572 6365  result['Resource
+000022b0: 4772 6f75 7049 6427 5d20 3d20 7365 6c66  GroupId'] = self
+000022c0: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
+000022d0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+000022e0: 6c66 2e72 6573 6f75 7263 655f 6964 2069  lf.resource_id i
+000022f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00002300: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00002310: 5265 736f 7572 6365 4964 275d 203d 2073  ResourceId'] = s
+00002320: 656c 662e 7265 736f 7572 6365 5f69 640a  elf.resource_id.
+00002330: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00002340: 7265 736f 7572 6365 5f72 6567 696f 6e5f  resource_region_
+00002350: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00002360: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00002370: 6c74 5b27 5265 736f 7572 6365 5265 6769  lt['ResourceRegi
+00002380: 6f6e 4964 275d 203d 2073 656c 662e 7265  onId'] = self.re
+00002390: 736f 7572 6365 5f72 6567 696f 6e5f 6964  source_region_id
+000023a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000023b0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+000023c0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+000023d0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000023e0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000023f0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00002400: 6966 206d 2e67 6574 2827 5265 736f 7572  if m.get('Resour
+00002410: 6365 4772 6f75 7049 6427 2920 6973 206e  ceGroupId') is n
+00002420: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00002430: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+00002440: 6365 5f67 726f 7570 5f69 6420 3d20 6d2e  ce_group_id = m.
+00002450: 6765 7428 2752 6573 6f75 7263 6547 726f  get('ResourceGro
+00002460: 7570 4964 2729 0a20 2020 2020 2020 2069  upId').        i
+00002470: 6620 6d2e 6765 7428 2752 6573 6f75 7263  f m.get('Resourc
+00002480: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+00002490: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000024a0: 656c 662e 7265 736f 7572 6365 5f69 6420  elf.resource_id 
+000024b0: 3d20 6d2e 6765 7428 2752 6573 6f75 7263  = m.get('Resourc
+000024c0: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
+000024d0: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+000024e0: 5265 6769 6f6e 4964 2729 2069 7320 6e6f  RegionId') is no
+000024f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00002500: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
+00002510: 655f 7265 6769 6f6e 5f69 6420 3d20 6d2e  e_region_id = m.
+00002520: 6765 7428 2752 6573 6f75 7263 6552 6567  get('ResourceReg
+00002530: 696f 6e49 6427 290a 2020 2020 2020 2020  ionId').        
+00002540: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00002550: 6173 7320 4368 616e 6765 5265 736f 7572  ass ChangeResour
+00002560: 6365 4772 6f75 7052 6573 706f 6e73 6542  ceGroupResponseB
+00002570: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
+00002580: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00002590: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000025a0: 2020 2020 2020 2072 6571 7565 7374 5f69         request_i
+000025b0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+000025c0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+000025d0: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+000025e0: 7265 7175 6573 745f 6964 0a0a 2020 2020  request_id..    
+000025f0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00002600: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00002610: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00002620: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00002630: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+00002640: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00002650: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00002660: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00002670: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00002680: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00002690: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000026a0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+000026b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000026c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000026d0: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
+000026e0: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
+000026f0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00002700: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00002710: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00002720: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00002730: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00002740: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00002750: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
+00002760: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00002770: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00002780: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+00002790: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+000027a0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+000027b0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2043  n self...class C
+000027c0: 6861 6e67 6552 6573 6f75 7263 6547 726f  hangeResourceGro
+000027d0: 7570 5265 7370 6f6e 7365 2854 6561 4d6f  upResponse(TeaMo
+000027e0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+000027f0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00002800: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+00002810: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+00002820: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+00002830: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+00002840: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+00002850: 2020 2020 2020 2062 6f64 793a 2043 6861         body: Cha
+00002860: 6e67 6552 6573 6f75 7263 6547 726f 7570  ngeResourceGroup
+00002870: 5265 7370 6f6e 7365 426f 6479 203d 204e  ResponseBody = N
+00002880: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+00002890: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000028a0: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
+000028b0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+000028c0: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+000028d0: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
+000028e0: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
+000028f0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00002900: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00002910: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+00002920: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
+00002930: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
+00002940: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+00002950: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+00002960: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
+00002970: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
+00002980: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+00002990: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+000029a0: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
+000029b0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+000029c0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
+000029d0: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
+000029e0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+000029f0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00002a00: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00002a10: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+00002a20: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00002a30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00002a40: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00002a50: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00002a60: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00002a70: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+00002a80: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00002a90: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00002aa0: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+00002ab0: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+00002ac0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00002ad0: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+00002ae0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00002af0: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+00002b00: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+00002b10: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+00002b20: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+00002b30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00002b40: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+00002b50: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+00002b60: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+00002b70: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00002b80: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00002b90: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+00002ba0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00002bb0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+00002bc0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00002bd0: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
+00002be0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00002bf0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+00002c00: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
+00002c10: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
+00002c20: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
+00002c30: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
+00002c40: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00002c50: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00002c60: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
+00002c70: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
+00002c80: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
+00002c90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00002ca0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+00002cb0: 656c 203d 2043 6861 6e67 6552 6573 6f75  el = ChangeResou
+00002cc0: 7263 6547 726f 7570 5265 7370 6f6e 7365  rceGroupResponse
+00002cd0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
+00002ce0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+00002cf0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+00002d00: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+00002d10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00002d20: 660a 0a0a 636c 6173 7320 4372 6561 7465  f...class Create
+00002d30: 4561 6952 6571 7565 7374 2854 6561 4d6f  EaiRequest(TeaMo
+00002d40: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00002d50: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00002d60: 7365 6c66 2c0a 2020 2020 2020 2020 636c  self,.        cl
+00002d70: 6965 6e74 5f74 6f6b 656e 3a20 7374 7220  ient_token: str 
+00002d80: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00002d90: 696d 6167 653a 2073 7472 203d 204e 6f6e  image: str = Non
+00002da0: 652c 0a20 2020 2020 2020 2069 6e73 7461  e,.        insta
+00002db0: 6e63 655f 6e61 6d65 3a20 7374 7220 3d20  nce_name: str = 
+00002dc0: 4e6f 6e65 2c0a 2020 2020 2020 2020 696e  None,.        in
+00002dd0: 7374 616e 6365 5f74 7970 653a 2073 7472  stance_type: str
+00002de0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00002df0: 2072 6567 696f 6e5f 6964 3a20 7374 7220   region_id: str 
+00002e00: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00002e10: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
+00002e20: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+00002e30: 2020 2020 2020 2073 6563 7572 6974 795f         security_
+00002e40: 6772 6f75 705f 6964 3a20 7374 7220 3d20  group_id: str = 
+00002e50: 4e6f 6e65 2c0a 2020 2020 2020 2020 765f  None,.        v_
+00002e60: 7377 6974 6368 5f69 643a 2073 7472 203d  switch_id: str =
+00002e70: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+00002e80: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
+00002e90: 745f 746f 6b65 6e20 3d20 636c 6965 6e74  t_token = client
+00002ea0: 5f74 6f6b 656e 0a20 2020 2020 2020 2073  _token.        s
+00002eb0: 656c 662e 696d 6167 6520 3d20 696d 6167  elf.image = imag
+00002ec0: 650a 2020 2020 2020 2020 7365 6c66 2e69  e.        self.i
+00002ed0: 6e73 7461 6e63 655f 6e61 6d65 203d 2069  nstance_name = i
+00002ee0: 6e73 7461 6e63 655f 6e61 6d65 0a20 2020  nstance_name.   
+00002ef0: 2020 2020 2073 656c 662e 696e 7374 616e       self.instan
+00002f00: 6365 5f74 7970 6520 3d20 696e 7374 616e  ce_type = instan
+00002f10: 6365 5f74 7970 650a 2020 2020 2020 2020  ce_type.        
+00002f20: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
+00002f30: 2072 6567 696f 6e5f 6964 0a20 2020 2020   region_id.     
+00002f40: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
+00002f50: 5f67 726f 7570 5f69 6420 3d20 7265 736f  _group_id = reso
+00002f60: 7572 6365 5f67 726f 7570 5f69 640a 2020  urce_group_id.  
+00002f70: 2020 2020 2020 7365 6c66 2e73 6563 7572        self.secur
+00002f80: 6974 795f 6772 6f75 705f 6964 203d 2073  ity_group_id = s
+00002f90: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
+00002fa0: 0a20 2020 2020 2020 2073 656c 662e 765f  .        self.v_
+00002fb0: 7377 6974 6368 5f69 6420 3d20 765f 7377  switch_id = v_sw
+00002fc0: 6974 6368 5f69 640a 0a20 2020 2064 6566  itch_id..    def
+00002fd0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00002fe0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00002ff0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00003000: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00003010: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+00003020: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00003030: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00003040: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00003050: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00003060: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00003070: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00003080: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
+00003090: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000030a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000030b0: 2743 6c69 656e 7454 6f6b 656e 275d 203d  'ClientToken'] =
+000030c0: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+000030d0: 656e 0a20 2020 2020 2020 2069 6620 7365  en.        if se
+000030e0: 6c66 2e69 6d61 6765 2069 7320 6e6f 7420  lf.image is not 
+000030f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00003100: 2020 7265 7375 6c74 5b27 496d 6167 6527    result['Image'
+00003110: 5d20 3d20 7365 6c66 2e69 6d61 6765 0a20  ] = self.image. 
+00003120: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+00003130: 6e73 7461 6e63 655f 6e61 6d65 2069 7320  nstance_name is 
+00003140: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00003150: 2020 2020 2020 7265 7375 6c74 5b27 496e        result['In
+00003160: 7374 616e 6365 4e61 6d65 275d 203d 2073  stanceName'] = s
+00003170: 656c 662e 696e 7374 616e 6365 5f6e 616d  elf.instance_nam
+00003180: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00003190: 662e 696e 7374 616e 6365 5f74 7970 6520  f.instance_type 
+000031a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000031b0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000031c0: 2749 6e73 7461 6e63 6554 7970 6527 5d20  'InstanceType'] 
+000031d0: 3d20 7365 6c66 2e69 6e73 7461 6e63 655f  = self.instance_
+000031e0: 7479 7065 0a20 2020 2020 2020 2069 6620  type.        if 
+000031f0: 7365 6c66 2e72 6567 696f 6e5f 6964 2069  self.region_id i
+00003200: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00003210: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00003220: 5265 6769 6f6e 4964 275d 203d 2073 656c  RegionId'] = sel
+00003230: 662e 7265 6769 6f6e 5f69 640a 2020 2020  f.region_id.    
+00003240: 2020 2020 6966 2073 656c 662e 7265 736f      if self.reso
+00003250: 7572 6365 5f67 726f 7570 5f69 6420 6973  urce_group_id is
+00003260: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00003270: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
+00003280: 6573 6f75 7263 6547 726f 7570 4964 275d  esourceGroupId']
+00003290: 203d 2073 656c 662e 7265 736f 7572 6365   = self.resource
+000032a0: 5f67 726f 7570 5f69 640a 2020 2020 2020  _group_id.      
+000032b0: 2020 6966 2073 656c 662e 7365 6375 7269    if self.securi
+000032c0: 7479 5f67 726f 7570 5f69 6420 6973 206e  ty_group_id is n
+000032d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000032e0: 2020 2020 2072 6573 756c 745b 2753 6563       result['Sec
+000032f0: 7572 6974 7947 726f 7570 4964 275d 203d  urityGroupId'] =
+00003300: 2073 656c 662e 7365 6375 7269 7479 5f67   self.security_g
+00003310: 726f 7570 5f69 640a 2020 2020 2020 2020  roup_id.        
+00003320: 6966 2073 656c 662e 765f 7377 6974 6368  if self.v_switch
+00003330: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00003340: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00003350: 756c 745b 2756 5377 6974 6368 4964 275d  ult['VSwitchId']
+00003360: 203d 2073 656c 662e 765f 7377 6974 6368   = self.v_switch
+00003370: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+00003380: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00003390: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+000033a0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+000033b0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+000033c0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+000033d0: 2020 2069 6620 6d2e 6765 7428 2743 6c69     if m.get('Cli
+000033e0: 656e 7454 6f6b 656e 2729 2069 7320 6e6f  entToken') is no
+000033f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00003400: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
+00003410: 746f 6b65 6e20 3d20 6d2e 6765 7428 2743  token = m.get('C
+00003420: 6c69 656e 7454 6f6b 656e 2729 0a20 2020  lientToken').   
+00003430: 2020 2020 2069 6620 6d2e 6765 7428 2749       if m.get('I
+00003440: 6d61 6765 2729 2069 7320 6e6f 7420 4e6f  mage') is not No
+00003450: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00003460: 7365 6c66 2e69 6d61 6765 203d 206d 2e67  self.image = m.g
+00003470: 6574 2827 496d 6167 6527 290a 2020 2020  et('Image').    
+00003480: 2020 2020 6966 206d 2e67 6574 2827 496e      if m.get('In
+00003490: 7374 616e 6365 4e61 6d65 2729 2069 7320  stanceName') is 
+000034a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000034b0: 2020 2020 2020 7365 6c66 2e69 6e73 7461        self.insta
+000034c0: 6e63 655f 6e61 6d65 203d 206d 2e67 6574  nce_name = m.get
+000034d0: 2827 496e 7374 616e 6365 4e61 6d65 2729  ('InstanceName')
+000034e0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000034f0: 7428 2749 6e73 7461 6e63 6554 7970 6527  t('InstanceType'
+00003500: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00003510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003520: 696e 7374 616e 6365 5f74 7970 6520 3d20  instance_type = 
+00003530: 6d2e 6765 7428 2749 6e73 7461 6e63 6554  m.get('InstanceT
+00003540: 7970 6527 290a 2020 2020 2020 2020 6966  ype').        if
+00003550: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
+00003560: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00003570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003580: 2e72 6567 696f 6e5f 6964 203d 206d 2e67  .region_id = m.g
+00003590: 6574 2827 5265 6769 6f6e 4964 2729 0a20  et('RegionId'). 
+000035a0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000035b0: 2752 6573 6f75 7263 6547 726f 7570 4964  'ResourceGroupId
+000035c0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000035d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000035e0: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
+000035f0: 6964 203d 206d 2e67 6574 2827 5265 736f  id = m.get('Reso
+00003600: 7572 6365 4772 6f75 7049 6427 290a 2020  urceGroupId').  
+00003610: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00003620: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
+00003630: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00003640: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003650: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
+00003660: 6420 3d20 6d2e 6765 7428 2753 6563 7572  d = m.get('Secur
+00003670: 6974 7947 726f 7570 4964 2729 0a20 2020  ityGroupId').   
+00003680: 2020 2020 2069 6620 6d2e 6765 7428 2756       if m.get('V
+00003690: 5377 6974 6368 4964 2729 2069 7320 6e6f  SwitchId') is no
+000036a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000036b0: 2020 2020 7365 6c66 2e76 5f73 7769 7463      self.v_switc
+000036c0: 685f 6964 203d 206d 2e67 6574 2827 5653  h_id = m.get('VS
+000036d0: 7769 7463 6849 6427 290a 2020 2020 2020  witchId').      
+000036e0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+000036f0: 636c 6173 7320 4372 6561 7465 4561 6952  class CreateEaiR
+00003700: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
+00003710: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00003720: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00003730: 2073 656c 662c 0a20 2020 2020 2020 2065   self,.        e
+00003740: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+00003750: 6564 5f69 6e73 7461 6e63 655f 6964 3a20  ed_instance_id: 
+00003760: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00003770: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
+00003780: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00003790: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000037a0: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
+000037b0: 7465 645f 696e 7374 616e 6365 5f69 6420  ted_instance_id 
+000037c0: 3d20 656c 6173 7469 635f 6163 6365 6c65  = elastic_accele
+000037d0: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
+000037e0: 640a 2020 2020 2020 2020 7365 6c66 2e72  d.        self.r
+000037f0: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
+00003800: 6573 745f 6964 0a0a 2020 2020 6465 6620  est_id..    def 
+00003810: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00003820: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00003830: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00003840: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00003850: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+00003860: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00003870: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00003880: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00003890: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000038a0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000038b0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000038c0: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
+000038d0: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
+000038e0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+000038f0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00003900: 745b 2745 6c61 7374 6963 4163 6365 6c65  t['ElasticAccele
+00003910: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
+00003920: 5d20 3d20 7365 6c66 2e65 6c61 7374 6963  ] = self.elastic
+00003930: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+00003940: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+00003950: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
+00003960: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00003970: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00003980: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
+00003990: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+000039a0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+000039b0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+000039c0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+000039d0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+000039e0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+000039f0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00003a00: 2020 6966 206d 2e67 6574 2827 456c 6173    if m.get('Elas
+00003a10: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
+00003a20: 7374 616e 6365 4964 2729 2069 7320 6e6f  stanceId') is no
+00003a30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00003a40: 2020 2020 7365 6c66 2e65 6c61 7374 6963      self.elastic
+00003a50: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+00003a60: 7461 6e63 655f 6964 203d 206d 2e67 6574  tance_id = m.get
+00003a70: 2827 456c 6173 7469 6341 6363 656c 6572  ('ElasticAcceler
+00003a80: 6174 6564 496e 7374 616e 6365 4964 2729  atedInstanceId')
+00003a90: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00003aa0: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
+00003ab0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00003ac0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+00003ad0: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
+00003ae0: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
+00003af0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00003b00: 0a0a 0a63 6c61 7373 2043 7265 6174 6545  ...class CreateE
+00003b10: 6169 5265 7370 6f6e 7365 2854 6561 4d6f  aiResponse(TeaMo
+00003b20: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00003b30: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00003b40: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+00003b50: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+00003b60: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+00003b70: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+00003b80: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+00003b90: 2020 2020 2020 2062 6f64 793a 2043 7265         body: Cre
+00003ba0: 6174 6545 6169 5265 7370 6f6e 7365 426f  ateEaiResponseBo
+00003bb0: 6479 203d 204e 6f6e 652c 0a20 2020 2029  dy = None,.    )
+00003bc0: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
+00003bd0: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
+00003be0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00003bf0: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
+00003c00: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+00003c10: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+00003c20: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00003c30: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00003c40: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00003c50: 7265 7175 6972 6564 2873 656c 662e 6865  required(self.he
+00003c60: 6164 6572 732c 2027 6865 6164 6572 7327  aders, 'headers'
+00003c70: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00003c80: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00003c90: 2873 656c 662e 7374 6174 7573 5f63 6f64  (self.status_cod
+00003ca0: 652c 2027 7374 6174 7573 5f63 6f64 6527  e, 'status_code'
+00003cb0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00003cc0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00003cd0: 2873 656c 662e 626f 6479 2c20 2762 6f64  (self.body, 'bod
+00003ce0: 7927 290a 2020 2020 2020 2020 6966 2073  y').        if s
+00003cf0: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+00003d00: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+00003d10: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+00003d20: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00003d30: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00003d40: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00003d50: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00003d60: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00003d70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00003d80: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00003d90: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00003da0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00003db0: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+00003dc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00003dd0: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
+00003de0: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
+00003df0: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00003e00: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
+00003e10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00003e20: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+00003e30: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
+00003e40: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
+00003e50: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00003e60: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+00003e70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00003e80: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
+00003e90: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
+00003ea0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003eb0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00003ec0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00003ed0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+00003ee0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00003ef0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00003f00: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+00003f10: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00003f20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003f30: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+00003f40: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+00003f50: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+00003f60: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+00003f70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00003f80: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00003f90: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+00003fa0: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+00003fb0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+00003fc0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+00003fd0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00003fe0: 6d70 5f6d 6f64 656c 203d 2043 7265 6174  mp_model = Creat
+00003ff0: 6545 6169 5265 7370 6f6e 7365 426f 6479  eEaiResponseBody
+00004000: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00004010: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
+00004020: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
+00004030: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
+00004040: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00004050: 636c 6173 7320 4372 6561 7465 4561 6941  class CreateEaiA
+00004060: 6c6c 5265 7175 6573 7428 5465 614d 6f64  llRequest(TeaMod
+00004070: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00004080: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00004090: 656c 662c 0a20 2020 2020 2020 2063 6c69  elf,.        cli
+000040a0: 656e 745f 696d 6167 655f 6964 3a20 7374  ent_image_id: st
+000040b0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000040c0: 2020 636c 6965 6e74 5f69 6e73 7461 6e63    client_instanc
+000040d0: 655f 6e61 6d65 3a20 7374 7220 3d20 4e6f  e_name: str = No
+000040e0: 6e65 2c0a 2020 2020 2020 2020 636c 6965  ne,.        clie
+000040f0: 6e74 5f69 6e73 7461 6e63 655f 7479 7065  nt_instance_type
+00004100: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00004110: 2020 2020 2020 636c 6965 6e74 5f69 6e74        client_int
+00004120: 6572 6e65 745f 6d61 785f 6261 6e64 7769  ernet_max_bandwi
+00004130: 6474 685f 696e 3a20 696e 7420 3d20 4e6f  dth_in: int = No
+00004140: 6e65 2c0a 2020 2020 2020 2020 636c 6965  ne,.        clie
+00004150: 6e74 5f69 6e74 6572 6e65 745f 6d61 785f  nt_internet_max_
+00004160: 6261 6e64 7769 6474 685f 6f75 743a 2069  bandwidth_out: i
+00004170: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+00004180: 2020 2063 6c69 656e 745f 7061 7373 776f     client_passwo
+00004190: 7264 3a20 7374 7220 3d20 4e6f 6e65 2c0a  rd: str = None,.
+000041a0: 2020 2020 2020 2020 636c 6965 6e74 5f73          client_s
+000041b0: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
+000041c0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000041d0: 2020 2020 2020 636c 6965 6e74 5f73 7973        client_sys
+000041e0: 7465 6d5f 6469 736b 5f63 6174 6567 6f72  tem_disk_categor
+000041f0: 793a 2073 7472 203d 204e 6f6e 652c 0a20  y: str = None,. 
+00004200: 2020 2020 2020 2063 6c69 656e 745f 7379         client_sy
+00004210: 7374 656d 5f64 6973 6b5f 7369 7a65 3a20  stem_disk_size: 
+00004220: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+00004230: 2020 2020 636c 6965 6e74 5f74 6f6b 656e      client_token
+00004240: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00004250: 2020 2020 2020 636c 6965 6e74 5f76 7377        client_vsw
+00004260: 6974 6368 5f69 643a 2073 7472 203d 204e  itch_id: str = N
+00004270: 6f6e 652c 0a20 2020 2020 2020 2063 6c69  one,.        cli
+00004280: 656e 745f 7a6f 6e65 5f69 643a 2073 7472  ent_zone_id: str
+00004290: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000042a0: 2065 6169 5f69 6e73 7461 6e63 655f 7479   eai_instance_ty
+000042b0: 7065 3a20 7374 7220 3d20 4e6f 6e65 2c0a  pe: str = None,.
+000042c0: 2020 2020 2020 2020 696e 7374 616e 6365          instance
+000042d0: 5f6e 616d 653a 2073 7472 203d 204e 6f6e  _name: str = Non
+000042e0: 652c 0a20 2020 2020 2020 2072 6567 696f  e,.        regio
+000042f0: 6e5f 6964 3a20 7374 7220 3d20 4e6f 6e65  n_id: str = None
+00004300: 2c0a 2020 2020 2020 2020 7265 736f 7572  ,.        resour
+00004310: 6365 5f67 726f 7570 5f69 643a 2073 7472  ce_group_id: str
+00004320: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00004330: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
+00004340: 656e 745f 696d 6167 655f 6964 203d 2063  ent_image_id = c
+00004350: 6c69 656e 745f 696d 6167 655f 6964 0a20  lient_image_id. 
+00004360: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00004370: 6e74 5f69 6e73 7461 6e63 655f 6e61 6d65  nt_instance_name
+00004380: 203d 2063 6c69 656e 745f 696e 7374 616e   = client_instan
+00004390: 6365 5f6e 616d 650a 2020 2020 2020 2020  ce_name.        
+000043a0: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
+000043b0: 616e 6365 5f74 7970 6520 3d20 636c 6965  ance_type = clie
+000043c0: 6e74 5f69 6e73 7461 6e63 655f 7479 7065  nt_instance_type
+000043d0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+000043e0: 6965 6e74 5f69 6e74 6572 6e65 745f 6d61  ient_internet_ma
+000043f0: 785f 6261 6e64 7769 6474 685f 696e 203d  x_bandwidth_in =
+00004400: 2063 6c69 656e 745f 696e 7465 726e 6574   client_internet
+00004410: 5f6d 6178 5f62 616e 6477 6964 7468 5f69  _max_bandwidth_i
+00004420: 6e0a 2020 2020 2020 2020 7365 6c66 2e63  n.        self.c
+00004430: 6c69 656e 745f 696e 7465 726e 6574 5f6d  lient_internet_m
+00004440: 6178 5f62 616e 6477 6964 7468 5f6f 7574  ax_bandwidth_out
+00004450: 203d 2063 6c69 656e 745f 696e 7465 726e   = client_intern
+00004460: 6574 5f6d 6178 5f62 616e 6477 6964 7468  et_max_bandwidth
+00004470: 5f6f 7574 0a20 2020 2020 2020 2073 656c  _out.        sel
+00004480: 662e 636c 6965 6e74 5f70 6173 7377 6f72  f.client_passwor
+00004490: 6420 3d20 636c 6965 6e74 5f70 6173 7377  d = client_passw
+000044a0: 6f72 640a 2020 2020 2020 2020 7365 6c66  ord.        self
+000044b0: 2e63 6c69 656e 745f 7365 6375 7269 7479  .client_security
+000044c0: 5f67 726f 7570 5f69 6420 3d20 636c 6965  _group_id = clie
+000044d0: 6e74 5f73 6563 7572 6974 795f 6772 6f75  nt_security_grou
+000044e0: 705f 6964 0a20 2020 2020 2020 2073 656c  p_id.        sel
+000044f0: 662e 636c 6965 6e74 5f73 7973 7465 6d5f  f.client_system_
+00004500: 6469 736b 5f63 6174 6567 6f72 7920 3d20  disk_category = 
+00004510: 636c 6965 6e74 5f73 7973 7465 6d5f 6469  client_system_di
+00004520: 736b 5f63 6174 6567 6f72 790a 2020 2020  sk_category.    
+00004530: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
+00004540: 7379 7374 656d 5f64 6973 6b5f 7369 7a65  system_disk_size
+00004550: 203d 2063 6c69 656e 745f 7379 7374 656d   = client_system
+00004560: 5f64 6973 6b5f 7369 7a65 0a20 2020 2020  _disk_size.     
+00004570: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
+00004580: 6f6b 656e 203d 2063 6c69 656e 745f 746f  oken = client_to
+00004590: 6b65 6e0a 2020 2020 2020 2020 7365 6c66  ken.        self
+000045a0: 2e63 6c69 656e 745f 7673 7769 7463 685f  .client_vswitch_
+000045b0: 6964 203d 2063 6c69 656e 745f 7673 7769  id = client_vswi
+000045c0: 7463 685f 6964 0a20 2020 2020 2020 2073  tch_id.        s
+000045d0: 656c 662e 636c 6965 6e74 5f7a 6f6e 655f  elf.client_zone_
+000045e0: 6964 203d 2063 6c69 656e 745f 7a6f 6e65  id = client_zone
+000045f0: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+00004600: 2e65 6169 5f69 6e73 7461 6e63 655f 7479  .eai_instance_ty
+00004610: 7065 203d 2065 6169 5f69 6e73 7461 6e63  pe = eai_instanc
+00004620: 655f 7479 7065 0a20 2020 2020 2020 2073  e_type.        s
+00004630: 656c 662e 696e 7374 616e 6365 5f6e 616d  elf.instance_nam
+00004640: 6520 3d20 696e 7374 616e 6365 5f6e 616d  e = instance_nam
+00004650: 650a 2020 2020 2020 2020 7365 6c66 2e72  e.        self.r
+00004660: 6567 696f 6e5f 6964 203d 2072 6567 696f  egion_id = regio
+00004670: 6e5f 6964 0a20 2020 2020 2020 2073 656c  n_id.        sel
+00004680: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
+00004690: 5f69 6420 3d20 7265 736f 7572 6365 5f67  _id = resource_g
+000046a0: 726f 7570 5f69 640a 0a20 2020 2064 6566  roup_id..    def
+000046b0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+000046c0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000046d0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+000046e0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+000046f0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+00004700: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00004710: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00004720: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00004730: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00004740: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00004750: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00004760: 6c66 2e63 6c69 656e 745f 696d 6167 655f  lf.client_image_
+00004770: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00004780: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00004790: 6c74 5b27 436c 6965 6e74 496d 6167 6549  lt['ClientImageI
+000047a0: 6427 5d20 3d20 7365 6c66 2e63 6c69 656e  d'] = self.clien
+000047b0: 745f 696d 6167 655f 6964 0a20 2020 2020  t_image_id.     
+000047c0: 2020 2069 6620 7365 6c66 2e63 6c69 656e     if self.clien
+000047d0: 745f 696e 7374 616e 6365 5f6e 616d 6520  t_instance_name 
+000047e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000047f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00004800: 2743 6c69 656e 7449 6e73 7461 6e63 654e  'ClientInstanceN
+00004810: 616d 6527 5d20 3d20 7365 6c66 2e63 6c69  ame'] = self.cli
+00004820: 656e 745f 696e 7374 616e 6365 5f6e 616d  ent_instance_nam
+00004830: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00004840: 662e 636c 6965 6e74 5f69 6e73 7461 6e63  f.client_instanc
+00004850: 655f 7479 7065 2069 7320 6e6f 7420 4e6f  e_type is not No
+00004860: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00004870: 7265 7375 6c74 5b27 436c 6965 6e74 496e  result['ClientIn
+00004880: 7374 616e 6365 5479 7065 275d 203d 2073  stanceType'] = s
+00004890: 656c 662e 636c 6965 6e74 5f69 6e73 7461  elf.client_insta
+000048a0: 6e63 655f 7479 7065 0a20 2020 2020 2020  nce_type.       
+000048b0: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
+000048c0: 696e 7465 726e 6574 5f6d 6178 5f62 616e  internet_max_ban
+000048d0: 6477 6964 7468 5f69 6e20 6973 206e 6f74  dwidth_in is not
+000048e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000048f0: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
+00004900: 7449 6e74 6572 6e65 744d 6178 4261 6e64  tInternetMaxBand
+00004910: 7769 6474 6849 6e27 5d20 3d20 7365 6c66  widthIn'] = self
+00004920: 2e63 6c69 656e 745f 696e 7465 726e 6574  .client_internet
+00004930: 5f6d 6178 5f62 616e 6477 6964 7468 5f69  _max_bandwidth_i
+00004940: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
+00004950: 662e 636c 6965 6e74 5f69 6e74 6572 6e65  f.client_interne
+00004960: 745f 6d61 785f 6261 6e64 7769 6474 685f  t_max_bandwidth_
+00004970: 6f75 7420 6973 206e 6f74 204e 6f6e 653a  out is not None:
+00004980: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00004990: 756c 745b 2743 6c69 656e 7449 6e74 6572  ult['ClientInter
+000049a0: 6e65 744d 6178 4261 6e64 7769 6474 684f  netMaxBandwidthO
+000049b0: 7574 275d 203d 2073 656c 662e 636c 6965  ut'] = self.clie
+000049c0: 6e74 5f69 6e74 6572 6e65 745f 6d61 785f  nt_internet_max_
+000049d0: 6261 6e64 7769 6474 685f 6f75 740a 2020  bandwidth_out.  
+000049e0: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
+000049f0: 6965 6e74 5f70 6173 7377 6f72 6420 6973  ient_password is
+00004a00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00004a10: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
+00004a20: 6c69 656e 7450 6173 7377 6f72 6427 5d20  lientPassword'] 
+00004a30: 3d20 7365 6c66 2e63 6c69 656e 745f 7061  = self.client_pa
+00004a40: 7373 776f 7264 0a20 2020 2020 2020 2069  ssword.        i
+00004a50: 6620 7365 6c66 2e63 6c69 656e 745f 7365  f self.client_se
+00004a60: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
+00004a70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00004a80: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00004a90: 2743 6c69 656e 7453 6563 7572 6974 7947  'ClientSecurityG
+00004aa0: 726f 7570 4964 275d 203d 2073 656c 662e  roupId'] = self.
+00004ab0: 636c 6965 6e74 5f73 6563 7572 6974 795f  client_security_
+00004ac0: 6772 6f75 705f 6964 0a20 2020 2020 2020  group_id.       
+00004ad0: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
+00004ae0: 7379 7374 656d 5f64 6973 6b5f 6361 7465  system_disk_cate
+00004af0: 676f 7279 2069 7320 6e6f 7420 4e6f 6e65  gory is not None
+00004b00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00004b10: 7375 6c74 5b27 436c 6965 6e74 5379 7374  sult['ClientSyst
+00004b20: 656d 4469 736b 4361 7465 676f 7279 275d  emDiskCategory']
+00004b30: 203d 2073 656c 662e 636c 6965 6e74 5f73   = self.client_s
+00004b40: 7973 7465 6d5f 6469 736b 5f63 6174 6567  ystem_disk_categ
+00004b50: 6f72 790a 2020 2020 2020 2020 6966 2073  ory.        if s
+00004b60: 656c 662e 636c 6965 6e74 5f73 7973 7465  elf.client_syste
+00004b70: 6d5f 6469 736b 5f73 697a 6520 6973 206e  m_disk_size is n
+00004b80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00004b90: 2020 2020 2072 6573 756c 745b 2743 6c69       result['Cli
+00004ba0: 656e 7453 7973 7465 6d44 6973 6b53 697a  entSystemDiskSiz
+00004bb0: 6527 5d20 3d20 7365 6c66 2e63 6c69 656e  e'] = self.clien
+00004bc0: 745f 7379 7374 656d 5f64 6973 6b5f 7369  t_system_disk_si
+00004bd0: 7a65 0a20 2020 2020 2020 2069 6620 7365  ze.        if se
+00004be0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
+00004bf0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00004c00: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00004c10: 2743 6c69 656e 7454 6f6b 656e 275d 203d  'ClientToken'] =
+00004c20: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+00004c30: 656e 0a20 2020 2020 2020 2069 6620 7365  en.        if se
+00004c40: 6c66 2e63 6c69 656e 745f 7673 7769 7463  lf.client_vswitc
+00004c50: 685f 6964 2069 7320 6e6f 7420 4e6f 6e65  h_id is not None
+00004c60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00004c70: 7375 6c74 5b27 436c 6965 6e74 5653 7769  sult['ClientVSwi
+00004c80: 7463 6849 6427 5d20 3d20 7365 6c66 2e63  tchId'] = self.c
+00004c90: 6c69 656e 745f 7673 7769 7463 685f 6964  lient_vswitch_id
+00004ca0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00004cb0: 2e63 6c69 656e 745f 7a6f 6e65 5f69 6420  .client_zone_id 
+00004cc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00004cd0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00004ce0: 2743 6c69 656e 745a 6f6e 6549 6427 5d20  'ClientZoneId'] 
+00004cf0: 3d20 7365 6c66 2e63 6c69 656e 745f 7a6f  = self.client_zo
+00004d00: 6e65 5f69 640a 2020 2020 2020 2020 6966  ne_id.        if
+00004d10: 2073 656c 662e 6561 695f 696e 7374 616e   self.eai_instan
+00004d20: 6365 5f74 7970 6520 6973 206e 6f74 204e  ce_type is not N
+00004d30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00004d40: 2072 6573 756c 745b 2745 6169 496e 7374   result['EaiInst
+00004d50: 616e 6365 5479 7065 275d 203d 2073 656c  anceType'] = sel
+00004d60: 662e 6561 695f 696e 7374 616e 6365 5f74  f.eai_instance_t
+00004d70: 7970 650a 2020 2020 2020 2020 6966 2073  ype.        if s
+00004d80: 656c 662e 696e 7374 616e 6365 5f6e 616d  elf.instance_nam
+00004d90: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00004da0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00004db0: 745b 2749 6e73 7461 6e63 654e 616d 6527  t['InstanceName'
+00004dc0: 5d20 3d20 7365 6c66 2e69 6e73 7461 6e63  ] = self.instanc
+00004dd0: 655f 6e61 6d65 0a20 2020 2020 2020 2069  e_name.        i
+00004de0: 6620 7365 6c66 2e72 6567 696f 6e5f 6964  f self.region_id
+00004df0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00004e00: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00004e10: 5b27 5265 6769 6f6e 4964 275d 203d 2073  ['RegionId'] = s
+00004e20: 656c 662e 7265 6769 6f6e 5f69 640a 2020  elf.region_id.  
+00004e30: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+00004e40: 736f 7572 6365 5f67 726f 7570 5f69 6420  source_group_id 
+00004e50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00004e60: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00004e70: 2752 6573 6f75 7263 6547 726f 7570 4964  'ResourceGroupId
+00004e80: 275d 203d 2073 656c 662e 7265 736f 7572  '] = self.resour
+00004e90: 6365 5f67 726f 7570 5f69 640a 2020 2020  ce_group_id.    
+00004ea0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00004eb0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+00004ec0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+00004ed0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+00004ee0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00004ef0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00004f00: 6765 7428 2743 6c69 656e 7449 6d61 6765  get('ClientImage
+00004f10: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00004f20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00004f30: 6c66 2e63 6c69 656e 745f 696d 6167 655f  lf.client_image_
+00004f40: 6964 203d 206d 2e67 6574 2827 436c 6965  id = m.get('Clie
+00004f50: 6e74 496d 6167 6549 6427 290a 2020 2020  ntImageId').    
+00004f60: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
+00004f70: 6965 6e74 496e 7374 616e 6365 4e61 6d65  ientInstanceName
+00004f80: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00004f90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004fa0: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
+00004fb0: 5f6e 616d 6520 3d20 6d2e 6765 7428 2743  _name = m.get('C
+00004fc0: 6c69 656e 7449 6e73 7461 6e63 654e 616d  lientInstanceNam
+00004fd0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00004fe0: 2e67 6574 2827 436c 6965 6e74 496e 7374  .get('ClientInst
+00004ff0: 616e 6365 5479 7065 2729 2069 7320 6e6f  anceType') is no
+00005000: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00005010: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
+00005020: 696e 7374 616e 6365 5f74 7970 6520 3d20  instance_type = 
+00005030: 6d2e 6765 7428 2743 6c69 656e 7449 6e73  m.get('ClientIns
+00005040: 7461 6e63 6554 7970 6527 290a 2020 2020  tanceType').    
+00005050: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
+00005060: 6965 6e74 496e 7465 726e 6574 4d61 7842  ientInternetMaxB
+00005070: 616e 6477 6964 7468 496e 2729 2069 7320  andwidthIn') is 
+00005080: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00005090: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
+000050a0: 745f 696e 7465 726e 6574 5f6d 6178 5f62  t_internet_max_b
+000050b0: 616e 6477 6964 7468 5f69 6e20 3d20 6d2e  andwidth_in = m.
+000050c0: 6765 7428 2743 6c69 656e 7449 6e74 6572  get('ClientInter
+000050d0: 6e65 744d 6178 4261 6e64 7769 6474 6849  netMaxBandwidthI
+000050e0: 6e27 290a 2020 2020 2020 2020 6966 206d  n').        if m
+000050f0: 2e67 6574 2827 436c 6965 6e74 496e 7465  .get('ClientInte
+00005100: 726e 6574 4d61 7842 616e 6477 6964 7468  rnetMaxBandwidth
+00005110: 4f75 7427 2920 6973 206e 6f74 204e 6f6e  Out') is not Non
+00005120: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00005130: 656c 662e 636c 6965 6e74 5f69 6e74 6572  elf.client_inter
+00005140: 6e65 745f 6d61 785f 6261 6e64 7769 6474  net_max_bandwidt
+00005150: 685f 6f75 7420 3d20 6d2e 6765 7428 2743  h_out = m.get('C
+00005160: 6c69 656e 7449 6e74 6572 6e65 744d 6178  lientInternetMax
+00005170: 4261 6e64 7769 6474 684f 7574 2729 0a20  BandwidthOut'). 
+00005180: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00005190: 2743 6c69 656e 7450 6173 7377 6f72 6427  'ClientPassword'
+000051a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000051b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000051c0: 636c 6965 6e74 5f70 6173 7377 6f72 6420  client_password 
+000051d0: 3d20 6d2e 6765 7428 2743 6c69 656e 7450  = m.get('ClientP
+000051e0: 6173 7377 6f72 6427 290a 2020 2020 2020  assword').      
+000051f0: 2020 6966 206d 2e67 6574 2827 436c 6965    if m.get('Clie
+00005200: 6e74 5365 6375 7269 7479 4772 6f75 7049  ntSecurityGroupI
+00005210: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00005220: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00005230: 662e 636c 6965 6e74 5f73 6563 7572 6974  f.client_securit
+00005240: 795f 6772 6f75 705f 6964 203d 206d 2e67  y_group_id = m.g
+00005250: 6574 2827 436c 6965 6e74 5365 6375 7269  et('ClientSecuri
+00005260: 7479 4772 6f75 7049 6427 290a 2020 2020  tyGroupId').    
+00005270: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
+00005280: 6965 6e74 5379 7374 656d 4469 736b 4361  ientSystemDiskCa
+00005290: 7465 676f 7279 2729 2069 7320 6e6f 7420  tegory') is not 
+000052a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000052b0: 2020 7365 6c66 2e63 6c69 656e 745f 7379    self.client_sy
+000052c0: 7374 656d 5f64 6973 6b5f 6361 7465 676f  stem_disk_catego
+000052d0: 7279 203d 206d 2e67 6574 2827 436c 6965  ry = m.get('Clie
+000052e0: 6e74 5379 7374 656d 4469 736b 4361 7465  ntSystemDiskCate
+000052f0: 676f 7279 2729 0a20 2020 2020 2020 2069  gory').        i
+00005300: 6620 6d2e 6765 7428 2743 6c69 656e 7453  f m.get('ClientS
+00005310: 7973 7465 6d44 6973 6b53 697a 6527 2920  ystemDiskSize') 
+00005320: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00005330: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
+00005340: 6965 6e74 5f73 7973 7465 6d5f 6469 736b  ient_system_disk
+00005350: 5f73 697a 6520 3d20 6d2e 6765 7428 2743  _size = m.get('C
+00005360: 6c69 656e 7453 7973 7465 6d44 6973 6b53  lientSystemDiskS
+00005370: 697a 6527 290a 2020 2020 2020 2020 6966  ize').        if
+00005380: 206d 2e67 6574 2827 436c 6965 6e74 546f   m.get('ClientTo
+00005390: 6b65 6e27 2920 6973 206e 6f74 204e 6f6e  ken') is not Non
+000053a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000053b0: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
+000053c0: 203d 206d 2e67 6574 2827 436c 6965 6e74   = m.get('Client
+000053d0: 546f 6b65 6e27 290a 2020 2020 2020 2020  Token').        
+000053e0: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
+000053f0: 5653 7769 7463 6849 6427 2920 6973 206e  VSwitchId') is n
+00005400: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00005410: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
+00005420: 5f76 7377 6974 6368 5f69 6420 3d20 6d2e  _vswitch_id = m.
+00005430: 6765 7428 2743 6c69 656e 7456 5377 6974  get('ClientVSwit
+00005440: 6368 4964 2729 0a20 2020 2020 2020 2069  chId').        i
+00005450: 6620 6d2e 6765 7428 2743 6c69 656e 745a  f m.get('ClientZ
+00005460: 6f6e 6549 6427 2920 6973 206e 6f74 204e  oneId') is not N
+00005470: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00005480: 2073 656c 662e 636c 6965 6e74 5f7a 6f6e   self.client_zon
+00005490: 655f 6964 203d 206d 2e67 6574 2827 436c  e_id = m.get('Cl
+000054a0: 6965 6e74 5a6f 6e65 4964 2729 0a20 2020  ientZoneId').   
+000054b0: 2020 2020 2069 6620 6d2e 6765 7428 2745       if m.get('E
+000054c0: 6169 496e 7374 616e 6365 5479 7065 2729  aiInstanceType')
+000054d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000054e0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+000054f0: 6169 5f69 6e73 7461 6e63 655f 7479 7065  ai_instance_type
+00005500: 203d 206d 2e67 6574 2827 4561 6949 6e73   = m.get('EaiIns
+00005510: 7461 6e63 6554 7970 6527 290a 2020 2020  tanceType').    
+00005520: 2020 2020 6966 206d 2e67 6574 2827 496e      if m.get('In
+00005530: 7374 616e 6365 4e61 6d65 2729 2069 7320  stanceName') is 
+00005540: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00005550: 2020 2020 2020 7365 6c66 2e69 6e73 7461        self.insta
+00005560: 6e63 655f 6e61 6d65 203d 206d 2e67 6574  nce_name = m.get
+00005570: 2827 496e 7374 616e 6365 4e61 6d65 2729  ('InstanceName')
+00005580: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00005590: 7428 2752 6567 696f 6e49 6427 2920 6973  t('RegionId') is
+000055a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000055b0: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
+000055c0: 6f6e 5f69 6420 3d20 6d2e 6765 7428 2752  on_id = m.get('R
+000055d0: 6567 696f 6e49 6427 290a 2020 2020 2020  egionId').      
+000055e0: 2020 6966 206d 2e67 6574 2827 5265 736f    if m.get('Reso
+000055f0: 7572 6365 4772 6f75 7049 6427 2920 6973  urceGroupId') is
+00005600: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00005610: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
+00005620: 7572 6365 5f67 726f 7570 5f69 6420 3d20  urce_group_id = 
+00005630: 6d2e 6765 7428 2752 6573 6f75 7263 6547  m.get('ResourceG
+00005640: 726f 7570 4964 2729 0a20 2020 2020 2020  roupId').       
+00005650: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00005660: 6c61 7373 2043 7265 6174 6545 6169 416c  lass CreateEaiAl
+00005670: 6c52 6573 706f 6e73 6542 6f64 7928 5465  lResponseBody(Te
+00005680: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00005690: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+000056a0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000056b0: 2063 6c69 656e 745f 696e 7374 616e 6365   client_instance
+000056c0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+000056d0: 0a20 2020 2020 2020 2065 6c61 7374 6963  .        elastic
+000056e0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+000056f0: 7461 6e63 655f 6964 3a20 7374 7220 3d20  tance_id: str = 
+00005700: 4e6f 6e65 2c0a 2020 2020 2020 2020 7265  None,.        re
+00005710: 7175 6573 745f 6964 3a20 7374 7220 3d20  quest_id: str = 
+00005720: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00005730: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
+00005740: 5f69 6e73 7461 6e63 655f 6964 203d 2063  _instance_id = c
+00005750: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
+00005760: 640a 2020 2020 2020 2020 7365 6c66 2e65  d.        self.e
+00005770: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+00005780: 6564 5f69 6e73 7461 6e63 655f 6964 203d  ed_instance_id =
+00005790: 2065 6c61 7374 6963 5f61 6363 656c 6572   elastic_acceler
+000057a0: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
+000057b0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+000057c0: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
+000057d0: 7374 5f69 640a 0a20 2020 2064 6566 2076  st_id..    def v
+000057e0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+000057f0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00005800: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+00005810: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+00005820: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+00005830: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00005840: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00005850: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00005860: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00005870: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00005880: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00005890: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
+000058a0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+000058b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000058c0: 756c 745b 2743 6c69 656e 7449 6e73 7461  ult['ClientInsta
+000058d0: 6e63 6549 6427 5d20 3d20 7365 6c66 2e63  nceId'] = self.c
+000058e0: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
+000058f0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+00005900: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
+00005910: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
+00005920: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00005930: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00005940: 745b 2745 6c61 7374 6963 4163 6365 6c65  t['ElasticAccele
+00005950: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
+00005960: 5d20 3d20 7365 6c66 2e65 6c61 7374 6963  ] = self.elastic
+00005970: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+00005980: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+00005990: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
+000059a0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+000059b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000059c0: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
+000059d0: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+000059e0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+000059f0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00005a00: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00005a10: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00005a20: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00005a30: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00005a40: 2020 6966 206d 2e67 6574 2827 436c 6965    if m.get('Clie
+00005a50: 6e74 496e 7374 616e 6365 4964 2729 2069  ntInstanceId') i
+00005a60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00005a70: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
+00005a80: 656e 745f 696e 7374 616e 6365 5f69 6420  ent_instance_id 
+00005a90: 3d20 6d2e 6765 7428 2743 6c69 656e 7449  = m.get('ClientI
+00005aa0: 6e73 7461 6e63 6549 6427 290a 2020 2020  nstanceId').    
+00005ab0: 2020 2020 6966 206d 2e67 6574 2827 456c      if m.get('El
+00005ac0: 6173 7469 6341 6363 656c 6572 6174 6564  asticAccelerated
+00005ad0: 496e 7374 616e 6365 4964 2729 2069 7320  InstanceId') is 
+00005ae0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00005af0: 2020 2020 2020 7365 6c66 2e65 6c61 7374        self.elast
+00005b00: 6963 5f61 6363 656c 6572 6174 6564 5f69  ic_accelerated_i
+00005b10: 6e73 7461 6e63 655f 6964 203d 206d 2e67  nstance_id = m.g
+00005b20: 6574 2827 456c 6173 7469 6341 6363 656c  et('ElasticAccel
+00005b30: 6572 6174 6564 496e 7374 616e 6365 4964  eratedInstanceId
+00005b40: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00005b50: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+00005b60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00005b70: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00005b80: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
+00005b90: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
+00005ba0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00005bb0: 6c66 0a0a 0a63 6c61 7373 2043 7265 6174  lf...class Creat
+00005bc0: 6545 6169 416c 6c52 6573 706f 6e73 6528  eEaiAllResponse(
+00005bd0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00005be0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00005bf0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00005c00: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
+00005c10: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
+00005c20: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
+00005c30: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
+00005c40: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
+00005c50: 3a20 4372 6561 7465 4561 6941 6c6c 5265  : CreateEaiAllRe
+00005c60: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
+00005c70: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00005c80: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00005c90: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
+00005ca0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00005cb0: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
+00005cc0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00005cd0: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
+00005ce0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00005cf0: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
+00005d00: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00005d10: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
+00005d20: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+00005d30: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00005d40: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
+00005d50: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
+00005d60: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
+00005d70: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00005d80: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
+00005d90: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
+00005da0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00005db0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00005dc0: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00005dd0: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00005de0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00005df0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+00005e00: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00005e10: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00005e20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005e30: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00005e40: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00005e50: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00005e60: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+00005e70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00005e80: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00005e90: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+00005ea0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+00005eb0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00005ec0: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00005ed0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00005ee0: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00005ef0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00005f00: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00005f10: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00005f20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00005f30: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+00005f40: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+00005f50: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00005f60: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00005f70: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00005f80: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00005f90: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00005fa0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00005fb0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00005fc0: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+00005fd0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00005fe0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00005ff0: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+00006000: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+00006010: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00006020: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00006030: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006040: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00006050: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00006060: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00006070: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+00006080: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00006090: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+000060a0: 203d 2043 7265 6174 6545 6169 416c 6c52   = CreateEaiAllR
+000060b0: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
+000060c0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+000060d0: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+000060e0: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+000060f0: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+00006100: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00006110: 2043 7265 6174 6545 6169 4563 6952 6571   CreateEaiEciReq
+00006120: 7565 7374 4563 6943 6f6e 7461 696e 6572  uestEciContainer
+00006130: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00006140: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00006150: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00006160: 2020 2020 6172 673a 2073 7472 203d 204e      arg: str = N
+00006170: 6f6e 652c 0a20 2020 2020 2020 2063 6f6d  one,.        com
+00006180: 6d61 6e64 3a20 7374 7220 3d20 4e6f 6e65  mand: str = None
+00006190: 2c0a 2020 2020 2020 2020 696d 6167 653a  ,.        image:
+000061a0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000061b0: 2020 2020 206e 616d 653a 2073 7472 203d       name: str =
+000061c0: 204e 6f6e 652c 0a20 2020 2020 2020 2076   None,.        v
+000061d0: 6f6c 756d 6573 3a20 7374 7220 3d20 4e6f  olumes: str = No
+000061e0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000061f0: 2020 2073 656c 662e 6172 6720 3d20 6172     self.arg = ar
+00006200: 670a 2020 2020 2020 2020 7365 6c66 2e63  g.        self.c
+00006210: 6f6d 6d61 6e64 203d 2063 6f6d 6d61 6e64  ommand = command
+00006220: 0a20 2020 2020 2020 2073 656c 662e 696d  .        self.im
+00006230: 6167 6520 3d20 696d 6167 650a 2020 2020  age = image.    
+00006240: 2020 2020 7365 6c66 2e6e 616d 6520 3d20      self.name = 
+00006250: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
+00006260: 662e 766f 6c75 6d65 7320 3d20 766f 6c75  f.volumes = volu
+00006270: 6d65 730a 0a20 2020 2064 6566 2076 616c  mes..    def val
+00006280: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00006290: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000062a0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+000062b0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+000062c0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+000062d0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+000062e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000062f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00006300: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00006310: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00006320: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
+00006330: 7267 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rg is not None:.
+00006340: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00006350: 6c74 5b27 4172 6727 5d20 3d20 7365 6c66  lt['Arg'] = self
+00006360: 2e61 7267 0a20 2020 2020 2020 2069 6620  .arg.        if 
+00006370: 7365 6c66 2e63 6f6d 6d61 6e64 2069 7320  self.command is 
+00006380: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00006390: 2020 2020 2020 7265 7375 6c74 5b27 436f        result['Co
+000063a0: 6d6d 616e 6427 5d20 3d20 7365 6c66 2e63  mmand'] = self.c
+000063b0: 6f6d 6d61 6e64 0a20 2020 2020 2020 2069  ommand.        i
+000063c0: 6620 7365 6c66 2e69 6d61 6765 2069 7320  f self.image is 
+000063d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000063e0: 2020 2020 2020 7265 7375 6c74 5b27 496d        result['Im
+000063f0: 6167 6527 5d20 3d20 7365 6c66 2e69 6d61  age'] = self.ima
+00006400: 6765 0a20 2020 2020 2020 2069 6620 7365  ge.        if se
+00006410: 6c66 2e6e 616d 6520 6973 206e 6f74 204e  lf.name is not N
+00006420: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00006430: 2072 6573 756c 745b 274e 616d 6527 5d20   result['Name'] 
+00006440: 3d20 7365 6c66 2e6e 616d 650a 2020 2020  = self.name.    
+00006450: 2020 2020 6966 2073 656c 662e 766f 6c75      if self.volu
+00006460: 6d65 7320 6973 206e 6f74 204e 6f6e 653a  mes is not None:
+00006470: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00006480: 756c 745b 2756 6f6c 756d 6573 275d 203d  ult['Volumes'] =
+00006490: 2073 656c 662e 766f 6c75 6d65 730a 2020   self.volumes.  
+000064a0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000064b0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+000064c0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+000064d0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+000064e0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+000064f0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00006500: 6d2e 6765 7428 2741 7267 2729 2069 7320  m.get('Arg') is 
+00006510: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00006520: 2020 2020 2020 7365 6c66 2e61 7267 203d        self.arg =
+00006530: 206d 2e67 6574 2827 4172 6727 290a 2020   m.get('Arg').  
+00006540: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00006550: 436f 6d6d 616e 6427 2920 6973 206e 6f74  Command') is not
+00006560: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
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
+000066d0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+000066e0: 0a20 2020 2020 2020 2063 6f6e 7461 696e  .        contain
+000066f0: 6572 3a20 4372 6561 7465 4561 6945 6369  er: CreateEaiEci
+00006700: 5265 7175 6573 7445 6369 436f 6e74 6169  RequestEciContai
+00006710: 6e65 7220 3d20 4e6f 6e65 2c0a 2020 2020  ner = None,.    
+00006720: 2020 2020 6569 705f 6964 3a20 7374 7220      eip_id: str 
+00006730: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00006740: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
+00006750: 2c0a 2020 2020 2020 2020 7479 7065 3a20  ,.        type: 
+00006760: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00006770: 2020 2020 766f 6c75 6d65 3a20 7374 7220      volume: str 
+00006780: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+00006790: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+000067a0: 6169 6e65 7220 3d20 636f 6e74 6169 6e65  ainer = containe
+000067b0: 720a 2020 2020 2020 2020 7365 6c66 2e65  r.        self.e
+000067c0: 6970 5f69 6420 3d20 6569 705f 6964 0a20  ip_id = eip_id. 
+000067d0: 2020 2020 2020 2073 656c 662e 6e61 6d65         self.name
+000067e0: 203d 206e 616d 650a 2020 2020 2020 2020   = name.        
+000067f0: 7365 6c66 2e74 7970 6520 3d20 7479 7065  self.type = type
+00006800: 0a20 2020 2020 2020 2073 656c 662e 766f  .        self.vo
+00006810: 6c75 6d65 203d 2076 6f6c 756d 650a 0a20  lume = volume.. 
+00006820: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+00006830: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00006840: 6620 7365 6c66 2e63 6f6e 7461 696e 6572  f self.container
+00006850: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00006860: 6c66 2e63 6f6e 7461 696e 6572 2e76 616c  lf.container.val
+00006870: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+00006880: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00006890: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000068a0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+000068b0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000068c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000068d0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000068e0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+000068f0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00006900: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+00006910: 7461 696e 6572 2069 7320 6e6f 7420 4e6f  tainer is not No
+00006920: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00006930: 7265 7375 6c74 5b27 436f 6e74 6169 6e65  result['Containe
+00006940: 7227 5d20 3d20 7365 6c66 2e63 6f6e 7461  r'] = self.conta
+00006950: 696e 6572 2e74 6f5f 6d61 7028 290a 2020  iner.to_map().  
+00006960: 2020 2020 2020 6966 2073 656c 662e 6569        if self.ei
+00006970: 705f 6964 2069 7320 6e6f 7420 4e6f 6e65  p_id is not None
+00006980: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00006990: 7375 6c74 5b27 4569 7049 6427 5d20 3d20  sult['EipId'] = 
+000069a0: 7365 6c66 2e65 6970 5f69 640a 2020 2020  self.eip_id.    
+000069b0: 2020 2020 6966 2073 656c 662e 6e61 6d65      if self.name
+000069c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000069d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000069e0: 5b27 4e61 6d65 275d 203d 2073 656c 662e  ['Name'] = self.
+000069f0: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
+00006a00: 7365 6c66 2e74 7970 6520 6973 206e 6f74  self.type is not
+00006a10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00006a20: 2020 2072 6573 756c 745b 2754 7970 6527     result['Type'
+00006a30: 5d20 3d20 7365 6c66 2e74 7970 650a 2020  ] = self.type.  
+00006a40: 2020 2020 2020 6966 2073 656c 662e 766f        if self.vo
+00006a50: 6c75 6d65 2069 7320 6e6f 7420 4e6f 6e65  lume is not None
+00006a60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00006a70: 7375 6c74 5b27 566f 6c75 6d65 275d 203d  sult['Volume'] =
+00006a80: 2073 656c 662e 766f 6c75 6d65 0a20 2020   self.volume.   
+00006a90: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00006aa0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00006ab0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+00006ac0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+00006ad0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00006ae0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00006af0: 2e67 6574 2827 436f 6e74 6169 6e65 7227  .get('Container'
+00006b00: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00006b10: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+00006b20: 6d6f 6465 6c20 3d20 4372 6561 7465 4561  model = CreateEa
+00006b30: 6945 6369 5265 7175 6573 7445 6369 436f  iEciRequestEciCo
+00006b40: 6e74 6169 6e65 7228 290a 2020 2020 2020  ntainer().      
+00006b50: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
+00006b60: 696e 6572 203d 2074 656d 705f 6d6f 6465  iner = temp_mode
+00006b70: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 436f  l.from_map(m['Co
+00006b80: 6e74 6169 6e65 7227 5d29 0a20 2020 2020  ntainer']).     
+00006b90: 2020 2069 6620 6d2e 6765 7428 2745 6970     if m.get('Eip
+00006ba0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00006bb0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00006bc0: 6c66 2e65 6970 5f69 6420 3d20 6d2e 6765  lf.eip_id = m.ge
+00006bd0: 7428 2745 6970 4964 2729 0a20 2020 2020  t('EipId').     
+00006be0: 2020 2069 6620 6d2e 6765 7428 274e 616d     if m.get('Nam
+00006bf0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00006c00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00006c10: 662e 6e61 6d65 203d 206d 2e67 6574 2827  f.name = m.get('
+00006c20: 4e61 6d65 2729 0a20 2020 2020 2020 2069  Name').        i
+00006c30: 6620 6d2e 6765 7428 2754 7970 6527 2920  f m.get('Type') 
+00006c40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00006c50: 2020 2020 2020 2020 2073 656c 662e 7479           self.ty
+00006c60: 7065 203d 206d 2e67 6574 2827 5479 7065  pe = m.get('Type
+00006c70: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00006c80: 6765 7428 2756 6f6c 756d 6527 2920 6973  get('Volume') is
+00006c90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00006ca0: 2020 2020 2020 2073 656c 662e 766f 6c75         self.volu
+00006cb0: 6d65 203d 206d 2e67 6574 2827 566f 6c75  me = m.get('Volu
+00006cc0: 6d65 2729 0a20 2020 2020 2020 2072 6574  me').        ret
+00006cd0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00006ce0: 2043 7265 6174 6545 6169 4563 6952 6571   CreateEaiEciReq
+00006cf0: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+00006d00: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00006d10: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00006d20: 2020 2020 2020 2020 636c 6965 6e74 5f74          client_t
+00006d30: 6f6b 656e 3a20 7374 7220 3d20 4e6f 6e65  oken: str = None
+00006d40: 2c0a 2020 2020 2020 2020 6561 6973 5f6e  ,.        eais_n
+00006d50: 616d 653a 2073 7472 203d 204e 6f6e 652c  ame: str = None,
+00006d60: 0a20 2020 2020 2020 2065 6169 735f 7479  .        eais_ty
+00006d70: 7065 3a20 7374 7220 3d20 4e6f 6e65 2c0a  pe: str = None,.
+00006d80: 2020 2020 2020 2020 6563 693a 2043 7265          eci: Cre
+00006d90: 6174 6545 6169 4563 6952 6571 7565 7374  ateEaiEciRequest
+00006da0: 4563 6920 3d20 4e6f 6e65 2c0a 2020 2020  Eci = None,.    
+00006db0: 2020 2020 7265 6769 6f6e 5f69 643a 2073      region_id: s
+00006dc0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+00006dd0: 2020 2072 6573 6f75 7263 655f 6772 6f75     resource_grou
+00006de0: 705f 6964 3a20 7374 7220 3d20 4e6f 6e65  p_id: str = None
+00006df0: 2c0a 2020 2020 2020 2020 7365 6375 7269  ,.        securi
+00006e00: 7479 5f67 726f 7570 5f69 643a 2073 7472  ty_group_id: str
+00006e10: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00006e20: 2076 5f73 7769 7463 685f 6964 3a20 7374   v_switch_id: st
+00006e30: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
+00006e40: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+00006e50: 6965 6e74 5f74 6f6b 656e 203d 2063 6c69  ient_token = cli
+00006e60: 656e 745f 746f 6b65 6e0a 2020 2020 2020  ent_token.      
+00006e70: 2020 7365 6c66 2e65 6169 735f 6e61 6d65    self.eais_name
+00006e80: 203d 2065 6169 735f 6e61 6d65 0a20 2020   = eais_name.   
+00006e90: 2020 2020 2073 656c 662e 6561 6973 5f74       self.eais_t
+00006ea0: 7970 6520 3d20 6561 6973 5f74 7970 650a  ype = eais_type.
+00006eb0: 2020 2020 2020 2020 7365 6c66 2e65 6369          self.eci
+00006ec0: 203d 2065 6369 0a20 2020 2020 2020 2073   = eci.        s
+00006ed0: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
+00006ee0: 7265 6769 6f6e 5f69 640a 2020 2020 2020  region_id.      
+00006ef0: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+00006f00: 6772 6f75 705f 6964 203d 2072 6573 6f75  group_id = resou
+00006f10: 7263 655f 6772 6f75 705f 6964 0a20 2020  rce_group_id.   
+00006f20: 2020 2020 2073 656c 662e 7365 6375 7269       self.securi
+00006f30: 7479 5f67 726f 7570 5f69 6420 3d20 7365  ty_group_id = se
+00006f40: 6375 7269 7479 5f67 726f 7570 5f69 640a  curity_group_id.
+00006f50: 2020 2020 2020 2020 7365 6c66 2e76 5f73          self.v_s
+00006f60: 7769 7463 685f 6964 203d 2076 5f73 7769  witch_id = v_swi
+00006f70: 7463 685f 6964 0a0a 2020 2020 6465 6620  tch_id..    def 
+00006f80: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00006f90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00006fa0: 6563 693a 0a20 2020 2020 2020 2020 2020  eci:.           
+00006fb0: 2073 656c 662e 6563 692e 7661 6c69 6461   self.eci.valida
+00006fc0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+00006fd0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00006fe0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00006ff0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+00007000: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00007010: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00007020: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00007030: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00007040: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00007050: 2020 6966 2073 656c 662e 636c 6965 6e74    if self.client
+00007060: 5f74 6f6b 656e 2069 7320 6e6f 7420 4e6f  _token is not No
+00007070: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00007080: 7265 7375 6c74 5b27 436c 6965 6e74 546f  result['ClientTo
+00007090: 6b65 6e27 5d20 3d20 7365 6c66 2e63 6c69  ken'] = self.cli
+000070a0: 656e 745f 746f 6b65 6e0a 2020 2020 2020  ent_token.      
+000070b0: 2020 6966 2073 656c 662e 6561 6973 5f6e    if self.eais_n
+000070c0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+000070d0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000070e0: 756c 745b 2745 6169 734e 616d 6527 5d20  ult['EaisName'] 
+000070f0: 3d20 7365 6c66 2e65 6169 735f 6e61 6d65  = self.eais_name
+00007100: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00007110: 2e65 6169 735f 7479 7065 2069 7320 6e6f  .eais_type is no
+00007120: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00007130: 2020 2020 7265 7375 6c74 5b27 4561 6973      result['Eais
+00007140: 5479 7065 275d 203d 2073 656c 662e 6561  Type'] = self.ea
+00007150: 6973 5f74 7970 650a 2020 2020 2020 2020  is_type.        
+00007160: 6966 2073 656c 662e 6563 6920 6973 206e  if self.eci is n
+00007170: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00007180: 2020 2020 2072 6573 756c 745b 2745 6369       result['Eci
+00007190: 275d 203d 2073 656c 662e 6563 692e 746f  '] = self.eci.to
+000071a0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000071b0: 6620 7365 6c66 2e72 6567 696f 6e5f 6964  f self.region_id
+000071c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000071d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000071e0: 5b27 5265 6769 6f6e 4964 275d 203d 2073  ['RegionId'] = s
+000071f0: 656c 662e 7265 6769 6f6e 5f69 640a 2020  elf.region_id.  
+00007200: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+00007210: 736f 7572 6365 5f67 726f 7570 5f69 6420  source_group_id 
+00007220: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007230: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00007240: 2752 6573 6f75 7263 6547 726f 7570 4964  'ResourceGroupId
+00007250: 275d 203d 2073 656c 662e 7265 736f 7572  '] = self.resour
+00007260: 6365 5f67 726f 7570 5f69 640a 2020 2020  ce_group_id.    
+00007270: 2020 2020 6966 2073 656c 662e 7365 6375      if self.secu
+00007280: 7269 7479 5f67 726f 7570 5f69 6420 6973  rity_group_id is
+00007290: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000072a0: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
+000072b0: 6563 7572 6974 7947 726f 7570 4964 275d  ecurityGroupId']
+000072c0: 203d 2073 656c 662e 7365 6375 7269 7479   = self.security
+000072d0: 5f67 726f 7570 5f69 640a 2020 2020 2020  _group_id.      
+000072e0: 2020 6966 2073 656c 662e 765f 7377 6974    if self.v_swit
+000072f0: 6368 5f69 6420 6973 206e 6f74 204e 6f6e  ch_id is not Non
+00007300: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00007310: 6573 756c 745b 2756 5377 6974 6368 4964  esult['VSwitchId
+00007320: 275d 203d 2073 656c 662e 765f 7377 6974  '] = self.v_swit
+00007330: 6368 5f69 640a 2020 2020 2020 2020 7265  ch_id.        re
+00007340: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00007350: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00007360: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00007370: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00007380: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00007390: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
+000073a0: 6c69 656e 7454 6f6b 656e 2729 2069 7320  lientToken') is 
+000073b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000073c0: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
+000073d0: 745f 746f 6b65 6e20 3d20 6d2e 6765 7428  t_token = m.get(
+000073e0: 2743 6c69 656e 7454 6f6b 656e 2729 0a20  'ClientToken'). 
+000073f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00007400: 2745 6169 734e 616d 6527 2920 6973 206e  'EaisName') is n
+00007410: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00007420: 2020 2020 2073 656c 662e 6561 6973 5f6e       self.eais_n
+00007430: 616d 6520 3d20 6d2e 6765 7428 2745 6169  ame = m.get('Eai
+00007440: 734e 616d 6527 290a 2020 2020 2020 2020  sName').        
+00007450: 6966 206d 2e67 6574 2827 4561 6973 5479  if m.get('EaisTy
+00007460: 7065 2729 2069 7320 6e6f 7420 4e6f 6e65  pe') is not None
+00007470: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00007480: 6c66 2e65 6169 735f 7479 7065 203d 206d  lf.eais_type = m
+00007490: 2e67 6574 2827 4561 6973 5479 7065 2729  .get('EaisType')
+000074a0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000074b0: 7428 2745 6369 2729 2069 7320 6e6f 7420  t('Eci') is not 
+000074c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000074d0: 2020 7465 6d70 5f6d 6f64 656c 203d 2043    temp_model = C
+000074e0: 7265 6174 6545 6169 4563 6952 6571 7565  reateEaiEciReque
+000074f0: 7374 4563 6928 290a 2020 2020 2020 2020  stEci().        
+00007500: 2020 2020 7365 6c66 2e65 6369 203d 2074      self.eci = t
+00007510: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+00007520: 6170 286d 5b27 4563 6927 5d29 0a20 2020  ap(m['Eci']).   
+00007530: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+00007540: 6567 696f 6e49 6427 2920 6973 206e 6f74  egionId') is not
+00007550: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00007560: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
+00007570: 6420 3d20 6d2e 6765 7428 2752 6567 696f  d = m.get('Regio
+00007580: 6e49 6427 290a 2020 2020 2020 2020 6966  nId').        if
+00007590: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+000075a0: 4772 6f75 7049 6427 2920 6973 206e 6f74  GroupId') is not
+000075b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000075c0: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
+000075d0: 5f67 726f 7570 5f69 6420 3d20 6d2e 6765  _group_id = m.ge
+000075e0: 7428 2752 6573 6f75 7263 6547 726f 7570  t('ResourceGroup
+000075f0: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+00007600: 6d2e 6765 7428 2753 6563 7572 6974 7947  m.get('SecurityG
+00007610: 726f 7570 4964 2729 2069 7320 6e6f 7420  roupId') is not 
+00007620: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00007630: 2020 7365 6c66 2e73 6563 7572 6974 795f    self.security_
+00007640: 6772 6f75 705f 6964 203d 206d 2e67 6574  group_id = m.get
+00007650: 2827 5365 6375 7269 7479 4772 6f75 7049  ('SecurityGroupI
+00007660: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+00007670: 2e67 6574 2827 5653 7769 7463 6849 6427  .get('VSwitchId'
+00007680: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00007690: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000076a0: 765f 7377 6974 6368 5f69 6420 3d20 6d2e  v_switch_id = m.
+000076b0: 6765 7428 2756 5377 6974 6368 4964 2729  get('VSwitchId')
+000076c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000076d0: 7365 6c66 0a0a 0a63 6c61 7373 2043 7265  self...class Cre
+000076e0: 6174 6545 6169 4563 6953 6872 696e 6b52  ateEaiEciShrinkR
+000076f0: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+00007700: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00007710: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00007720: 2c0a 2020 2020 2020 2020 636c 6965 6e74  ,.        client
+00007730: 5f74 6f6b 656e 3a20 7374 7220 3d20 4e6f  _token: str = No
+00007740: 6e65 2c0a 2020 2020 2020 2020 6561 6973  ne,.        eais
+00007750: 5f6e 616d 653a 2073 7472 203d 204e 6f6e  _name: str = Non
+00007760: 652c 0a20 2020 2020 2020 2065 6169 735f  e,.        eais_
+00007770: 7479 7065 3a20 7374 7220 3d20 4e6f 6e65  type: str = None
+00007780: 2c0a 2020 2020 2020 2020 6563 695f 7368  ,.        eci_sh
+00007790: 7269 6e6b 3a20 7374 7220 3d20 4e6f 6e65  rink: str = None
+000077a0: 2c0a 2020 2020 2020 2020 7265 6769 6f6e  ,.        region
+000077b0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+000077c0: 0a20 2020 2020 2020 2072 6573 6f75 7263  .        resourc
+000077d0: 655f 6772 6f75 705f 6964 3a20 7374 7220  e_group_id: str 
+000077e0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000077f0: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
+00007800: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+00007810: 2020 2020 2020 2076 5f73 7769 7463 685f         v_switch_
+00007820: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+00007830: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00007840: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
+00007850: 203d 2063 6c69 656e 745f 746f 6b65 6e0a   = client_token.
+00007860: 2020 2020 2020 2020 7365 6c66 2e65 6169          self.eai
+00007870: 735f 6e61 6d65 203d 2065 6169 735f 6e61  s_name = eais_na
+00007880: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
+00007890: 6561 6973 5f74 7970 6520 3d20 6561 6973  eais_type = eais
+000078a0: 5f74 7970 650a 2020 2020 2020 2020 7365  _type.        se
+000078b0: 6c66 2e65 6369 5f73 6872 696e 6b20 3d20  lf.eci_shrink = 
+000078c0: 6563 695f 7368 7269 6e6b 0a20 2020 2020  eci_shrink.     
+000078d0: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
+000078e0: 6420 3d20 7265 6769 6f6e 5f69 640a 2020  d = region_id.  
+000078f0: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
+00007900: 7263 655f 6772 6f75 705f 6964 203d 2072  rce_group_id = r
+00007910: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
+00007920: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00007930: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
+00007940: 3d20 7365 6375 7269 7479 5f67 726f 7570  = security_group
+00007950: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+00007960: 2e76 5f73 7769 7463 685f 6964 203d 2076  .v_switch_id = v
+00007970: 5f73 7769 7463 685f 6964 0a0a 2020 2020  _switch_id..    
+00007980: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00007990: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+000079a0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+000079b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000079c0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+000079d0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+000079e0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+000079f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007a00: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00007a10: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00007a20: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00007a30: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+00007a40: 656e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  en is not None:.
+00007a50: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00007a60: 6c74 5b27 436c 6965 6e74 546f 6b65 6e27  lt['ClientToken'
+00007a70: 5d20 3d20 7365 6c66 2e63 6c69 656e 745f  ] = self.client_
+00007a80: 746f 6b65 6e0a 2020 2020 2020 2020 6966  token.        if
+00007a90: 2073 656c 662e 6561 6973 5f6e 616d 6520   self.eais_name 
+00007aa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007ab0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00007ac0: 2745 6169 734e 616d 6527 5d20 3d20 7365  'EaisName'] = se
+00007ad0: 6c66 2e65 6169 735f 6e61 6d65 0a20 2020  lf.eais_name.   
+00007ae0: 2020 2020 2069 6620 7365 6c66 2e65 6169       if self.eai
+00007af0: 735f 7479 7065 2069 7320 6e6f 7420 4e6f  s_type is not No
+00007b00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00007b10: 7265 7375 6c74 5b27 4561 6973 5479 7065  result['EaisType
+00007b20: 275d 203d 2073 656c 662e 6561 6973 5f74  '] = self.eais_t
+00007b30: 7970 650a 2020 2020 2020 2020 6966 2073  ype.        if s
+00007b40: 656c 662e 6563 695f 7368 7269 6e6b 2069  elf.eci_shrink i
+00007b50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00007b60: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00007b70: 4563 6927 5d20 3d20 7365 6c66 2e65 6369  Eci'] = self.eci
+00007b80: 5f73 6872 696e 6b0a 2020 2020 2020 2020  _shrink.        
+00007b90: 6966 2073 656c 662e 7265 6769 6f6e 5f69  if self.region_i
+00007ba0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00007bb0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00007bc0: 745b 2752 6567 696f 6e49 6427 5d20 3d20  t['RegionId'] = 
+00007bd0: 7365 6c66 2e72 6567 696f 6e5f 6964 0a20  self.region_id. 
+00007be0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00007bf0: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
+00007c00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00007c10: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00007c20: 5b27 5265 736f 7572 6365 4772 6f75 7049  ['ResourceGroupI
+00007c30: 6427 5d20 3d20 7365 6c66 2e72 6573 6f75  d'] = self.resou
+00007c40: 7263 655f 6772 6f75 705f 6964 0a20 2020  rce_group_id.   
+00007c50: 2020 2020 2069 6620 7365 6c66 2e73 6563       if self.sec
+00007c60: 7572 6974 795f 6772 6f75 705f 6964 2069  urity_group_id i
+00007c70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00007c80: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00007c90: 5365 6375 7269 7479 4772 6f75 7049 6427  SecurityGroupId'
+00007ca0: 5d20 3d20 7365 6c66 2e73 6563 7572 6974  ] = self.securit
+00007cb0: 795f 6772 6f75 705f 6964 0a20 2020 2020  y_group_id.     
+00007cc0: 2020 2069 6620 7365 6c66 2e76 5f73 7769     if self.v_swi
+00007cd0: 7463 685f 6964 2069 7320 6e6f 7420 4e6f  tch_id is not No
+00007ce0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00007cf0: 7265 7375 6c74 5b27 5653 7769 7463 6849  result['VSwitchI
+00007d00: 6427 5d20 3d20 7365 6c66 2e76 5f73 7769  d'] = self.v_swi
+00007d10: 7463 685f 6964 0a20 2020 2020 2020 2072  tch_id.        r
+00007d20: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+00007d30: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+00007d40: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+00007d50: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00007d60: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00007d70: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00007d80: 436c 6965 6e74 546f 6b65 6e27 2920 6973  ClientToken') is
+00007d90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00007da0: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00007db0: 6e74 5f74 6f6b 656e 203d 206d 2e67 6574  nt_token = m.get
+00007dc0: 2827 436c 6965 6e74 546f 6b65 6e27 290a  ('ClientToken').
+00007dd0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00007de0: 2827 4561 6973 4e61 6d65 2729 2069 7320  ('EaisName') is 
+00007df0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00007e00: 2020 2020 2020 7365 6c66 2e65 6169 735f        self.eais_
+00007e10: 6e61 6d65 203d 206d 2e67 6574 2827 4561  name = m.get('Ea
+00007e20: 6973 4e61 6d65 2729 0a20 2020 2020 2020  isName').       
+00007e30: 2069 6620 6d2e 6765 7428 2745 6169 7354   if m.get('EaisT
+00007e40: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
+00007e50: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00007e60: 656c 662e 6561 6973 5f74 7970 6520 3d20  elf.eais_type = 
+00007e70: 6d2e 6765 7428 2745 6169 7354 7970 6527  m.get('EaisType'
+00007e80: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00007e90: 6574 2827 4563 6927 2920 6973 206e 6f74  et('Eci') is not
 00007ea0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007eb0: 2020 2072 6573 756c 745b 2749 6e74 6572     result['Inter
-00007ec0: 6e65 744d 6178 4261 6e64 7769 6474 6849  netMaxBandwidthI
-00007ed0: 6e27 5d20 3d20 7365 6c66 2e69 6e74 6572  n'] = self.inter
-00007ee0: 6e65 745f 6d61 785f 6261 6e64 7769 6474  net_max_bandwidt
-00007ef0: 685f 696e 0a20 2020 2020 2020 2069 6620  h_in.        if 
-00007f00: 7365 6c66 2e69 6e74 6572 6e65 745f 6d61  self.internet_ma
-00007f10: 785f 6261 6e64 7769 6474 685f 6f75 7420  x_bandwidth_out 
-00007f20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00007f30: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00007f40: 2749 6e74 6572 6e65 744d 6178 4261 6e64  'InternetMaxBand
-00007f50: 7769 6474 684f 7574 275d 203d 2073 656c  widthOut'] = sel
-00007f60: 662e 696e 7465 726e 6574 5f6d 6178 5f62  f.internet_max_b
-00007f70: 616e 6477 6964 7468 5f6f 7574 0a20 2020  andwidth_out.   
-00007f80: 2020 2020 2069 6620 7365 6c66 2e6e 616d       if self.nam
-00007f90: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00007fa0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00007fb0: 745b 274e 616d 6527 5d20 3d20 7365 6c66  t['Name'] = self
-00007fc0: 2e6e 616d 650a 2020 2020 2020 2020 6966  .name.        if
-00007fd0: 2073 656c 662e 7061 7373 776f 7264 2069   self.password i
-00007fe0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00007ff0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00008000: 5061 7373 776f 7264 275d 203d 2073 656c  Password'] = sel
-00008010: 662e 7061 7373 776f 7264 0a20 2020 2020  f.password.     
-00008020: 2020 2069 6620 7365 6c66 2e73 7973 7465     if self.syste
-00008030: 6d5f 6469 736b 5f63 6174 6567 6f72 7920  m_disk_category 
-00008040: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00008050: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00008060: 2753 7973 7465 6d44 6973 6b43 6174 6567  'SystemDiskCateg
-00008070: 6f72 7927 5d20 3d20 7365 6c66 2e73 7973  ory'] = self.sys
-00008080: 7465 6d5f 6469 736b 5f63 6174 6567 6f72  tem_disk_categor
-00008090: 790a 2020 2020 2020 2020 6966 2073 656c  y.        if sel
-000080a0: 662e 7379 7374 656d 5f64 6973 6b5f 7369  f.system_disk_si
-000080b0: 7a65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ze is not None:.
-000080c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000080d0: 6c74 5b27 5379 7374 656d 4469 736b 5369  lt['SystemDiskSi
-000080e0: 7a65 275d 203d 2073 656c 662e 7379 7374  ze'] = self.syst
-000080f0: 656d 5f64 6973 6b5f 7369 7a65 0a20 2020  em_disk_size.   
-00008100: 2020 2020 2069 6620 7365 6c66 2e74 7970       if self.typ
-00008110: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00008120: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00008130: 745b 2754 7970 6527 5d20 3d20 7365 6c66  t['Type'] = self
-00008140: 2e74 7970 650a 2020 2020 2020 2020 6966  .type.        if
-00008150: 2073 656c 662e 7a6f 6e65 5f69 6420 6973   self.zone_id is
-00008160: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00008170: 2020 2020 2020 2072 6573 756c 745b 275a         result['Z
-00008180: 6f6e 6549 6427 5d20 3d20 7365 6c66 2e7a  oneId'] = self.z
-00008190: 6f6e 655f 6964 0a20 2020 2020 2020 2072  one_id.        r
-000081a0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-000081b0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000081c0: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-000081d0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-000081e0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-000081f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00008200: 496d 6167 6549 6427 2920 6973 206e 6f74  ImageId') is not
-00008210: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00008220: 2020 2073 656c 662e 696d 6167 655f 6964     self.image_id
-00008230: 203d 206d 2e67 6574 2827 496d 6167 6549   = m.get('ImageI
-00008240: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00008250: 2e67 6574 2827 496e 7465 726e 6574 4d61  .get('InternetMa
-00008260: 7842 616e 6477 6964 7468 496e 2729 2069  xBandwidthIn') i
-00008270: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00008280: 2020 2020 2020 2020 7365 6c66 2e69 6e74          self.int
-00008290: 6572 6e65 745f 6d61 785f 6261 6e64 7769  ernet_max_bandwi
-000082a0: 6474 685f 696e 203d 206d 2e67 6574 2827  dth_in = m.get('
-000082b0: 496e 7465 726e 6574 4d61 7842 616e 6477  InternetMaxBandw
-000082c0: 6964 7468 496e 2729 0a20 2020 2020 2020  idthIn').       
-000082d0: 2069 6620 6d2e 6765 7428 2749 6e74 6572   if m.get('Inter
-000082e0: 6e65 744d 6178 4261 6e64 7769 6474 684f  netMaxBandwidthO
-000082f0: 7574 2729 2069 7320 6e6f 7420 4e6f 6e65  ut') is not None
-00008300: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008310: 6c66 2e69 6e74 6572 6e65 745f 6d61 785f  lf.internet_max_
-00008320: 6261 6e64 7769 6474 685f 6f75 7420 3d20  bandwidth_out = 
-00008330: 6d2e 6765 7428 2749 6e74 6572 6e65 744d  m.get('InternetM
-00008340: 6178 4261 6e64 7769 6474 684f 7574 2729  axBandwidthOut')
-00008350: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00008360: 7428 274e 616d 6527 2920 6973 206e 6f74  t('Name') is not
-00008370: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00008380: 2020 2073 656c 662e 6e61 6d65 203d 206d     self.name = m
-00008390: 2e67 6574 2827 4e61 6d65 2729 0a20 2020  .get('Name').   
-000083a0: 2020 2020 2069 6620 6d2e 6765 7428 2750       if m.get('P
-000083b0: 6173 7377 6f72 6427 2920 6973 206e 6f74  assword') is not
-000083c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000083d0: 2020 2073 656c 662e 7061 7373 776f 7264     self.password
-000083e0: 203d 206d 2e67 6574 2827 5061 7373 776f   = m.get('Passwo
-000083f0: 7264 2729 0a20 2020 2020 2020 2069 6620  rd').        if 
-00008400: 6d2e 6765 7428 2753 7973 7465 6d44 6973  m.get('SystemDis
-00008410: 6b43 6174 6567 6f72 7927 2920 6973 206e  kCategory') is n
-00008420: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00008430: 2020 2020 2073 656c 662e 7379 7374 656d       self.system
-00008440: 5f64 6973 6b5f 6361 7465 676f 7279 203d  _disk_category =
-00008450: 206d 2e67 6574 2827 5379 7374 656d 4469   m.get('SystemDi
-00008460: 736b 4361 7465 676f 7279 2729 0a20 2020  skCategory').   
-00008470: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
-00008480: 7973 7465 6d44 6973 6b53 697a 6527 2920  ystemDiskSize') 
-00008490: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000084a0: 2020 2020 2020 2020 2073 656c 662e 7379           self.sy
-000084b0: 7374 656d 5f64 6973 6b5f 7369 7a65 203d  stem_disk_size =
-000084c0: 206d 2e67 6574 2827 5379 7374 656d 4469   m.get('SystemDi
-000084d0: 736b 5369 7a65 2729 0a20 2020 2020 2020  skSize').       
-000084e0: 2069 6620 6d2e 6765 7428 2754 7970 6527   if m.get('Type'
-000084f0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00008500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008510: 7479 7065 203d 206d 2e67 6574 2827 5479  type = m.get('Ty
-00008520: 7065 2729 0a20 2020 2020 2020 2069 6620  pe').        if 
-00008530: 6d2e 6765 7428 275a 6f6e 6549 6427 2920  m.get('ZoneId') 
-00008540: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00008550: 2020 2020 2020 2020 2073 656c 662e 7a6f           self.zo
-00008560: 6e65 5f69 6420 3d20 6d2e 6765 7428 275a  ne_id = m.get('Z
-00008570: 6f6e 6549 6427 290a 2020 2020 2020 2020  oneId').        
-00008580: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00008590: 6173 7320 4372 6561 7465 4561 6945 6373  ass CreateEaiEcs
-000085a0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
-000085b0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-000085c0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000085d0: 662c 0a20 2020 2020 2020 2063 6c69 656e  f,.        clien
-000085e0: 745f 746f 6b65 6e3a 2073 7472 203d 204e  t_token: str = N
-000085f0: 6f6e 652c 0a20 2020 2020 2020 2065 6169  one,.        eai
-00008600: 735f 6e61 6d65 3a20 7374 7220 3d20 4e6f  s_name: str = No
-00008610: 6e65 2c0a 2020 2020 2020 2020 6561 6973  ne,.        eais
-00008620: 5f74 7970 653a 2073 7472 203d 204e 6f6e  _type: str = Non
-00008630: 652c 0a20 2020 2020 2020 2065 6373 3a20  e,.        ecs: 
-00008640: 4372 6561 7465 4561 6945 6373 5265 7175  CreateEaiEcsRequ
-00008650: 6573 7445 6373 203d 204e 6f6e 652c 0a20  estEcs = None,. 
-00008660: 2020 2020 2020 2072 6567 696f 6e5f 6964         region_id
-00008670: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00008680: 2020 2020 2020 7265 736f 7572 6365 5f67        resource_g
-00008690: 726f 7570 5f69 643a 2073 7472 203d 204e  roup_id: str = N
-000086a0: 6f6e 652c 0a20 2020 2020 2020 2073 6563  one,.        sec
-000086b0: 7572 6974 795f 6772 6f75 705f 6964 3a20  urity_group_id: 
-000086c0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000086d0: 2020 2020 765f 7377 6974 6368 5f69 643a      v_switch_id:
-000086e0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000086f0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-00008700: 2e63 6c69 656e 745f 746f 6b65 6e20 3d20  .client_token = 
-00008710: 636c 6965 6e74 5f74 6f6b 656e 0a20 2020  client_token.   
-00008720: 2020 2020 2073 656c 662e 6561 6973 5f6e       self.eais_n
-00008730: 616d 6520 3d20 6561 6973 5f6e 616d 650a  ame = eais_name.
-00008740: 2020 2020 2020 2020 7365 6c66 2e65 6169          self.eai
-00008750: 735f 7479 7065 203d 2065 6169 735f 7479  s_type = eais_ty
-00008760: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
-00008770: 6563 7320 3d20 6563 730a 2020 2020 2020  ecs = ecs.      
-00008780: 2020 7365 6c66 2e72 6567 696f 6e5f 6964    self.region_id
-00008790: 203d 2072 6567 696f 6e5f 6964 0a20 2020   = region_id.   
-000087a0: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
-000087b0: 6365 5f67 726f 7570 5f69 6420 3d20 7265  ce_group_id = re
-000087c0: 736f 7572 6365 5f67 726f 7570 5f69 640a  source_group_id.
-000087d0: 2020 2020 2020 2020 7365 6c66 2e73 6563          self.sec
-000087e0: 7572 6974 795f 6772 6f75 705f 6964 203d  urity_group_id =
-000087f0: 2073 6563 7572 6974 795f 6772 6f75 705f   security_group_
-00008800: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
-00008810: 765f 7377 6974 6368 5f69 6420 3d20 765f  v_switch_id = v_
-00008820: 7377 6974 6368 5f69 640a 0a20 2020 2064  switch_id..    d
-00008830: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-00008840: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-00008850: 6c66 2e65 6373 3a0a 2020 2020 2020 2020  lf.ecs:.        
-00008860: 2020 2020 7365 6c66 2e65 6373 2e76 616c      self.ecs.val
-00008870: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-00008880: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00008890: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-000088a0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-000088b0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-000088c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000088d0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000088e0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-000088f0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00008900: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
-00008910: 656e 745f 746f 6b65 6e20 6973 206e 6f74  ent_token is not
-00008920: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00008930: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
-00008940: 7454 6f6b 656e 275d 203d 2073 656c 662e  tToken'] = self.
-00008950: 636c 6965 6e74 5f74 6f6b 656e 0a20 2020  client_token.   
-00008960: 2020 2020 2069 6620 7365 6c66 2e65 6169       if self.eai
-00008970: 735f 6e61 6d65 2069 7320 6e6f 7420 4e6f  s_name is not No
-00008980: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00008990: 7265 7375 6c74 5b27 4561 6973 4e61 6d65  result['EaisName
-000089a0: 275d 203d 2073 656c 662e 6561 6973 5f6e  '] = self.eais_n
-000089b0: 616d 650a 2020 2020 2020 2020 6966 2073  ame.        if s
-000089c0: 656c 662e 6561 6973 5f74 7970 6520 6973  elf.eais_type is
-000089d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000089e0: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
-000089f0: 6169 7354 7970 6527 5d20 3d20 7365 6c66  aisType'] = self
-00008a00: 2e65 6169 735f 7479 7065 0a20 2020 2020  .eais_type.     
-00008a10: 2020 2069 6620 7365 6c66 2e65 6373 2069     if self.ecs i
-00008a20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00008a30: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00008a40: 4563 7327 5d20 3d20 7365 6c66 2e65 6373  Ecs'] = self.ecs
-00008a50: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00008a60: 2020 6966 2073 656c 662e 7265 6769 6f6e    if self.region
-00008a70: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00008a80: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00008a90: 756c 745b 2752 6567 696f 6e49 6427 5d20  ult['RegionId'] 
-00008aa0: 3d20 7365 6c66 2e72 6567 696f 6e5f 6964  = self.region_id
-00008ab0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00008ac0: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
-00008ad0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00008ae0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00008af0: 6c74 5b27 5265 736f 7572 6365 4772 6f75  lt['ResourceGrou
-00008b00: 7049 6427 5d20 3d20 7365 6c66 2e72 6573  pId'] = self.res
-00008b10: 6f75 7263 655f 6772 6f75 705f 6964 0a20  ource_group_id. 
-00008b20: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00008b30: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
-00008b40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00008b50: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00008b60: 5b27 5365 6375 7269 7479 4772 6f75 7049  ['SecurityGroupI
-00008b70: 6427 5d20 3d20 7365 6c66 2e73 6563 7572  d'] = self.secur
-00008b80: 6974 795f 6772 6f75 705f 6964 0a20 2020  ity_group_id.   
-00008b90: 2020 2020 2069 6620 7365 6c66 2e76 5f73       if self.v_s
-00008ba0: 7769 7463 685f 6964 2069 7320 6e6f 7420  witch_id is not 
-00008bb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00008bc0: 2020 7265 7375 6c74 5b27 5653 7769 7463    result['VSwitc
-00008bd0: 6849 6427 5d20 3d20 7365 6c66 2e76 5f73  hId'] = self.v_s
-00008be0: 7769 7463 685f 6964 0a20 2020 2020 2020  witch_id.       
-00008bf0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00008c00: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-00008c10: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-00008c20: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00008c30: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00008c40: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00008c50: 2827 436c 6965 6e74 546f 6b65 6e27 2920  ('ClientToken') 
-00008c60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00008c70: 2020 2020 2020 2020 2073 656c 662e 636c           self.cl
-00008c80: 6965 6e74 5f74 6f6b 656e 203d 206d 2e67  ient_token = m.g
-00008c90: 6574 2827 436c 6965 6e74 546f 6b65 6e27  et('ClientToken'
-00008ca0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00008cb0: 6574 2827 4561 6973 4e61 6d65 2729 2069  et('EaisName') i
-00008cc0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00008cd0: 2020 2020 2020 2020 7365 6c66 2e65 6169          self.eai
-00008ce0: 735f 6e61 6d65 203d 206d 2e67 6574 2827  s_name = m.get('
-00008cf0: 4561 6973 4e61 6d65 2729 0a20 2020 2020  EaisName').     
-00008d00: 2020 2069 6620 6d2e 6765 7428 2745 6169     if m.get('Eai
-00008d10: 7354 7970 6527 2920 6973 206e 6f74 204e  sType') is not N
-00008d20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00008d30: 2073 656c 662e 6561 6973 5f74 7970 6520   self.eais_type 
-00008d40: 3d20 6d2e 6765 7428 2745 6169 7354 7970  = m.get('EaisTyp
-00008d50: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-00008d60: 2e67 6574 2827 4563 7327 2920 6973 206e  .get('Ecs') is n
-00008d70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00008d80: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-00008d90: 3d20 4372 6561 7465 4561 6945 6373 5265  = CreateEaiEcsRe
-00008da0: 7175 6573 7445 6373 2829 0a20 2020 2020  questEcs().     
-00008db0: 2020 2020 2020 2073 656c 662e 6563 7320         self.ecs 
-00008dc0: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
-00008dd0: 6d5f 6d61 7028 6d5b 2745 6373 275d 290a  m_map(m['Ecs']).
-00008de0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00008df0: 2827 5265 6769 6f6e 4964 2729 2069 7320  ('RegionId') is 
-00008e00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00008e10: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-00008e20: 6e5f 6964 203d 206d 2e67 6574 2827 5265  n_id = m.get('Re
-00008e30: 6769 6f6e 4964 2729 0a20 2020 2020 2020  gionId').       
-00008e40: 2069 6620 6d2e 6765 7428 2752 6573 6f75   if m.get('Resou
-00008e50: 7263 6547 726f 7570 4964 2729 2069 7320  rceGroupId') is 
-00008e60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00008e70: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
-00008e80: 7263 655f 6772 6f75 705f 6964 203d 206d  rce_group_id = m
-00008e90: 2e67 6574 2827 5265 736f 7572 6365 4772  .get('ResourceGr
-00008ea0: 6f75 7049 6427 290a 2020 2020 2020 2020  oupId').        
-00008eb0: 6966 206d 2e67 6574 2827 5365 6375 7269  if m.get('Securi
-00008ec0: 7479 4772 6f75 7049 6427 2920 6973 206e  tyGroupId') is n
-00008ed0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00008ee0: 2020 2020 2073 656c 662e 7365 6375 7269       self.securi
-00008ef0: 7479 5f67 726f 7570 5f69 6420 3d20 6d2e  ty_group_id = m.
-00008f00: 6765 7428 2753 6563 7572 6974 7947 726f  get('SecurityGro
-00008f10: 7570 4964 2729 0a20 2020 2020 2020 2069  upId').        i
-00008f20: 6620 6d2e 6765 7428 2756 5377 6974 6368  f m.get('VSwitch
-00008f30: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00008f40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00008f50: 6c66 2e76 5f73 7769 7463 685f 6964 203d  lf.v_switch_id =
-00008f60: 206d 2e67 6574 2827 5653 7769 7463 6849   m.get('VSwitchI
-00008f70: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
-00008f80: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00008f90: 4372 6561 7465 4561 6945 6373 5368 7269  CreateEaiEcsShri
-00008fa0: 6e6b 5265 7175 6573 7428 5465 614d 6f64  nkRequest(TeaMod
-00008fb0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-00008fc0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00008fd0: 656c 662c 0a20 2020 2020 2020 2063 6c69  elf,.        cli
-00008fe0: 656e 745f 746f 6b65 6e3a 2073 7472 203d  ent_token: str =
-00008ff0: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
-00009000: 6169 735f 6e61 6d65 3a20 7374 7220 3d20  ais_name: str = 
-00009010: 4e6f 6e65 2c0a 2020 2020 2020 2020 6561  None,.        ea
-00009020: 6973 5f74 7970 653a 2073 7472 203d 204e  is_type: str = N
-00009030: 6f6e 652c 0a20 2020 2020 2020 2065 6373  one,.        ecs
-00009040: 5f73 6872 696e 6b3a 2073 7472 203d 204e  _shrink: str = N
-00009050: 6f6e 652c 0a20 2020 2020 2020 2072 6567  one,.        reg
-00009060: 696f 6e5f 6964 3a20 7374 7220 3d20 4e6f  ion_id: str = No
-00009070: 6e65 2c0a 2020 2020 2020 2020 7265 736f  ne,.        reso
-00009080: 7572 6365 5f67 726f 7570 5f69 643a 2073  urce_group_id: s
-00009090: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000090a0: 2020 2073 6563 7572 6974 795f 6772 6f75     security_grou
-000090b0: 705f 6964 3a20 7374 7220 3d20 4e6f 6e65  p_id: str = None
-000090c0: 2c0a 2020 2020 2020 2020 765f 7377 6974  ,.        v_swit
-000090d0: 6368 5f69 643a 2073 7472 203d 204e 6f6e  ch_id: str = Non
-000090e0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-000090f0: 2020 7365 6c66 2e63 6c69 656e 745f 746f    self.client_to
-00009100: 6b65 6e20 3d20 636c 6965 6e74 5f74 6f6b  ken = client_tok
-00009110: 656e 0a20 2020 2020 2020 2073 656c 662e  en.        self.
-00009120: 6561 6973 5f6e 616d 6520 3d20 6561 6973  eais_name = eais
-00009130: 5f6e 616d 650a 2020 2020 2020 2020 7365  _name.        se
-00009140: 6c66 2e65 6169 735f 7479 7065 203d 2065  lf.eais_type = e
-00009150: 6169 735f 7479 7065 0a20 2020 2020 2020  ais_type.       
-00009160: 2073 656c 662e 6563 735f 7368 7269 6e6b   self.ecs_shrink
-00009170: 203d 2065 6373 5f73 6872 696e 6b0a 2020   = ecs_shrink.  
-00009180: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-00009190: 6e5f 6964 203d 2072 6567 696f 6e5f 6964  n_id = region_id
-000091a0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-000091b0: 736f 7572 6365 5f67 726f 7570 5f69 6420  source_group_id 
-000091c0: 3d20 7265 736f 7572 6365 5f67 726f 7570  = resource_group
-000091d0: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
-000091e0: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
-000091f0: 6964 203d 2073 6563 7572 6974 795f 6772  id = security_gr
-00009200: 6f75 705f 6964 0a20 2020 2020 2020 2073  oup_id.        s
-00009210: 656c 662e 765f 7377 6974 6368 5f69 6420  elf.v_switch_id 
-00009220: 3d20 765f 7377 6974 6368 5f69 640a 0a20  = v_switch_id.. 
-00009230: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00009240: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00009250: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00009260: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00009270: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00009280: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00009290: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-000092a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000092b0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-000092c0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-000092d0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-000092e0: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
-000092f0: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
-00009300: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00009310: 6573 756c 745b 2743 6c69 656e 7454 6f6b  esult['ClientTok
-00009320: 656e 275d 203d 2073 656c 662e 636c 6965  en'] = self.clie
-00009330: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
-00009340: 2069 6620 7365 6c66 2e65 6169 735f 6e61   if self.eais_na
-00009350: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
-00009360: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00009370: 6c74 5b27 4561 6973 4e61 6d65 275d 203d  lt['EaisName'] =
-00009380: 2073 656c 662e 6561 6973 5f6e 616d 650a   self.eais_name.
-00009390: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000093a0: 6561 6973 5f74 7970 6520 6973 206e 6f74  eais_type is not
-000093b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000093c0: 2020 2072 6573 756c 745b 2745 6169 7354     result['EaisT
-000093d0: 7970 6527 5d20 3d20 7365 6c66 2e65 6169  ype'] = self.eai
-000093e0: 735f 7479 7065 0a20 2020 2020 2020 2069  s_type.        i
-000093f0: 6620 7365 6c66 2e65 6373 5f73 6872 696e  f self.ecs_shrin
-00009400: 6b20 6973 206e 6f74 204e 6f6e 653a 0a20  k is not None:. 
-00009410: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00009420: 745b 2745 6373 275d 203d 2073 656c 662e  t['Ecs'] = self.
-00009430: 6563 735f 7368 7269 6e6b 0a20 2020 2020  ecs_shrink.     
-00009440: 2020 2069 6620 7365 6c66 2e72 6567 696f     if self.regio
-00009450: 6e5f 6964 2069 7320 6e6f 7420 4e6f 6e65  n_id is not None
-00009460: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00009470: 7375 6c74 5b27 5265 6769 6f6e 4964 275d  sult['RegionId']
-00009480: 203d 2073 656c 662e 7265 6769 6f6e 5f69   = self.region_i
-00009490: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-000094a0: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
-000094b0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-000094c0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000094d0: 756c 745b 2752 6573 6f75 7263 6547 726f  ult['ResourceGro
-000094e0: 7570 4964 275d 203d 2073 656c 662e 7265  upId'] = self.re
-000094f0: 736f 7572 6365 5f67 726f 7570 5f69 640a  source_group_id.
-00009500: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00009510: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
-00009520: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00009530: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00009540: 745b 2753 6563 7572 6974 7947 726f 7570  t['SecurityGroup
-00009550: 4964 275d 203d 2073 656c 662e 7365 6375  Id'] = self.secu
-00009560: 7269 7479 5f67 726f 7570 5f69 640a 2020  rity_group_id.  
-00009570: 2020 2020 2020 6966 2073 656c 662e 765f        if self.v_
-00009580: 7377 6974 6368 5f69 6420 6973 206e 6f74  switch_id is not
-00009590: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000095a0: 2020 2072 6573 756c 745b 2756 5377 6974     result['VSwit
-000095b0: 6368 4964 275d 203d 2073 656c 662e 765f  chId'] = self.v_
-000095c0: 7377 6974 6368 5f69 640a 2020 2020 2020  switch_id.      
-000095d0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-000095e0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-000095f0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-00009600: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-00009610: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00009620: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00009630: 7428 2743 6c69 656e 7454 6f6b 656e 2729  t('ClientToken')
-00009640: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00009650: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00009660: 6c69 656e 745f 746f 6b65 6e20 3d20 6d2e  lient_token = m.
-00009670: 6765 7428 2743 6c69 656e 7454 6f6b 656e  get('ClientToken
-00009680: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00009690: 6765 7428 2745 6169 734e 616d 6527 2920  get('EaisName') 
-000096a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000096b0: 2020 2020 2020 2020 2073 656c 662e 6561           self.ea
-000096c0: 6973 5f6e 616d 6520 3d20 6d2e 6765 7428  is_name = m.get(
-000096d0: 2745 6169 734e 616d 6527 290a 2020 2020  'EaisName').    
-000096e0: 2020 2020 6966 206d 2e67 6574 2827 4561      if m.get('Ea
-000096f0: 6973 5479 7065 2729 2069 7320 6e6f 7420  isType') is not 
-00009700: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00009710: 2020 7365 6c66 2e65 6169 735f 7479 7065    self.eais_type
-00009720: 203d 206d 2e67 6574 2827 4561 6973 5479   = m.get('EaisTy
-00009730: 7065 2729 0a20 2020 2020 2020 2069 6620  pe').        if 
-00009740: 6d2e 6765 7428 2745 6373 2729 2069 7320  m.get('Ecs') is 
-00009750: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00009760: 2020 2020 2020 7365 6c66 2e65 6373 5f73        self.ecs_s
-00009770: 6872 696e 6b20 3d20 6d2e 6765 7428 2745  hrink = m.get('E
-00009780: 6373 2729 0a20 2020 2020 2020 2069 6620  cs').        if 
-00009790: 6d2e 6765 7428 2752 6567 696f 6e49 6427  m.get('RegionId'
-000097a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000097b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000097c0: 7265 6769 6f6e 5f69 6420 3d20 6d2e 6765  region_id = m.ge
-000097d0: 7428 2752 6567 696f 6e49 6427 290a 2020  t('RegionId').  
-000097e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000097f0: 5265 736f 7572 6365 4772 6f75 7049 6427  ResourceGroupId'
-00009800: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00009810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00009820: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-00009830: 6420 3d20 6d2e 6765 7428 2752 6573 6f75  d = m.get('Resou
-00009840: 7263 6547 726f 7570 4964 2729 0a20 2020  rceGroupId').   
-00009850: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
-00009860: 6563 7572 6974 7947 726f 7570 4964 2729  ecurityGroupId')
-00009870: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00009880: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00009890: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
-000098a0: 203d 206d 2e67 6574 2827 5365 6375 7269   = m.get('Securi
-000098b0: 7479 4772 6f75 7049 6427 290a 2020 2020  tyGroupId').    
-000098c0: 2020 2020 6966 206d 2e67 6574 2827 5653      if m.get('VS
-000098d0: 7769 7463 6849 6427 2920 6973 206e 6f74  witchId') is not
-000098e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000098f0: 2020 2073 656c 662e 765f 7377 6974 6368     self.v_switch
-00009900: 5f69 6420 3d20 6d2e 6765 7428 2756 5377  _id = m.get('VSw
-00009910: 6974 6368 4964 2729 0a20 2020 2020 2020  itchId').       
-00009920: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-00009930: 6c61 7373 2043 7265 6174 6545 6169 4563  lass CreateEaiEc
-00009940: 7352 6573 706f 6e73 6542 6f64 7928 5465  sResponseBody(Te
-00009950: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00009960: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00009970: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00009980: 2063 6c69 656e 745f 696e 7374 616e 6365   client_instance
-00009990: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-000099a0: 0a20 2020 2020 2020 2065 6c61 7374 6963  .        elastic
-000099b0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
-000099c0: 7461 6e63 655f 6964 3a20 7374 7220 3d20  tance_id: str = 
-000099d0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7265  None,.        re
-000099e0: 7175 6573 745f 6964 3a20 7374 7220 3d20  quest_id: str = 
-000099f0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00009a00: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-00009a10: 5f69 6e73 7461 6e63 655f 6964 203d 2063  _instance_id = c
-00009a20: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
-00009a30: 640a 2020 2020 2020 2020 7365 6c66 2e65  d.        self.e
-00009a40: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
-00009a50: 6564 5f69 6e73 7461 6e63 655f 6964 203d  ed_instance_id =
-00009a60: 2065 6c61 7374 6963 5f61 6363 656c 6572   elastic_acceler
-00009a70: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
-00009a80: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00009a90: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
-00009aa0: 7374 5f69 640a 0a20 2020 2064 6566 2076  st_id..    def v
-00009ab0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-00009ac0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00009ad0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-00009ae0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-00009af0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-00009b00: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-00009b10: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-00009b20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009b30: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-00009b40: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-00009b50: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00009b60: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
-00009b70: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00009b80: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00009b90: 756c 745b 2743 6c69 656e 7449 6e73 7461  ult['ClientInsta
-00009ba0: 6e63 6549 6427 5d20 3d20 7365 6c66 2e63  nceId'] = self.c
-00009bb0: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
-00009bc0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00009bd0: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-00009be0: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-00009bf0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00009c00: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00009c10: 745b 2745 6c61 7374 6963 4163 6365 6c65  t['ElasticAccele
-00009c20: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
-00009c30: 5d20 3d20 7365 6c66 2e65 6c61 7374 6963  ] = self.elastic
-00009c40: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
-00009c50: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
-00009c60: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
-00009c70: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00009c80: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00009c90: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
-00009ca0: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
-00009cb0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-00009cc0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00009cd0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00009ce0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-00009cf0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00009d00: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-00009d10: 2020 6966 206d 2e67 6574 2827 436c 6965    if m.get('Clie
-00009d20: 6e74 496e 7374 616e 6365 4964 2729 2069  ntInstanceId') i
-00009d30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00009d40: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-00009d50: 656e 745f 696e 7374 616e 6365 5f69 6420  ent_instance_id 
-00009d60: 3d20 6d2e 6765 7428 2743 6c69 656e 7449  = m.get('ClientI
-00009d70: 6e73 7461 6e63 6549 6427 290a 2020 2020  nstanceId').    
-00009d80: 2020 2020 6966 206d 2e67 6574 2827 456c      if m.get('El
-00009d90: 6173 7469 6341 6363 656c 6572 6174 6564  asticAccelerated
-00009da0: 496e 7374 616e 6365 4964 2729 2069 7320  InstanceId') is 
-00009db0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00009dc0: 2020 2020 2020 7365 6c66 2e65 6c61 7374        self.elast
-00009dd0: 6963 5f61 6363 656c 6572 6174 6564 5f69  ic_accelerated_i
-00009de0: 6e73 7461 6e63 655f 6964 203d 206d 2e67  nstance_id = m.g
-00009df0: 6574 2827 456c 6173 7469 6341 6363 656c  et('ElasticAccel
-00009e00: 6572 6174 6564 496e 7374 616e 6365 4964  eratedInstanceId
-00009e10: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00009e20: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-00009e30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00009e40: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00009e50: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
-00009e60: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
-00009e70: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00009e80: 6c66 0a0a 0a63 6c61 7373 2043 7265 6174  lf...class Creat
-00009e90: 6545 6169 4563 7352 6573 706f 6e73 6528  eEaiEcsResponse(
-00009ea0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00009eb0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00009ec0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00009ed0: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
-00009ee0: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
-00009ef0: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
-00009f00: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
-00009f10: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
-00009f20: 3a20 4372 6561 7465 4561 6945 6373 5265  : CreateEaiEcsRe
-00009f30: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
-00009f40: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00009f50: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-00009f60: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
-00009f70: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00009f80: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
-00009f90: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00009fa0: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
-00009fb0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-00009fc0: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
-00009fd0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
-00009fe0: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
-00009ff0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-0000a000: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
-0000a010: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
-0000a020: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
-0000a030: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
-0000a040: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
-0000a050: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
-0000a060: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
-0000a070: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-0000a080: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000a090: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
-0000a0a0: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-0000a0b0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-0000a0c0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-0000a0d0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0000a0e0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0000a0f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000a100: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0000a110: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0000a120: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0000a130: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-0000a140: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000a150: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000a160: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-0000a170: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-0000a180: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-0000a190: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-0000a1a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000a1b0: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-0000a1c0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-0000a1d0: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-0000a1e0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-0000a1f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000a200: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-0000a210: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-0000a220: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0000a230: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0000a240: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0000a250: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-0000a260: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-0000a270: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-0000a280: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0000a290: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
-0000a2a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000a2b0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-0000a2c0: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
-0000a2d0: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
-0000a2e0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-0000a2f0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-0000a300: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000a310: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-0000a320: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-0000a330: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-0000a340: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
-0000a350: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000a360: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-0000a370: 203d 2043 7265 6174 6545 6169 4563 7352   = CreateEaiEcsR
-0000a380: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
-0000a390: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-0000a3a0: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
-0000a3b0: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
-0000a3c0: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
-0000a3d0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-0000a3e0: 2043 7265 6174 6545 6169 4a75 7079 7465   CreateEaiJupyte
-0000a3f0: 7252 6571 7565 7374 456e 7669 726f 6e6d  rRequestEnvironm
-0000a400: 656e 7456 6172 2854 6561 4d6f 6465 6c29  entVar(TeaModel)
-0000a410: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0000a420: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0000a430: 2c0a 2020 2020 2020 2020 6b65 793a 2073  ,.        key: s
-0000a440: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0000a450: 2020 2076 616c 7565 3a20 7374 7220 3d20     value: str = 
-0000a460: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0000a470: 2020 2020 2073 656c 662e 6b65 7920 3d20       self.key = 
-0000a480: 6b65 790a 2020 2020 2020 2020 7365 6c66  key.        self
-0000a490: 2e76 616c 7565 203d 2076 616c 7565 0a0a  .value = value..
-0000a4a0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0000a4b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000a4c0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-0000a4d0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0000a4e0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0000a4f0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-0000a500: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0000a510: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000a520: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0000a530: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0000a540: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0000a550: 2020 6966 2073 656c 662e 6b65 7920 6973    if self.key is
-0000a560: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000a570: 2020 2020 2020 2072 6573 756c 745b 274b         result['K
-0000a580: 6579 275d 203d 2073 656c 662e 6b65 790a  ey'] = self.key.
-0000a590: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000a5a0: 7661 6c75 6520 6973 206e 6f74 204e 6f6e  value is not Non
-0000a5b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000a5c0: 6573 756c 745b 2756 616c 7565 275d 203d  esult['Value'] =
-0000a5d0: 2073 656c 662e 7661 6c75 650a 2020 2020   self.value.    
-0000a5e0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0000a5f0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-0000a600: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-0000a610: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-0000a620: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0000a630: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0000a640: 6765 7428 274b 6579 2729 2069 7320 6e6f  get('Key') is no
-0000a650: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000a660: 2020 2020 7365 6c66 2e6b 6579 203d 206d      self.key = m
-0000a670: 2e67 6574 2827 4b65 7927 290a 2020 2020  .get('Key').    
-0000a680: 2020 2020 6966 206d 2e67 6574 2827 5661      if m.get('Va
-0000a690: 6c75 6527 2920 6973 206e 6f74 204e 6f6e  lue') is not Non
-0000a6a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000a6b0: 656c 662e 7661 6c75 6520 3d20 6d2e 6765  elf.value = m.ge
-0000a6c0: 7428 2756 616c 7565 2729 0a20 2020 2020  t('Value').     
-0000a6d0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0000a6e0: 0a63 6c61 7373 2043 7265 6174 6545 6169  .class CreateEai
-0000a6f0: 4a75 7079 7465 7252 6571 7565 7374 2854  JupyterRequest(T
-0000a700: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-0000a710: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-0000a720: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000a730: 2020 636c 6965 6e74 5f74 6f6b 656e 3a20    client_token: 
-0000a740: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0000a750: 2020 2020 6561 6973 5f74 7970 653a 2073      eais_type: s
-0000a760: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0000a770: 2020 2065 6e76 6972 6f6e 6d65 6e74 5f76     environment_v
-0000a780: 6172 3a20 4c69 7374 5b43 7265 6174 6545  ar: List[CreateE
-0000a790: 6169 4a75 7079 7465 7252 6571 7565 7374  aiJupyterRequest
-0000a7a0: 456e 7669 726f 6e6d 656e 7456 6172 5d20  EnvironmentVar] 
-0000a7b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000a7c0: 7265 6769 6f6e 5f69 643a 2073 7472 203d  region_id: str =
-0000a7d0: 204e 6f6e 652c 0a20 2020 2020 2020 2072   None,.        r
-0000a7e0: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-0000a7f0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0000a800: 2020 2020 2020 7365 6375 7269 7479 5f67        security_g
-0000a810: 726f 7570 5f69 643a 2073 7472 203d 204e  roup_id: str = N
-0000a820: 6f6e 652c 0a20 2020 2020 2020 2076 5f73  one,.        v_s
-0000a830: 7769 7463 685f 6964 3a20 7374 7220 3d20  witch_id: str = 
-0000a840: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0000a850: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-0000a860: 5f74 6f6b 656e 203d 2063 6c69 656e 745f  _token = client_
-0000a870: 746f 6b65 6e0a 2020 2020 2020 2020 7365  token.        se
-0000a880: 6c66 2e65 6169 735f 7479 7065 203d 2065  lf.eais_type = e
-0000a890: 6169 735f 7479 7065 0a20 2020 2020 2020  ais_type.       
-0000a8a0: 2073 656c 662e 656e 7669 726f 6e6d 656e   self.environmen
-0000a8b0: 745f 7661 7220 3d20 656e 7669 726f 6e6d  t_var = environm
-0000a8c0: 656e 745f 7661 720a 2020 2020 2020 2020  ent_var.        
-0000a8d0: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
-0000a8e0: 2072 6567 696f 6e5f 6964 0a20 2020 2020   region_id.     
-0000a8f0: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
-0000a900: 5f67 726f 7570 5f69 6420 3d20 7265 736f  _group_id = reso
-0000a910: 7572 6365 5f67 726f 7570 5f69 640a 2020  urce_group_id.  
-0000a920: 2020 2020 2020 7365 6c66 2e73 6563 7572        self.secur
-0000a930: 6974 795f 6772 6f75 705f 6964 203d 2073  ity_group_id = s
-0000a940: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
-0000a950: 0a20 2020 2020 2020 2073 656c 662e 765f  .        self.v_
-0000a960: 7377 6974 6368 5f69 6420 3d20 765f 7377  switch_id = v_sw
-0000a970: 6974 6368 5f69 640a 0a20 2020 2064 6566  itch_id..    def
-0000a980: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0000a990: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000a9a0: 2e65 6e76 6972 6f6e 6d65 6e74 5f76 6172  .environment_var
-0000a9b0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0000a9c0: 7220 6b20 696e 2073 656c 662e 656e 7669  r k in self.envi
-0000a9d0: 726f 6e6d 656e 745f 7661 723a 0a20 2020  ronment_var:.   
-0000a9e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000a9f0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
-0000aa00: 2020 2020 2020 206b 2e76 616c 6964 6174         k.validat
-0000aa10: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-0000aa20: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0000aa30: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0000aa40: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0000aa50: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0000aa60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000aa70: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0000aa80: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0000aa90: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0000aaa0: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
-0000aab0: 746f 6b65 6e20 6973 206e 6f74 204e 6f6e  token is not Non
-0000aac0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000aad0: 6573 756c 745b 2743 6c69 656e 7454 6f6b  esult['ClientTok
-0000aae0: 656e 275d 203d 2073 656c 662e 636c 6965  en'] = self.clie
-0000aaf0: 6e74 5f74 6f6b 656e 0a20 2020 2020 2020  nt_token.       
-0000ab00: 2069 6620 7365 6c66 2e65 6169 735f 7479   if self.eais_ty
-0000ab10: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
-0000ab20: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000ab30: 6c74 5b27 4561 6973 5479 7065 275d 203d  lt['EaisType'] =
-0000ab40: 2073 656c 662e 6561 6973 5f74 7970 650a   self.eais_type.
-0000ab50: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0000ab60: 456e 7669 726f 6e6d 656e 7456 6172 275d  EnvironmentVar']
-0000ab70: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
-0000ab80: 2073 656c 662e 656e 7669 726f 6e6d 656e   self.environmen
-0000ab90: 745f 7661 7220 6973 206e 6f74 204e 6f6e  t_var is not Non
-0000aba0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-0000abb0: 6f72 206b 2069 6e20 7365 6c66 2e65 6e76  or k in self.env
-0000abc0: 6972 6f6e 6d65 6e74 5f76 6172 3a0a 2020  ironment_var:.  
-0000abd0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000abe0: 7375 6c74 5b27 456e 7669 726f 6e6d 656e  sult['Environmen
-0000abf0: 7456 6172 275d 2e61 7070 656e 6428 6b2e  tVar'].append(k.
-0000ac00: 746f 5f6d 6170 2829 2069 6620 6b20 656c  to_map() if k el
-0000ac10: 7365 204e 6f6e 6529 0a20 2020 2020 2020  se None).       
-0000ac20: 2069 6620 7365 6c66 2e72 6567 696f 6e5f   if self.region_
-0000ac30: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0000ac40: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000ac50: 6c74 5b27 5265 6769 6f6e 4964 275d 203d  lt['RegionId'] =
-0000ac60: 2073 656c 662e 7265 6769 6f6e 5f69 640a   self.region_id.
-0000ac70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000ac80: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-0000ac90: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-0000aca0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000acb0: 745b 2752 6573 6f75 7263 6547 726f 7570  t['ResourceGroup
-0000acc0: 4964 275d 203d 2073 656c 662e 7265 736f  Id'] = self.reso
-0000acd0: 7572 6365 5f67 726f 7570 5f69 640a 2020  urce_group_id.  
-0000ace0: 2020 2020 2020 6966 2073 656c 662e 7365        if self.se
-0000acf0: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
-0000ad00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000ad10: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000ad20: 2753 6563 7572 6974 7947 726f 7570 4964  'SecurityGroupId
-0000ad30: 275d 203d 2073 656c 662e 7365 6375 7269  '] = self.securi
-0000ad40: 7479 5f67 726f 7570 5f69 640a 2020 2020  ty_group_id.    
-0000ad50: 2020 2020 6966 2073 656c 662e 765f 7377      if self.v_sw
-0000ad60: 6974 6368 5f69 6420 6973 206e 6f74 204e  itch_id is not N
-0000ad70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000ad80: 2072 6573 756c 745b 2756 5377 6974 6368   result['VSwitch
-0000ad90: 4964 275d 203d 2073 656c 662e 765f 7377  Id'] = self.v_sw
-0000ada0: 6974 6368 5f69 640a 2020 2020 2020 2020  itch_id.        
-0000adb0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0000adc0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0000add0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-0000ade0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-0000adf0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-0000ae00: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0000ae10: 2743 6c69 656e 7454 6f6b 656e 2729 2069  'ClientToken') i
-0000ae20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000ae30: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
-0000ae40: 656e 745f 746f 6b65 6e20 3d20 6d2e 6765  ent_token = m.ge
-0000ae50: 7428 2743 6c69 656e 7454 6f6b 656e 2729  t('ClientToken')
-0000ae60: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0000ae70: 7428 2745 6169 7354 7970 6527 2920 6973  t('EaisType') is
-0000ae80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000ae90: 2020 2020 2020 2073 656c 662e 6561 6973         self.eais
-0000aea0: 5f74 7970 6520 3d20 6d2e 6765 7428 2745  _type = m.get('E
-0000aeb0: 6169 7354 7970 6527 290a 2020 2020 2020  aisType').      
-0000aec0: 2020 7365 6c66 2e65 6e76 6972 6f6e 6d65    self.environme
-0000aed0: 6e74 5f76 6172 203d 205b 5d0a 2020 2020  nt_var = [].    
-0000aee0: 2020 2020 6966 206d 2e67 6574 2827 456e      if m.get('En
-0000aef0: 7669 726f 6e6d 656e 7456 6172 2729 2069  vironmentVar') i
-0000af00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000af10: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-0000af20: 206d 2e67 6574 2827 456e 7669 726f 6e6d   m.get('Environm
-0000af30: 656e 7456 6172 2729 3a0a 2020 2020 2020  entVar'):.      
-0000af40: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-0000af50: 6f64 656c 203d 2043 7265 6174 6545 6169  odel = CreateEai
-0000af60: 4a75 7079 7465 7252 6571 7565 7374 456e  JupyterRequestEn
-0000af70: 7669 726f 6e6d 656e 7456 6172 2829 0a20  vironmentVar(). 
-0000af80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000af90: 656c 662e 656e 7669 726f 6e6d 656e 745f  elf.environment_
-0000afa0: 7661 722e 6170 7065 6e64 2874 656d 705f  var.append(temp_
-0000afb0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286b  model.from_map(k
-0000afc0: 2929 0a20 2020 2020 2020 2069 6620 6d2e  )).        if m.
-0000afd0: 6765 7428 2752 6567 696f 6e49 6427 2920  get('RegionId') 
-0000afe0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000aff0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0000b000: 6769 6f6e 5f69 6420 3d20 6d2e 6765 7428  gion_id = m.get(
-0000b010: 2752 6567 696f 6e49 6427 290a 2020 2020  'RegionId').    
-0000b020: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-0000b030: 736f 7572 6365 4772 6f75 7049 6427 2920  sourceGroupId') 
-0000b040: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000b050: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0000b060: 736f 7572 6365 5f67 726f 7570 5f69 6420  source_group_id 
-0000b070: 3d20 6d2e 6765 7428 2752 6573 6f75 7263  = m.get('Resourc
-0000b080: 6547 726f 7570 4964 2729 0a20 2020 2020  eGroupId').     
-0000b090: 2020 2069 6620 6d2e 6765 7428 2753 6563     if m.get('Sec
-0000b0a0: 7572 6974 7947 726f 7570 4964 2729 2069  urityGroupId') i
-0000b0b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000b0c0: 2020 2020 2020 2020 7365 6c66 2e73 6563          self.sec
-0000b0d0: 7572 6974 795f 6772 6f75 705f 6964 203d  urity_group_id =
-0000b0e0: 206d 2e67 6574 2827 5365 6375 7269 7479   m.get('Security
-0000b0f0: 4772 6f75 7049 6427 290a 2020 2020 2020  GroupId').      
-0000b100: 2020 6966 206d 2e67 6574 2827 5653 7769    if m.get('VSwi
-0000b110: 7463 6849 6427 2920 6973 206e 6f74 204e  tchId') is not N
-0000b120: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000b130: 2073 656c 662e 765f 7377 6974 6368 5f69   self.v_switch_i
-0000b140: 6420 3d20 6d2e 6765 7428 2756 5377 6974  d = m.get('VSwit
-0000b150: 6368 4964 2729 0a20 2020 2020 2020 2072  chId').        r
-0000b160: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-0000b170: 7373 2043 7265 6174 6545 6169 4a75 7079  ss CreateEaiJupy
-0000b180: 7465 7253 6872 696e 6b52 6571 7565 7374  terShrinkRequest
-0000b190: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-0000b1a0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-0000b1b0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000b1c0: 2020 2020 636c 6965 6e74 5f74 6f6b 656e      client_token
-0000b1d0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0000b1e0: 2020 2020 2020 6561 6973 5f74 7970 653a        eais_type:
-0000b1f0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0000b200: 2020 2020 2065 6e76 6972 6f6e 6d65 6e74       environment
-0000b210: 5f76 6172 5f73 6872 696e 6b3a 2073 7472  _var_shrink: str
-0000b220: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000b230: 2072 6567 696f 6e5f 6964 3a20 7374 7220   region_id: str 
-0000b240: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000b250: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-0000b260: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-0000b270: 2020 2020 2020 2073 6563 7572 6974 795f         security_
-0000b280: 6772 6f75 705f 6964 3a20 7374 7220 3d20  group_id: str = 
-0000b290: 4e6f 6e65 2c0a 2020 2020 2020 2020 765f  None,.        v_
-0000b2a0: 7377 6974 6368 5f69 643a 2073 7472 203d  switch_id: str =
-0000b2b0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-0000b2c0: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-0000b2d0: 745f 746f 6b65 6e20 3d20 636c 6965 6e74  t_token = client
-0000b2e0: 5f74 6f6b 656e 0a20 2020 2020 2020 2073  _token.        s
-0000b2f0: 656c 662e 6561 6973 5f74 7970 6520 3d20  elf.eais_type = 
-0000b300: 6561 6973 5f74 7970 650a 2020 2020 2020  eais_type.      
-0000b310: 2020 7365 6c66 2e65 6e76 6972 6f6e 6d65    self.environme
-0000b320: 6e74 5f76 6172 5f73 6872 696e 6b20 3d20  nt_var_shrink = 
-0000b330: 656e 7669 726f 6e6d 656e 745f 7661 725f  environment_var_
-0000b340: 7368 7269 6e6b 0a20 2020 2020 2020 2073  shrink.        s
-0000b350: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
-0000b360: 7265 6769 6f6e 5f69 640a 2020 2020 2020  region_id.      
-0000b370: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
-0000b380: 6772 6f75 705f 6964 203d 2072 6573 6f75  group_id = resou
-0000b390: 7263 655f 6772 6f75 705f 6964 0a20 2020  rce_group_id.   
-0000b3a0: 2020 2020 2073 656c 662e 7365 6375 7269       self.securi
-0000b3b0: 7479 5f67 726f 7570 5f69 6420 3d20 7365  ty_group_id = se
-0000b3c0: 6375 7269 7479 5f67 726f 7570 5f69 640a  curity_group_id.
-0000b3d0: 2020 2020 2020 2020 7365 6c66 2e76 5f73          self.v_s
-0000b3e0: 7769 7463 685f 6964 203d 2076 5f73 7769  witch_id = v_swi
-0000b3f0: 7463 685f 6964 0a0a 2020 2020 6465 6620  tch_id..    def 
-0000b400: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0000b410: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0000b420: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0000b430: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0000b440: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-0000b450: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0000b460: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0000b470: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000b480: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0000b490: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0000b4a0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000b4b0: 662e 636c 6965 6e74 5f74 6f6b 656e 2069  f.client_token i
-0000b4c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000b4d0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0000b4e0: 436c 6965 6e74 546f 6b65 6e27 5d20 3d20  ClientToken'] = 
-0000b4f0: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
-0000b500: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-0000b510: 662e 6561 6973 5f74 7970 6520 6973 206e  f.eais_type is n
-0000b520: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000b530: 2020 2020 2072 6573 756c 745b 2745 6169       result['Eai
-0000b540: 7354 7970 6527 5d20 3d20 7365 6c66 2e65  sType'] = self.e
-0000b550: 6169 735f 7479 7065 0a20 2020 2020 2020  ais_type.       
-0000b560: 2069 6620 7365 6c66 2e65 6e76 6972 6f6e   if self.environ
-0000b570: 6d65 6e74 5f76 6172 5f73 6872 696e 6b20  ment_var_shrink 
-0000b580: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000b590: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000b5a0: 2745 6e76 6972 6f6e 6d65 6e74 5661 7227  'EnvironmentVar'
-0000b5b0: 5d20 3d20 7365 6c66 2e65 6e76 6972 6f6e  ] = self.environ
-0000b5c0: 6d65 6e74 5f76 6172 5f73 6872 696e 6b0a  ment_var_shrink.
-0000b5d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b5e0: 7265 6769 6f6e 5f69 6420 6973 206e 6f74  region_id is not
-0000b5f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000b600: 2020 2072 6573 756c 745b 2752 6567 696f     result['Regio
-0000b610: 6e49 6427 5d20 3d20 7365 6c66 2e72 6567  nId'] = self.reg
-0000b620: 696f 6e5f 6964 0a20 2020 2020 2020 2069  ion_id.        i
-0000b630: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
-0000b640: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
-0000b650: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000b660: 2020 7265 7375 6c74 5b27 5265 736f 7572    result['Resour
-0000b670: 6365 4772 6f75 7049 6427 5d20 3d20 7365  ceGroupId'] = se
-0000b680: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
-0000b690: 705f 6964 0a20 2020 2020 2020 2069 6620  p_id.        if 
-0000b6a0: 7365 6c66 2e73 6563 7572 6974 795f 6772  self.security_gr
-0000b6b0: 6f75 705f 6964 2069 7320 6e6f 7420 4e6f  oup_id is not No
-0000b6c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000b6d0: 7265 7375 6c74 5b27 5365 6375 7269 7479  result['Security
-0000b6e0: 4772 6f75 7049 6427 5d20 3d20 7365 6c66  GroupId'] = self
-0000b6f0: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
-0000b700: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-0000b710: 6c66 2e76 5f73 7769 7463 685f 6964 2069  lf.v_switch_id i
-0000b720: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000b730: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0000b740: 5653 7769 7463 6849 6427 5d20 3d20 7365  VSwitchId'] = se
-0000b750: 6c66 2e76 5f73 7769 7463 685f 6964 0a20  lf.v_switch_id. 
-0000b760: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0000b770: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0000b780: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-0000b790: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-0000b7a0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0000b7b0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0000b7c0: 206d 2e67 6574 2827 436c 6965 6e74 546f   m.get('ClientTo
-0000b7d0: 6b65 6e27 2920 6973 206e 6f74 204e 6f6e  ken') is not Non
-0000b7e0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000b7f0: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
-0000b800: 203d 206d 2e67 6574 2827 436c 6965 6e74   = m.get('Client
-0000b810: 546f 6b65 6e27 290a 2020 2020 2020 2020  Token').        
-0000b820: 6966 206d 2e67 6574 2827 4561 6973 5479  if m.get('EaisTy
-0000b830: 7065 2729 2069 7320 6e6f 7420 4e6f 6e65  pe') is not None
-0000b840: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000b850: 6c66 2e65 6169 735f 7479 7065 203d 206d  lf.eais_type = m
-0000b860: 2e67 6574 2827 4561 6973 5479 7065 2729  .get('EaisType')
-0000b870: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0000b880: 7428 2745 6e76 6972 6f6e 6d65 6e74 5661  t('EnvironmentVa
-0000b890: 7227 2920 6973 206e 6f74 204e 6f6e 653a  r') is not None:
-0000b8a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000b8b0: 662e 656e 7669 726f 6e6d 656e 745f 7661  f.environment_va
-0000b8c0: 725f 7368 7269 6e6b 203d 206d 2e67 6574  r_shrink = m.get
-0000b8d0: 2827 456e 7669 726f 6e6d 656e 7456 6172  ('EnvironmentVar
-0000b8e0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0000b8f0: 6765 7428 2752 6567 696f 6e49 6427 2920  get('RegionId') 
-0000b900: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000b910: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0000b920: 6769 6f6e 5f69 6420 3d20 6d2e 6765 7428  gion_id = m.get(
-0000b930: 2752 6567 696f 6e49 6427 290a 2020 2020  'RegionId').    
-0000b940: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-0000b950: 736f 7572 6365 4772 6f75 7049 6427 2920  sourceGroupId') 
-0000b960: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000b970: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0000b980: 736f 7572 6365 5f67 726f 7570 5f69 6420  source_group_id 
-0000b990: 3d20 6d2e 6765 7428 2752 6573 6f75 7263  = m.get('Resourc
-0000b9a0: 6547 726f 7570 4964 2729 0a20 2020 2020  eGroupId').     
-0000b9b0: 2020 2069 6620 6d2e 6765 7428 2753 6563     if m.get('Sec
-0000b9c0: 7572 6974 7947 726f 7570 4964 2729 2069  urityGroupId') i
-0000b9d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000b9e0: 2020 2020 2020 2020 7365 6c66 2e73 6563          self.sec
-0000b9f0: 7572 6974 795f 6772 6f75 705f 6964 203d  urity_group_id =
-0000ba00: 206d 2e67 6574 2827 5365 6375 7269 7479   m.get('Security
-0000ba10: 4772 6f75 7049 6427 290a 2020 2020 2020  GroupId').      
-0000ba20: 2020 6966 206d 2e67 6574 2827 5653 7769    if m.get('VSwi
-0000ba30: 7463 6849 6427 2920 6973 206e 6f74 204e  tchId') is not N
-0000ba40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000ba50: 2073 656c 662e 765f 7377 6974 6368 5f69   self.v_switch_i
-0000ba60: 6420 3d20 6d2e 6765 7428 2756 5377 6974  d = m.get('VSwit
-0000ba70: 6368 4964 2729 0a20 2020 2020 2020 2072  chId').        r
-0000ba80: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-0000ba90: 7373 2043 7265 6174 6545 6169 4a75 7079  ss CreateEaiJupy
-0000baa0: 7465 7252 6573 706f 6e73 6542 6f64 7928  terResponseBody(
-0000bab0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0000bac0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0000bad0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000bae0: 2020 2065 6c61 7374 6963 5f61 6363 656c     elastic_accel
-0000baf0: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
-0000bb00: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-0000bb10: 2020 2020 2020 2020 7265 7175 6573 745f          request_
-0000bb20: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-0000bb30: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-0000bb40: 656c 662e 656c 6173 7469 635f 6163 6365  elf.elastic_acce
-0000bb50: 6c65 7261 7465 645f 696e 7374 616e 6365  lerated_instance
-0000bb60: 5f69 6420 3d20 656c 6173 7469 635f 6163  _id = elastic_ac
-0000bb70: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
-0000bb80: 6365 5f69 640a 2020 2020 2020 2020 7365  ce_id.        se
-0000bb90: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-0000bba0: 7265 7175 6573 745f 6964 0a0a 2020 2020  request_id..    
-0000bbb0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0000bbc0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-0000bbd0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-0000bbe0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000bbf0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-0000bc00: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0000bc10: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-0000bc20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000bc30: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-0000bc40: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-0000bc50: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0000bc60: 2073 656c 662e 656c 6173 7469 635f 6163   self.elastic_ac
-0000bc70: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
-0000bc80: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
-0000bc90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000bca0: 6573 756c 745b 2745 6c61 7374 6963 4163  esult['ElasticAc
-0000bcb0: 6365 6c65 7261 7465 6449 6e73 7461 6e63  celeratedInstanc
-0000bcc0: 6549 6427 5d20 3d20 7365 6c66 2e65 6c61  eId'] = self.ela
-0000bcd0: 7374 6963 5f61 6363 656c 6572 6174 6564  stic_accelerated
-0000bce0: 5f69 6e73 7461 6e63 655f 6964 0a20 2020  _instance_id.   
-0000bcf0: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
-0000bd00: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
-0000bd10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000bd20: 2072 6573 756c 745b 2752 6571 7565 7374   result['Request
-0000bd30: 4964 275d 203d 2073 656c 662e 7265 7175  Id'] = self.requ
-0000bd40: 6573 745f 6964 0a20 2020 2020 2020 2072  est_id.        r
-0000bd50: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-0000bd60: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-0000bd70: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-0000bd80: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0000bd90: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0000bda0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0000bdb0: 456c 6173 7469 6341 6363 656c 6572 6174  ElasticAccelerat
-0000bdc0: 6564 496e 7374 616e 6365 4964 2729 2069  edInstanceId') i
-0000bdd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000bde0: 2020 2020 2020 2020 7365 6c66 2e65 6c61          self.ela
-0000bdf0: 7374 6963 5f61 6363 656c 6572 6174 6564  stic_accelerated
-0000be00: 5f69 6e73 7461 6e63 655f 6964 203d 206d  _instance_id = m
-0000be10: 2e67 6574 2827 456c 6173 7469 6341 6363  .get('ElasticAcc
-0000be20: 656c 6572 6174 6564 496e 7374 616e 6365  eleratedInstance
-0000be30: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-0000be40: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-0000be50: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0000be60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000be70: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
-0000be80: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-0000be90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000bea0: 7365 6c66 0a0a 0a63 6c61 7373 2043 7265  self...class Cre
-0000beb0: 6174 6545 6169 4a75 7079 7465 7252 6573  ateEaiJupyterRes
-0000bec0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-0000bed0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000bee0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-0000bef0: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-0000bf00: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-0000bf10: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000bf20: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-0000bf30: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-0000bf40: 2020 626f 6479 3a20 4372 6561 7465 4561    body: CreateEa
-0000bf50: 694a 7570 7974 6572 5265 7370 6f6e 7365  iJupyterResponse
-0000bf60: 426f 6479 203d 204e 6f6e 652c 0a20 2020  Body = None,.   
-0000bf70: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-0000bf80: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
-0000bf90: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
-0000bfa0: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
-0000bfb0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-0000bfc0: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-0000bfd0: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
-0000bfe0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-0000bff0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0000c000: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0000c010: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
-0000c020: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
-0000c030: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0000c040: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
-0000c050: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
-0000c060: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
-0000c070: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0000c080: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
-0000c090: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
-0000c0a0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-0000c0b0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0000c0c0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-0000c0d0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0000c0e0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0000c0f0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-0000c100: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0000c110: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0000c120: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000c130: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0000c140: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0000c150: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000c160: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-0000c170: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000c180: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-0000c190: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-0000c1a0: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-0000c1b0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0000c1c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000c1d0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000c1e0: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-0000c1f0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0000c200: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000c210: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-0000c220: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000c230: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-0000c240: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-0000c250: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-0000c260: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0000c270: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0000c280: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-0000c290: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-0000c2a0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-0000c2b0: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-0000c2c0: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-0000c2d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000c2e0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-0000c2f0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-0000c300: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0000c310: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-0000c320: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000c330: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000c340: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-0000c350: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-0000c360: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0000c370: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-0000c380: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000c390: 7465 6d70 5f6d 6f64 656c 203d 2043 7265  temp_model = Cre
-0000c3a0: 6174 6545 6169 4a75 7079 7465 7252 6573  ateEaiJupyterRes
-0000c3b0: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
-0000c3c0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0000c3d0: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
-0000c3e0: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
-0000c3f0: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-0000c400: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2044  n self...class D
-0000c410: 656c 6574 6545 6169 5265 7175 6573 7428  eleteEaiRequest(
-0000c420: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0000c430: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0000c440: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000c450: 2020 2065 6c61 7374 6963 5f61 6363 656c     elastic_accel
-0000c460: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
-0000c470: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-0000c480: 2020 2020 2020 2020 666f 7263 653a 2062          force: b
-0000c490: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
-0000c4a0: 2020 2020 7265 6769 6f6e 5f69 643a 2073      region_id: s
-0000c4b0: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
-0000c4c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e65  :.        self.e
-0000c4d0: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
-0000c4e0: 6564 5f69 6e73 7461 6e63 655f 6964 203d  ed_instance_id =
-0000c4f0: 2065 6c61 7374 6963 5f61 6363 656c 6572   elastic_acceler
-0000c500: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
-0000c510: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
-0000c520: 7263 6520 3d20 666f 7263 650a 2020 2020  rce = force.    
-0000c530: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
-0000c540: 6964 203d 2072 6567 696f 6e5f 6964 0a0a  id = region_id..
-0000c550: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0000c560: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000c570: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-0000c580: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0000c590: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0000c5a0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-0000c5b0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0000c5c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000c5d0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0000c5e0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0000c5f0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0000c600: 2020 6966 2073 656c 662e 656c 6173 7469    if self.elasti
-0000c610: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
-0000c620: 7374 616e 6365 5f69 6420 6973 206e 6f74  stance_id is not
-0000c630: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000c640: 2020 2072 6573 756c 745b 2745 6c61 7374     result['Elast
-0000c650: 6963 4163 6365 6c65 7261 7465 6449 6e73  icAcceleratedIns
-0000c660: 7461 6e63 6549 6427 5d20 3d20 7365 6c66  tanceId'] = self
-0000c670: 2e65 6c61 7374 6963 5f61 6363 656c 6572  .elastic_acceler
-0000c680: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
-0000c690: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000c6a0: 2e66 6f72 6365 2069 7320 6e6f 7420 4e6f  .force is not No
-0000c6b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000c6c0: 7265 7375 6c74 5b27 466f 7263 6527 5d20  result['Force'] 
-0000c6d0: 3d20 7365 6c66 2e66 6f72 6365 0a20 2020  = self.force.   
-0000c6e0: 2020 2020 2069 6620 7365 6c66 2e72 6567       if self.reg
-0000c6f0: 696f 6e5f 6964 2069 7320 6e6f 7420 4e6f  ion_id is not No
-0000c700: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000c710: 7265 7375 6c74 5b27 5265 6769 6f6e 4964  result['RegionId
-0000c720: 275d 203d 2073 656c 662e 7265 6769 6f6e  '] = self.region
-0000c730: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-0000c740: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0000c750: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0000c760: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-0000c770: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0000c780: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0000c790: 2020 2069 6620 6d2e 6765 7428 2745 6c61     if m.get('Ela
-0000c7a0: 7374 6963 4163 6365 6c65 7261 7465 6449  sticAcceleratedI
-0000c7b0: 6e73 7461 6e63 6549 6427 2920 6973 206e  nstanceId') is n
-0000c7c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000c7d0: 2020 2020 2073 656c 662e 656c 6173 7469       self.elasti
-0000c7e0: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
-0000c7f0: 7374 616e 6365 5f69 6420 3d20 6d2e 6765  stance_id = m.ge
-0000c800: 7428 2745 6c61 7374 6963 4163 6365 6c65  t('ElasticAccele
-0000c810: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
-0000c820: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0000c830: 6574 2827 466f 7263 6527 2920 6973 206e  et('Force') is n
+00007eb0: 2020 2073 656c 662e 6563 695f 7368 7269     self.eci_shri
+00007ec0: 6e6b 203d 206d 2e67 6574 2827 4563 6927  nk = m.get('Eci'
+00007ed0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00007ee0: 6574 2827 5265 6769 6f6e 4964 2729 2069  et('RegionId') i
+00007ef0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00007f00: 2020 2020 2020 2020 7365 6c66 2e72 6567          self.reg
+00007f10: 696f 6e5f 6964 203d 206d 2e67 6574 2827  ion_id = m.get('
+00007f20: 5265 6769 6f6e 4964 2729 0a20 2020 2020  RegionId').     
+00007f30: 2020 2069 6620 6d2e 6765 7428 2752 6573     if m.get('Res
+00007f40: 6f75 7263 6547 726f 7570 4964 2729 2069  ourceGroupId') i
+00007f50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00007f60: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
+00007f70: 6f75 7263 655f 6772 6f75 705f 6964 203d  ource_group_id =
+00007f80: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+00007f90: 4772 6f75 7049 6427 290a 2020 2020 2020  GroupId').      
+00007fa0: 2020 6966 206d 2e67 6574 2827 5365 6375    if m.get('Secu
+00007fb0: 7269 7479 4772 6f75 7049 6427 2920 6973  rityGroupId') is
+00007fc0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00007fd0: 2020 2020 2020 2073 656c 662e 7365 6375         self.secu
+00007fe0: 7269 7479 5f67 726f 7570 5f69 6420 3d20  rity_group_id = 
+00007ff0: 6d2e 6765 7428 2753 6563 7572 6974 7947  m.get('SecurityG
+00008000: 726f 7570 4964 2729 0a20 2020 2020 2020  roupId').       
+00008010: 2069 6620 6d2e 6765 7428 2756 5377 6974   if m.get('VSwit
+00008020: 6368 4964 2729 2069 7320 6e6f 7420 4e6f  chId') is not No
+00008030: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00008040: 7365 6c66 2e76 5f73 7769 7463 685f 6964  self.v_switch_id
+00008050: 203d 206d 2e67 6574 2827 5653 7769 7463   = m.get('VSwitc
+00008060: 6849 6427 290a 2020 2020 2020 2020 7265  hId').        re
+00008070: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00008080: 7320 4372 6561 7465 4561 6945 6369 5265  s CreateEaiEciRe
+00008090: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
+000080a0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+000080b0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000080c0: 7365 6c66 2c0a 2020 2020 2020 2020 636c  self,.        cl
+000080d0: 6965 6e74 5f69 6e73 7461 6e63 655f 6964  ient_instance_id
+000080e0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+000080f0: 2020 2020 2020 656c 6173 7469 635f 6163        elastic_ac
+00008100: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+00008110: 6365 5f69 643a 2073 7472 203d 204e 6f6e  ce_id: str = Non
+00008120: 652c 0a20 2020 2020 2020 2072 6571 7565  e,.        reque
+00008130: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+00008140: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00008150: 2020 7365 6c66 2e63 6c69 656e 745f 696e    self.client_in
+00008160: 7374 616e 6365 5f69 6420 3d20 636c 6965  stance_id = clie
+00008170: 6e74 5f69 6e73 7461 6e63 655f 6964 0a20  nt_instance_id. 
+00008180: 2020 2020 2020 2073 656c 662e 656c 6173         self.elas
+00008190: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
+000081a0: 696e 7374 616e 6365 5f69 6420 3d20 656c  instance_id = el
+000081b0: 6173 7469 635f 6163 6365 6c65 7261 7465  astic_accelerate
+000081c0: 645f 696e 7374 616e 6365 5f69 640a 2020  d_instance_id.  
+000081d0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+000081e0: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
+000081f0: 6964 0a0a 2020 2020 6465 6620 7661 6c69  id..    def vali
+00008200: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00008210: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00008220: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00008230: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00008240: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+00008250: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+00008260: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00008270: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008280: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+00008290: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+000082a0: 2020 2020 2020 6966 2073 656c 662e 636c        if self.cl
+000082b0: 6965 6e74 5f69 6e73 7461 6e63 655f 6964  ient_instance_id
+000082c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000082d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000082e0: 5b27 436c 6965 6e74 496e 7374 616e 6365  ['ClientInstance
+000082f0: 4964 275d 203d 2073 656c 662e 636c 6965  Id'] = self.clie
+00008300: 6e74 5f69 6e73 7461 6e63 655f 6964 0a20  nt_instance_id. 
+00008310: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+00008320: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+00008330: 6564 5f69 6e73 7461 6e63 655f 6964 2069  ed_instance_id i
+00008340: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00008350: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00008360: 456c 6173 7469 6341 6363 656c 6572 6174  ElasticAccelerat
+00008370: 6564 496e 7374 616e 6365 4964 275d 203d  edInstanceId'] =
+00008380: 2073 656c 662e 656c 6173 7469 635f 6163   self.elastic_ac
+00008390: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+000083a0: 6365 5f69 640a 2020 2020 2020 2020 6966  ce_id.        if
+000083b0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+000083c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000083d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000083e0: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
+000083f0: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
+00008400: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00008410: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00008420: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00008430: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00008440: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00008450: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00008460: 6620 6d2e 6765 7428 2743 6c69 656e 7449  f m.get('ClientI
+00008470: 6e73 7461 6e63 6549 6427 2920 6973 206e  nstanceId') is n
+00008480: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00008490: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
+000084a0: 5f69 6e73 7461 6e63 655f 6964 203d 206d  _instance_id = m
+000084b0: 2e67 6574 2827 436c 6965 6e74 496e 7374  .get('ClientInst
+000084c0: 616e 6365 4964 2729 0a20 2020 2020 2020  anceId').       
+000084d0: 2069 6620 6d2e 6765 7428 2745 6c61 7374   if m.get('Elast
+000084e0: 6963 4163 6365 6c65 7261 7465 6449 6e73  icAcceleratedIns
+000084f0: 7461 6e63 6549 6427 2920 6973 206e 6f74  tanceId') is not
+00008500: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00008510: 2020 2073 656c 662e 656c 6173 7469 635f     self.elastic_
+00008520: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
+00008530: 616e 6365 5f69 6420 3d20 6d2e 6765 7428  ance_id = m.get(
+00008540: 2745 6c61 7374 6963 4163 6365 6c65 7261  'ElasticAccelera
+00008550: 7465 6449 6e73 7461 6e63 6549 6427 290a  tedInstanceId').
+00008560: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00008570: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
+00008580: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00008590: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+000085a0: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
+000085b0: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
+000085c0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000085d0: 0a0a 636c 6173 7320 4372 6561 7465 4561  ..class CreateEa
+000085e0: 6945 6369 5265 7370 6f6e 7365 2854 6561  iEciResponse(Tea
+000085f0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+00008600: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00008610: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00008620: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
+00008630: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+00008640: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+00008650: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
+00008660: 0a20 2020 2020 2020 2062 6f64 793a 2043  .        body: C
+00008670: 7265 6174 6545 6169 4563 6952 6573 706f  reateEaiEciRespo
+00008680: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
+00008690: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+000086a0: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
+000086b0: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
+000086c0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+000086d0: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
+000086e0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+000086f0: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
+00008700: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00008710: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+00008720: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+00008730: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
+00008740: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
+00008750: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+00008760: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
+00008770: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
+00008780: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
+00008790: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+000087a0: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
+000087b0: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
+000087c0: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
+000087d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000087e0: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
+000087f0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+00008800: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+00008810: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+00008820: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00008830: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00008840: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00008850: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00008860: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00008870: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00008880: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+00008890: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000088a0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+000088b0: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+000088c0: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+000088d0: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+000088e0: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+000088f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00008900: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+00008910: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+00008920: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+00008930: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+00008940: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00008950: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+00008960: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+00008970: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+00008980: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00008990: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000089a0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+000089b0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+000089c0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+000089d0: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+000089e0: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+000089f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00008a00: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00008a10: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+00008a20: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00008a30: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00008a40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00008a50: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00008a60: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+00008a70: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+00008a80: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00008a90: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+00008aa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00008ab0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+00008ac0: 4372 6561 7465 4561 6945 6369 5265 7370  CreateEaiEciResp
+00008ad0: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+00008ae0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00008af0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+00008b00: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+00008b10: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00008b20: 2073 656c 660a 0a0a 636c 6173 7320 4372   self...class Cr
+00008b30: 6561 7465 4561 6945 6373 5265 7175 6573  eateEaiEcsReques
+00008b40: 7445 6373 2854 6561 4d6f 6465 6c29 3a0a  tEcs(TeaModel):.
+00008b50: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00008b60: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00008b70: 2020 2020 2020 2020 696d 6167 655f 6964          image_id
+00008b80: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00008b90: 2020 2020 2020 696e 7465 726e 6574 5f6d        internet_m
+00008ba0: 6178 5f62 616e 6477 6964 7468 5f69 6e3a  ax_bandwidth_in:
+00008bb0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00008bc0: 2020 2020 2069 6e74 6572 6e65 745f 6d61       internet_ma
+00008bd0: 785f 6261 6e64 7769 6474 685f 6f75 743a  x_bandwidth_out:
+00008be0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00008bf0: 2020 2020 206e 616d 653a 2073 7472 203d       name: str =
+00008c00: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
+00008c10: 6173 7377 6f72 643a 2073 7472 203d 204e  assword: str = N
+00008c20: 6f6e 652c 0a20 2020 2020 2020 2073 7973  one,.        sys
+00008c30: 7465 6d5f 6469 736b 5f63 6174 6567 6f72  tem_disk_categor
+00008c40: 793a 2073 7472 203d 204e 6f6e 652c 0a20  y: str = None,. 
+00008c50: 2020 2020 2020 2073 7973 7465 6d5f 6469         system_di
+00008c60: 736b 5f73 697a 653a 2069 6e74 203d 204e  sk_size: int = N
+00008c70: 6f6e 652c 0a20 2020 2020 2020 2074 7970  one,.        typ
+00008c80: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+00008c90: 2020 2020 2020 207a 6f6e 655f 6964 3a20         zone_id: 
+00008ca0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00008cb0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00008cc0: 696d 6167 655f 6964 203d 2069 6d61 6765  image_id = image
+00008cd0: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+00008ce0: 2e69 6e74 6572 6e65 745f 6d61 785f 6261  .internet_max_ba
+00008cf0: 6e64 7769 6474 685f 696e 203d 2069 6e74  ndwidth_in = int
+00008d00: 6572 6e65 745f 6d61 785f 6261 6e64 7769  ernet_max_bandwi
+00008d10: 6474 685f 696e 0a20 2020 2020 2020 2073  dth_in.        s
+00008d20: 656c 662e 696e 7465 726e 6574 5f6d 6178  elf.internet_max
+00008d30: 5f62 616e 6477 6964 7468 5f6f 7574 203d  _bandwidth_out =
+00008d40: 2069 6e74 6572 6e65 745f 6d61 785f 6261   internet_max_ba
+00008d50: 6e64 7769 6474 685f 6f75 740a 2020 2020  ndwidth_out.    
+00008d60: 2020 2020 7365 6c66 2e6e 616d 6520 3d20      self.name = 
+00008d70: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
+00008d80: 662e 7061 7373 776f 7264 203d 2070 6173  f.password = pas
+00008d90: 7377 6f72 640a 2020 2020 2020 2020 7365  sword.        se
+00008da0: 6c66 2e73 7973 7465 6d5f 6469 736b 5f63  lf.system_disk_c
+00008db0: 6174 6567 6f72 7920 3d20 7379 7374 656d  ategory = system
+00008dc0: 5f64 6973 6b5f 6361 7465 676f 7279 0a20  _disk_category. 
+00008dd0: 2020 2020 2020 2073 656c 662e 7379 7374         self.syst
+00008de0: 656d 5f64 6973 6b5f 7369 7a65 203d 2073  em_disk_size = s
+00008df0: 7973 7465 6d5f 6469 736b 5f73 697a 650a  ystem_disk_size.
+00008e00: 2020 2020 2020 2020 7365 6c66 2e74 7970          self.typ
+00008e10: 6520 3d20 7479 7065 0a20 2020 2020 2020  e = type.       
+00008e20: 2073 656c 662e 7a6f 6e65 5f69 6420 3d20   self.zone_id = 
+00008e30: 7a6f 6e65 5f69 640a 0a20 2020 2064 6566  zone_id..    def
+00008e40: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00008e50: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00008e60: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00008e70: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00008e80: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+00008e90: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00008ea0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00008eb0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00008ec0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00008ed0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00008ee0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00008ef0: 6c66 2e69 6d61 6765 5f69 6420 6973 206e  lf.image_id is n
+00008f00: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00008f10: 2020 2020 2072 6573 756c 745b 2749 6d61       result['Ima
+00008f20: 6765 4964 275d 203d 2073 656c 662e 696d  geId'] = self.im
+00008f30: 6167 655f 6964 0a20 2020 2020 2020 2069  age_id.        i
+00008f40: 6620 7365 6c66 2e69 6e74 6572 6e65 745f  f self.internet_
+00008f50: 6d61 785f 6261 6e64 7769 6474 685f 696e  max_bandwidth_in
+00008f60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00008f70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00008f80: 5b27 496e 7465 726e 6574 4d61 7842 616e  ['InternetMaxBan
+00008f90: 6477 6964 7468 496e 275d 203d 2073 656c  dwidthIn'] = sel
+00008fa0: 662e 696e 7465 726e 6574 5f6d 6178 5f62  f.internet_max_b
+00008fb0: 616e 6477 6964 7468 5f69 6e0a 2020 2020  andwidth_in.    
+00008fc0: 2020 2020 6966 2073 656c 662e 696e 7465      if self.inte
+00008fd0: 726e 6574 5f6d 6178 5f62 616e 6477 6964  rnet_max_bandwid
+00008fe0: 7468 5f6f 7574 2069 7320 6e6f 7420 4e6f  th_out is not No
+00008ff0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00009000: 7265 7375 6c74 5b27 496e 7465 726e 6574  result['Internet
+00009010: 4d61 7842 616e 6477 6964 7468 4f75 7427  MaxBandwidthOut'
+00009020: 5d20 3d20 7365 6c66 2e69 6e74 6572 6e65  ] = self.interne
+00009030: 745f 6d61 785f 6261 6e64 7769 6474 685f  t_max_bandwidth_
+00009040: 6f75 740a 2020 2020 2020 2020 6966 2073  out.        if s
+00009050: 656c 662e 6e61 6d65 2069 7320 6e6f 7420  elf.name is not 
+00009060: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00009070: 2020 7265 7375 6c74 5b27 4e61 6d65 275d    result['Name']
+00009080: 203d 2073 656c 662e 6e61 6d65 0a20 2020   = self.name.   
+00009090: 2020 2020 2069 6620 7365 6c66 2e70 6173       if self.pas
+000090a0: 7377 6f72 6420 6973 206e 6f74 204e 6f6e  sword is not Non
+000090b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000090c0: 6573 756c 745b 2750 6173 7377 6f72 6427  esult['Password'
+000090d0: 5d20 3d20 7365 6c66 2e70 6173 7377 6f72  ] = self.passwor
+000090e0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+000090f0: 662e 7379 7374 656d 5f64 6973 6b5f 6361  f.system_disk_ca
+00009100: 7465 676f 7279 2069 7320 6e6f 7420 4e6f  tegory is not No
+00009110: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00009120: 7265 7375 6c74 5b27 5379 7374 656d 4469  result['SystemDi
+00009130: 736b 4361 7465 676f 7279 275d 203d 2073  skCategory'] = s
+00009140: 656c 662e 7379 7374 656d 5f64 6973 6b5f  elf.system_disk_
+00009150: 6361 7465 676f 7279 0a20 2020 2020 2020  category.       
+00009160: 2069 6620 7365 6c66 2e73 7973 7465 6d5f   if self.system_
+00009170: 6469 736b 5f73 697a 6520 6973 206e 6f74  disk_size is not
+00009180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00009190: 2020 2072 6573 756c 745b 2753 7973 7465     result['Syste
+000091a0: 6d44 6973 6b53 697a 6527 5d20 3d20 7365  mDiskSize'] = se
+000091b0: 6c66 2e73 7973 7465 6d5f 6469 736b 5f73  lf.system_disk_s
+000091c0: 697a 650a 2020 2020 2020 2020 6966 2073  ize.        if s
+000091d0: 656c 662e 7479 7065 2069 7320 6e6f 7420  elf.type is not 
+000091e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000091f0: 2020 7265 7375 6c74 5b27 5479 7065 275d    result['Type']
+00009200: 203d 2073 656c 662e 7479 7065 0a20 2020   = self.type.   
+00009210: 2020 2020 2069 6620 7365 6c66 2e7a 6f6e       if self.zon
+00009220: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+00009230: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00009240: 7375 6c74 5b27 5a6f 6e65 4964 275d 203d  sult['ZoneId'] =
+00009250: 2073 656c 662e 7a6f 6e65 5f69 640a 2020   self.zone_id.  
+00009260: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00009270: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00009280: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00009290: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+000092a0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+000092b0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000092c0: 6d2e 6765 7428 2749 6d61 6765 4964 2729  m.get('ImageId')
+000092d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000092e0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+000092f0: 6d61 6765 5f69 6420 3d20 6d2e 6765 7428  mage_id = m.get(
+00009300: 2749 6d61 6765 4964 2729 0a20 2020 2020  'ImageId').     
+00009310: 2020 2069 6620 6d2e 6765 7428 2749 6e74     if m.get('Int
+00009320: 6572 6e65 744d 6178 4261 6e64 7769 6474  ernetMaxBandwidt
+00009330: 6849 6e27 2920 6973 206e 6f74 204e 6f6e  hIn') is not Non
+00009340: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00009350: 656c 662e 696e 7465 726e 6574 5f6d 6178  elf.internet_max
+00009360: 5f62 616e 6477 6964 7468 5f69 6e20 3d20  _bandwidth_in = 
+00009370: 6d2e 6765 7428 2749 6e74 6572 6e65 744d  m.get('InternetM
+00009380: 6178 4261 6e64 7769 6474 6849 6e27 290a  axBandwidthIn').
+00009390: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000093a0: 2827 496e 7465 726e 6574 4d61 7842 616e  ('InternetMaxBan
+000093b0: 6477 6964 7468 4f75 7427 2920 6973 206e  dwidthOut') is n
+000093c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000093d0: 2020 2020 2073 656c 662e 696e 7465 726e       self.intern
+000093e0: 6574 5f6d 6178 5f62 616e 6477 6964 7468  et_max_bandwidth
+000093f0: 5f6f 7574 203d 206d 2e67 6574 2827 496e  _out = m.get('In
+00009400: 7465 726e 6574 4d61 7842 616e 6477 6964  ternetMaxBandwid
+00009410: 7468 4f75 7427 290a 2020 2020 2020 2020  thOut').        
+00009420: 6966 206d 2e67 6574 2827 4e61 6d65 2729  if m.get('Name')
+00009430: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00009440: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00009450: 616d 6520 3d20 6d2e 6765 7428 274e 616d  ame = m.get('Nam
+00009460: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00009470: 2e67 6574 2827 5061 7373 776f 7264 2729  .get('Password')
+00009480: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00009490: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+000094a0: 6173 7377 6f72 6420 3d20 6d2e 6765 7428  assword = m.get(
+000094b0: 2750 6173 7377 6f72 6427 290a 2020 2020  'Password').    
+000094c0: 2020 2020 6966 206d 2e67 6574 2827 5379      if m.get('Sy
+000094d0: 7374 656d 4469 736b 4361 7465 676f 7279  stemDiskCategory
+000094e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000094f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009500: 2e73 7973 7465 6d5f 6469 736b 5f63 6174  .system_disk_cat
+00009510: 6567 6f72 7920 3d20 6d2e 6765 7428 2753  egory = m.get('S
+00009520: 7973 7465 6d44 6973 6b43 6174 6567 6f72  ystemDiskCategor
+00009530: 7927 290a 2020 2020 2020 2020 6966 206d  y').        if m
+00009540: 2e67 6574 2827 5379 7374 656d 4469 736b  .get('SystemDisk
+00009550: 5369 7a65 2729 2069 7320 6e6f 7420 4e6f  Size') is not No
+00009560: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00009570: 7365 6c66 2e73 7973 7465 6d5f 6469 736b  self.system_disk
+00009580: 5f73 697a 6520 3d20 6d2e 6765 7428 2753  _size = m.get('S
+00009590: 7973 7465 6d44 6973 6b53 697a 6527 290a  ystemDiskSize').
+000095a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000095b0: 2827 5479 7065 2729 2069 7320 6e6f 7420  ('Type') is not 
+000095c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000095d0: 2020 7365 6c66 2e74 7970 6520 3d20 6d2e    self.type = m.
+000095e0: 6765 7428 2754 7970 6527 290a 2020 2020  get('Type').    
+000095f0: 2020 2020 6966 206d 2e67 6574 2827 5a6f      if m.get('Zo
+00009600: 6e65 4964 2729 2069 7320 6e6f 7420 4e6f  neId') is not No
+00009610: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00009620: 7365 6c66 2e7a 6f6e 655f 6964 203d 206d  self.zone_id = m
+00009630: 2e67 6574 2827 5a6f 6e65 4964 2729 0a20  .get('ZoneId'). 
+00009640: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00009650: 6c66 0a0a 0a63 6c61 7373 2043 7265 6174  lf...class Creat
+00009660: 6545 6169 4563 7352 6571 7565 7374 2854  eEaiEcsRequest(T
+00009670: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00009680: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00009690: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000096a0: 2020 636c 6965 6e74 5f74 6f6b 656e 3a20    client_token: 
+000096b0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+000096c0: 2020 2020 6561 6973 5f6e 616d 653a 2073      eais_name: s
+000096d0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000096e0: 2020 2065 6169 735f 7479 7065 3a20 7374     eais_type: st
+000096f0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00009700: 2020 6563 733a 2043 7265 6174 6545 6169    ecs: CreateEai
+00009710: 4563 7352 6571 7565 7374 4563 7320 3d20  EcsRequestEcs = 
+00009720: 4e6f 6e65 2c0a 2020 2020 2020 2020 7265  None,.        re
+00009730: 6769 6f6e 5f69 643a 2073 7472 203d 204e  gion_id: str = N
+00009740: 6f6e 652c 0a20 2020 2020 2020 2072 6573  one,.        res
+00009750: 6f75 7263 655f 6772 6f75 705f 6964 3a20  ource_group_id: 
+00009760: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00009770: 2020 2020 7365 6375 7269 7479 5f67 726f      security_gro
+00009780: 7570 5f69 643a 2073 7472 203d 204e 6f6e  up_id: str = Non
+00009790: 652c 0a20 2020 2020 2020 2076 5f73 7769  e,.        v_swi
+000097a0: 7463 685f 6964 3a20 7374 7220 3d20 4e6f  tch_id: str = No
+000097b0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000097c0: 2020 2073 656c 662e 636c 6965 6e74 5f74     self.client_t
+000097d0: 6f6b 656e 203d 2063 6c69 656e 745f 746f  oken = client_to
+000097e0: 6b65 6e0a 2020 2020 2020 2020 7365 6c66  ken.        self
+000097f0: 2e65 6169 735f 6e61 6d65 203d 2065 6169  .eais_name = eai
+00009800: 735f 6e61 6d65 0a20 2020 2020 2020 2073  s_name.        s
+00009810: 656c 662e 6561 6973 5f74 7970 6520 3d20  elf.eais_type = 
+00009820: 6561 6973 5f74 7970 650a 2020 2020 2020  eais_type.      
+00009830: 2020 7365 6c66 2e65 6373 203d 2065 6373    self.ecs = ecs
+00009840: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00009850: 6769 6f6e 5f69 6420 3d20 7265 6769 6f6e  gion_id = region
+00009860: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+00009870: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
+00009880: 6964 203d 2072 6573 6f75 7263 655f 6772  id = resource_gr
+00009890: 6f75 705f 6964 0a20 2020 2020 2020 2073  oup_id.        s
+000098a0: 656c 662e 7365 6375 7269 7479 5f67 726f  elf.security_gro
+000098b0: 7570 5f69 6420 3d20 7365 6375 7269 7479  up_id = security
+000098c0: 5f67 726f 7570 5f69 640a 2020 2020 2020  _group_id.      
+000098d0: 2020 7365 6c66 2e76 5f73 7769 7463 685f    self.v_switch_
+000098e0: 6964 203d 2076 5f73 7769 7463 685f 6964  id = v_switch_id
+000098f0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00009900: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00009910: 2020 6966 2073 656c 662e 6563 733a 0a20    if self.ecs:. 
+00009920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00009930: 6563 732e 7661 6c69 6461 7465 2829 0a0a  ecs.validate()..
+00009940: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00009950: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00009960: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00009970: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00009980: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00009990: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000099a0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000099b0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+000099c0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000099d0: 656c 662e 636c 6965 6e74 5f74 6f6b 656e  elf.client_token
+000099e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000099f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00009a00: 5b27 436c 6965 6e74 546f 6b65 6e27 5d20  ['ClientToken'] 
+00009a10: 3d20 7365 6c66 2e63 6c69 656e 745f 746f  = self.client_to
+00009a20: 6b65 6e0a 2020 2020 2020 2020 6966 2073  ken.        if s
+00009a30: 656c 662e 6561 6973 5f6e 616d 6520 6973  elf.eais_name is
+00009a40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00009a50: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
+00009a60: 6169 734e 616d 6527 5d20 3d20 7365 6c66  aisName'] = self
+00009a70: 2e65 6169 735f 6e61 6d65 0a20 2020 2020  .eais_name.     
+00009a80: 2020 2069 6620 7365 6c66 2e65 6169 735f     if self.eais_
+00009a90: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
+00009aa0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00009ab0: 7375 6c74 5b27 4561 6973 5479 7065 275d  sult['EaisType']
+00009ac0: 203d 2073 656c 662e 6561 6973 5f74 7970   = self.eais_typ
+00009ad0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00009ae0: 662e 6563 7320 6973 206e 6f74 204e 6f6e  f.ecs is not Non
+00009af0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00009b00: 6573 756c 745b 2745 6373 275d 203d 2073  esult['Ecs'] = s
+00009b10: 656c 662e 6563 732e 746f 5f6d 6170 2829  elf.ecs.to_map()
+00009b20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00009b30: 2e72 6567 696f 6e5f 6964 2069 7320 6e6f  .region_id is no
+00009b40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00009b50: 2020 2020 7265 7375 6c74 5b27 5265 6769      result['Regi
+00009b60: 6f6e 4964 275d 203d 2073 656c 662e 7265  onId'] = self.re
+00009b70: 6769 6f6e 5f69 640a 2020 2020 2020 2020  gion_id.        
+00009b80: 6966 2073 656c 662e 7265 736f 7572 6365  if self.resource
+00009b90: 5f67 726f 7570 5f69 6420 6973 206e 6f74  _group_id is not
+00009ba0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00009bb0: 2020 2072 6573 756c 745b 2752 6573 6f75     result['Resou
+00009bc0: 7263 6547 726f 7570 4964 275d 203d 2073  rceGroupId'] = s
+00009bd0: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
+00009be0: 7570 5f69 640a 2020 2020 2020 2020 6966  up_id.        if
+00009bf0: 2073 656c 662e 7365 6375 7269 7479 5f67   self.security_g
+00009c00: 726f 7570 5f69 6420 6973 206e 6f74 204e  roup_id is not N
+00009c10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00009c20: 2072 6573 756c 745b 2753 6563 7572 6974   result['Securit
+00009c30: 7947 726f 7570 4964 275d 203d 2073 656c  yGroupId'] = sel
+00009c40: 662e 7365 6375 7269 7479 5f67 726f 7570  f.security_group
+00009c50: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00009c60: 656c 662e 765f 7377 6974 6368 5f69 6420  elf.v_switch_id 
+00009c70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00009c80: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00009c90: 2756 5377 6974 6368 4964 275d 203d 2073  'VSwitchId'] = s
+00009ca0: 656c 662e 765f 7377 6974 6368 5f69 640a  elf.v_switch_id.
+00009cb0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00009cc0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00009cd0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00009ce0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00009cf0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00009d00: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00009d10: 6620 6d2e 6765 7428 2743 6c69 656e 7454  f m.get('ClientT
+00009d20: 6f6b 656e 2729 2069 7320 6e6f 7420 4e6f  oken') is not No
+00009d30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00009d40: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
+00009d50: 6e20 3d20 6d2e 6765 7428 2743 6c69 656e  n = m.get('Clien
+00009d60: 7454 6f6b 656e 2729 0a20 2020 2020 2020  tToken').       
+00009d70: 2069 6620 6d2e 6765 7428 2745 6169 734e   if m.get('EaisN
+00009d80: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
+00009d90: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00009da0: 656c 662e 6561 6973 5f6e 616d 6520 3d20  elf.eais_name = 
+00009db0: 6d2e 6765 7428 2745 6169 734e 616d 6527  m.get('EaisName'
+00009dc0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00009dd0: 6574 2827 4561 6973 5479 7065 2729 2069  et('EaisType') i
+00009de0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00009df0: 2020 2020 2020 2020 7365 6c66 2e65 6169          self.eai
+00009e00: 735f 7479 7065 203d 206d 2e67 6574 2827  s_type = m.get('
+00009e10: 4561 6973 5479 7065 2729 0a20 2020 2020  EaisType').     
+00009e20: 2020 2069 6620 6d2e 6765 7428 2745 6373     if m.get('Ecs
+00009e30: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00009e40: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00009e50: 5f6d 6f64 656c 203d 2043 7265 6174 6545  _model = CreateE
+00009e60: 6169 4563 7352 6571 7565 7374 4563 7328  aiEcsRequestEcs(
+00009e70: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00009e80: 6c66 2e65 6373 203d 2074 656d 705f 6d6f  lf.ecs = temp_mo
+00009e90: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+00009ea0: 4563 7327 5d29 0a20 2020 2020 2020 2069  Ecs']).        i
+00009eb0: 6620 6d2e 6765 7428 2752 6567 696f 6e49  f m.get('RegionI
+00009ec0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00009ed0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009ee0: 662e 7265 6769 6f6e 5f69 6420 3d20 6d2e  f.region_id = m.
+00009ef0: 6765 7428 2752 6567 696f 6e49 6427 290a  get('RegionId').
+00009f00: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00009f10: 2827 5265 736f 7572 6365 4772 6f75 7049  ('ResourceGroupI
+00009f20: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00009f30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00009f40: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
+00009f50: 5f69 6420 3d20 6d2e 6765 7428 2752 6573  _id = m.get('Res
+00009f60: 6f75 7263 6547 726f 7570 4964 2729 0a20  ourceGroupId'). 
+00009f70: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00009f80: 2753 6563 7572 6974 7947 726f 7570 4964  'SecurityGroupId
+00009f90: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00009fa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009fb0: 2e73 6563 7572 6974 795f 6772 6f75 705f  .security_group_
+00009fc0: 6964 203d 206d 2e67 6574 2827 5365 6375  id = m.get('Secu
+00009fd0: 7269 7479 4772 6f75 7049 6427 290a 2020  rityGroupId').  
+00009fe0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00009ff0: 5653 7769 7463 6849 6427 2920 6973 206e  VSwitchId') is n
+0000a000: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000a010: 2020 2020 2073 656c 662e 765f 7377 6974       self.v_swit
+0000a020: 6368 5f69 6420 3d20 6d2e 6765 7428 2756  ch_id = m.get('V
+0000a030: 5377 6974 6368 4964 2729 0a20 2020 2020  SwitchId').     
+0000a040: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0000a050: 0a63 6c61 7373 2043 7265 6174 6545 6169  .class CreateEai
+0000a060: 4563 7353 6872 696e 6b52 6571 7565 7374  EcsShrinkRequest
+0000a070: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+0000a080: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0000a090: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000a0a0: 2020 2020 636c 6965 6e74 5f74 6f6b 656e      client_token
+0000a0b0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0000a0c0: 2020 2020 2020 6561 6973 5f6e 616d 653a        eais_name:
+0000a0d0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0000a0e0: 2020 2020 2065 6169 735f 7479 7065 3a20       eais_type: 
+0000a0f0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0000a100: 2020 2020 6563 735f 7368 7269 6e6b 3a20      ecs_shrink: 
+0000a110: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0000a120: 2020 2020 7265 6769 6f6e 5f69 643a 2073      region_id: s
+0000a130: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0000a140: 2020 2072 6573 6f75 7263 655f 6772 6f75     resource_grou
+0000a150: 705f 6964 3a20 7374 7220 3d20 4e6f 6e65  p_id: str = None
+0000a160: 2c0a 2020 2020 2020 2020 7365 6375 7269  ,.        securi
+0000a170: 7479 5f67 726f 7570 5f69 643a 2073 7472  ty_group_id: str
+0000a180: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000a190: 2076 5f73 7769 7463 685f 6964 3a20 7374   v_switch_id: st
+0000a1a0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
+0000a1b0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+0000a1c0: 6965 6e74 5f74 6f6b 656e 203d 2063 6c69  ient_token = cli
+0000a1d0: 656e 745f 746f 6b65 6e0a 2020 2020 2020  ent_token.      
+0000a1e0: 2020 7365 6c66 2e65 6169 735f 6e61 6d65    self.eais_name
+0000a1f0: 203d 2065 6169 735f 6e61 6d65 0a20 2020   = eais_name.   
+0000a200: 2020 2020 2073 656c 662e 6561 6973 5f74       self.eais_t
+0000a210: 7970 6520 3d20 6561 6973 5f74 7970 650a  ype = eais_type.
+0000a220: 2020 2020 2020 2020 7365 6c66 2e65 6373          self.ecs
+0000a230: 5f73 6872 696e 6b20 3d20 6563 735f 7368  _shrink = ecs_sh
+0000a240: 7269 6e6b 0a20 2020 2020 2020 2073 656c  rink.        sel
+0000a250: 662e 7265 6769 6f6e 5f69 6420 3d20 7265  f.region_id = re
+0000a260: 6769 6f6e 5f69 640a 2020 2020 2020 2020  gion_id.        
+0000a270: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
+0000a280: 6f75 705f 6964 203d 2072 6573 6f75 7263  oup_id = resourc
+0000a290: 655f 6772 6f75 705f 6964 0a20 2020 2020  e_group_id.     
+0000a2a0: 2020 2073 656c 662e 7365 6375 7269 7479     self.security
+0000a2b0: 5f67 726f 7570 5f69 6420 3d20 7365 6375  _group_id = secu
+0000a2c0: 7269 7479 5f67 726f 7570 5f69 640a 2020  rity_group_id.  
+0000a2d0: 2020 2020 2020 7365 6c66 2e76 5f73 7769        self.v_swi
+0000a2e0: 7463 685f 6964 203d 2076 5f73 7769 7463  tch_id = v_switc
+0000a2f0: 685f 6964 0a0a 2020 2020 6465 6620 7661  h_id..    def va
+0000a300: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+0000a310: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0000a320: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+0000a330: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+0000a340: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+0000a350: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0000a360: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0000a370: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a380: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0000a390: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0000a3a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000a3b0: 636c 6965 6e74 5f74 6f6b 656e 2069 7320  client_token is 
+0000a3c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000a3d0: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
+0000a3e0: 6965 6e74 546f 6b65 6e27 5d20 3d20 7365  ientToken'] = se
+0000a3f0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e0a  lf.client_token.
+0000a400: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000a410: 6561 6973 5f6e 616d 6520 6973 206e 6f74  eais_name is not
+0000a420: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000a430: 2020 2072 6573 756c 745b 2745 6169 734e     result['EaisN
+0000a440: 616d 6527 5d20 3d20 7365 6c66 2e65 6169  ame'] = self.eai
+0000a450: 735f 6e61 6d65 0a20 2020 2020 2020 2069  s_name.        i
+0000a460: 6620 7365 6c66 2e65 6169 735f 7479 7065  f self.eais_type
+0000a470: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000a480: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000a490: 5b27 4561 6973 5479 7065 275d 203d 2073  ['EaisType'] = s
+0000a4a0: 656c 662e 6561 6973 5f74 7970 650a 2020  elf.eais_type.  
+0000a4b0: 2020 2020 2020 6966 2073 656c 662e 6563        if self.ec
+0000a4c0: 735f 7368 7269 6e6b 2069 7320 6e6f 7420  s_shrink is not 
+0000a4d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000a4e0: 2020 7265 7375 6c74 5b27 4563 7327 5d20    result['Ecs'] 
+0000a4f0: 3d20 7365 6c66 2e65 6373 5f73 6872 696e  = self.ecs_shrin
+0000a500: 6b0a 2020 2020 2020 2020 6966 2073 656c  k.        if sel
+0000a510: 662e 7265 6769 6f6e 5f69 6420 6973 206e  f.region_id is n
+0000a520: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000a530: 2020 2020 2072 6573 756c 745b 2752 6567       result['Reg
+0000a540: 696f 6e49 6427 5d20 3d20 7365 6c66 2e72  ionId'] = self.r
+0000a550: 6567 696f 6e5f 6964 0a20 2020 2020 2020  egion_id.       
+0000a560: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
+0000a570: 655f 6772 6f75 705f 6964 2069 7320 6e6f  e_group_id is no
+0000a580: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000a590: 2020 2020 7265 7375 6c74 5b27 5265 736f      result['Reso
+0000a5a0: 7572 6365 4772 6f75 7049 6427 5d20 3d20  urceGroupId'] = 
+0000a5b0: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
+0000a5c0: 6f75 705f 6964 0a20 2020 2020 2020 2069  oup_id.        i
+0000a5d0: 6620 7365 6c66 2e73 6563 7572 6974 795f  f self.security_
+0000a5e0: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
+0000a5f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000a600: 2020 7265 7375 6c74 5b27 5365 6375 7269    result['Securi
+0000a610: 7479 4772 6f75 7049 6427 5d20 3d20 7365  tyGroupId'] = se
+0000a620: 6c66 2e73 6563 7572 6974 795f 6772 6f75  lf.security_grou
+0000a630: 705f 6964 0a20 2020 2020 2020 2069 6620  p_id.        if 
+0000a640: 7365 6c66 2e76 5f73 7769 7463 685f 6964  self.v_switch_id
+0000a650: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000a660: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000a670: 5b27 5653 7769 7463 6849 6427 5d20 3d20  ['VSwitchId'] = 
+0000a680: 7365 6c66 2e76 5f73 7769 7463 685f 6964  self.v_switch_id
+0000a690: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000a6a0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0000a6b0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+0000a6c0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+0000a6d0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0000a6e0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0000a6f0: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
+0000a700: 546f 6b65 6e27 2920 6973 206e 6f74 204e  Token') is not N
+0000a710: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000a720: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+0000a730: 656e 203d 206d 2e67 6574 2827 436c 6965  en = m.get('Clie
+0000a740: 6e74 546f 6b65 6e27 290a 2020 2020 2020  ntToken').      
+0000a750: 2020 6966 206d 2e67 6574 2827 4561 6973    if m.get('Eais
+0000a760: 4e61 6d65 2729 2069 7320 6e6f 7420 4e6f  Name') is not No
+0000a770: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000a780: 7365 6c66 2e65 6169 735f 6e61 6d65 203d  self.eais_name =
+0000a790: 206d 2e67 6574 2827 4561 6973 4e61 6d65   m.get('EaisName
+0000a7a0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0000a7b0: 6765 7428 2745 6169 7354 7970 6527 2920  get('EaisType') 
+0000a7c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000a7d0: 2020 2020 2020 2020 2073 656c 662e 6561           self.ea
+0000a7e0: 6973 5f74 7970 6520 3d20 6d2e 6765 7428  is_type = m.get(
+0000a7f0: 2745 6169 7354 7970 6527 290a 2020 2020  'EaisType').    
+0000a800: 2020 2020 6966 206d 2e67 6574 2827 4563      if m.get('Ec
+0000a810: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+0000a820: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000a830: 662e 6563 735f 7368 7269 6e6b 203d 206d  f.ecs_shrink = m
+0000a840: 2e67 6574 2827 4563 7327 290a 2020 2020  .get('Ecs').    
+0000a850: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+0000a860: 6769 6f6e 4964 2729 2069 7320 6e6f 7420  gionId') is not 
+0000a870: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000a880: 2020 7365 6c66 2e72 6567 696f 6e5f 6964    self.region_id
+0000a890: 203d 206d 2e67 6574 2827 5265 6769 6f6e   = m.get('Region
+0000a8a0: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0000a8b0: 6d2e 6765 7428 2752 6573 6f75 7263 6547  m.get('ResourceG
+0000a8c0: 726f 7570 4964 2729 2069 7320 6e6f 7420  roupId') is not 
+0000a8d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000a8e0: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+0000a8f0: 6772 6f75 705f 6964 203d 206d 2e67 6574  group_id = m.get
+0000a900: 2827 5265 736f 7572 6365 4772 6f75 7049  ('ResourceGroupI
+0000a910: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+0000a920: 2e67 6574 2827 5365 6375 7269 7479 4772  .get('SecurityGr
+0000a930: 6f75 7049 6427 2920 6973 206e 6f74 204e  oupId') is not N
+0000a940: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000a950: 2073 656c 662e 7365 6375 7269 7479 5f67   self.security_g
+0000a960: 726f 7570 5f69 6420 3d20 6d2e 6765 7428  roup_id = m.get(
+0000a970: 2753 6563 7572 6974 7947 726f 7570 4964  'SecurityGroupId
+0000a980: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0000a990: 6765 7428 2756 5377 6974 6368 4964 2729  get('VSwitchId')
+0000a9a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000a9b0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+0000a9c0: 5f73 7769 7463 685f 6964 203d 206d 2e67  _switch_id = m.g
+0000a9d0: 6574 2827 5653 7769 7463 6849 6427 290a  et('VSwitchId').
+0000a9e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000a9f0: 656c 660a 0a0a 636c 6173 7320 4372 6561  elf...class Crea
+0000aa00: 7465 4561 6945 6373 5265 7370 6f6e 7365  teEaiEcsResponse
+0000aa10: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
+0000aa20: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0000aa30: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000aa40: 2020 2020 2020 2020 636c 6965 6e74 5f69          client_i
+0000aa50: 6e73 7461 6e63 655f 6964 3a20 7374 7220  nstance_id: str 
+0000aa60: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000aa70: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
+0000aa80: 7465 645f 696e 7374 616e 6365 5f69 643a  ted_instance_id:
+0000aa90: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0000aaa0: 2020 2020 2072 6571 7565 7374 5f69 643a       request_id:
+0000aab0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0000aac0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+0000aad0: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
+0000aae0: 5f69 6420 3d20 636c 6965 6e74 5f69 6e73  _id = client_ins
+0000aaf0: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+0000ab00: 2073 656c 662e 656c 6173 7469 635f 6163   self.elastic_ac
+0000ab10: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+0000ab20: 6365 5f69 6420 3d20 656c 6173 7469 635f  ce_id = elastic_
+0000ab30: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
+0000ab40: 616e 6365 5f69 640a 2020 2020 2020 2020  ance_id.        
+0000ab50: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0000ab60: 3d20 7265 7175 6573 745f 6964 0a0a 2020  = request_id..  
+0000ab70: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+0000ab80: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+0000ab90: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+0000aba0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+0000abb0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+0000abc0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0000abd0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0000abe0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000abf0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0000ac00: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0000ac10: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0000ac20: 6966 2073 656c 662e 636c 6965 6e74 5f69  if self.client_i
+0000ac30: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
+0000ac40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000ac50: 2020 2020 7265 7375 6c74 5b27 436c 6965      result['Clie
+0000ac60: 6e74 496e 7374 616e 6365 4964 275d 203d  ntInstanceId'] =
+0000ac70: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
+0000ac80: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+0000ac90: 2069 6620 7365 6c66 2e65 6c61 7374 6963   if self.elastic
+0000aca0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+0000acb0: 7461 6e63 655f 6964 2069 7320 6e6f 7420  tance_id is not 
+0000acc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000acd0: 2020 7265 7375 6c74 5b27 456c 6173 7469    result['Elasti
+0000ace0: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
+0000acf0: 616e 6365 4964 275d 203d 2073 656c 662e  anceId'] = self.
+0000ad00: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
+0000ad10: 7465 645f 696e 7374 616e 6365 5f69 640a  ted_instance_id.
+0000ad20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ad30: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
+0000ad40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000ad50: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
+0000ad60: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
+0000ad70: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
+0000ad80: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0000ad90: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+0000ada0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+0000adb0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+0000adc0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+0000add0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0000ade0: 7428 2743 6c69 656e 7449 6e73 7461 6e63  t('ClientInstanc
+0000adf0: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+0000ae00: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000ae10: 656c 662e 636c 6965 6e74 5f69 6e73 7461  elf.client_insta
+0000ae20: 6e63 655f 6964 203d 206d 2e67 6574 2827  nce_id = m.get('
+0000ae30: 436c 6965 6e74 496e 7374 616e 6365 4964  ClientInstanceId
+0000ae40: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0000ae50: 6765 7428 2745 6c61 7374 6963 4163 6365  get('ElasticAcce
+0000ae60: 6c65 7261 7465 6449 6e73 7461 6e63 6549  leratedInstanceI
+0000ae70: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0000ae80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000ae90: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
+0000aea0: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
+0000aeb0: 6420 3d20 6d2e 6765 7428 2745 6c61 7374  d = m.get('Elast
+0000aec0: 6963 4163 6365 6c65 7261 7465 6449 6e73  icAcceleratedIns
+0000aed0: 7461 6e63 6549 6427 290a 2020 2020 2020  tanceId').      
+0000aee0: 2020 6966 206d 2e67 6574 2827 5265 7175    if m.get('Requ
+0000aef0: 6573 7449 6427 2920 6973 206e 6f74 204e  estId') is not N
+0000af00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000af10: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+0000af20: 203d 206d 2e67 6574 2827 5265 7175 6573   = m.get('Reques
+0000af30: 7449 6427 290a 2020 2020 2020 2020 7265  tId').        re
+0000af40: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0000af50: 7320 4372 6561 7465 4561 6945 6373 5265  s CreateEaiEcsRe
+0000af60: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+0000af70: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0000af80: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0000af90: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+0000afa0: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+0000afb0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000afc0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
+0000afd0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+0000afe0: 2020 2062 6f64 793a 2043 7265 6174 6545     body: CreateE
+0000aff0: 6169 4563 7352 6573 706f 6e73 6542 6f64  aiEcsResponseBod
+0000b000: 7920 3d20 4e6f 6e65 2c0a 2020 2020 293a  y = None,.    ):
+0000b010: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+0000b020: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
+0000b030: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000b040: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+0000b050: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
+0000b060: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+0000b070: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0000b080: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0000b090: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+0000b0a0: 6571 7569 7265 6428 7365 6c66 2e68 6561  equired(self.hea
+0000b0b0: 6465 7273 2c20 2768 6561 6465 7273 2729  ders, 'headers')
+0000b0c0: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+0000b0d0: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+0000b0e0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0000b0f0: 2c20 2773 7461 7475 735f 636f 6465 2729  , 'status_code')
+0000b100: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+0000b110: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+0000b120: 7365 6c66 2e62 6f64 792c 2027 626f 6479  self.body, 'body
+0000b130: 2729 0a20 2020 2020 2020 2069 6620 7365  ').        if se
+0000b140: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+0000b150: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+0000b160: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+0000b170: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0000b180: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0000b190: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+0000b1a0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0000b1b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000b1c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000b1d0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0000b1e0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0000b1f0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+0000b200: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+0000b210: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000b220: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+0000b230: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+0000b240: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000b250: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+0000b260: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000b270: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+0000b280: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+0000b290: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+0000b2a0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+0000b2b0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+0000b2c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000b2d0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+0000b2e0: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+0000b2f0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000b300: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0000b310: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0000b320: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0000b330: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0000b340: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0000b350: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+0000b360: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0000b370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000b380: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+0000b390: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+0000b3a0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+0000b3b0: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+0000b3c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000b3d0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+0000b3e0: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+0000b3f0: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+0000b400: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+0000b410: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+0000b420: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0000b430: 705f 6d6f 6465 6c20 3d20 4372 6561 7465  p_model = Create
+0000b440: 4561 6945 6373 5265 7370 6f6e 7365 426f  EaiEcsResponseBo
+0000b450: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+0000b460: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+0000b470: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+0000b480: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+0000b490: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0000b4a0: 0a0a 636c 6173 7320 4372 6561 7465 4561  ..class CreateEa
+0000b4b0: 694a 7570 7974 6572 5265 7175 6573 7445  iJupyterRequestE
+0000b4c0: 6e76 6972 6f6e 6d65 6e74 5661 7228 5465  nvironmentVar(Te
+0000b4d0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0000b4e0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+0000b4f0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000b500: 206b 6579 3a20 7374 7220 3d20 4e6f 6e65   key: str = None
+0000b510: 2c0a 2020 2020 2020 2020 7661 6c75 653a  ,.        value:
+0000b520: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0000b530: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+0000b540: 2e6b 6579 203d 206b 6579 0a20 2020 2020  .key = key.     
+0000b550: 2020 2073 656c 662e 7661 6c75 6520 3d20     self.value = 
+0000b560: 7661 6c75 650a 0a20 2020 2064 6566 2076  value..    def v
+0000b570: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+0000b580: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0000b590: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0000b5a0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0000b5b0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+0000b5c0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+0000b5d0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+0000b5e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000b5f0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+0000b600: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+0000b610: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000b620: 2e6b 6579 2069 7320 6e6f 7420 4e6f 6e65  .key is not None
+0000b630: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000b640: 7375 6c74 5b27 4b65 7927 5d20 3d20 7365  sult['Key'] = se
+0000b650: 6c66 2e6b 6579 0a20 2020 2020 2020 2069  lf.key.        i
+0000b660: 6620 7365 6c66 2e76 616c 7565 2069 7320  f self.value is 
+0000b670: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000b680: 2020 2020 2020 7265 7375 6c74 5b27 5661        result['Va
+0000b690: 6c75 6527 5d20 3d20 7365 6c66 2e76 616c  lue'] = self.val
+0000b6a0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+0000b6b0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0000b6c0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0000b6d0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+0000b6e0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0000b6f0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0000b700: 2020 6966 206d 2e67 6574 2827 4b65 7927    if m.get('Key'
+0000b710: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0000b720: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000b730: 6b65 7920 3d20 6d2e 6765 7428 274b 6579  key = m.get('Key
+0000b740: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0000b750: 6765 7428 2756 616c 7565 2729 2069 7320  get('Value') is 
+0000b760: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000b770: 2020 2020 2020 7365 6c66 2e76 616c 7565        self.value
+0000b780: 203d 206d 2e67 6574 2827 5661 6c75 6527   = m.get('Value'
+0000b790: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000b7a0: 2073 656c 660a 0a0a 636c 6173 7320 4372   self...class Cr
+0000b7b0: 6561 7465 4561 694a 7570 7974 6572 5265  eateEaiJupyterRe
+0000b7c0: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
+0000b7d0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+0000b7e0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+0000b7f0: 0a20 2020 2020 2020 2063 6c69 656e 745f  .        client_
+0000b800: 746f 6b65 6e3a 2073 7472 203d 204e 6f6e  token: str = Non
+0000b810: 652c 0a20 2020 2020 2020 2065 6169 735f  e,.        eais_
+0000b820: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
+0000b830: 2c0a 2020 2020 2020 2020 6561 6973 5f74  ,.        eais_t
+0000b840: 7970 653a 2073 7472 203d 204e 6f6e 652c  ype: str = None,
+0000b850: 0a20 2020 2020 2020 2065 6e76 6972 6f6e  .        environ
+0000b860: 6d65 6e74 5f76 6172 3a20 4c69 7374 5b43  ment_var: List[C
+0000b870: 7265 6174 6545 6169 4a75 7079 7465 7252  reateEaiJupyterR
+0000b880: 6571 7565 7374 456e 7669 726f 6e6d 656e  equestEnvironmen
+0000b890: 7456 6172 5d20 3d20 4e6f 6e65 2c0a 2020  tVar] = None,.  
+0000b8a0: 2020 2020 2020 7265 6769 6f6e 5f69 643a        region_id:
+0000b8b0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0000b8c0: 2020 2020 2072 6573 6f75 7263 655f 6772       resource_gr
+0000b8d0: 6f75 705f 6964 3a20 7374 7220 3d20 4e6f  oup_id: str = No
+0000b8e0: 6e65 2c0a 2020 2020 2020 2020 7365 6375  ne,.        secu
+0000b8f0: 7269 7479 5f67 726f 7570 5f69 643a 2073  rity_group_id: s
+0000b900: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0000b910: 2020 2076 5f73 7769 7463 685f 6964 3a20     v_switch_id: 
+0000b920: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0000b930: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0000b940: 636c 6965 6e74 5f74 6f6b 656e 203d 2063  client_token = c
+0000b950: 6c69 656e 745f 746f 6b65 6e0a 2020 2020  lient_token.    
+0000b960: 2020 2020 7365 6c66 2e65 6169 735f 6e61      self.eais_na
+0000b970: 6d65 203d 2065 6169 735f 6e61 6d65 0a20  me = eais_name. 
+0000b980: 2020 2020 2020 2073 656c 662e 6561 6973         self.eais
+0000b990: 5f74 7970 6520 3d20 6561 6973 5f74 7970  _type = eais_typ
+0000b9a0: 650a 2020 2020 2020 2020 7365 6c66 2e65  e.        self.e
+0000b9b0: 6e76 6972 6f6e 6d65 6e74 5f76 6172 203d  nvironment_var =
+0000b9c0: 2065 6e76 6972 6f6e 6d65 6e74 5f76 6172   environment_var
+0000b9d0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0000b9e0: 6769 6f6e 5f69 6420 3d20 7265 6769 6f6e  gion_id = region
+0000b9f0: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+0000ba00: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
+0000ba10: 6964 203d 2072 6573 6f75 7263 655f 6772  id = resource_gr
+0000ba20: 6f75 705f 6964 0a20 2020 2020 2020 2073  oup_id.        s
+0000ba30: 656c 662e 7365 6375 7269 7479 5f67 726f  elf.security_gro
+0000ba40: 7570 5f69 6420 3d20 7365 6375 7269 7479  up_id = security
+0000ba50: 5f67 726f 7570 5f69 640a 2020 2020 2020  _group_id.      
+0000ba60: 2020 7365 6c66 2e76 5f73 7769 7463 685f    self.v_switch_
+0000ba70: 6964 203d 2076 5f73 7769 7463 685f 6964  id = v_switch_id
+0000ba80: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0000ba90: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0000baa0: 2020 6966 2073 656c 662e 656e 7669 726f    if self.enviro
+0000bab0: 6e6d 656e 745f 7661 723a 0a20 2020 2020  nment_var:.     
+0000bac0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+0000bad0: 7365 6c66 2e65 6e76 6972 6f6e 6d65 6e74  self.environment
+0000bae0: 5f76 6172 3a0a 2020 2020 2020 2020 2020  _var:.          
+0000baf0: 2020 2020 2020 6966 206b 3a0a 2020 2020        if k:.    
+0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb10: 6b2e 7661 6c69 6461 7465 2829 0a0a 2020  k.validate()..  
+0000bb20: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0000bb30: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0000bb40: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+0000bb50: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+0000bb60: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+0000bb70: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000bb80: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+0000bb90: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+0000bba0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000bbb0: 662e 636c 6965 6e74 5f74 6f6b 656e 2069  f.client_token i
+0000bbc0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000bbd0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0000bbe0: 436c 6965 6e74 546f 6b65 6e27 5d20 3d20  ClientToken'] = 
+0000bbf0: 7365 6c66 2e63 6c69 656e 745f 746f 6b65  self.client_toke
+0000bc00: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
+0000bc10: 662e 6561 6973 5f6e 616d 6520 6973 206e  f.eais_name is n
+0000bc20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000bc30: 2020 2020 2072 6573 756c 745b 2745 6169       result['Eai
+0000bc40: 734e 616d 6527 5d20 3d20 7365 6c66 2e65  sName'] = self.e
+0000bc50: 6169 735f 6e61 6d65 0a20 2020 2020 2020  ais_name.       
+0000bc60: 2069 6620 7365 6c66 2e65 6169 735f 7479   if self.eais_ty
+0000bc70: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
+0000bc80: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000bc90: 6c74 5b27 4561 6973 5479 7065 275d 203d  lt['EaisType'] =
+0000bca0: 2073 656c 662e 6561 6973 5f74 7970 650a   self.eais_type.
+0000bcb0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0000bcc0: 456e 7669 726f 6e6d 656e 7456 6172 275d  EnvironmentVar']
+0000bcd0: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
+0000bce0: 2073 656c 662e 656e 7669 726f 6e6d 656e   self.environmen
+0000bcf0: 745f 7661 7220 6973 206e 6f74 204e 6f6e  t_var is not Non
+0000bd00: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+0000bd10: 6f72 206b 2069 6e20 7365 6c66 2e65 6e76  or k in self.env
+0000bd20: 6972 6f6e 6d65 6e74 5f76 6172 3a0a 2020  ironment_var:.  
+0000bd30: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000bd40: 7375 6c74 5b27 456e 7669 726f 6e6d 656e  sult['Environmen
+0000bd50: 7456 6172 275d 2e61 7070 656e 6428 6b2e  tVar'].append(k.
+0000bd60: 746f 5f6d 6170 2829 2069 6620 6b20 656c  to_map() if k el
+0000bd70: 7365 204e 6f6e 6529 0a20 2020 2020 2020  se None).       
+0000bd80: 2069 6620 7365 6c66 2e72 6567 696f 6e5f   if self.region_
+0000bd90: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0000bda0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000bdb0: 6c74 5b27 5265 6769 6f6e 4964 275d 203d  lt['RegionId'] =
+0000bdc0: 2073 656c 662e 7265 6769 6f6e 5f69 640a   self.region_id.
+0000bdd0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000bde0: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
+0000bdf0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+0000be00: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0000be10: 745b 2752 6573 6f75 7263 6547 726f 7570  t['ResourceGroup
+0000be20: 4964 275d 203d 2073 656c 662e 7265 736f  Id'] = self.reso
+0000be30: 7572 6365 5f67 726f 7570 5f69 640a 2020  urce_group_id.  
+0000be40: 2020 2020 2020 6966 2073 656c 662e 7365        if self.se
+0000be50: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
+0000be60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000be70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0000be80: 2753 6563 7572 6974 7947 726f 7570 4964  'SecurityGroupId
+0000be90: 275d 203d 2073 656c 662e 7365 6375 7269  '] = self.securi
+0000bea0: 7479 5f67 726f 7570 5f69 640a 2020 2020  ty_group_id.    
+0000beb0: 2020 2020 6966 2073 656c 662e 765f 7377      if self.v_sw
+0000bec0: 6974 6368 5f69 6420 6973 206e 6f74 204e  itch_id is not N
+0000bed0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000bee0: 2072 6573 756c 745b 2756 5377 6974 6368   result['VSwitch
+0000bef0: 4964 275d 203d 2073 656c 662e 765f 7377  Id'] = self.v_sw
+0000bf00: 6974 6368 5f69 640a 2020 2020 2020 2020  itch_id.        
+0000bf10: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0000bf20: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+0000bf30: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+0000bf40: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0000bf50: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0000bf60: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0000bf70: 2743 6c69 656e 7454 6f6b 656e 2729 2069  'ClientToken') i
+0000bf80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000bf90: 2020 2020 2020 2020 7365 6c66 2e63 6c69          self.cli
+0000bfa0: 656e 745f 746f 6b65 6e20 3d20 6d2e 6765  ent_token = m.ge
+0000bfb0: 7428 2743 6c69 656e 7454 6f6b 656e 2729  t('ClientToken')
+0000bfc0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0000bfd0: 7428 2745 6169 734e 616d 6527 2920 6973  t('EaisName') is
+0000bfe0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000bff0: 2020 2020 2020 2073 656c 662e 6561 6973         self.eais
+0000c000: 5f6e 616d 6520 3d20 6d2e 6765 7428 2745  _name = m.get('E
+0000c010: 6169 734e 616d 6527 290a 2020 2020 2020  aisName').      
+0000c020: 2020 6966 206d 2e67 6574 2827 4561 6973    if m.get('Eais
+0000c030: 5479 7065 2729 2069 7320 6e6f 7420 4e6f  Type') is not No
+0000c040: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000c050: 7365 6c66 2e65 6169 735f 7479 7065 203d  self.eais_type =
+0000c060: 206d 2e67 6574 2827 4561 6973 5479 7065   m.get('EaisType
+0000c070: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0000c080: 656e 7669 726f 6e6d 656e 745f 7661 7220  environment_var 
+0000c090: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
+0000c0a0: 6d2e 6765 7428 2745 6e76 6972 6f6e 6d65  m.get('Environme
+0000c0b0: 6e74 5661 7227 2920 6973 206e 6f74 204e  ntVar') is not N
+0000c0c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000c0d0: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
+0000c0e0: 2745 6e76 6972 6f6e 6d65 6e74 5661 7227  'EnvironmentVar'
+0000c0f0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000c100: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+0000c110: 4372 6561 7465 4561 694a 7570 7974 6572  CreateEaiJupyter
+0000c120: 5265 7175 6573 7445 6e76 6972 6f6e 6d65  RequestEnvironme
+0000c130: 6e74 5661 7228 290a 2020 2020 2020 2020  ntVar().        
+0000c140: 2020 2020 2020 2020 7365 6c66 2e65 6e76          self.env
+0000c150: 6972 6f6e 6d65 6e74 5f76 6172 2e61 7070  ironment_var.app
+0000c160: 656e 6428 7465 6d70 5f6d 6f64 656c 2e66  end(temp_model.f
+0000c170: 726f 6d5f 6d61 7028 6b29 290a 2020 2020  rom_map(k)).    
+0000c180: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+0000c190: 6769 6f6e 4964 2729 2069 7320 6e6f 7420  gionId') is not 
+0000c1a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000c1b0: 2020 7365 6c66 2e72 6567 696f 6e5f 6964    self.region_id
+0000c1c0: 203d 206d 2e67 6574 2827 5265 6769 6f6e   = m.get('Region
+0000c1d0: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0000c1e0: 6d2e 6765 7428 2752 6573 6f75 7263 6547  m.get('ResourceG
+0000c1f0: 726f 7570 4964 2729 2069 7320 6e6f 7420  roupId') is not 
+0000c200: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000c210: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+0000c220: 6772 6f75 705f 6964 203d 206d 2e67 6574  group_id = m.get
+0000c230: 2827 5265 736f 7572 6365 4772 6f75 7049  ('ResourceGroupI
+0000c240: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+0000c250: 2e67 6574 2827 5365 6375 7269 7479 4772  .get('SecurityGr
+0000c260: 6f75 7049 6427 2920 6973 206e 6f74 204e  oupId') is not N
+0000c270: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000c280: 2073 656c 662e 7365 6375 7269 7479 5f67   self.security_g
+0000c290: 726f 7570 5f69 6420 3d20 6d2e 6765 7428  roup_id = m.get(
+0000c2a0: 2753 6563 7572 6974 7947 726f 7570 4964  'SecurityGroupId
+0000c2b0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0000c2c0: 6765 7428 2756 5377 6974 6368 4964 2729  get('VSwitchId')
+0000c2d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000c2e0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+0000c2f0: 5f73 7769 7463 685f 6964 203d 206d 2e67  _switch_id = m.g
+0000c300: 6574 2827 5653 7769 7463 6849 6427 290a  et('VSwitchId').
+0000c310: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000c320: 656c 660a 0a0a 636c 6173 7320 4372 6561  elf...class Crea
+0000c330: 7465 4561 694a 7570 7974 6572 5368 7269  teEaiJupyterShri
+0000c340: 6e6b 5265 7175 6573 7428 5465 614d 6f64  nkRequest(TeaMod
+0000c350: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+0000c360: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+0000c370: 656c 662c 0a20 2020 2020 2020 2063 6c69  elf,.        cli
+0000c380: 656e 745f 746f 6b65 6e3a 2073 7472 203d  ent_token: str =
+0000c390: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
+0000c3a0: 6169 735f 6e61 6d65 3a20 7374 7220 3d20  ais_name: str = 
+0000c3b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6561  None,.        ea
+0000c3c0: 6973 5f74 7970 653a 2073 7472 203d 204e  is_type: str = N
+0000c3d0: 6f6e 652c 0a20 2020 2020 2020 2065 6e76  one,.        env
+0000c3e0: 6972 6f6e 6d65 6e74 5f76 6172 5f73 6872  ironment_var_shr
+0000c3f0: 696e 6b3a 2073 7472 203d 204e 6f6e 652c  ink: str = None,
+0000c400: 0a20 2020 2020 2020 2072 6567 696f 6e5f  .        region_
+0000c410: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0000c420: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+0000c430: 5f67 726f 7570 5f69 643a 2073 7472 203d  _group_id: str =
+0000c440: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+0000c450: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
+0000c460: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0000c470: 2020 2020 2020 765f 7377 6974 6368 5f69        v_switch_i
+0000c480: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0000c490: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+0000c4a0: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
+0000c4b0: 3d20 636c 6965 6e74 5f74 6f6b 656e 0a20  = client_token. 
+0000c4c0: 2020 2020 2020 2073 656c 662e 6561 6973         self.eais
+0000c4d0: 5f6e 616d 6520 3d20 6561 6973 5f6e 616d  _name = eais_nam
+0000c4e0: 650a 2020 2020 2020 2020 7365 6c66 2e65  e.        self.e
+0000c4f0: 6169 735f 7479 7065 203d 2065 6169 735f  ais_type = eais_
+0000c500: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
+0000c510: 662e 656e 7669 726f 6e6d 656e 745f 7661  f.environment_va
+0000c520: 725f 7368 7269 6e6b 203d 2065 6e76 6972  r_shrink = envir
+0000c530: 6f6e 6d65 6e74 5f76 6172 5f73 6872 696e  onment_var_shrin
+0000c540: 6b0a 2020 2020 2020 2020 7365 6c66 2e72  k.        self.r
+0000c550: 6567 696f 6e5f 6964 203d 2072 6567 696f  egion_id = regio
+0000c560: 6e5f 6964 0a20 2020 2020 2020 2073 656c  n_id.        sel
+0000c570: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
+0000c580: 5f69 6420 3d20 7265 736f 7572 6365 5f67  _id = resource_g
+0000c590: 726f 7570 5f69 640a 2020 2020 2020 2020  roup_id.        
+0000c5a0: 7365 6c66 2e73 6563 7572 6974 795f 6772  self.security_gr
+0000c5b0: 6f75 705f 6964 203d 2073 6563 7572 6974  oup_id = securit
+0000c5c0: 795f 6772 6f75 705f 6964 0a20 2020 2020  y_group_id.     
+0000c5d0: 2020 2073 656c 662e 765f 7377 6974 6368     self.v_switch
+0000c5e0: 5f69 6420 3d20 765f 7377 6974 6368 5f69  _id = v_switch_i
+0000c5f0: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
+0000c600: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+0000c610: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+0000c620: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0000c630: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0000c640: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+0000c650: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0000c660: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000c670: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0000c680: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0000c690: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0000c6a0: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
+0000c6b0: 656e 745f 746f 6b65 6e20 6973 206e 6f74  ent_token is not
+0000c6c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000c6d0: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
+0000c6e0: 7454 6f6b 656e 275d 203d 2073 656c 662e  tToken'] = self.
+0000c6f0: 636c 6965 6e74 5f74 6f6b 656e 0a20 2020  client_token.   
+0000c700: 2020 2020 2069 6620 7365 6c66 2e65 6169       if self.eai
+0000c710: 735f 6e61 6d65 2069 7320 6e6f 7420 4e6f  s_name is not No
+0000c720: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000c730: 7265 7375 6c74 5b27 4561 6973 4e61 6d65  result['EaisName
+0000c740: 275d 203d 2073 656c 662e 6561 6973 5f6e  '] = self.eais_n
+0000c750: 616d 650a 2020 2020 2020 2020 6966 2073  ame.        if s
+0000c760: 656c 662e 6561 6973 5f74 7970 6520 6973  elf.eais_type is
+0000c770: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000c780: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
+0000c790: 6169 7354 7970 6527 5d20 3d20 7365 6c66  aisType'] = self
+0000c7a0: 2e65 6169 735f 7479 7065 0a20 2020 2020  .eais_type.     
+0000c7b0: 2020 2069 6620 7365 6c66 2e65 6e76 6972     if self.envir
+0000c7c0: 6f6e 6d65 6e74 5f76 6172 5f73 6872 696e  onment_var_shrin
+0000c7d0: 6b20 6973 206e 6f74 204e 6f6e 653a 0a20  k is not None:. 
+0000c7e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0000c7f0: 745b 2745 6e76 6972 6f6e 6d65 6e74 5661  t['EnvironmentVa
+0000c800: 7227 5d20 3d20 7365 6c66 2e65 6e76 6972  r'] = self.envir
+0000c810: 6f6e 6d65 6e74 5f76 6172 5f73 6872 696e  onment_var_shrin
+0000c820: 6b0a 2020 2020 2020 2020 6966 2073 656c  k.        if sel
+0000c830: 662e 7265 6769 6f6e 5f69 6420 6973 206e  f.region_id is n
 0000c840: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000c850: 2020 2020 2073 656c 662e 666f 7263 6520       self.force 
-0000c860: 3d20 6d2e 6765 7428 2746 6f72 6365 2729  = m.get('Force')
-0000c870: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0000c880: 7428 2752 6567 696f 6e49 6427 2920 6973  t('RegionId') is
-0000c890: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000c8a0: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
-0000c8b0: 6f6e 5f69 6420 3d20 6d2e 6765 7428 2752  on_id = m.get('R
-0000c8c0: 6567 696f 6e49 6427 290a 2020 2020 2020  egionId').      
-0000c8d0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0000c8e0: 636c 6173 7320 4465 6c65 7465 4561 6952  class DeleteEaiR
-0000c8f0: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-0000c900: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0000c910: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0000c920: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
-0000c930: 6571 7565 7374 5f69 643a 2073 7472 203d  equest_id: str =
-0000c940: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-0000c950: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-0000c960: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
-0000c970: 6964 0a0a 2020 2020 6465 6620 7661 6c69  id..    def vali
-0000c980: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-0000c990: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-0000c9a0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0000c9b0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0000c9c0: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-0000c9d0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0000c9e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000c9f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000ca00: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0000ca10: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0000ca20: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-0000ca30: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
-0000ca40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000ca50: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
-0000ca60: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
-0000ca70: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
-0000ca80: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0000ca90: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0000caa0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-0000cab0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-0000cac0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-0000cad0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0000cae0: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
-0000caf0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000cb00: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-0000cb10: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
-0000cb20: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
-0000cb30: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0000cb40: 0a63 6c61 7373 2044 656c 6574 6545 6169  .class DeleteEai
-0000cb50: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-0000cb60: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-0000cb70: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0000cb80: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-0000cb90: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-0000cba0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0000cbb0: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-0000cbc0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-0000cbd0: 2020 2020 2062 6f64 793a 2044 656c 6574       body: Delet
-0000cbe0: 6545 6169 5265 7370 6f6e 7365 426f 6479  eEaiResponseBody
-0000cbf0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-0000cc00: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0000cc10: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-0000cc20: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000cc30: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-0000cc40: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
-0000cc50: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
-0000cc60: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0000cc70: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000cc80: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-0000cc90: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
-0000cca0: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
-0000ccb0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-0000ccc0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-0000ccd0: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
-0000cce0: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
-0000ccf0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-0000cd00: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-0000cd10: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
-0000cd20: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000cd30: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-0000cd40: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-0000cd50: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-0000cd60: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0000cd70: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0000cd80: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-0000cd90: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0000cda0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000cdb0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000cdc0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0000cdd0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0000cde0: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-0000cdf0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-0000ce00: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000ce10: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-0000ce20: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-0000ce30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000ce40: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-0000ce50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000ce60: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-0000ce70: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-0000ce80: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-0000ce90: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0000cea0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-0000ceb0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000cec0: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-0000ced0: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-0000cee0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0000cef0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0000cf00: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-0000cf10: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-0000cf20: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0000cf30: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0000cf40: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-0000cf50: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0000cf60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000cf70: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-0000cf80: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-0000cf90: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-0000cfa0: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-0000cfb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000cfc0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-0000cfd0: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-0000cfe0: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-0000cff0: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-0000d000: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0000d010: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000d020: 5f6d 6f64 656c 203d 2044 656c 6574 6545  _model = DeleteE
-0000d030: 6169 5265 7370 6f6e 7365 426f 6479 2829  aiResponseBody()
-0000d040: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d050: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
-0000d060: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
-0000d070: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
-0000d080: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-0000d090: 6173 7320 4465 6c65 7465 4561 6941 6c6c  ass DeleteEaiAll
-0000d0a0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
-0000d0b0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-0000d0c0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-0000d0d0: 662c 0a20 2020 2020 2020 2063 6c69 656e  f,.        clien
-0000d0e0: 745f 696e 7374 616e 6365 5f69 643a 2073  t_instance_id: s
-0000d0f0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0000d100: 2020 2065 6c61 7374 6963 5f61 6363 656c     elastic_accel
-0000d110: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
-0000d120: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-0000d130: 2020 2020 2020 2020 7265 6769 6f6e 5f69          region_i
-0000d140: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-0000d150: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-0000d160: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
-0000d170: 6365 5f69 6420 3d20 636c 6965 6e74 5f69  ce_id = client_i
-0000d180: 6e73 7461 6e63 655f 6964 0a20 2020 2020  nstance_id.     
-0000d190: 2020 2073 656c 662e 656c 6173 7469 635f     self.elastic_
-0000d1a0: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
-0000d1b0: 616e 6365 5f69 6420 3d20 656c 6173 7469  ance_id = elasti
-0000d1c0: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
-0000d1d0: 7374 616e 6365 5f69 640a 2020 2020 2020  stance_id.      
-0000d1e0: 2020 7365 6c66 2e72 6567 696f 6e5f 6964    self.region_id
-0000d1f0: 203d 2072 6567 696f 6e5f 6964 0a0a 2020   = region_id..  
-0000d200: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0000d210: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-0000d220: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-0000d230: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-0000d240: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-0000d250: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0000d260: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0000d270: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000d280: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0000d290: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0000d2a0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0000d2b0: 6966 2073 656c 662e 636c 6965 6e74 5f69  if self.client_i
-0000d2c0: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
-0000d2d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000d2e0: 2020 2020 7265 7375 6c74 5b27 436c 6965      result['Clie
-0000d2f0: 6e74 496e 7374 616e 6365 4964 275d 203d  ntInstanceId'] =
-0000d300: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
-0000d310: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
-0000d320: 2069 6620 7365 6c66 2e65 6c61 7374 6963   if self.elastic
-0000d330: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
-0000d340: 7461 6e63 655f 6964 2069 7320 6e6f 7420  tance_id is not 
-0000d350: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000d360: 2020 7265 7375 6c74 5b27 456c 6173 7469    result['Elasti
-0000d370: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
-0000d380: 616e 6365 4964 275d 203d 2073 656c 662e  anceId'] = self.
-0000d390: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
-0000d3a0: 7465 645f 696e 7374 616e 6365 5f69 640a  ted_instance_id.
-0000d3b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d3c0: 7265 6769 6f6e 5f69 6420 6973 206e 6f74  region_id is not
-0000d3d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000d3e0: 2020 2072 6573 756c 745b 2752 6567 696f     result['Regio
-0000d3f0: 6e49 6427 5d20 3d20 7365 6c66 2e72 6567  nId'] = self.reg
-0000d400: 696f 6e5f 6964 0a20 2020 2020 2020 2072  ion_id.        r
-0000d410: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-0000d420: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-0000d430: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-0000d440: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0000d450: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0000d460: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0000d470: 436c 6965 6e74 496e 7374 616e 6365 4964  ClientInstanceId
-0000d480: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0000d490: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d4a0: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
-0000d4b0: 5f69 6420 3d20 6d2e 6765 7428 2743 6c69  _id = m.get('Cli
-0000d4c0: 656e 7449 6e73 7461 6e63 6549 6427 290a  entInstanceId').
-0000d4d0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0000d4e0: 2827 456c 6173 7469 6341 6363 656c 6572  ('ElasticAcceler
-0000d4f0: 6174 6564 496e 7374 616e 6365 4964 2729  atedInstanceId')
-0000d500: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000d510: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-0000d520: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
-0000d530: 6564 5f69 6e73 7461 6e63 655f 6964 203d  ed_instance_id =
-0000d540: 206d 2e67 6574 2827 456c 6173 7469 6341   m.get('ElasticA
-0000d550: 6363 656c 6572 6174 6564 496e 7374 616e  cceleratedInstan
-0000d560: 6365 4964 2729 0a20 2020 2020 2020 2069  ceId').        i
-0000d570: 6620 6d2e 6765 7428 2752 6567 696f 6e49  f m.get('RegionI
-0000d580: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-0000d590: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d5a0: 662e 7265 6769 6f6e 5f69 6420 3d20 6d2e  f.region_id = m.
-0000d5b0: 6765 7428 2752 6567 696f 6e49 6427 290a  get('RegionId').
-0000d5c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000d5d0: 656c 660a 0a0a 636c 6173 7320 4465 6c65  elf...class Dele
-0000d5e0: 7465 4561 6941 6c6c 5265 7370 6f6e 7365  teEaiAllResponse
-0000d5f0: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
-0000d600: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000d610: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000d620: 2020 2020 2020 2020 7265 7175 6573 745f          request_
-0000d630: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-0000d640: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-0000d650: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-0000d660: 2072 6571 7565 7374 5f69 640a 0a20 2020   request_id..   
-0000d670: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0000d680: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-0000d690: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-0000d6a0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0000d6b0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-0000d6c0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0000d6d0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-0000d6e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000d6f0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-0000d700: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0000d710: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0000d720: 6620 7365 6c66 2e72 6571 7565 7374 5f69  f self.request_i
-0000d730: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-0000d740: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000d750: 745b 2752 6571 7565 7374 4964 275d 203d  t['RequestId'] =
-0000d760: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-0000d770: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000d780: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-0000d790: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-0000d7a0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-0000d7b0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0000d7c0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0000d7d0: 6966 206d 2e67 6574 2827 5265 7175 6573  if m.get('Reques
-0000d7e0: 7449 6427 2920 6973 206e 6f74 204e 6f6e  tId') is not Non
-0000d7f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0000d800: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-0000d810: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
-0000d820: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
-0000d830: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-0000d840: 4465 6c65 7465 4561 6941 6c6c 5265 7370  DeleteEaiAllResp
-0000d850: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-0000d860: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0000d870: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0000d880: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-0000d890: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
-0000d8a0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000d8b0: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
-0000d8c0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000d8d0: 2062 6f64 793a 2044 656c 6574 6545 6169   body: DeleteEai
-0000d8e0: 416c 6c52 6573 706f 6e73 6542 6f64 7920  AllResponseBody 
-0000d8f0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0000d900: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0000d910: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
-0000d920: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0000d930: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-0000d940: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
-0000d950: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
-0000d960: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0000d970: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-0000d980: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0000d990: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
-0000d9a0: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
-0000d9b0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0000d9c0: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0000d9d0: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
-0000d9e0: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
-0000d9f0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0000da00: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0000da10: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
-0000da20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000da30: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
-0000da40: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
-0000da50: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-0000da60: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0000da70: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0000da80: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-0000da90: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-0000daa0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000dab0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-0000dac0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-0000dad0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-0000dae0: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
-0000daf0: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
-0000db00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000db10: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
-0000db20: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
-0000db30: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0000db40: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
-0000db50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000db60: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
-0000db70: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
-0000db80: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-0000db90: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-0000dba0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000dbb0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000dbc0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
-0000dbd0: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
-0000dbe0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0000dbf0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0000dc00: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-0000dc10: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-0000dc20: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-0000dc30: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0000dc40: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-0000dc50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000dc60: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-0000dc70: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
-0000dc80: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-0000dc90: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
-0000dca0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
-0000dcb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000dcc0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-0000dcd0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
-0000dce0: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
-0000dcf0: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-0000dd00: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0000dd10: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-0000dd20: 6d6f 6465 6c20 3d20 4465 6c65 7465 4561  model = DeleteEa
-0000dd30: 6941 6c6c 5265 7370 6f6e 7365 426f 6479  iAllResponseBody
-0000dd40: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-0000dd50: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-0000dd60: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-0000dd70: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-0000dd80: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0000dd90: 636c 6173 7320 4465 7363 7269 6265 4561  class DescribeEa
-0000dda0: 6973 5265 7175 6573 7428 5465 614d 6f64  isRequest(TeaMod
-0000ddb0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-0000ddc0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0000ddd0: 656c 662c 0a20 2020 2020 2020 2065 6c61  elf,.        ela
-0000dde0: 7374 6963 5f61 6363 656c 6572 6174 6564  stic_accelerated
-0000ddf0: 5f69 6e73 7461 6e63 655f 6964 733a 2073  _instance_ids: s
-0000de00: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0000de10: 2020 2069 6e73 7461 6e63 655f 6e61 6d65     instance_name
-0000de20: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0000de30: 2020 2020 2020 696e 7374 616e 6365 5f74        instance_t
-0000de40: 7970 653a 2073 7472 203d 204e 6f6e 652c  ype: str = None,
-0000de50: 0a20 2020 2020 2020 2070 6167 655f 6e75  .        page_nu
-0000de60: 6d62 6572 3a20 696e 7420 3d20 4e6f 6e65  mber: int = None
-0000de70: 2c0a 2020 2020 2020 2020 7061 6765 5f73  ,.        page_s
-0000de80: 697a 653a 2069 6e74 203d 204e 6f6e 652c  ize: int = None,
-0000de90: 0a20 2020 2020 2020 2072 6567 696f 6e5f  .        region_
-0000dea0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-0000deb0: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-0000dec0: 5f67 726f 7570 5f69 643a 2073 7472 203d  _group_id: str =
-0000ded0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-0000dee0: 7461 7475 733a 2073 7472 203d 204e 6f6e  tatus: str = Non
-0000def0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-0000df00: 2020 7365 6c66 2e65 6c61 7374 6963 5f61    self.elastic_a
-0000df10: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
-0000df20: 6e63 655f 6964 7320 3d20 656c 6173 7469  nce_ids = elasti
-0000df30: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
-0000df40: 7374 616e 6365 5f69 6473 0a20 2020 2020  stance_ids.     
-0000df50: 2020 2073 656c 662e 696e 7374 616e 6365     self.instance
-0000df60: 5f6e 616d 6520 3d20 696e 7374 616e 6365  _name = instance
-0000df70: 5f6e 616d 650a 2020 2020 2020 2020 7365  _name.        se
-0000df80: 6c66 2e69 6e73 7461 6e63 655f 7479 7065  lf.instance_type
-0000df90: 203d 2069 6e73 7461 6e63 655f 7479 7065   = instance_type
-0000dfa0: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
-0000dfb0: 6765 5f6e 756d 6265 7220 3d20 7061 6765  ge_number = page
-0000dfc0: 5f6e 756d 6265 720a 2020 2020 2020 2020  _number.        
-0000dfd0: 7365 6c66 2e70 6167 655f 7369 7a65 203d  self.page_size =
-0000dfe0: 2070 6167 655f 7369 7a65 0a20 2020 2020   page_size.     
-0000dff0: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
-0000e000: 6420 3d20 7265 6769 6f6e 5f69 640a 2020  d = region_id.  
-0000e010: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
-0000e020: 7263 655f 6772 6f75 705f 6964 203d 2072  rce_group_id = r
-0000e030: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-0000e040: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000e050: 6174 7573 203d 2073 7461 7475 730a 0a20  atus = status.. 
-0000e060: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0000e070: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0000e080: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-0000e090: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0000e0a0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0000e0b0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0000e0c0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0000e0d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000e0e0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0000e0f0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0000e100: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0000e110: 2069 6620 7365 6c66 2e65 6c61 7374 6963   if self.elastic
-0000e120: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
-0000e130: 7461 6e63 655f 6964 7320 6973 206e 6f74  tance_ids is not
-0000e140: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000e150: 2020 2072 6573 756c 745b 2745 6c61 7374     result['Elast
-0000e160: 6963 4163 6365 6c65 7261 7465 6449 6e73  icAcceleratedIns
-0000e170: 7461 6e63 6549 6473 275d 203d 2073 656c  tanceIds'] = sel
-0000e180: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-0000e190: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-0000e1a0: 6473 0a20 2020 2020 2020 2069 6620 7365  ds.        if se
-0000e1b0: 6c66 2e69 6e73 7461 6e63 655f 6e61 6d65  lf.instance_name
-0000e1c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e1d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000e1e0: 5b27 496e 7374 616e 6365 4e61 6d65 275d  ['InstanceName']
-0000e1f0: 203d 2073 656c 662e 696e 7374 616e 6365   = self.instance
-0000e200: 5f6e 616d 650a 2020 2020 2020 2020 6966  _name.        if
-0000e210: 2073 656c 662e 696e 7374 616e 6365 5f74   self.instance_t
-0000e220: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
-0000e230: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000e240: 756c 745b 2749 6e73 7461 6e63 6554 7970  ult['InstanceTyp
-0000e250: 6527 5d20 3d20 7365 6c66 2e69 6e73 7461  e'] = self.insta
-0000e260: 6e63 655f 7479 7065 0a20 2020 2020 2020  nce_type.       
-0000e270: 2069 6620 7365 6c66 2e70 6167 655f 6e75   if self.page_nu
-0000e280: 6d62 6572 2069 7320 6e6f 7420 4e6f 6e65  mber is not None
-0000e290: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000e2a0: 7375 6c74 5b27 5061 6765 4e75 6d62 6572  sult['PageNumber
-0000e2b0: 275d 203d 2073 656c 662e 7061 6765 5f6e  '] = self.page_n
-0000e2c0: 756d 6265 720a 2020 2020 2020 2020 6966  umber.        if
-0000e2d0: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
-0000e2e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000e2f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000e300: 2750 6167 6553 697a 6527 5d20 3d20 7365  'PageSize'] = se
-0000e310: 6c66 2e70 6167 655f 7369 7a65 0a20 2020  lf.page_size.   
-0000e320: 2020 2020 2069 6620 7365 6c66 2e72 6567       if self.reg
-0000e330: 696f 6e5f 6964 2069 7320 6e6f 7420 4e6f  ion_id is not No
-0000e340: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000e350: 7265 7375 6c74 5b27 5265 6769 6f6e 4964  result['RegionId
-0000e360: 275d 203d 2073 656c 662e 7265 6769 6f6e  '] = self.region
-0000e370: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-0000e380: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
-0000e390: 7570 5f69 6420 6973 206e 6f74 204e 6f6e  up_id is not Non
-0000e3a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000e3b0: 6573 756c 745b 2752 6573 6f75 7263 6547  esult['ResourceG
-0000e3c0: 726f 7570 4964 275d 203d 2073 656c 662e  roupId'] = self.
-0000e3d0: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
-0000e3e0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-0000e3f0: 662e 7374 6174 7573 2069 7320 6e6f 7420  f.status is not 
-0000e400: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000e410: 2020 7265 7375 6c74 5b27 5374 6174 7573    result['Status
-0000e420: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-0000e430: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000e440: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-0000e450: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-0000e460: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-0000e470: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0000e480: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0000e490: 6966 206d 2e67 6574 2827 456c 6173 7469  if m.get('Elasti
-0000e4a0: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
-0000e4b0: 616e 6365 4964 7327 2920 6973 206e 6f74  anceIds') is not
-0000e4c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000e4d0: 2020 2073 656c 662e 656c 6173 7469 635f     self.elastic_
-0000e4e0: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
-0000e4f0: 616e 6365 5f69 6473 203d 206d 2e67 6574  ance_ids = m.get
-0000e500: 2827 456c 6173 7469 6341 6363 656c 6572  ('ElasticAcceler
-0000e510: 6174 6564 496e 7374 616e 6365 4964 7327  atedInstanceIds'
-0000e520: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0000e530: 6574 2827 496e 7374 616e 6365 4e61 6d65  et('InstanceName
-0000e540: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0000e550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e560: 2e69 6e73 7461 6e63 655f 6e61 6d65 203d  .instance_name =
-0000e570: 206d 2e67 6574 2827 496e 7374 616e 6365   m.get('Instance
-0000e580: 4e61 6d65 2729 0a20 2020 2020 2020 2069  Name').        i
-0000e590: 6620 6d2e 6765 7428 2749 6e73 7461 6e63  f m.get('Instanc
-0000e5a0: 6554 7970 6527 2920 6973 206e 6f74 204e  eType') is not N
-0000e5b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000e5c0: 2073 656c 662e 696e 7374 616e 6365 5f74   self.instance_t
-0000e5d0: 7970 6520 3d20 6d2e 6765 7428 2749 6e73  ype = m.get('Ins
-0000e5e0: 7461 6e63 6554 7970 6527 290a 2020 2020  tanceType').    
-0000e5f0: 2020 2020 6966 206d 2e67 6574 2827 5061      if m.get('Pa
-0000e600: 6765 4e75 6d62 6572 2729 2069 7320 6e6f  geNumber') is no
-0000e610: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000e620: 2020 2020 7365 6c66 2e70 6167 655f 6e75      self.page_nu
-0000e630: 6d62 6572 203d 206d 2e67 6574 2827 5061  mber = m.get('Pa
-0000e640: 6765 4e75 6d62 6572 2729 0a20 2020 2020  geNumber').     
-0000e650: 2020 2069 6620 6d2e 6765 7428 2750 6167     if m.get('Pag
-0000e660: 6553 697a 6527 2920 6973 206e 6f74 204e  eSize') is not N
-0000e670: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000e680: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
-0000e690: 3d20 6d2e 6765 7428 2750 6167 6553 697a  = m.get('PageSiz
-0000e6a0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-0000e6b0: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
-0000e6c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e6d0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000e6e0: 6567 696f 6e5f 6964 203d 206d 2e67 6574  egion_id = m.get
-0000e6f0: 2827 5265 6769 6f6e 4964 2729 0a20 2020  ('RegionId').   
-0000e700: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-0000e710: 6573 6f75 7263 6547 726f 7570 4964 2729  esourceGroupId')
-0000e720: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e730: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000e740: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-0000e750: 203d 206d 2e67 6574 2827 5265 736f 7572   = m.get('Resour
-0000e760: 6365 4772 6f75 7049 6427 290a 2020 2020  ceGroupId').    
-0000e770: 2020 2020 6966 206d 2e67 6574 2827 5374      if m.get('St
-0000e780: 6174 7573 2729 2069 7320 6e6f 7420 4e6f  atus') is not No
-0000e790: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0000e7a0: 7365 6c66 2e73 7461 7475 7320 3d20 6d2e  self.status = m.
-0000e7b0: 6765 7428 2753 7461 7475 7327 290a 2020  get('Status').  
-0000e7c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000e7d0: 660a 0a0a 636c 6173 7320 4465 7363 7269  f...class Descri
-0000e7e0: 6265 4561 6973 5265 7370 6f6e 7365 426f  beEaisResponseBo
-0000e7f0: 6479 496e 7374 616e 6365 7349 6e73 7461  dyInstancesInsta
-0000e800: 6e63 6554 6167 7354 6167 2854 6561 4d6f  nceTagsTag(TeaMo
-0000e810: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0000e820: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0000e830: 7365 6c66 2c0a 2020 2020 2020 2020 7461  self,.        ta
-0000e840: 675f 6b65 793a 2073 7472 203d 204e 6f6e  g_key: str = Non
-0000e850: 652c 0a20 2020 2020 2020 2074 6167 5f76  e,.        tag_v
-0000e860: 616c 7565 3a20 7374 7220 3d20 4e6f 6e65  alue: str = None
-0000e870: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0000e880: 2073 656c 662e 7461 675f 6b65 7920 3d20   self.tag_key = 
-0000e890: 7461 675f 6b65 790a 2020 2020 2020 2020  tag_key.        
-0000e8a0: 7365 6c66 2e74 6167 5f76 616c 7565 203d  self.tag_value =
-0000e8b0: 2074 6167 5f76 616c 7565 0a0a 2020 2020   tag_value..    
-0000e8c0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0000e8d0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-0000e8e0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-0000e8f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000e900: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-0000e910: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0000e920: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-0000e930: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000e940: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-0000e950: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-0000e960: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0000e970: 2073 656c 662e 7461 675f 6b65 7920 6973   self.tag_key is
-0000e980: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000e990: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
-0000e9a0: 6167 4b65 7927 5d20 3d20 7365 6c66 2e74  agKey'] = self.t
-0000e9b0: 6167 5f6b 6579 0a20 2020 2020 2020 2069  ag_key.        i
-0000e9c0: 6620 7365 6c66 2e74 6167 5f76 616c 7565  f self.tag_value
-0000e9d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e9e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000e9f0: 5b27 5461 6756 616c 7565 275d 203d 2073  ['TagValue'] = s
-0000ea00: 656c 662e 7461 675f 7661 6c75 650a 2020  elf.tag_value.  
-0000ea10: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0000ea20: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0000ea30: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-0000ea40: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-0000ea50: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-0000ea60: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0000ea70: 6d2e 6765 7428 2754 6167 4b65 7927 2920  m.get('TagKey') 
-0000ea80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000ea90: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
-0000eaa0: 675f 6b65 7920 3d20 6d2e 6765 7428 2754  g_key = m.get('T
-0000eab0: 6167 4b65 7927 290a 2020 2020 2020 2020  agKey').        
-0000eac0: 6966 206d 2e67 6574 2827 5461 6756 616c  if m.get('TagVal
-0000ead0: 7565 2729 2069 7320 6e6f 7420 4e6f 6e65  ue') is not None
-0000eae0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000eaf0: 6c66 2e74 6167 5f76 616c 7565 203d 206d  lf.tag_value = m
-0000eb00: 2e67 6574 2827 5461 6756 616c 7565 2729  .get('TagValue')
-0000eb10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000eb20: 7365 6c66 0a0a 0a63 6c61 7373 2044 6573  self...class Des
-0000eb30: 6372 6962 6545 6169 7352 6573 706f 6e73  cribeEaisRespons
-0000eb40: 6542 6f64 7949 6e73 7461 6e63 6573 496e  eBodyInstancesIn
-0000eb50: 7374 616e 6365 5461 6773 2854 6561 4d6f  stanceTags(TeaMo
-0000eb60: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0000eb70: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0000eb80: 7365 6c66 2c0a 2020 2020 2020 2020 7461  self,.        ta
-0000eb90: 673a 204c 6973 745b 4465 7363 7269 6265  g: List[Describe
-0000eba0: 4561 6973 5265 7370 6f6e 7365 426f 6479  EaisResponseBody
-0000ebb0: 496e 7374 616e 6365 7349 6e73 7461 6e63  InstancesInstanc
-0000ebc0: 6554 6167 7354 6167 5d20 3d20 4e6f 6e65  eTagsTag] = None
-0000ebd0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0000ebe0: 2073 656c 662e 7461 6720 3d20 7461 670a   self.tag = tag.
-0000ebf0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0000ec00: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0000ec10: 2069 6620 7365 6c66 2e74 6167 3a0a 2020   if self.tag:.  
-0000ec20: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
-0000ec30: 696e 2073 656c 662e 7461 673a 0a20 2020  in self.tag:.   
-0000ec40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000ec50: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
-0000ec60: 2020 2020 2020 206b 2e76 616c 6964 6174         k.validat
-0000ec70: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-0000ec80: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0000ec90: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0000eca0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0000ecb0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+0000c850: 2020 2020 2072 6573 756c 745b 2752 6567       result['Reg
+0000c860: 696f 6e49 6427 5d20 3d20 7365 6c66 2e72  ionId'] = self.r
+0000c870: 6567 696f 6e5f 6964 0a20 2020 2020 2020  egion_id.       
+0000c880: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
+0000c890: 655f 6772 6f75 705f 6964 2069 7320 6e6f  e_group_id is no
+0000c8a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000c8b0: 2020 2020 7265 7375 6c74 5b27 5265 736f      result['Reso
+0000c8c0: 7572 6365 4772 6f75 7049 6427 5d20 3d20  urceGroupId'] = 
+0000c8d0: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
+0000c8e0: 6f75 705f 6964 0a20 2020 2020 2020 2069  oup_id.        i
+0000c8f0: 6620 7365 6c66 2e73 6563 7572 6974 795f  f self.security_
+0000c900: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
+0000c910: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000c920: 2020 7265 7375 6c74 5b27 5365 6375 7269    result['Securi
+0000c930: 7479 4772 6f75 7049 6427 5d20 3d20 7365  tyGroupId'] = se
+0000c940: 6c66 2e73 6563 7572 6974 795f 6772 6f75  lf.security_grou
+0000c950: 705f 6964 0a20 2020 2020 2020 2069 6620  p_id.        if 
+0000c960: 7365 6c66 2e76 5f73 7769 7463 685f 6964  self.v_switch_id
+0000c970: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000c980: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000c990: 5b27 5653 7769 7463 6849 6427 5d20 3d20  ['VSwitchId'] = 
+0000c9a0: 7365 6c66 2e76 5f73 7769 7463 685f 6964  self.v_switch_id
+0000c9b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000c9c0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0000c9d0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+0000c9e0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+0000c9f0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0000ca00: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0000ca10: 6966 206d 2e67 6574 2827 436c 6965 6e74  if m.get('Client
+0000ca20: 546f 6b65 6e27 2920 6973 206e 6f74 204e  Token') is not N
+0000ca30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000ca40: 2073 656c 662e 636c 6965 6e74 5f74 6f6b   self.client_tok
+0000ca50: 656e 203d 206d 2e67 6574 2827 436c 6965  en = m.get('Clie
+0000ca60: 6e74 546f 6b65 6e27 290a 2020 2020 2020  ntToken').      
+0000ca70: 2020 6966 206d 2e67 6574 2827 4561 6973    if m.get('Eais
+0000ca80: 4e61 6d65 2729 2069 7320 6e6f 7420 4e6f  Name') is not No
+0000ca90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000caa0: 7365 6c66 2e65 6169 735f 6e61 6d65 203d  self.eais_name =
+0000cab0: 206d 2e67 6574 2827 4561 6973 4e61 6d65   m.get('EaisName
+0000cac0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0000cad0: 6765 7428 2745 6169 7354 7970 6527 2920  get('EaisType') 
+0000cae0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000caf0: 2020 2020 2020 2020 2073 656c 662e 6561           self.ea
+0000cb00: 6973 5f74 7970 6520 3d20 6d2e 6765 7428  is_type = m.get(
+0000cb10: 2745 6169 7354 7970 6527 290a 2020 2020  'EaisType').    
+0000cb20: 2020 2020 6966 206d 2e67 6574 2827 456e      if m.get('En
+0000cb30: 7669 726f 6e6d 656e 7456 6172 2729 2069  vironmentVar') i
+0000cb40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000cb50: 2020 2020 2020 2020 7365 6c66 2e65 6e76          self.env
+0000cb60: 6972 6f6e 6d65 6e74 5f76 6172 5f73 6872  ironment_var_shr
+0000cb70: 696e 6b20 3d20 6d2e 6765 7428 2745 6e76  ink = m.get('Env
+0000cb80: 6972 6f6e 6d65 6e74 5661 7227 290a 2020  ironmentVar').  
+0000cb90: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0000cba0: 5265 6769 6f6e 4964 2729 2069 7320 6e6f  RegionId') is no
+0000cbb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000cbc0: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
+0000cbd0: 6964 203d 206d 2e67 6574 2827 5265 6769  id = m.get('Regi
+0000cbe0: 6f6e 4964 2729 0a20 2020 2020 2020 2069  onId').        i
+0000cbf0: 6620 6d2e 6765 7428 2752 6573 6f75 7263  f m.get('Resourc
+0000cc00: 6547 726f 7570 4964 2729 2069 7320 6e6f  eGroupId') is no
+0000cc10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000cc20: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
+0000cc30: 655f 6772 6f75 705f 6964 203d 206d 2e67  e_group_id = m.g
+0000cc40: 6574 2827 5265 736f 7572 6365 4772 6f75  et('ResourceGrou
+0000cc50: 7049 6427 290a 2020 2020 2020 2020 6966  pId').        if
+0000cc60: 206d 2e67 6574 2827 5365 6375 7269 7479   m.get('Security
+0000cc70: 4772 6f75 7049 6427 2920 6973 206e 6f74  GroupId') is not
+0000cc80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000cc90: 2020 2073 656c 662e 7365 6375 7269 7479     self.security
+0000cca0: 5f67 726f 7570 5f69 6420 3d20 6d2e 6765  _group_id = m.ge
+0000ccb0: 7428 2753 6563 7572 6974 7947 726f 7570  t('SecurityGroup
+0000ccc0: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0000ccd0: 6d2e 6765 7428 2756 5377 6974 6368 4964  m.get('VSwitchId
+0000cce0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0000ccf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cd00: 2e76 5f73 7769 7463 685f 6964 203d 206d  .v_switch_id = m
+0000cd10: 2e67 6574 2827 5653 7769 7463 6849 6427  .get('VSwitchId'
+0000cd20: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000cd30: 2073 656c 660a 0a0a 636c 6173 7320 4372   self...class Cr
+0000cd40: 6561 7465 4561 694a 7570 7974 6572 5265  eateEaiJupyterRe
+0000cd50: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
+0000cd60: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+0000cd70: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+0000cd80: 7365 6c66 2c0a 2020 2020 2020 2020 656c  self,.        el
+0000cd90: 6173 7469 635f 6163 6365 6c65 7261 7465  astic_accelerate
+0000cda0: 645f 696e 7374 616e 6365 5f69 643a 2073  d_instance_id: s
+0000cdb0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0000cdc0: 2020 2072 6571 7565 7374 5f69 643a 2073     request_id: s
+0000cdd0: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+0000cde0: 3a0a 2020 2020 2020 2020 7365 6c66 2e65  :.        self.e
+0000cdf0: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+0000ce00: 6564 5f69 6e73 7461 6e63 655f 6964 203d  ed_instance_id =
+0000ce10: 2065 6c61 7374 6963 5f61 6363 656c 6572   elastic_acceler
+0000ce20: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
+0000ce30: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0000ce40: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
+0000ce50: 7374 5f69 640a 0a20 2020 2064 6566 2076  st_id..    def v
+0000ce60: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+0000ce70: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0000ce80: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0000ce90: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0000cea0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+0000ceb0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+0000cec0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+0000ced0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000cee0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+0000cef0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+0000cf00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000cf10: 2e65 6c61 7374 6963 5f61 6363 656c 6572  .elastic_acceler
+0000cf20: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
+0000cf30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000cf40: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000cf50: 5b27 456c 6173 7469 6341 6363 656c 6572  ['ElasticAcceler
+0000cf60: 6174 6564 496e 7374 616e 6365 4964 275d  atedInstanceId']
+0000cf70: 203d 2073 656c 662e 656c 6173 7469 635f   = self.elastic_
+0000cf80: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
+0000cf90: 616e 6365 5f69 640a 2020 2020 2020 2020  ance_id.        
+0000cfa0: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+0000cfb0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0000cfc0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000cfd0: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
+0000cfe0: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
+0000cff0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+0000d000: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+0000d010: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+0000d020: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+0000d030: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+0000d040: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+0000d050: 2069 6620 6d2e 6765 7428 2745 6c61 7374   if m.get('Elast
+0000d060: 6963 4163 6365 6c65 7261 7465 6449 6e73  icAcceleratedIns
+0000d070: 7461 6e63 6549 6427 2920 6973 206e 6f74  tanceId') is not
+0000d080: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000d090: 2020 2073 656c 662e 656c 6173 7469 635f     self.elastic_
+0000d0a0: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
+0000d0b0: 616e 6365 5f69 6420 3d20 6d2e 6765 7428  ance_id = m.get(
+0000d0c0: 2745 6c61 7374 6963 4163 6365 6c65 7261  'ElasticAccelera
+0000d0d0: 7465 6449 6e73 7461 6e63 6549 6427 290a  tedInstanceId').
+0000d0e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0000d0f0: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
+0000d100: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000d110: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+0000d120: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
+0000d130: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
+0000d140: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0000d150: 0a0a 636c 6173 7320 4372 6561 7465 4561  ..class CreateEa
+0000d160: 694a 7570 7974 6572 5265 7370 6f6e 7365  iJupyterResponse
+0000d170: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+0000d180: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0000d190: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000d1a0: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+0000d1b0: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+0000d1c0: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+0000d1d0: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+0000d1e0: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+0000d1f0: 793a 2043 7265 6174 6545 6169 4a75 7079  y: CreateEaiJupy
+0000d200: 7465 7252 6573 706f 6e73 6542 6f64 7920  terResponseBody 
+0000d210: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+0000d220: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+0000d230: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
+0000d240: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+0000d250: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
+0000d260: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
+0000d270: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
+0000d280: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0000d290: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+0000d2a0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+0000d2b0: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
+0000d2c0: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
+0000d2d0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0000d2e0: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0000d2f0: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
+0000d300: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
+0000d310: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0000d320: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0000d330: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
+0000d340: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000d350: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+0000d360: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+0000d370: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+0000d380: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0000d390: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0000d3a0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+0000d3b0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0000d3c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000d3d0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0000d3e0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0000d3f0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0000d400: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+0000d410: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+0000d420: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000d430: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+0000d440: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+0000d450: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0000d460: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+0000d470: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000d480: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+0000d490: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+0000d4a0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+0000d4b0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+0000d4c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000d4d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000d4e0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+0000d4f0: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+0000d500: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0000d510: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+0000d520: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+0000d530: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+0000d540: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0000d550: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0000d560: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+0000d570: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000d580: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+0000d590: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+0000d5a0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+0000d5b0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+0000d5c0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+0000d5d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000d5e0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0000d5f0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+0000d600: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+0000d610: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+0000d620: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0000d630: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+0000d640: 6d6f 6465 6c20 3d20 4372 6561 7465 4561  model = CreateEa
+0000d650: 694a 7570 7974 6572 5265 7370 6f6e 7365  iJupyterResponse
+0000d660: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
+0000d670: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+0000d680: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+0000d690: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+0000d6a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000d6b0: 660a 0a0a 636c 6173 7320 4372 6561 7465  f...class Create
+0000d6c0: 4561 6973 4569 5265 7175 6573 7428 5465  EaisEiRequest(Te
+0000d6d0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0000d6e0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+0000d6f0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000d700: 2063 6c69 656e 745f 746f 6b65 6e3a 2073   client_token: s
+0000d710: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0000d720: 2020 2069 6e73 7461 6e63 655f 6e61 6d65     instance_name
+0000d730: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0000d740: 2020 2020 2020 696e 7374 616e 6365 5f74        instance_t
+0000d750: 7970 653a 2073 7472 203d 204e 6f6e 652c  ype: str = None,
+0000d760: 0a20 2020 2020 2020 2072 6567 696f 6e5f  .        region_
+0000d770: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0000d780: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+0000d790: 5f67 726f 7570 5f69 643a 2073 7472 203d  _group_id: str =
+0000d7a0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+0000d7b0: 6563 7572 6974 795f 6772 6f75 705f 6964  ecurity_group_id
+0000d7c0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0000d7d0: 2020 2020 2020 765f 7377 6974 6368 5f69        v_switch_i
+0000d7e0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0000d7f0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+0000d800: 6c66 2e63 6c69 656e 745f 746f 6b65 6e20  lf.client_token 
+0000d810: 3d20 636c 6965 6e74 5f74 6f6b 656e 0a20  = client_token. 
+0000d820: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
+0000d830: 616e 6365 5f6e 616d 6520 3d20 696e 7374  ance_name = inst
+0000d840: 616e 6365 5f6e 616d 650a 2020 2020 2020  ance_name.      
+0000d850: 2020 7365 6c66 2e69 6e73 7461 6e63 655f    self.instance_
+0000d860: 7479 7065 203d 2069 6e73 7461 6e63 655f  type = instance_
+0000d870: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
+0000d880: 662e 7265 6769 6f6e 5f69 6420 3d20 7265  f.region_id = re
+0000d890: 6769 6f6e 5f69 640a 2020 2020 2020 2020  gion_id.        
+0000d8a0: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
+0000d8b0: 6f75 705f 6964 203d 2072 6573 6f75 7263  oup_id = resourc
+0000d8c0: 655f 6772 6f75 705f 6964 0a20 2020 2020  e_group_id.     
+0000d8d0: 2020 2073 656c 662e 7365 6375 7269 7479     self.security
+0000d8e0: 5f67 726f 7570 5f69 6420 3d20 7365 6375  _group_id = secu
+0000d8f0: 7269 7479 5f67 726f 7570 5f69 640a 2020  rity_group_id.  
+0000d900: 2020 2020 2020 7365 6c66 2e76 5f73 7769        self.v_swi
+0000d910: 7463 685f 6964 203d 2076 5f73 7769 7463  tch_id = v_switc
+0000d920: 685f 6964 0a0a 2020 2020 6465 6620 7661  h_id..    def va
+0000d930: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+0000d940: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0000d950: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+0000d960: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+0000d970: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+0000d980: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0000d990: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0000d9a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000d9b0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0000d9c0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0000d9d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000d9e0: 636c 6965 6e74 5f74 6f6b 656e 2069 7320  client_token is 
+0000d9f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000da00: 2020 2020 2020 7265 7375 6c74 5b27 436c        result['Cl
+0000da10: 6965 6e74 546f 6b65 6e27 5d20 3d20 7365  ientToken'] = se
+0000da20: 6c66 2e63 6c69 656e 745f 746f 6b65 6e0a  lf.client_token.
+0000da30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000da40: 696e 7374 616e 6365 5f6e 616d 6520 6973  instance_name is
+0000da50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000da60: 2020 2020 2020 2072 6573 756c 745b 2749         result['I
+0000da70: 6e73 7461 6e63 654e 616d 6527 5d20 3d20  nstanceName'] = 
+0000da80: 7365 6c66 2e69 6e73 7461 6e63 655f 6e61  self.instance_na
+0000da90: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
+0000daa0: 6c66 2e69 6e73 7461 6e63 655f 7479 7065  lf.instance_type
+0000dab0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000dac0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000dad0: 5b27 496e 7374 616e 6365 5479 7065 275d  ['InstanceType']
+0000dae0: 203d 2073 656c 662e 696e 7374 616e 6365   = self.instance
+0000daf0: 5f74 7970 650a 2020 2020 2020 2020 6966  _type.        if
+0000db00: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+0000db10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000db20: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0000db30: 2752 6567 696f 6e49 6427 5d20 3d20 7365  'RegionId'] = se
+0000db40: 6c66 2e72 6567 696f 6e5f 6964 0a20 2020  lf.region_id.   
+0000db50: 2020 2020 2069 6620 7365 6c66 2e72 6573       if self.res
+0000db60: 6f75 7263 655f 6772 6f75 705f 6964 2069  ource_group_id i
+0000db70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000db80: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0000db90: 5265 736f 7572 6365 4772 6f75 7049 6427  ResourceGroupId'
+0000dba0: 5d20 3d20 7365 6c66 2e72 6573 6f75 7263  ] = self.resourc
+0000dbb0: 655f 6772 6f75 705f 6964 0a20 2020 2020  e_group_id.     
+0000dbc0: 2020 2069 6620 7365 6c66 2e73 6563 7572     if self.secur
+0000dbd0: 6974 795f 6772 6f75 705f 6964 2069 7320  ity_group_id is 
+0000dbe0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000dbf0: 2020 2020 2020 7265 7375 6c74 5b27 5365        result['Se
+0000dc00: 6375 7269 7479 4772 6f75 7049 6427 5d20  curityGroupId'] 
+0000dc10: 3d20 7365 6c66 2e73 6563 7572 6974 795f  = self.security_
+0000dc20: 6772 6f75 705f 6964 0a20 2020 2020 2020  group_id.       
+0000dc30: 2069 6620 7365 6c66 2e76 5f73 7769 7463   if self.v_switc
+0000dc40: 685f 6964 2069 7320 6e6f 7420 4e6f 6e65  h_id is not None
+0000dc50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000dc60: 7375 6c74 5b27 5653 7769 7463 6849 6427  sult['VSwitchId'
+0000dc70: 5d20 3d20 7365 6c66 2e76 5f73 7769 7463  ] = self.v_switc
+0000dc80: 685f 6964 0a20 2020 2020 2020 2072 6574  h_id.        ret
+0000dc90: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0000dca0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0000dcb0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+0000dcc0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+0000dcd0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+0000dce0: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
+0000dcf0: 6965 6e74 546f 6b65 6e27 2920 6973 206e  ientToken') is n
+0000dd00: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000dd10: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
+0000dd20: 5f74 6f6b 656e 203d 206d 2e67 6574 2827  _token = m.get('
+0000dd30: 436c 6965 6e74 546f 6b65 6e27 290a 2020  ClientToken').  
+0000dd40: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0000dd50: 496e 7374 616e 6365 4e61 6d65 2729 2069  InstanceName') i
+0000dd60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000dd70: 2020 2020 2020 2020 7365 6c66 2e69 6e73          self.ins
+0000dd80: 7461 6e63 655f 6e61 6d65 203d 206d 2e67  tance_name = m.g
+0000dd90: 6574 2827 496e 7374 616e 6365 4e61 6d65  et('InstanceName
+0000dda0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0000ddb0: 6765 7428 2749 6e73 7461 6e63 6554 7970  get('InstanceTyp
+0000ddc0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+0000ddd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000dde0: 662e 696e 7374 616e 6365 5f74 7970 6520  f.instance_type 
+0000ddf0: 3d20 6d2e 6765 7428 2749 6e73 7461 6e63  = m.get('Instanc
+0000de00: 6554 7970 6527 290a 2020 2020 2020 2020  eType').        
+0000de10: 6966 206d 2e67 6574 2827 5265 6769 6f6e  if m.get('Region
+0000de20: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+0000de30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000de40: 6c66 2e72 6567 696f 6e5f 6964 203d 206d  lf.region_id = m
+0000de50: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
+0000de60: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0000de70: 7428 2752 6573 6f75 7263 6547 726f 7570  t('ResourceGroup
+0000de80: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+0000de90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000dea0: 6c66 2e72 6573 6f75 7263 655f 6772 6f75  lf.resource_grou
+0000deb0: 705f 6964 203d 206d 2e67 6574 2827 5265  p_id = m.get('Re
+0000dec0: 736f 7572 6365 4772 6f75 7049 6427 290a  sourceGroupId').
+0000ded0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0000dee0: 2827 5365 6375 7269 7479 4772 6f75 7049  ('SecurityGroupI
+0000def0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0000df00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000df10: 662e 7365 6375 7269 7479 5f67 726f 7570  f.security_group
+0000df20: 5f69 6420 3d20 6d2e 6765 7428 2753 6563  _id = m.get('Sec
+0000df30: 7572 6974 7947 726f 7570 4964 2729 0a20  urityGroupId'). 
+0000df40: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0000df50: 2756 5377 6974 6368 4964 2729 2069 7320  'VSwitchId') is 
+0000df60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000df70: 2020 2020 2020 7365 6c66 2e76 5f73 7769        self.v_swi
+0000df80: 7463 685f 6964 203d 206d 2e67 6574 2827  tch_id = m.get('
+0000df90: 5653 7769 7463 6849 6427 290a 2020 2020  VSwitchId').    
+0000dfa0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0000dfb0: 0a0a 636c 6173 7320 4372 6561 7465 4561  ..class CreateEa
+0000dfc0: 6973 4569 5265 7370 6f6e 7365 426f 6479  isEiResponseBody
+0000dfd0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+0000dfe0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0000dff0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000e000: 2020 2020 6569 5f69 6e73 7461 6e63 655f      ei_instance_
+0000e010: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0000e020: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+0000e030: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0000e040: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+0000e050: 656c 662e 6569 5f69 6e73 7461 6e63 655f  elf.ei_instance_
+0000e060: 6964 203d 2065 695f 696e 7374 616e 6365  id = ei_instance
+0000e070: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+0000e080: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
+0000e090: 7175 6573 745f 6964 0a0a 2020 2020 6465  quest_id..    de
+0000e0a0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+0000e0b0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0000e0c0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+0000e0d0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+0000e0e0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+0000e0f0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+0000e100: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+0000e110: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000e120: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+0000e130: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+0000e140: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+0000e150: 656c 662e 6569 5f69 6e73 7461 6e63 655f  elf.ei_instance_
+0000e160: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0000e170: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000e180: 6c74 5b27 4569 496e 7374 616e 6365 4964  lt['EiInstanceId
+0000e190: 275d 203d 2073 656c 662e 6569 5f69 6e73  '] = self.ei_ins
+0000e1a0: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+0000e1b0: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
+0000e1c0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+0000e1d0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000e1e0: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
+0000e1f0: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+0000e200: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+0000e210: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0000e220: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0000e230: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+0000e240: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0000e250: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0000e260: 2020 6966 206d 2e67 6574 2827 4569 496e    if m.get('EiIn
+0000e270: 7374 616e 6365 4964 2729 2069 7320 6e6f  stanceId') is no
+0000e280: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000e290: 2020 2020 7365 6c66 2e65 695f 696e 7374      self.ei_inst
+0000e2a0: 616e 6365 5f69 6420 3d20 6d2e 6765 7428  ance_id = m.get(
+0000e2b0: 2745 6949 6e73 7461 6e63 6549 6427 290a  'EiInstanceId').
+0000e2c0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0000e2d0: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
+0000e2e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000e2f0: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+0000e300: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
+0000e310: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
+0000e320: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0000e330: 0a0a 636c 6173 7320 4372 6561 7465 4561  ..class CreateEa
+0000e340: 6973 4569 5265 7370 6f6e 7365 2854 6561  isEiResponse(Tea
+0000e350: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0000e360: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+0000e370: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000e380: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
+0000e390: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+0000e3a0: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+0000e3b0: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
+0000e3c0: 0a20 2020 2020 2020 2062 6f64 793a 2043  .        body: C
+0000e3d0: 7265 6174 6545 6169 7345 6952 6573 706f  reateEaisEiRespo
+0000e3e0: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
+0000e3f0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+0000e400: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
+0000e410: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
+0000e420: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+0000e430: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
+0000e440: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+0000e450: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
+0000e460: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+0000e470: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0000e480: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0000e490: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
+0000e4a0: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
+0000e4b0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+0000e4c0: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
+0000e4d0: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
+0000e4e0: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
+0000e4f0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+0000e500: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
+0000e510: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
+0000e520: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
+0000e530: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e540: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
+0000e550: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+0000e560: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+0000e570: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+0000e580: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0000e590: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0000e5a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000e5b0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0000e5c0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0000e5d0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0000e5e0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+0000e5f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000e600: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+0000e610: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+0000e620: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+0000e630: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+0000e640: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+0000e650: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000e660: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+0000e670: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+0000e680: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+0000e690: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+0000e6a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000e6b0: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+0000e6c0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+0000e6d0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+0000e6e0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+0000e6f0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+0000e700: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+0000e710: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+0000e720: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+0000e730: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+0000e740: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+0000e750: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000e760: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+0000e770: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+0000e780: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0000e790: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+0000e7a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000e7b0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000e7c0: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+0000e7d0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+0000e7e0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0000e7f0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+0000e800: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000e810: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+0000e820: 4372 6561 7465 4561 6973 4569 5265 7370  CreateEaisEiResp
+0000e830: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+0000e840: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0000e850: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+0000e860: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+0000e870: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0000e880: 2073 656c 660a 0a0a 636c 6173 7320 4465   self...class De
+0000e890: 6c65 7465 4561 6952 6571 7565 7374 2854  leteEaiRequest(T
+0000e8a0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0000e8b0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0000e8c0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000e8d0: 2020 656c 6173 7469 635f 6163 6365 6c65    elastic_accele
+0000e8e0: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
+0000e8f0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0000e900: 2020 2020 2020 2066 6f72 6365 3a20 626f         force: bo
+0000e910: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
+0000e920: 2020 2072 6567 696f 6e5f 6964 3a20 7374     region_id: st
+0000e930: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
+0000e940: 0a20 2020 2020 2020 2073 656c 662e 656c  .        self.el
+0000e950: 6173 7469 635f 6163 6365 6c65 7261 7465  astic_accelerate
+0000e960: 645f 696e 7374 616e 6365 5f69 6420 3d20  d_instance_id = 
+0000e970: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
+0000e980: 7465 645f 696e 7374 616e 6365 5f69 640a  ted_instance_id.
+0000e990: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
+0000e9a0: 6365 203d 2066 6f72 6365 0a20 2020 2020  ce = force.     
+0000e9b0: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
+0000e9c0: 6420 3d20 7265 6769 6f6e 5f69 640a 0a20  d = region_id.. 
+0000e9d0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0000e9e0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+0000e9f0: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+0000ea00: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+0000ea10: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+0000ea20: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+0000ea30: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+0000ea40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000ea50: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+0000ea60: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0000ea70: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+0000ea80: 2069 6620 7365 6c66 2e65 6c61 7374 6963   if self.elastic
+0000ea90: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+0000eaa0: 7461 6e63 655f 6964 2069 7320 6e6f 7420  tance_id is not 
+0000eab0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000eac0: 2020 7265 7375 6c74 5b27 456c 6173 7469    result['Elasti
+0000ead0: 6341 6363 656c 6572 6174 6564 496e 7374  cAcceleratedInst
+0000eae0: 616e 6365 4964 275d 203d 2073 656c 662e  anceId'] = self.
+0000eaf0: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
+0000eb00: 7465 645f 696e 7374 616e 6365 5f69 640a  ted_instance_id.
+0000eb10: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000eb20: 666f 7263 6520 6973 206e 6f74 204e 6f6e  force is not Non
+0000eb30: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000eb40: 6573 756c 745b 2746 6f72 6365 275d 203d  esult['Force'] =
+0000eb50: 2073 656c 662e 666f 7263 650a 2020 2020   self.force.    
+0000eb60: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
+0000eb70: 6f6e 5f69 6420 6973 206e 6f74 204e 6f6e  on_id is not Non
+0000eb80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000eb90: 6573 756c 745b 2752 6567 696f 6e49 6427  esult['RegionId'
+0000eba0: 5d20 3d20 7365 6c66 2e72 6567 696f 6e5f  ] = self.region_
+0000ebb0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
+0000ebc0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0000ebd0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0000ebe0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+0000ebf0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0000ec00: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0000ec10: 2020 6966 206d 2e67 6574 2827 456c 6173    if m.get('Elas
+0000ec20: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
+0000ec30: 7374 616e 6365 4964 2729 2069 7320 6e6f  stanceId') is no
+0000ec40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000ec50: 2020 2020 7365 6c66 2e65 6c61 7374 6963      self.elastic
+0000ec60: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+0000ec70: 7461 6e63 655f 6964 203d 206d 2e67 6574  tance_id = m.get
+0000ec80: 2827 456c 6173 7469 6341 6363 656c 6572  ('ElasticAcceler
+0000ec90: 6174 6564 496e 7374 616e 6365 4964 2729  atedInstanceId')
+0000eca0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0000ecb0: 7428 2746 6f72 6365 2729 2069 7320 6e6f  t('Force') is no
 0000ecc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000ecd0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0000ece0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0000ecf0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0000ed00: 2072 6573 756c 745b 2754 6167 275d 203d   result['Tag'] =
-0000ed10: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
-0000ed20: 656c 662e 7461 6720 6973 206e 6f74 204e  elf.tag is not N
-0000ed30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000ed40: 2066 6f72 206b 2069 6e20 7365 6c66 2e74   for k in self.t
-0000ed50: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
-0000ed60: 2020 2020 7265 7375 6c74 5b27 5461 6727      result['Tag'
-0000ed70: 5d2e 6170 7065 6e64 286b 2e74 6f5f 6d61  ].append(k.to_ma
-0000ed80: 7028 2920 6966 206b 2065 6c73 6520 4e6f  p() if k else No
-0000ed90: 6e65 290a 2020 2020 2020 2020 7265 7475  ne).        retu
-0000eda0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0000edb0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0000edc0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-0000edd0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0000ede0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0000edf0: 2020 2073 656c 662e 7461 6720 3d20 5b5d     self.tag = []
-0000ee00: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0000ee10: 7428 2754 6167 2729 2069 7320 6e6f 7420  t('Tag') is not 
-0000ee20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000ee30: 2020 666f 7220 6b20 696e 206d 2e67 6574    for k in m.get
-0000ee40: 2827 5461 6727 293a 0a20 2020 2020 2020  ('Tag'):.       
-0000ee50: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-0000ee60: 6465 6c20 3d20 4465 7363 7269 6265 4561  del = DescribeEa
-0000ee70: 6973 5265 7370 6f6e 7365 426f 6479 496e  isResponseBodyIn
-0000ee80: 7374 616e 6365 7349 6e73 7461 6e63 6554  stancesInstanceT
-0000ee90: 6167 7354 6167 2829 0a20 2020 2020 2020  agsTag().       
-0000eea0: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
-0000eeb0: 672e 6170 7065 6e64 2874 656d 705f 6d6f  g.append(temp_mo
-0000eec0: 6465 6c2e 6672 6f6d 5f6d 6170 286b 2929  del.from_map(k))
-0000eed0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000eee0: 7365 6c66 0a0a 0a63 6c61 7373 2044 6573  self...class Des
-0000eef0: 6372 6962 6545 6169 7352 6573 706f 6e73  cribeEaisRespons
-0000ef00: 6542 6f64 7949 6e73 7461 6e63 6573 496e  eBodyInstancesIn
-0000ef10: 7374 616e 6365 2854 6561 4d6f 6465 6c29  stance(TeaModel)
-0000ef20: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0000ef30: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0000ef40: 2c0a 2020 2020 2020 2020 6361 7465 676f  ,.        catego
-0000ef50: 7279 3a20 7374 7220 3d20 4e6f 6e65 2c0a  ry: str = None,.
-0000ef60: 2020 2020 2020 2020 636c 6965 6e74 5f69          client_i
-0000ef70: 6e73 7461 6e63 655f 6964 3a20 7374 7220  nstance_id: str 
-0000ef80: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000ef90: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
-0000efa0: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
-0000efb0: 2c0a 2020 2020 2020 2020 636c 6965 6e74  ,.        client
-0000efc0: 5f69 6e73 7461 6e63 655f 7479 7065 3a20  _instance_type: 
-0000efd0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0000efe0: 2020 2020 6372 6561 7469 6f6e 5f74 696d      creation_tim
-0000eff0: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-0000f000: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-0000f010: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
-0000f020: 2020 2020 2020 2020 656c 6173 7469 635f          elastic_
-0000f030: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
-0000f040: 616e 6365 5f69 643a 2073 7472 203d 204e  ance_id: str = N
-0000f050: 6f6e 652c 0a20 2020 2020 2020 2069 6e73  one,.        ins
-0000f060: 7461 6e63 655f 6e61 6d65 3a20 7374 7220  tance_name: str 
-0000f070: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000f080: 696e 7374 616e 6365 5f74 7970 653a 2073  instance_type: s
-0000f090: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0000f0a0: 2020 206a 7570 7974 6572 5f75 726c 3a20     jupyter_url: 
-0000f0b0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0000f0c0: 2020 2020 7265 6769 6f6e 5f69 643a 2073      region_id: s
-0000f0d0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0000f0e0: 2020 2072 6573 6f75 7263 655f 6772 6f75     resource_grou
-0000f0f0: 705f 6964 3a20 7374 7220 3d20 4e6f 6e65  p_id: str = None
-0000f100: 2c0a 2020 2020 2020 2020 7365 6375 7269  ,.        securi
-0000f110: 7479 5f67 726f 7570 5f69 643a 2073 7472  ty_group_id: str
-0000f120: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000f130: 2073 7461 7274 5f74 696d 653a 2073 7472   start_time: str
-0000f140: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000f150: 2073 7461 7475 733a 2073 7472 203d 204e   status: str = N
-0000f160: 6f6e 652c 0a20 2020 2020 2020 2074 6167  one,.        tag
-0000f170: 733a 2044 6573 6372 6962 6545 6169 7352  s: DescribeEaisR
-0000f180: 6573 706f 6e73 6542 6f64 7949 6e73 7461  esponseBodyInsta
-0000f190: 6e63 6573 496e 7374 616e 6365 5461 6773  ncesInstanceTags
-0000f1a0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000f1b0: 2076 5f73 7769 7463 685f 6964 3a20 7374   v_switch_id: st
-0000f1c0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0000f1d0: 2020 7a6f 6e65 5f69 643a 2073 7472 203d    zone_id: str =
-0000f1e0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-0000f1f0: 2020 2020 2020 7365 6c66 2e63 6174 6567        self.categ
-0000f200: 6f72 7920 3d20 6361 7465 676f 7279 0a20  ory = category. 
-0000f210: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
-0000f220: 6e74 5f69 6e73 7461 6e63 655f 6964 203d  nt_instance_id =
-0000f230: 2063 6c69 656e 745f 696e 7374 616e 6365   client_instance
-0000f240: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
-0000f250: 2e63 6c69 656e 745f 696e 7374 616e 6365  .client_instance
-0000f260: 5f6e 616d 6520 3d20 636c 6965 6e74 5f69  _name = client_i
-0000f270: 6e73 7461 6e63 655f 6e61 6d65 0a20 2020  nstance_name.   
-0000f280: 2020 2020 2073 656c 662e 636c 6965 6e74       self.client
-0000f290: 5f69 6e73 7461 6e63 655f 7479 7065 203d  _instance_type =
-0000f2a0: 2063 6c69 656e 745f 696e 7374 616e 6365   client_instance
-0000f2b0: 5f74 7970 650a 2020 2020 2020 2020 7365  _type.        se
-0000f2c0: 6c66 2e63 7265 6174 696f 6e5f 7469 6d65  lf.creation_time
-0000f2d0: 203d 2063 7265 6174 696f 6e5f 7469 6d65   = creation_time
-0000f2e0: 0a20 2020 2020 2020 2073 656c 662e 6465  .        self.de
-0000f2f0: 7363 7269 7074 696f 6e20 3d20 6465 7363  scription = desc
-0000f300: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
-0000f310: 7365 6c66 2e65 6c61 7374 6963 5f61 6363  self.elastic_acc
-0000f320: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
-0000f330: 655f 6964 203d 2065 6c61 7374 6963 5f61  e_id = elastic_a
-0000f340: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
-0000f350: 6e63 655f 6964 0a20 2020 2020 2020 2073  nce_id.        s
-0000f360: 656c 662e 696e 7374 616e 6365 5f6e 616d  elf.instance_nam
-0000f370: 6520 3d20 696e 7374 616e 6365 5f6e 616d  e = instance_nam
-0000f380: 650a 2020 2020 2020 2020 7365 6c66 2e69  e.        self.i
-0000f390: 6e73 7461 6e63 655f 7479 7065 203d 2069  nstance_type = i
-0000f3a0: 6e73 7461 6e63 655f 7479 7065 0a20 2020  nstance_type.   
-0000f3b0: 2020 2020 2073 656c 662e 6a75 7079 7465       self.jupyte
-0000f3c0: 725f 7572 6c20 3d20 6a75 7079 7465 725f  r_url = jupyter_
-0000f3d0: 7572 6c0a 2020 2020 2020 2020 7365 6c66  url.        self
-0000f3e0: 2e72 6567 696f 6e5f 6964 203d 2072 6567  .region_id = reg
-0000f3f0: 696f 6e5f 6964 0a20 2020 2020 2020 2073  ion_id.        s
-0000f400: 656c 662e 7265 736f 7572 6365 5f67 726f  elf.resource_gro
-0000f410: 7570 5f69 6420 3d20 7265 736f 7572 6365  up_id = resource
-0000f420: 5f67 726f 7570 5f69 640a 2020 2020 2020  _group_id.      
-0000f430: 2020 7365 6c66 2e73 6563 7572 6974 795f    self.security_
-0000f440: 6772 6f75 705f 6964 203d 2073 6563 7572  group_id = secur
-0000f450: 6974 795f 6772 6f75 705f 6964 0a20 2020  ity_group_id.   
-0000f460: 2020 2020 2073 656c 662e 7374 6172 745f       self.start_
-0000f470: 7469 6d65 203d 2073 7461 7274 5f74 696d  time = start_tim
-0000f480: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
-0000f490: 7461 7475 7320 3d20 7374 6174 7573 0a20  tatus = status. 
-0000f4a0: 2020 2020 2020 2073 656c 662e 7461 6773         self.tags
-0000f4b0: 203d 2074 6167 730a 2020 2020 2020 2020   = tags.        
-0000f4c0: 7365 6c66 2e76 5f73 7769 7463 685f 6964  self.v_switch_id
-0000f4d0: 203d 2076 5f73 7769 7463 685f 6964 0a20   = v_switch_id. 
-0000f4e0: 2020 2020 2020 2073 656c 662e 7a6f 6e65         self.zone
-0000f4f0: 5f69 6420 3d20 7a6f 6e65 5f69 640a 0a20  _id = zone_id.. 
-0000f500: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0000f510: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-0000f520: 6620 7365 6c66 2e74 6167 733a 0a20 2020  f self.tags:.   
-0000f530: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
-0000f540: 6773 2e76 616c 6964 6174 6528 290a 0a20  gs.validate().. 
-0000f550: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0000f560: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0000f570: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-0000f580: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0000f590: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0000f5a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000f5b0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0000f5c0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0000f5d0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0000f5e0: 6c66 2e63 6174 6567 6f72 7920 6973 206e  lf.category is n
-0000f5f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000f600: 2020 2020 2072 6573 756c 745b 2743 6174       result['Cat
-0000f610: 6567 6f72 7927 5d20 3d20 7365 6c66 2e63  egory'] = self.c
-0000f620: 6174 6567 6f72 790a 2020 2020 2020 2020  ategory.        
-0000f630: 6966 2073 656c 662e 636c 6965 6e74 5f69  if self.client_i
-0000f640: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
-0000f650: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000f660: 2020 2020 7265 7375 6c74 5b27 436c 6965      result['Clie
-0000f670: 6e74 496e 7374 616e 6365 4964 275d 203d  ntInstanceId'] =
-0000f680: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
-0000f690: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
-0000f6a0: 2069 6620 7365 6c66 2e63 6c69 656e 745f   if self.client_
-0000f6b0: 696e 7374 616e 6365 5f6e 616d 6520 6973  instance_name is
-0000f6c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000f6d0: 2020 2020 2020 2072 6573 756c 745b 2743         result['C
-0000f6e0: 6c69 656e 7449 6e73 7461 6e63 654e 616d  lientInstanceNam
-0000f6f0: 6527 5d20 3d20 7365 6c66 2e63 6c69 656e  e'] = self.clien
-0000f700: 745f 696e 7374 616e 6365 5f6e 616d 650a  t_instance_name.
-0000f710: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f720: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
-0000f730: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-0000f740: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000f750: 7375 6c74 5b27 436c 6965 6e74 496e 7374  sult['ClientInst
-0000f760: 616e 6365 5479 7065 275d 203d 2073 656c  anceType'] = sel
-0000f770: 662e 636c 6965 6e74 5f69 6e73 7461 6e63  f.client_instanc
-0000f780: 655f 7479 7065 0a20 2020 2020 2020 2069  e_type.        i
-0000f790: 6620 7365 6c66 2e63 7265 6174 696f 6e5f  f self.creation_
-0000f7a0: 7469 6d65 2069 7320 6e6f 7420 4e6f 6e65  time is not None
-0000f7b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000f7c0: 7375 6c74 5b27 4372 6561 7469 6f6e 5469  sult['CreationTi
-0000f7d0: 6d65 275d 203d 2073 656c 662e 6372 6561  me'] = self.crea
-0000f7e0: 7469 6f6e 5f74 696d 650a 2020 2020 2020  tion_time.      
-0000f7f0: 2020 6966 2073 656c 662e 6465 7363 7269    if self.descri
-0000f800: 7074 696f 6e20 6973 206e 6f74 204e 6f6e  ption is not Non
-0000f810: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000f820: 6573 756c 745b 2744 6573 6372 6970 7469  esult['Descripti
-0000f830: 6f6e 275d 203d 2073 656c 662e 6465 7363  on'] = self.desc
-0000f840: 7269 7074 696f 6e0a 2020 2020 2020 2020  ription.        
-0000f850: 6966 2073 656c 662e 656c 6173 7469 635f  if self.elastic_
-0000f860: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
-0000f870: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
-0000f880: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000f890: 2072 6573 756c 745b 2745 6c61 7374 6963   result['Elastic
-0000f8a0: 4163 6365 6c65 7261 7465 6449 6e73 7461  AcceleratedInsta
-0000f8b0: 6e63 6549 6427 5d20 3d20 7365 6c66 2e65  nceId'] = self.e
-0000f8c0: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
-0000f8d0: 6564 5f69 6e73 7461 6e63 655f 6964 0a20  ed_instance_id. 
-0000f8e0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-0000f8f0: 6e73 7461 6e63 655f 6e61 6d65 2069 7320  nstance_name is 
-0000f900: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000f910: 2020 2020 2020 7265 7375 6c74 5b27 496e        result['In
-0000f920: 7374 616e 6365 4e61 6d65 275d 203d 2073  stanceName'] = s
-0000f930: 656c 662e 696e 7374 616e 6365 5f6e 616d  elf.instance_nam
-0000f940: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0000f950: 662e 696e 7374 616e 6365 5f74 7970 6520  f.instance_type 
-0000f960: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000f970: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000f980: 2749 6e73 7461 6e63 6554 7970 6527 5d20  'InstanceType'] 
-0000f990: 3d20 7365 6c66 2e69 6e73 7461 6e63 655f  = self.instance_
-0000f9a0: 7479 7065 0a20 2020 2020 2020 2069 6620  type.        if 
-0000f9b0: 7365 6c66 2e6a 7570 7974 6572 5f75 726c  self.jupyter_url
-0000f9c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000f9d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000f9e0: 5b27 4a75 7079 7465 7255 726c 275d 203d  ['JupyterUrl'] =
-0000f9f0: 2073 656c 662e 6a75 7079 7465 725f 7572   self.jupyter_ur
-0000fa00: 6c0a 2020 2020 2020 2020 6966 2073 656c  l.        if sel
-0000fa10: 662e 7265 6769 6f6e 5f69 6420 6973 206e  f.region_id is n
-0000fa20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000fa30: 2020 2020 2072 6573 756c 745b 2752 6567       result['Reg
-0000fa40: 696f 6e49 6427 5d20 3d20 7365 6c66 2e72  ionId'] = self.r
-0000fa50: 6567 696f 6e5f 6964 0a20 2020 2020 2020  egion_id.       
-0000fa60: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
-0000fa70: 655f 6772 6f75 705f 6964 2069 7320 6e6f  e_group_id is no
-0000fa80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000fa90: 2020 2020 7265 7375 6c74 5b27 5265 736f      result['Reso
-0000faa0: 7572 6365 4772 6f75 7049 6427 5d20 3d20  urceGroupId'] = 
-0000fab0: 7365 6c66 2e72 6573 6f75 7263 655f 6772  self.resource_gr
-0000fac0: 6f75 705f 6964 0a20 2020 2020 2020 2069  oup_id.        i
-0000fad0: 6620 7365 6c66 2e73 6563 7572 6974 795f  f self.security_
-0000fae0: 6772 6f75 705f 6964 2069 7320 6e6f 7420  group_id is not 
-0000faf0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000fb00: 2020 7265 7375 6c74 5b27 5365 6375 7269    result['Securi
-0000fb10: 7479 4772 6f75 7049 6427 5d20 3d20 7365  tyGroupId'] = se
-0000fb20: 6c66 2e73 6563 7572 6974 795f 6772 6f75  lf.security_grou
-0000fb30: 705f 6964 0a20 2020 2020 2020 2069 6620  p_id.        if 
-0000fb40: 7365 6c66 2e73 7461 7274 5f74 696d 6520  self.start_time 
-0000fb50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000fb60: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0000fb70: 2753 7461 7274 5469 6d65 275d 203d 2073  'StartTime'] = s
-0000fb80: 656c 662e 7374 6172 745f 7469 6d65 0a20  elf.start_time. 
-0000fb90: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0000fba0: 7461 7475 7320 6973 206e 6f74 204e 6f6e  tatus is not Non
-0000fbb0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0000fbc0: 6573 756c 745b 2753 7461 7475 7327 5d20  esult['Status'] 
-0000fbd0: 3d20 7365 6c66 2e73 7461 7475 730a 2020  = self.status.  
-0000fbe0: 2020 2020 2020 6966 2073 656c 662e 7461        if self.ta
-0000fbf0: 6773 2069 7320 6e6f 7420 4e6f 6e65 3a0a  gs is not None:.
-0000fc00: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000fc10: 6c74 5b27 5461 6773 275d 203d 2073 656c  lt['Tags'] = sel
-0000fc20: 662e 7461 6773 2e74 6f5f 6d61 7028 290a  f.tags.to_map().
-0000fc30: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000fc40: 765f 7377 6974 6368 5f69 6420 6973 206e  v_switch_id is n
-0000fc50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000fc60: 2020 2020 2072 6573 756c 745b 2756 5377       result['VSw
-0000fc70: 6974 6368 4964 275d 203d 2073 656c 662e  itchId'] = self.
-0000fc80: 765f 7377 6974 6368 5f69 640a 2020 2020  v_switch_id.    
-0000fc90: 2020 2020 6966 2073 656c 662e 7a6f 6e65      if self.zone
-0000fca0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-0000fcb0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0000fcc0: 756c 745b 275a 6f6e 6549 6427 5d20 3d20  ult['ZoneId'] = 
-0000fcd0: 7365 6c66 2e7a 6f6e 655f 6964 0a20 2020  self.zone_id.   
-0000fce0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0000fcf0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0000fd00: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-0000fd10: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-0000fd20: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0000fd30: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0000fd40: 2e67 6574 2827 4361 7465 676f 7279 2729  .get('Category')
-0000fd50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000fd60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000fd70: 6174 6567 6f72 7920 3d20 6d2e 6765 7428  ategory = m.get(
-0000fd80: 2743 6174 6567 6f72 7927 290a 2020 2020  'Category').    
-0000fd90: 2020 2020 6966 206d 2e67 6574 2827 436c      if m.get('Cl
-0000fda0: 6965 6e74 496e 7374 616e 6365 4964 2729  ientInstanceId')
-0000fdb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000fdc0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000fdd0: 6c69 656e 745f 696e 7374 616e 6365 5f69  lient_instance_i
-0000fde0: 6420 3d20 6d2e 6765 7428 2743 6c69 656e  d = m.get('Clien
-0000fdf0: 7449 6e73 7461 6e63 6549 6427 290a 2020  tInstanceId').  
-0000fe00: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0000fe10: 436c 6965 6e74 496e 7374 616e 6365 4e61  ClientInstanceNa
-0000fe20: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
-0000fe30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000fe40: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
-0000fe50: 6365 5f6e 616d 6520 3d20 6d2e 6765 7428  ce_name = m.get(
-0000fe60: 2743 6c69 656e 7449 6e73 7461 6e63 654e  'ClientInstanceN
-0000fe70: 616d 6527 290a 2020 2020 2020 2020 6966  ame').        if
-0000fe80: 206d 2e67 6574 2827 436c 6965 6e74 496e   m.get('ClientIn
-0000fe90: 7374 616e 6365 5479 7065 2729 2069 7320  stanceType') is 
-0000fea0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000feb0: 2020 2020 2020 7365 6c66 2e63 6c69 656e        self.clien
-0000fec0: 745f 696e 7374 616e 6365 5f74 7970 6520  t_instance_type 
-0000fed0: 3d20 6d2e 6765 7428 2743 6c69 656e 7449  = m.get('ClientI
-0000fee0: 6e73 7461 6e63 6554 7970 6527 290a 2020  nstanceType').  
-0000fef0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0000ff00: 4372 6561 7469 6f6e 5469 6d65 2729 2069  CreationTime') i
-0000ff10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000ff20: 2020 2020 2020 2020 7365 6c66 2e63 7265          self.cre
-0000ff30: 6174 696f 6e5f 7469 6d65 203d 206d 2e67  ation_time = m.g
-0000ff40: 6574 2827 4372 6561 7469 6f6e 5469 6d65  et('CreationTime
-0000ff50: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0000ff60: 6765 7428 2744 6573 6372 6970 7469 6f6e  get('Description
-0000ff70: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0000ff80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ff90: 2e64 6573 6372 6970 7469 6f6e 203d 206d  .description = m
-0000ffa0: 2e67 6574 2827 4465 7363 7269 7074 696f  .get('Descriptio
-0000ffb0: 6e27 290a 2020 2020 2020 2020 6966 206d  n').        if m
-0000ffc0: 2e67 6574 2827 456c 6173 7469 6341 6363  .get('ElasticAcc
-0000ffd0: 656c 6572 6174 6564 496e 7374 616e 6365  eleratedInstance
-0000ffe0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-0000fff0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00010000: 6c66 2e65 6c61 7374 6963 5f61 6363 656c  lf.elastic_accel
-00010010: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
-00010020: 6964 203d 206d 2e67 6574 2827 456c 6173  id = m.get('Elas
-00010030: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
-00010040: 7374 616e 6365 4964 2729 0a20 2020 2020  stanceId').     
-00010050: 2020 2069 6620 6d2e 6765 7428 2749 6e73     if m.get('Ins
-00010060: 7461 6e63 654e 616d 6527 2920 6973 206e  tanceName') is n
-00010070: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00010080: 2020 2020 2073 656c 662e 696e 7374 616e       self.instan
-00010090: 6365 5f6e 616d 6520 3d20 6d2e 6765 7428  ce_name = m.get(
-000100a0: 2749 6e73 7461 6e63 654e 616d 6527 290a  'InstanceName').
-000100b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000100c0: 2827 496e 7374 616e 6365 5479 7065 2729  ('InstanceType')
-000100d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000100e0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-000100f0: 6e73 7461 6e63 655f 7479 7065 203d 206d  nstance_type = m
-00010100: 2e67 6574 2827 496e 7374 616e 6365 5479  .get('InstanceTy
-00010110: 7065 2729 0a20 2020 2020 2020 2069 6620  pe').        if 
-00010120: 6d2e 6765 7428 274a 7570 7974 6572 5572  m.get('JupyterUr
-00010130: 6c27 2920 6973 206e 6f74 204e 6f6e 653a  l') is not None:
-00010140: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010150: 662e 6a75 7079 7465 725f 7572 6c20 3d20  f.jupyter_url = 
-00010160: 6d2e 6765 7428 274a 7570 7974 6572 5572  m.get('JupyterUr
-00010170: 6c27 290a 2020 2020 2020 2020 6966 206d  l').        if m
-00010180: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
-00010190: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000101a0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000101b0: 6567 696f 6e5f 6964 203d 206d 2e67 6574  egion_id = m.get
-000101c0: 2827 5265 6769 6f6e 4964 2729 0a20 2020  ('RegionId').   
-000101d0: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-000101e0: 6573 6f75 7263 6547 726f 7570 4964 2729  esourceGroupId')
-000101f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00010200: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00010210: 6573 6f75 7263 655f 6772 6f75 705f 6964  esource_group_id
-00010220: 203d 206d 2e67 6574 2827 5265 736f 7572   = m.get('Resour
-00010230: 6365 4772 6f75 7049 6427 290a 2020 2020  ceGroupId').    
-00010240: 2020 2020 6966 206d 2e67 6574 2827 5365      if m.get('Se
-00010250: 6375 7269 7479 4772 6f75 7049 6427 2920  curityGroupId') 
-00010260: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00010270: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00010280: 6375 7269 7479 5f67 726f 7570 5f69 6420  curity_group_id 
-00010290: 3d20 6d2e 6765 7428 2753 6563 7572 6974  = m.get('Securit
-000102a0: 7947 726f 7570 4964 2729 0a20 2020 2020  yGroupId').     
-000102b0: 2020 2069 6620 6d2e 6765 7428 2753 7461     if m.get('Sta
-000102c0: 7274 5469 6d65 2729 2069 7320 6e6f 7420  rtTime') is not 
-000102d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000102e0: 2020 7365 6c66 2e73 7461 7274 5f74 696d    self.start_tim
-000102f0: 6520 3d20 6d2e 6765 7428 2753 7461 7274  e = m.get('Start
-00010300: 5469 6d65 2729 0a20 2020 2020 2020 2069  Time').        i
-00010310: 6620 6d2e 6765 7428 2753 7461 7475 7327  f m.get('Status'
-00010320: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00010330: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010340: 7374 6174 7573 203d 206d 2e67 6574 2827  status = m.get('
-00010350: 5374 6174 7573 2729 0a20 2020 2020 2020  Status').       
-00010360: 2069 6620 6d2e 6765 7428 2754 6167 7327   if m.get('Tags'
-00010370: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00010380: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-00010390: 6d6f 6465 6c20 3d20 4465 7363 7269 6265  model = Describe
-000103a0: 4561 6973 5265 7370 6f6e 7365 426f 6479  EaisResponseBody
-000103b0: 496e 7374 616e 6365 7349 6e73 7461 6e63  InstancesInstanc
-000103c0: 6554 6167 7328 290a 2020 2020 2020 2020  eTags().        
-000103d0: 2020 2020 7365 6c66 2e74 6167 7320 3d20      self.tags = 
-000103e0: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-000103f0: 6d61 7028 6d5b 2754 6167 7327 5d29 0a20  map(m['Tags']). 
-00010400: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00010410: 2756 5377 6974 6368 4964 2729 2069 7320  'VSwitchId') is 
-00010420: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00010430: 2020 2020 2020 7365 6c66 2e76 5f73 7769        self.v_swi
-00010440: 7463 685f 6964 203d 206d 2e67 6574 2827  tch_id = m.get('
-00010450: 5653 7769 7463 6849 6427 290a 2020 2020  VSwitchId').    
-00010460: 2020 2020 6966 206d 2e67 6574 2827 5a6f      if m.get('Zo
-00010470: 6e65 4964 2729 2069 7320 6e6f 7420 4e6f  neId') is not No
-00010480: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00010490: 7365 6c66 2e7a 6f6e 655f 6964 203d 206d  self.zone_id = m
-000104a0: 2e67 6574 2827 5a6f 6e65 4964 2729 0a20  .get('ZoneId'). 
-000104b0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000104c0: 6c66 0a0a 0a63 6c61 7373 2044 6573 6372  lf...class Descr
-000104d0: 6962 6545 6169 7352 6573 706f 6e73 6542  ibeEaisResponseB
-000104e0: 6f64 7949 6e73 7461 6e63 6573 2854 6561  odyInstances(Tea
-000104f0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00010500: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00010510: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00010520: 696e 7374 616e 6365 3a20 4c69 7374 5b44  instance: List[D
-00010530: 6573 6372 6962 6545 6169 7352 6573 706f  escribeEaisRespo
-00010540: 6e73 6542 6f64 7949 6e73 7461 6e63 6573  nseBodyInstances
-00010550: 496e 7374 616e 6365 5d20 3d20 4e6f 6e65  Instance] = None
-00010560: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00010570: 2073 656c 662e 696e 7374 616e 6365 203d   self.instance =
-00010580: 2069 6e73 7461 6e63 650a 0a20 2020 2064   instance..    d
-00010590: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000105a0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
-000105b0: 6c66 2e69 6e73 7461 6e63 653a 0a20 2020  lf.instance:.   
-000105c0: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
-000105d0: 6e20 7365 6c66 2e69 6e73 7461 6e63 653a  n self.instance:
-000105e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000105f0: 2069 6620 6b3a 0a20 2020 2020 2020 2020   if k:.         
-00010600: 2020 2020 2020 2020 2020 206b 2e76 616c             k.val
-00010610: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-00010620: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00010630: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-00010640: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-00010650: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-00010660: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00010670: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00010680: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00010690: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-000106a0: 2020 2020 2072 6573 756c 745b 2749 6e73       result['Ins
-000106b0: 7461 6e63 6527 5d20 3d20 5b5d 0a20 2020  tance'] = [].   
-000106c0: 2020 2020 2069 6620 7365 6c66 2e69 6e73       if self.ins
-000106d0: 7461 6e63 6520 6973 206e 6f74 204e 6f6e  tance is not Non
-000106e0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-000106f0: 6f72 206b 2069 6e20 7365 6c66 2e69 6e73  or k in self.ins
-00010700: 7461 6e63 653a 0a20 2020 2020 2020 2020  tance:.         
-00010710: 2020 2020 2020 2072 6573 756c 745b 2749         result['I
-00010720: 6e73 7461 6e63 6527 5d2e 6170 7065 6e64  nstance'].append
-00010730: 286b 2e74 6f5f 6d61 7028 2920 6966 206b  (k.to_map() if k
-00010740: 2065 6c73 6520 4e6f 6e65 290a 2020 2020   else None).    
-00010750: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00010760: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00010770: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00010780: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00010790: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-000107a0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-000107b0: 696e 7374 616e 6365 203d 205b 5d0a 2020  instance = [].  
-000107c0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-000107d0: 496e 7374 616e 6365 2729 2069 7320 6e6f  Instance') is no
-000107e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000107f0: 2020 2020 666f 7220 6b20 696e 206d 2e67      for k in m.g
-00010800: 6574 2827 496e 7374 616e 6365 2729 3a0a  et('Instance'):.
-00010810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010820: 7465 6d70 5f6d 6f64 656c 203d 2044 6573  temp_model = Des
-00010830: 6372 6962 6545 6169 7352 6573 706f 6e73  cribeEaisRespons
-00010840: 6542 6f64 7949 6e73 7461 6e63 6573 496e  eBodyInstancesIn
-00010850: 7374 616e 6365 2829 0a20 2020 2020 2020  stance().       
-00010860: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
-00010870: 7374 616e 6365 2e61 7070 656e 6428 7465  stance.append(te
-00010880: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-00010890: 7028 6b29 290a 2020 2020 2020 2020 7265  p(k)).        re
-000108a0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-000108b0: 7320 4465 7363 7269 6265 4561 6973 5265  s DescribeEaisRe
-000108c0: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
-000108d0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-000108e0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000108f0: 7365 6c66 2c0a 2020 2020 2020 2020 696e  self,.        in
-00010900: 7374 616e 6365 733a 2044 6573 6372 6962  stances: Describ
-00010910: 6545 6169 7352 6573 706f 6e73 6542 6f64  eEaisResponseBod
-00010920: 7949 6e73 7461 6e63 6573 203d 204e 6f6e  yInstances = Non
-00010930: 652c 0a20 2020 2020 2020 2070 6167 655f  e,.        page_
-00010940: 6e75 6d62 6572 3a20 696e 7420 3d20 4e6f  number: int = No
-00010950: 6e65 2c0a 2020 2020 2020 2020 7061 6765  ne,.        page
-00010960: 5f73 697a 653a 2069 6e74 203d 204e 6f6e  _size: int = Non
-00010970: 652c 0a20 2020 2020 2020 2072 6571 7565  e,.        reque
-00010980: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
-00010990: 652c 0a20 2020 2020 2020 2074 6f74 616c  e,.        total
-000109a0: 5f63 6f75 6e74 3a20 696e 7420 3d20 4e6f  _count: int = No
-000109b0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-000109c0: 2020 2073 656c 662e 696e 7374 616e 6365     self.instance
-000109d0: 7320 3d20 696e 7374 616e 6365 730a 2020  s = instances.  
-000109e0: 2020 2020 2020 7365 6c66 2e70 6167 655f        self.page_
-000109f0: 6e75 6d62 6572 203d 2070 6167 655f 6e75  number = page_nu
-00010a00: 6d62 6572 0a20 2020 2020 2020 2073 656c  mber.        sel
-00010a10: 662e 7061 6765 5f73 697a 6520 3d20 7061  f.page_size = pa
-00010a20: 6765 5f73 697a 650a 2020 2020 2020 2020  ge_size.        
-00010a30: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-00010a40: 3d20 7265 7175 6573 745f 6964 0a20 2020  = request_id.   
-00010a50: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
-00010a60: 636f 756e 7420 3d20 746f 7461 6c5f 636f  count = total_co
-00010a70: 756e 740a 0a20 2020 2064 6566 2076 616c  unt..    def val
-00010a80: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00010a90: 2020 2020 2069 6620 7365 6c66 2e69 6e73       if self.ins
-00010aa0: 7461 6e63 6573 3a0a 2020 2020 2020 2020  tances:.        
-00010ab0: 2020 2020 7365 6c66 2e69 6e73 7461 6e63      self.instanc
-00010ac0: 6573 2e76 616c 6964 6174 6528 290a 0a20  es.validate().. 
-00010ad0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00010ae0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00010af0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-00010b00: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00010b10: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00010b20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00010b30: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00010b40: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00010b50: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00010b60: 6c66 2e69 6e73 7461 6e63 6573 2069 7320  lf.instances is 
-00010b70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00010b80: 2020 2020 2020 7265 7375 6c74 5b27 496e        result['In
-00010b90: 7374 616e 6365 7327 5d20 3d20 7365 6c66  stances'] = self
-00010ba0: 2e69 6e73 7461 6e63 6573 2e74 6f5f 6d61  .instances.to_ma
-00010bb0: 7028 290a 2020 2020 2020 2020 6966 2073  p().        if s
-00010bc0: 656c 662e 7061 6765 5f6e 756d 6265 7220  elf.page_number 
-00010bd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00010be0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00010bf0: 2750 6167 654e 756d 6265 7227 5d20 3d20  'PageNumber'] = 
-00010c00: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
-00010c10: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00010c20: 2e70 6167 655f 7369 7a65 2069 7320 6e6f  .page_size is no
-00010c30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00010c40: 2020 2020 7265 7375 6c74 5b27 5061 6765      result['Page
-00010c50: 5369 7a65 275d 203d 2073 656c 662e 7061  Size'] = self.pa
-00010c60: 6765 5f73 697a 650a 2020 2020 2020 2020  ge_size.        
-00010c70: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
-00010c80: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00010c90: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00010ca0: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
-00010cb0: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
-00010cc0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-00010cd0: 662e 746f 7461 6c5f 636f 756e 7420 6973  f.total_count is
-00010ce0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00010cf0: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
-00010d00: 6f74 616c 436f 756e 7427 5d20 3d20 7365  otalCount'] = se
-00010d10: 6c66 2e74 6f74 616c 5f63 6f75 6e74 0a20  lf.total_count. 
-00010d20: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00010d30: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00010d40: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-00010d50: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-00010d60: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00010d70: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00010d80: 206d 2e67 6574 2827 496e 7374 616e 6365   m.get('Instance
-00010d90: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-00010da0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-00010db0: 705f 6d6f 6465 6c20 3d20 4465 7363 7269  p_model = Descri
-00010dc0: 6265 4561 6973 5265 7370 6f6e 7365 426f  beEaisResponseBo
-00010dd0: 6479 496e 7374 616e 6365 7328 290a 2020  dyInstances().  
-00010de0: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
-00010df0: 6e73 7461 6e63 6573 203d 2074 656d 705f  nstances = temp_
-00010e00: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-00010e10: 5b27 496e 7374 616e 6365 7327 5d29 0a20  ['Instances']). 
-00010e20: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00010e30: 2750 6167 654e 756d 6265 7227 2920 6973  'PageNumber') is
-00010e40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00010e50: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
-00010e60: 5f6e 756d 6265 7220 3d20 6d2e 6765 7428  _number = m.get(
-00010e70: 2750 6167 654e 756d 6265 7227 290a 2020  'PageNumber').  
-00010e80: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00010e90: 5061 6765 5369 7a65 2729 2069 7320 6e6f  PageSize') is no
-00010ea0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00010eb0: 2020 2020 7365 6c66 2e70 6167 655f 7369      self.page_si
-00010ec0: 7a65 203d 206d 2e67 6574 2827 5061 6765  ze = m.get('Page
-00010ed0: 5369 7a65 2729 0a20 2020 2020 2020 2069  Size').        i
-00010ee0: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
-00010ef0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00010f00: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00010f10: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-00010f20: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-00010f30: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00010f40: 6765 7428 2754 6f74 616c 436f 756e 7427  get('TotalCount'
-00010f50: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00010f60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010f70: 746f 7461 6c5f 636f 756e 7420 3d20 6d2e  total_count = m.
-00010f80: 6765 7428 2754 6f74 616c 436f 756e 7427  get('TotalCount'
-00010f90: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00010fa0: 2073 656c 660a 0a0a 636c 6173 7320 4465   self...class De
-00010fb0: 7363 7269 6265 4561 6973 5265 7370 6f6e  scribeEaisRespon
-00010fc0: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-00010fd0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00010fe0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00010ff0: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
-00011000: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
-00011010: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00011020: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
-00011030: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
-00011040: 6f64 793a 2044 6573 6372 6962 6545 6169  ody: DescribeEai
-00011050: 7352 6573 706f 6e73 6542 6f64 7920 3d20  sResponseBody = 
-00011060: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00011070: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-00011080: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
-00011090: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-000110a0: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
-000110b0: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
-000110c0: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
-000110d0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-000110e0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-000110f0: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00011100: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
-00011110: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
-00011120: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00011130: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-00011140: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
-00011150: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
-00011160: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00011170: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-00011180: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
-00011190: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-000111a0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-000111b0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-000111c0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-000111d0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-000111e0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-000111f0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-00011200: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00011210: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00011220: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00011230: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00011240: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00011250: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-00011260: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-00011270: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00011280: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-00011290: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-000112a0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-000112b0: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-000112c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000112d0: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-000112e0: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-000112f0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-00011300: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-00011310: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00011320: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00011330: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-00011340: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-00011350: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00011360: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00011370: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00011380: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00011390: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-000113a0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000113b0: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-000113c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000113d0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000113e0: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-000113f0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-00011400: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-00011410: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-00011420: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00011430: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00011440: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-00011450: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-00011460: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-00011470: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00011480: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-00011490: 6465 6c20 3d20 4465 7363 7269 6265 4561  del = DescribeEa
-000114a0: 6973 5265 7370 6f6e 7365 426f 6479 2829  isResponseBody()
-000114b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000114c0: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
-000114d0: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
-000114e0: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
-000114f0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00011500: 6173 7320 4465 7363 7269 6265 5265 6769  ass DescribeRegi
-00011510: 6f6e 7352 6573 706f 6e73 6542 6f64 7952  onsResponseBodyR
-00011520: 6567 696f 6e73 5265 6769 6f6e 2854 6561  egionsRegion(Tea
-00011530: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00011540: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00011550: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00011560: 6c6f 6361 6c5f 6e61 6d65 3a20 7374 7220  local_name: str 
-00011570: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00011580: 7265 6769 6f6e 5f65 6e64 706f 696e 743a  region_endpoint:
-00011590: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000115a0: 2020 2020 2072 6567 696f 6e5f 6964 3a20       region_id: 
-000115b0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-000115c0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-000115d0: 6c6f 6361 6c5f 6e61 6d65 203d 206c 6f63  local_name = loc
-000115e0: 616c 5f6e 616d 650a 2020 2020 2020 2020  al_name.        
-000115f0: 7365 6c66 2e72 6567 696f 6e5f 656e 6470  self.region_endp
-00011600: 6f69 6e74 203d 2072 6567 696f 6e5f 656e  oint = region_en
-00011610: 6470 6f69 6e74 0a20 2020 2020 2020 2073  dpoint.        s
-00011620: 656c 662e 7265 6769 6f6e 5f69 6420 3d20  elf.region_id = 
-00011630: 7265 6769 6f6e 5f69 640a 0a20 2020 2064  region_id..    d
-00011640: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-00011650: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00011660: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00011670: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00011680: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-00011690: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-000116a0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-000116b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000116c0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-000116d0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-000116e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000116f0: 7365 6c66 2e6c 6f63 616c 5f6e 616d 6520  self.local_name 
-00011700: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00011710: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00011720: 274c 6f63 616c 4e61 6d65 275d 203d 2073  'LocalName'] = s
-00011730: 656c 662e 6c6f 6361 6c5f 6e61 6d65 0a20  elf.local_name. 
-00011740: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-00011750: 6567 696f 6e5f 656e 6470 6f69 6e74 2069  egion_endpoint i
-00011760: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00011770: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00011780: 5265 6769 6f6e 456e 6470 6f69 6e74 275d  RegionEndpoint']
-00011790: 203d 2073 656c 662e 7265 6769 6f6e 5f65   = self.region_e
-000117a0: 6e64 706f 696e 740a 2020 2020 2020 2020  ndpoint.        
-000117b0: 6966 2073 656c 662e 7265 6769 6f6e 5f69  if self.region_i
-000117c0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000117d0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000117e0: 745b 2752 6567 696f 6e49 6427 5d20 3d20  t['RegionId'] = 
-000117f0: 7365 6c66 2e72 6567 696f 6e5f 6964 0a20  self.region_id. 
-00011800: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00011810: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00011820: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-00011830: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-00011840: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00011850: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00011860: 206d 2e67 6574 2827 4c6f 6361 6c4e 616d   m.get('LocalNam
-00011870: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00011880: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00011890: 662e 6c6f 6361 6c5f 6e61 6d65 203d 206d  f.local_name = m
-000118a0: 2e67 6574 2827 4c6f 6361 6c4e 616d 6527  .get('LocalName'
-000118b0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000118c0: 6574 2827 5265 6769 6f6e 456e 6470 6f69  et('RegionEndpoi
-000118d0: 6e74 2729 2069 7320 6e6f 7420 4e6f 6e65  nt') is not None
-000118e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000118f0: 6c66 2e72 6567 696f 6e5f 656e 6470 6f69  lf.region_endpoi
-00011900: 6e74 203d 206d 2e67 6574 2827 5265 6769  nt = m.get('Regi
-00011910: 6f6e 456e 6470 6f69 6e74 2729 0a20 2020  onEndpoint').   
-00011920: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-00011930: 6567 696f 6e49 6427 2920 6973 206e 6f74  egionId') is not
-00011940: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00011950: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
-00011960: 6420 3d20 6d2e 6765 7428 2752 6567 696f  d = m.get('Regio
-00011970: 6e49 6427 290a 2020 2020 2020 2020 7265  nId').        re
-00011980: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-00011990: 7320 4465 7363 7269 6265 5265 6769 6f6e  s DescribeRegion
-000119a0: 7352 6573 706f 6e73 6542 6f64 7952 6567  sResponseBodyReg
-000119b0: 696f 6e73 2854 6561 4d6f 6465 6c29 3a0a  ions(TeaModel):.
-000119c0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-000119d0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000119e0: 2020 2020 2020 2020 7265 6769 6f6e 3a20          region: 
-000119f0: 4c69 7374 5b44 6573 6372 6962 6552 6567  List[DescribeReg
-00011a00: 696f 6e73 5265 7370 6f6e 7365 426f 6479  ionsResponseBody
-00011a10: 5265 6769 6f6e 7352 6567 696f 6e5d 203d  RegionsRegion] =
-00011a20: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-00011a30: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-00011a40: 6e20 3d20 7265 6769 6f6e 0a0a 2020 2020  n = region..    
-00011a50: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00011a60: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00011a70: 656c 662e 7265 6769 6f6e 3a0a 2020 2020  elf.region:.    
-00011a80: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00011a90: 2073 656c 662e 7265 6769 6f6e 3a0a 2020   self.region:.  
-00011aa0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011ab0: 206b 3a0a 2020 2020 2020 2020 2020 2020   k:.            
-00011ac0: 2020 2020 2020 2020 6b2e 7661 6c69 6461          k.valida
-00011ad0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-00011ae0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00011af0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00011b00: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-00011b10: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00011b20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00011b30: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00011b40: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00011b50: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00011b60: 2020 7265 7375 6c74 5b27 5265 6769 6f6e    result['Region
-00011b70: 275d 203d 205b 5d0a 2020 2020 2020 2020  '] = [].        
-00011b80: 6966 2073 656c 662e 7265 6769 6f6e 2069  if self.region i
-00011b90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00011ba0: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00011bb0: 2073 656c 662e 7265 6769 6f6e 3a0a 2020   self.region:.  
-00011bc0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00011bd0: 7375 6c74 5b27 5265 6769 6f6e 275d 2e61  sult['Region'].a
-00011be0: 7070 656e 6428 6b2e 746f 5f6d 6170 2829  ppend(k.to_map()
-00011bf0: 2069 6620 6b20 656c 7365 204e 6f6e 6529   if k else None)
-00011c00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011c10: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
-00011c20: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
-00011c30: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
-00011c40: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00011c50: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00011c60: 7365 6c66 2e72 6567 696f 6e20 3d20 5b5d  self.region = []
-00011c70: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00011c80: 7428 2752 6567 696f 6e27 2920 6973 206e  t('Region') is n
-00011c90: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00011ca0: 2020 2020 2066 6f72 206b 2069 6e20 6d2e       for k in m.
-00011cb0: 6765 7428 2752 6567 696f 6e27 293a 0a20  get('Region'):. 
-00011cc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00011cd0: 656d 705f 6d6f 6465 6c20 3d20 4465 7363  emp_model = Desc
-00011ce0: 7269 6265 5265 6769 6f6e 7352 6573 706f  ribeRegionsRespo
-00011cf0: 6e73 6542 6f64 7952 6567 696f 6e73 5265  nseBodyRegionsRe
-00011d00: 6769 6f6e 2829 0a20 2020 2020 2020 2020  gion().         
-00011d10: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
-00011d20: 6f6e 2e61 7070 656e 6428 7465 6d70 5f6d  on.append(temp_m
-00011d30: 6f64 656c 2e66 726f 6d5f 6d61 7028 6b29  odel.from_map(k)
-00011d40: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00011d50: 2073 656c 660a 0a0a 636c 6173 7320 4465   self...class De
-00011d60: 7363 7269 6265 5265 6769 6f6e 7352 6573  scribeRegionsRes
-00011d70: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
-00011d80: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-00011d90: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00011da0: 656c 662c 0a20 2020 2020 2020 2072 6567  elf,.        reg
-00011db0: 696f 6e73 3a20 4465 7363 7269 6265 5265  ions: DescribeRe
-00011dc0: 6769 6f6e 7352 6573 706f 6e73 6542 6f64  gionsResponseBod
-00011dd0: 7952 6567 696f 6e73 203d 204e 6f6e 652c  yRegions = None,
-00011de0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-00011df0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-00011e00: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00011e10: 7365 6c66 2e72 6567 696f 6e73 203d 2072  self.regions = r
-00011e20: 6567 696f 6e73 0a20 2020 2020 2020 2073  egions.        s
-00011e30: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-00011e40: 2072 6571 7565 7374 5f69 640a 0a20 2020   request_id..   
-00011e50: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00011e60: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-00011e70: 7365 6c66 2e72 6567 696f 6e73 3a0a 2020  self.regions:.  
-00011e80: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00011e90: 6567 696f 6e73 2e76 616c 6964 6174 6528  egions.validate(
-00011ea0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-00011eb0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00011ec0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-00011ed0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00011ee0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00011ef0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00011f00: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00011f10: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00011f20: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00011f30: 6620 7365 6c66 2e72 6567 696f 6e73 2069  f self.regions i
-00011f40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00011f50: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00011f60: 5265 6769 6f6e 7327 5d20 3d20 7365 6c66  Regions'] = self
-00011f70: 2e72 6567 696f 6e73 2e74 6f5f 6d61 7028  .regions.to_map(
-00011f80: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00011f90: 662e 7265 7175 6573 745f 6964 2069 7320  f.request_id is 
-00011fa0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00011fb0: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-00011fc0: 7175 6573 7449 6427 5d20 3d20 7365 6c66  questId'] = self
-00011fd0: 2e72 6571 7565 7374 5f69 640a 2020 2020  .request_id.    
-00011fe0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00011ff0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00012000: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00012010: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-00012020: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00012030: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00012040: 6765 7428 2752 6567 696f 6e73 2729 2069  get('Regions') i
-00012050: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00012060: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-00012070: 656c 203d 2044 6573 6372 6962 6552 6567  el = DescribeReg
-00012080: 696f 6e73 5265 7370 6f6e 7365 426f 6479  ionsResponseBody
-00012090: 5265 6769 6f6e 7328 290a 2020 2020 2020  Regions().      
-000120a0: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
-000120b0: 6e73 203d 2074 656d 705f 6d6f 6465 6c2e  ns = temp_model.
-000120c0: 6672 6f6d 5f6d 6170 286d 5b27 5265 6769  from_map(m['Regi
-000120d0: 6f6e 7327 5d29 0a20 2020 2020 2020 2069  ons']).        i
-000120e0: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
-000120f0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00012100: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00012110: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-00012120: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-00012130: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00012140: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2044  n self...class D
-00012150: 6573 6372 6962 6552 6567 696f 6e73 5265  escribeRegionsRe
-00012160: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-00012170: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00012180: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-00012190: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-000121a0: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-000121b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000121c0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-000121d0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-000121e0: 2020 2062 6f64 793a 2044 6573 6372 6962     body: Describ
-000121f0: 6552 6567 696f 6e73 5265 7370 6f6e 7365  eRegionsResponse
-00012200: 426f 6479 203d 204e 6f6e 652c 0a20 2020  Body = None,.   
-00012210: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-00012220: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
-00012230: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
-00012240: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
-00012250: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-00012260: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-00012270: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
-00012280: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00012290: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-000122a0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-000122b0: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
-000122c0: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
-000122d0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-000122e0: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
-000122f0: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
-00012300: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
-00012310: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-00012320: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
-00012330: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
-00012340: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-00012350: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-00012360: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-00012370: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-00012380: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00012390: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-000123a0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-000123b0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-000123c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000123d0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-000123e0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-000123f0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00012400: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-00012410: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00012420: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-00012430: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-00012440: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-00012450: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-00012460: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00012470: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00012480: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-00012490: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000124a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000124b0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-000124c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000124d0: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-000124e0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-000124f0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00012500: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00012510: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00012520: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-00012530: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00012540: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-00012550: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-00012560: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-00012570: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00012580: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-00012590: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-000125a0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000125b0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-000125c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000125d0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000125e0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-000125f0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-00012600: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00012610: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-00012620: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00012630: 7465 6d70 5f6d 6f64 656c 203d 2044 6573  temp_model = Des
-00012640: 6372 6962 6552 6567 696f 6e73 5265 7370  cribeRegionsResp
-00012650: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
-00012660: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-00012670: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-00012680: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
-00012690: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000126a0: 2073 656c 660a 0a0a 636c 6173 7320 4465   self...class De
-000126b0: 7461 6368 4561 6952 6571 7565 7374 2854  tachEaiRequest(T
-000126c0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-000126d0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-000126e0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-000126f0: 2020 656c 6173 7469 635f 6163 6365 6c65    elastic_accele
-00012700: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-00012710: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00012720: 2020 2020 2020 2072 6567 696f 6e5f 6964         region_id
-00012730: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00012740: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-00012750: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-00012760: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-00012770: 6420 3d20 656c 6173 7469 635f 6163 6365  d = elastic_acce
-00012780: 6c65 7261 7465 645f 696e 7374 616e 6365  lerated_instance
-00012790: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
-000127a0: 2e72 6567 696f 6e5f 6964 203d 2072 6567  .region_id = reg
-000127b0: 696f 6e5f 6964 0a0a 2020 2020 6465 6620  ion_id..    def 
-000127c0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-000127d0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000127e0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-000127f0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-00012800: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-00012810: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00012820: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00012830: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00012840: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00012850: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00012860: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00012870: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
-00012880: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
-00012890: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000128a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000128b0: 745b 2745 6c61 7374 6963 4163 6365 6c65  t['ElasticAccele
-000128c0: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
-000128d0: 5d20 3d20 7365 6c66 2e65 6c61 7374 6963  ] = self.elastic
-000128e0: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
-000128f0: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
-00012900: 2069 6620 7365 6c66 2e72 6567 696f 6e5f   if self.region_
-00012910: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-00012920: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00012930: 6c74 5b27 5265 6769 6f6e 4964 275d 203d  lt['RegionId'] =
-00012940: 2073 656c 662e 7265 6769 6f6e 5f69 640a   self.region_id.
-00012950: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00012960: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-00012970: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-00012980: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-00012990: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-000129a0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000129b0: 6620 6d2e 6765 7428 2745 6c61 7374 6963  f m.get('Elastic
-000129c0: 4163 6365 6c65 7261 7465 6449 6e73 7461  AcceleratedInsta
-000129d0: 6e63 6549 6427 2920 6973 206e 6f74 204e  nceId') is not N
-000129e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000129f0: 2073 656c 662e 656c 6173 7469 635f 6163   self.elastic_ac
-00012a00: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
-00012a10: 6365 5f69 6420 3d20 6d2e 6765 7428 2745  ce_id = m.get('E
-00012a20: 6c61 7374 6963 4163 6365 6c65 7261 7465  lasticAccelerate
-00012a30: 6449 6e73 7461 6e63 6549 6427 290a 2020  dInstanceId').  
-00012a40: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00012a50: 5265 6769 6f6e 4964 2729 2069 7320 6e6f  RegionId') is no
-00012a60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00012a70: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
-00012a80: 6964 203d 206d 2e67 6574 2827 5265 6769  id = m.get('Regi
-00012a90: 6f6e 4964 2729 0a20 2020 2020 2020 2072  onId').        r
-00012aa0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-00012ab0: 7373 2044 6574 6163 6845 6169 5265 7370  ss DetachEaiResp
-00012ac0: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
-00012ad0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00012ae0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00012af0: 6c66 2c0a 2020 2020 2020 2020 7265 7175  lf,.        requ
-00012b00: 6573 745f 6964 3a20 7374 7220 3d20 4e6f  est_id: str = No
-00012b10: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00012b20: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-00012b30: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
-00012b40: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00012b50: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00012b60: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00012b70: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00012b80: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00012b90: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-00012ba0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00012bb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00012bc0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00012bd0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00012be0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00012bf0: 2020 2069 6620 7365 6c66 2e72 6571 7565     if self.reque
-00012c00: 7374 5f69 6420 6973 206e 6f74 204e 6f6e  st_id is not Non
-00012c10: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00012c20: 6573 756c 745b 2752 6571 7565 7374 4964  esult['RequestId
-00012c30: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
-00012c40: 745f 6964 0a20 2020 2020 2020 2072 6574  t_id.        ret
-00012c50: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00012c60: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00012c70: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-00012c80: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00012c90: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-00012ca0: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-00012cb0: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
-00012cc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00012cd0: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-00012ce0: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
-00012cf0: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
-00012d00: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00012d10: 6173 7320 4465 7461 6368 4561 6952 6573  ass DetachEaiRes
-00012d20: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-00012d30: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00012d40: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00012d50: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-00012d60: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-00012d70: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00012d80: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-00012d90: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-00012da0: 2020 626f 6479 3a20 4465 7461 6368 4561    body: DetachEa
-00012db0: 6952 6573 706f 6e73 6542 6f64 7920 3d20  iResponseBody = 
-00012dc0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00012dd0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-00012de0: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
-00012df0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-00012e00: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
-00012e10: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
-00012e20: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
-00012e30: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00012e40: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00012e50: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00012e60: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
-00012e70: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
-00012e80: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00012e90: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-00012ea0: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
-00012eb0: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
-00012ec0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00012ed0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-00012ee0: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
-00012ef0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00012f00: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-00012f10: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-00012f20: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-00012f30: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00012f40: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00012f50: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-00012f60: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-00012f70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00012f80: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00012f90: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-00012fa0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-00012fb0: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-00012fc0: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-00012fd0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00012fe0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-00012ff0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-00013000: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00013010: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-00013020: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00013030: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-00013040: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-00013050: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-00013060: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-00013070: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00013080: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00013090: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-000130a0: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-000130b0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-000130c0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-000130d0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-000130e0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-000130f0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00013100: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00013110: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-00013120: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00013130: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-00013140: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-00013150: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-00013160: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-00013170: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-00013180: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00013190: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000131a0: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-000131b0: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-000131c0: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-000131d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000131e0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-000131f0: 6465 6c20 3d20 4465 7461 6368 4561 6952  del = DetachEaiR
-00013200: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
-00013210: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00013220: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
-00013230: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
-00013240: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
-00013250: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-00013260: 2047 6574 496e 7374 616e 6365 4d65 7472   GetInstanceMetr
-00013270: 6963 7352 6571 7565 7374 2854 6561 4d6f  icsRequest(TeaMo
-00013280: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00013290: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000132a0: 7365 6c66 2c0a 2020 2020 2020 2020 656e  self,.        en
-000132b0: 645f 7469 6d65 3a20 7374 7220 3d20 4e6f  d_time: str = No
-000132c0: 6e65 2c0a 2020 2020 2020 2020 696e 7374  ne,.        inst
-000132d0: 616e 6365 5f69 643a 2073 7472 203d 204e  ance_id: str = N
-000132e0: 6f6e 652c 0a20 2020 2020 2020 206d 6574  one,.        met
-000132f0: 7269 635f 7479 7065 3a20 7374 7220 3d20  ric_type: str = 
-00013300: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00013310: 6172 745f 7469 6d65 3a20 7374 7220 3d20  art_time: str = 
-00013320: 4e6f 6e65 2c0a 2020 2020 2020 2020 7469  None,.        ti
-00013330: 6d65 5f73 7465 703a 2073 7472 203d 204e  me_step: str = N
-00013340: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-00013350: 2020 2020 7365 6c66 2e65 6e64 5f74 696d      self.end_tim
-00013360: 6520 3d20 656e 645f 7469 6d65 0a20 2020  e = end_time.   
-00013370: 2020 2020 2073 656c 662e 696e 7374 616e       self.instan
-00013380: 6365 5f69 6420 3d20 696e 7374 616e 6365  ce_id = instance
-00013390: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
-000133a0: 2e6d 6574 7269 635f 7479 7065 203d 206d  .metric_type = m
-000133b0: 6574 7269 635f 7479 7065 0a20 2020 2020  etric_type.     
-000133c0: 2020 2073 656c 662e 7374 6172 745f 7469     self.start_ti
-000133d0: 6d65 203d 2073 7461 7274 5f74 696d 650a  me = start_time.
-000133e0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-000133f0: 655f 7374 6570 203d 2074 696d 655f 7374  e_step = time_st
-00013400: 6570 0a0a 2020 2020 6465 6620 7661 6c69  ep..    def vali
-00013410: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00013420: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00013430: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00013440: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00013450: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-00013460: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00013470: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00013480: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00013490: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-000134a0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-000134b0: 2020 2020 2020 6966 2073 656c 662e 656e        if self.en
-000134c0: 645f 7469 6d65 2069 7320 6e6f 7420 4e6f  d_time is not No
-000134d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000134e0: 7265 7375 6c74 5b27 456e 6454 696d 6527  result['EndTime'
-000134f0: 5d20 3d20 7365 6c66 2e65 6e64 5f74 696d  ] = self.end_tim
-00013500: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00013510: 662e 696e 7374 616e 6365 5f69 6420 6973  f.instance_id is
-00013520: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00013530: 2020 2020 2020 2072 6573 756c 745b 2749         result['I
-00013540: 6e73 7461 6e63 6549 6427 5d20 3d20 7365  nstanceId'] = se
-00013550: 6c66 2e69 6e73 7461 6e63 655f 6964 0a20  lf.instance_id. 
-00013560: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
-00013570: 6574 7269 635f 7479 7065 2069 7320 6e6f  etric_type is no
-00013580: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00013590: 2020 2020 7265 7375 6c74 5b27 4d65 7472      result['Metr
-000135a0: 6963 5479 7065 275d 203d 2073 656c 662e  icType'] = self.
-000135b0: 6d65 7472 6963 5f74 7970 650a 2020 2020  metric_type.    
-000135c0: 2020 2020 6966 2073 656c 662e 7374 6172      if self.star
-000135d0: 745f 7469 6d65 2069 7320 6e6f 7420 4e6f  t_time is not No
-000135e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000135f0: 7265 7375 6c74 5b27 5374 6172 7454 696d  result['StartTim
-00013600: 6527 5d20 3d20 7365 6c66 2e73 7461 7274  e'] = self.start
-00013610: 5f74 696d 650a 2020 2020 2020 2020 6966  _time.        if
-00013620: 2073 656c 662e 7469 6d65 5f73 7465 7020   self.time_step 
-00013630: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00013640: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00013650: 2754 696d 6553 7465 7027 5d20 3d20 7365  'TimeStep'] = se
-00013660: 6c66 2e74 696d 655f 7374 6570 0a20 2020  lf.time_step.   
-00013670: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00013680: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-00013690: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-000136a0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-000136b0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-000136c0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-000136d0: 2e67 6574 2827 456e 6454 696d 6527 2920  .get('EndTime') 
-000136e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000136f0: 2020 2020 2020 2020 2073 656c 662e 656e           self.en
-00013700: 645f 7469 6d65 203d 206d 2e67 6574 2827  d_time = m.get('
-00013710: 456e 6454 696d 6527 290a 2020 2020 2020  EndTime').      
-00013720: 2020 6966 206d 2e67 6574 2827 496e 7374    if m.get('Inst
-00013730: 616e 6365 4964 2729 2069 7320 6e6f 7420  anceId') is not 
-00013740: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00013750: 2020 7365 6c66 2e69 6e73 7461 6e63 655f    self.instance_
-00013760: 6964 203d 206d 2e67 6574 2827 496e 7374  id = m.get('Inst
-00013770: 616e 6365 4964 2729 0a20 2020 2020 2020  anceId').       
-00013780: 2069 6620 6d2e 6765 7428 274d 6574 7269   if m.get('Metri
-00013790: 6354 7970 6527 2920 6973 206e 6f74 204e  cType') is not N
-000137a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000137b0: 2073 656c 662e 6d65 7472 6963 5f74 7970   self.metric_typ
-000137c0: 6520 3d20 6d2e 6765 7428 274d 6574 7269  e = m.get('Metri
-000137d0: 6354 7970 6527 290a 2020 2020 2020 2020  cType').        
-000137e0: 6966 206d 2e67 6574 2827 5374 6172 7454  if m.get('StartT
-000137f0: 696d 6527 2920 6973 206e 6f74 204e 6f6e  ime') is not Non
-00013800: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00013810: 656c 662e 7374 6172 745f 7469 6d65 203d  elf.start_time =
-00013820: 206d 2e67 6574 2827 5374 6172 7454 696d   m.get('StartTim
-00013830: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-00013840: 2e67 6574 2827 5469 6d65 5374 6570 2729  .get('TimeStep')
-00013850: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00013860: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00013870: 696d 655f 7374 6570 203d 206d 2e67 6574  ime_step = m.get
-00013880: 2827 5469 6d65 5374 6570 2729 0a20 2020  ('TimeStep').   
-00013890: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000138a0: 0a0a 0a63 6c61 7373 2047 6574 496e 7374  ...class GetInst
-000138b0: 616e 6365 4d65 7472 6963 7352 6573 706f  anceMetricsRespo
-000138c0: 6e73 6542 6f64 7950 6f64 4d65 7472 6963  nseBodyPodMetric
-000138d0: 734d 6574 7269 6373 2854 6561 4d6f 6465  sMetrics(TeaMode
-000138e0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-000138f0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00013900: 6c66 2c0a 2020 2020 2020 2020 7469 6d65  lf,.        time
-00013910: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00013920: 2020 2020 2020 7661 6c75 653a 2073 7472        value: str
-00013930: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-00013940: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-00013950: 6520 3d20 7469 6d65 0a20 2020 2020 2020  e = time.       
-00013960: 2073 656c 662e 7661 6c75 6520 3d20 7661   self.value = va
-00013970: 6c75 650a 0a20 2020 2064 6566 2076 616c  lue..    def val
-00013980: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00013990: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000139a0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-000139b0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-000139c0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-000139d0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-000139e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000139f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00013a00: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00013a10: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00013a20: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-00013a30: 696d 6520 6973 206e 6f74 204e 6f6e 653a  ime is not None:
-00013a40: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00013a50: 756c 745b 2754 696d 6527 5d20 3d20 7365  ult['Time'] = se
-00013a60: 6c66 2e74 696d 650a 2020 2020 2020 2020  lf.time.        
-00013a70: 6966 2073 656c 662e 7661 6c75 6520 6973  if self.value is
-00013a80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00013a90: 2020 2020 2020 2072 6573 756c 745b 2756         result['V
-00013aa0: 616c 7565 275d 203d 2073 656c 662e 7661  alue'] = self.va
-00013ab0: 6c75 650a 2020 2020 2020 2020 7265 7475  lue.        retu
-00013ac0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00013ad0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00013ae0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-00013af0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00013b00: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00013b10: 2020 2069 6620 6d2e 6765 7428 2754 696d     if m.get('Tim
-00013b20: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00013b30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013b40: 662e 7469 6d65 203d 206d 2e67 6574 2827  f.time = m.get('
-00013b50: 5469 6d65 2729 0a20 2020 2020 2020 2069  Time').        i
-00013b60: 6620 6d2e 6765 7428 2756 616c 7565 2729  f m.get('Value')
-00013b70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00013b80: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-00013b90: 616c 7565 203d 206d 2e67 6574 2827 5661  alue = m.get('Va
-00013ba0: 6c75 6527 290a 2020 2020 2020 2020 7265  lue').        re
-00013bb0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-00013bc0: 7320 4765 7449 6e73 7461 6e63 654d 6574  s GetInstanceMet
-00013bd0: 7269 6373 5265 7370 6f6e 7365 426f 6479  ricsResponseBody
-00013be0: 506f 644d 6574 7269 6373 2854 6561 4d6f  PodMetrics(TeaMo
-00013bf0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-00013c00: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-00013c10: 7365 6c66 2c0a 2020 2020 2020 2020 6d65  self,.        me
-00013c20: 7472 6963 733a 204c 6973 745b 4765 7449  trics: List[GetI
-00013c30: 6e73 7461 6e63 654d 6574 7269 6373 5265  nstanceMetricsRe
-00013c40: 7370 6f6e 7365 426f 6479 506f 644d 6574  sponseBodyPodMet
-00013c50: 7269 6373 4d65 7472 6963 735d 203d 204e  ricsMetrics] = N
-00013c60: 6f6e 652c 0a20 2020 2020 2020 2070 6f64  one,.        pod
-00013c70: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-00013c80: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00013c90: 7365 6c66 2e6d 6574 7269 6373 203d 206d  self.metrics = m
-00013ca0: 6574 7269 6373 0a20 2020 2020 2020 2023  etrics.        #
-00013cb0: 2050 6f64 2049 44e3 8082 0a20 2020 2020   Pod ID....     
-00013cc0: 2020 2073 656c 662e 706f 645f 6964 203d     self.pod_id =
-00013cd0: 2070 6f64 5f69 640a 0a20 2020 2064 6566   pod_id..    def
-00013ce0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-00013cf0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00013d00: 2e6d 6574 7269 6373 3a0a 2020 2020 2020  .metrics:.      
-00013d10: 2020 2020 2020 666f 7220 6b20 696e 2073        for k in s
-00013d20: 656c 662e 6d65 7472 6963 733a 0a20 2020  elf.metrics:.   
-00013d30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00013d40: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
-00013d50: 2020 2020 2020 206b 2e76 616c 6964 6174         k.validat
-00013d60: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-00013d70: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00013d80: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00013d90: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00013da0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00013db0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00013dc0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00013dd0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00013de0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00013df0: 2072 6573 756c 745b 274d 6574 7269 6373   result['Metrics
-00013e00: 275d 203d 205b 5d0a 2020 2020 2020 2020  '] = [].        
-00013e10: 6966 2073 656c 662e 6d65 7472 6963 7320  if self.metrics 
-00013e20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00013e30: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
-00013e40: 6e20 7365 6c66 2e6d 6574 7269 6373 3a0a  n self.metrics:.
-00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e60: 7265 7375 6c74 5b27 4d65 7472 6963 7327  result['Metrics'
-00013e70: 5d2e 6170 7065 6e64 286b 2e74 6f5f 6d61  ].append(k.to_ma
-00013e80: 7028 2920 6966 206b 2065 6c73 6520 4e6f  p() if k else No
-00013e90: 6e65 290a 2020 2020 2020 2020 6966 2073  ne).        if s
-00013ea0: 656c 662e 706f 645f 6964 2069 7320 6e6f  elf.pod_id is no
-00013eb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00013ec0: 2020 2020 7265 7375 6c74 5b27 506f 6449      result['PodI
-00013ed0: 6427 5d20 3d20 7365 6c66 2e70 6f64 5f69  d'] = self.pod_i
-00013ee0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
-00013ef0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-00013f00: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-00013f10: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
-00013f20: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00013f30: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-00013f40: 2073 656c 662e 6d65 7472 6963 7320 3d20   self.metrics = 
-00013f50: 5b5d 0a20 2020 2020 2020 2069 6620 6d2e  [].        if m.
-00013f60: 6765 7428 274d 6574 7269 6373 2729 2069  get('Metrics') i
-00013f70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00013f80: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00013f90: 206d 2e67 6574 2827 4d65 7472 6963 7327   m.get('Metrics'
-00013fa0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00013fb0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-00013fc0: 4765 7449 6e73 7461 6e63 654d 6574 7269  GetInstanceMetri
-00013fd0: 6373 5265 7370 6f6e 7365 426f 6479 506f  csResponseBodyPo
-00013fe0: 644d 6574 7269 6373 4d65 7472 6963 7328  dMetricsMetrics(
-00013ff0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014000: 2020 7365 6c66 2e6d 6574 7269 6373 2e61    self.metrics.a
-00014010: 7070 656e 6428 7465 6d70 5f6d 6f64 656c  ppend(temp_model
-00014020: 2e66 726f 6d5f 6d61 7028 6b29 290a 2020  .from_map(k)).  
-00014030: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00014040: 506f 6449 6427 2920 6973 206e 6f74 204e  PodId') is not N
-00014050: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00014060: 2073 656c 662e 706f 645f 6964 203d 206d   self.pod_id = m
-00014070: 2e67 6574 2827 506f 6449 6427 290a 2020  .get('PodId').  
-00014080: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00014090: 660a 0a0a 636c 6173 7320 4765 7449 6e73  f...class GetIns
-000140a0: 7461 6e63 654d 6574 7269 6373 5265 7370  tanceMetricsResp
-000140b0: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
-000140c0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-000140d0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-000140e0: 6c66 2c0a 2020 2020 2020 2020 696e 7374  lf,.        inst
-000140f0: 616e 6365 5f69 643a 2073 7472 203d 204e  ance_id: str = N
-00014100: 6f6e 652c 0a20 2020 2020 2020 2070 6f64  one,.        pod
-00014110: 5f6d 6574 7269 6373 3a20 4c69 7374 5b47  _metrics: List[G
-00014120: 6574 496e 7374 616e 6365 4d65 7472 6963  etInstanceMetric
-00014130: 7352 6573 706f 6e73 6542 6f64 7950 6f64  sResponseBodyPod
-00014140: 4d65 7472 6963 735d 203d 204e 6f6e 652c  Metrics] = None,
-00014150: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-00014160: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-00014170: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00014180: 7365 6c66 2e69 6e73 7461 6e63 655f 6964  self.instance_id
-00014190: 203d 2069 6e73 7461 6e63 655f 6964 0a20   = instance_id. 
-000141a0: 2020 2020 2020 2073 656c 662e 706f 645f         self.pod_
-000141b0: 6d65 7472 6963 7320 3d20 706f 645f 6d65  metrics = pod_me
-000141c0: 7472 6963 730a 2020 2020 2020 2020 7365  trics.        se
-000141d0: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-000141e0: 7265 7175 6573 745f 6964 0a0a 2020 2020  request_id..    
-000141f0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00014200: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00014210: 656c 662e 706f 645f 6d65 7472 6963 733a  elf.pod_metrics:
-00014220: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00014230: 206b 2069 6e20 7365 6c66 2e70 6f64 5f6d   k in self.pod_m
-00014240: 6574 7269 6373 3a0a 2020 2020 2020 2020  etrics:.        
-00014250: 2020 2020 2020 2020 6966 206b 3a0a 2020          if k:.  
-00014260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014270: 2020 6b2e 7661 6c69 6461 7465 2829 0a0a    k.validate()..
-00014280: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-00014290: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000142a0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-000142b0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-000142c0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-000142d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000142e0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-000142f0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00014300: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00014310: 656c 662e 696e 7374 616e 6365 5f69 6420  elf.instance_id 
-00014320: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00014330: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00014340: 2749 6e73 7461 6e63 6549 6427 5d20 3d20  'InstanceId'] = 
-00014350: 7365 6c66 2e69 6e73 7461 6e63 655f 6964  self.instance_id
-00014360: 0a20 2020 2020 2020 2072 6573 756c 745b  .        result[
-00014370: 2750 6f64 4d65 7472 6963 7327 5d20 3d20  'PodMetrics'] = 
-00014380: 5b5d 0a20 2020 2020 2020 2069 6620 7365  [].        if se
-00014390: 6c66 2e70 6f64 5f6d 6574 7269 6373 2069  lf.pod_metrics i
-000143a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000143b0: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-000143c0: 2073 656c 662e 706f 645f 6d65 7472 6963   self.pod_metric
-000143d0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000143e0: 2020 2072 6573 756c 745b 2750 6f64 4d65     result['PodMe
-000143f0: 7472 6963 7327 5d2e 6170 7065 6e64 286b  trics'].append(k
-00014400: 2e74 6f5f 6d61 7028 2920 6966 206b 2065  .to_map() if k e
-00014410: 6c73 6520 4e6f 6e65 290a 2020 2020 2020  lse None).      
-00014420: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-00014430: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-00014440: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00014450: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
-00014460: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
-00014470: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-00014480: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00014490: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-000144a0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-000144b0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-000144c0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-000144d0: 2020 2069 6620 6d2e 6765 7428 2749 6e73     if m.get('Ins
-000144e0: 7461 6e63 6549 6427 2920 6973 206e 6f74  tanceId') is not
-000144f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00014500: 2020 2073 656c 662e 696e 7374 616e 6365     self.instance
-00014510: 5f69 6420 3d20 6d2e 6765 7428 2749 6e73  _id = m.get('Ins
-00014520: 7461 6e63 6549 6427 290a 2020 2020 2020  tanceId').      
-00014530: 2020 7365 6c66 2e70 6f64 5f6d 6574 7269    self.pod_metri
-00014540: 6373 203d 205b 5d0a 2020 2020 2020 2020  cs = [].        
-00014550: 6966 206d 2e67 6574 2827 506f 644d 6574  if m.get('PodMet
-00014560: 7269 6373 2729 2069 7320 6e6f 7420 4e6f  rics') is not No
-00014570: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00014580: 666f 7220 6b20 696e 206d 2e67 6574 2827  for k in m.get('
-00014590: 506f 644d 6574 7269 6373 2729 3a0a 2020  PodMetrics'):.  
-000145a0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-000145b0: 6d70 5f6d 6f64 656c 203d 2047 6574 496e  mp_model = GetIn
-000145c0: 7374 616e 6365 4d65 7472 6963 7352 6573  stanceMetricsRes
-000145d0: 706f 6e73 6542 6f64 7950 6f64 4d65 7472  ponseBodyPodMetr
-000145e0: 6963 7328 290a 2020 2020 2020 2020 2020  ics().          
-000145f0: 2020 2020 2020 7365 6c66 2e70 6f64 5f6d        self.pod_m
-00014600: 6574 7269 6373 2e61 7070 656e 6428 7465  etrics.append(te
-00014610: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-00014620: 7028 6b29 290a 2020 2020 2020 2020 6966  p(k)).        if
-00014630: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
-00014640: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00014650: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014660: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
-00014670: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-00014680: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00014690: 2073 656c 660a 0a0a 636c 6173 7320 4765   self...class Ge
-000146a0: 7449 6e73 7461 6e63 654d 6574 7269 6373  tInstanceMetrics
-000146b0: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-000146c0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-000146d0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-000146e0: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-000146f0: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-00014700: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-00014710: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-00014720: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-00014730: 2020 2020 2062 6f64 793a 2047 6574 496e       body: GetIn
-00014740: 7374 616e 6365 4d65 7472 6963 7352 6573  stanceMetricsRes
-00014750: 706f 6e73 6542 6f64 7920 3d20 4e6f 6e65  ponseBody = None
-00014760: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-00014770: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-00014780: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-00014790: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000147a0: 203d 2073 7461 7475 735f 636f 6465 0a20   = status_code. 
-000147b0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-000147c0: 203d 2062 6f64 790a 0a20 2020 2064 6566   = body..    def
-000147d0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-000147e0: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
-000147f0: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
-00014800: 7365 6c66 2e68 6561 6465 7273 2c20 2768  self.headers, 'h
-00014810: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
-00014820: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
-00014830: 6571 7569 7265 6428 7365 6c66 2e73 7461  equired(self.sta
-00014840: 7475 735f 636f 6465 2c20 2773 7461 7475  tus_code, 'statu
-00014850: 735f 636f 6465 2729 0a20 2020 2020 2020  s_code').       
-00014860: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
-00014870: 6571 7569 7265 6428 7365 6c66 2e62 6f64  equired(self.bod
-00014880: 792c 2027 626f 6479 2729 0a20 2020 2020  y, 'body').     
-00014890: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
-000148a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000148b0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
-000148c0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-000148d0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000148e0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000148f0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00014900: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00014910: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00014920: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00014930: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00014940: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00014950: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
-00014960: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00014970: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00014980: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
-00014990: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
-000149a0: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
-000149b0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-000149c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000149d0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
-000149e0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-000149f0: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
-00014a00: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-00014a10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00014a20: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-00014a30: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-00014a40: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00014a50: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00014a60: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00014a70: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-00014a80: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00014a90: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00014aa0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00014ab0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-00014ac0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00014ad0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-00014ae0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-00014af0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-00014b00: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00014b10: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00014b20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014b30: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
-00014b40: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-00014b50: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00014b60: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
-00014b70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00014b80: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-00014b90: 3d20 4765 7449 6e73 7461 6e63 654d 6574  = GetInstanceMet
-00014ba0: 7269 6373 5265 7370 6f6e 7365 426f 6479  ricsResponseBody
-00014bb0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00014bc0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-00014bd0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-00014be0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-00014bf0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+0000ecd0: 2020 2020 7365 6c66 2e66 6f72 6365 203d      self.force =
+0000ece0: 206d 2e67 6574 2827 466f 7263 6527 290a   m.get('Force').
+0000ecf0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0000ed00: 2827 5265 6769 6f6e 4964 2729 2069 7320  ('RegionId') is 
+0000ed10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000ed20: 2020 2020 2020 7365 6c66 2e72 6567 696f        self.regio
+0000ed30: 6e5f 6964 203d 206d 2e67 6574 2827 5265  n_id = m.get('Re
+0000ed40: 6769 6f6e 4964 2729 0a20 2020 2020 2020  gionId').       
+0000ed50: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+0000ed60: 6c61 7373 2044 656c 6574 6545 6169 5265  lass DeleteEaiRe
+0000ed70: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
+0000ed80: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+0000ed90: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+0000eda0: 7365 6c66 2c0a 2020 2020 2020 2020 7265  self,.        re
+0000edb0: 7175 6573 745f 6964 3a20 7374 7220 3d20  quest_id: str = 
+0000edc0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+0000edd0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+0000ede0: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
+0000edf0: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
+0000ee00: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+0000ee10: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+0000ee20: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0000ee30: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0000ee40: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+0000ee50: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0000ee60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000ee70: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0000ee80: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0000ee90: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0000eea0: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
+0000eeb0: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
+0000eec0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000eed0: 2072 6573 756c 745b 2752 6571 7565 7374   result['Request
+0000eee0: 4964 275d 203d 2073 656c 662e 7265 7175  Id'] = self.requ
+0000eef0: 6573 745f 6964 0a20 2020 2020 2020 2072  est_id.        r
+0000ef00: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+0000ef10: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+0000ef20: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+0000ef30: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+0000ef40: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+0000ef50: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0000ef60: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
+0000ef70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000ef80: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+0000ef90: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
+0000efa0: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
+0000efb0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+0000efc0: 636c 6173 7320 4465 6c65 7465 4561 6952  class DeleteEaiR
+0000efd0: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
+0000efe0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0000eff0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0000f000: 662c 0a20 2020 2020 2020 2068 6561 6465  f,.        heade
+0000f010: 7273 3a20 4469 6374 5b73 7472 2c20 7374  rs: Dict[str, st
+0000f020: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000f030: 2020 2073 7461 7475 735f 636f 6465 3a20     status_code: 
+0000f040: 696e 7420 3d20 4e6f 6e65 2c0a 2020 2020  int = None,.    
+0000f050: 2020 2020 626f 6479 3a20 4465 6c65 7465      body: Delete
+0000f060: 4561 6952 6573 706f 6e73 6542 6f64 7920  EaiResponseBody 
+0000f070: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+0000f080: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+0000f090: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
+0000f0a0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+0000f0b0: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
+0000f0c0: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
+0000f0d0: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
+0000f0e0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0000f0f0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+0000f100: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+0000f110: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
+0000f120: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
+0000f130: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0000f140: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0000f150: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
+0000f160: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
+0000f170: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0000f180: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0000f190: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
+0000f1a0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000f1b0: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+0000f1c0: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+0000f1d0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+0000f1e0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0000f1f0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0000f200: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+0000f210: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0000f220: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000f230: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0000f240: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0000f250: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0000f260: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+0000f270: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+0000f280: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000f290: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+0000f2a0: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+0000f2b0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0000f2c0: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+0000f2d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000f2e0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+0000f2f0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+0000f300: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+0000f310: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+0000f320: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000f330: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000f340: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+0000f350: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+0000f360: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0000f370: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+0000f380: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+0000f390: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+0000f3a0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0000f3b0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0000f3c0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+0000f3d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000f3e0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+0000f3f0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+0000f400: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+0000f410: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+0000f420: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+0000f430: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000f440: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0000f450: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+0000f460: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+0000f470: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+0000f480: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0000f490: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+0000f4a0: 6d6f 6465 6c20 3d20 4465 6c65 7465 4561  model = DeleteEa
+0000f4b0: 6952 6573 706f 6e73 6542 6f64 7928 290a  iResponseBody().
+0000f4c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f4d0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+0000f4e0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+0000f4f0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+0000f500: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+0000f510: 7373 2044 656c 6574 6545 6169 416c 6c52  ss DeleteEaiAllR
+0000f520: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+0000f530: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0000f540: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0000f550: 2c0a 2020 2020 2020 2020 636c 6965 6e74  ,.        client
+0000f560: 5f69 6e73 7461 6e63 655f 6964 3a20 7374  _instance_id: st
+0000f570: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0000f580: 2020 656c 6173 7469 635f 6163 6365 6c65    elastic_accele
+0000f590: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
+0000f5a0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0000f5b0: 2020 2020 2020 2072 6567 696f 6e5f 6964         region_id
+0000f5c0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0000f5d0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+0000f5e0: 662e 636c 6965 6e74 5f69 6e73 7461 6e63  f.client_instanc
+0000f5f0: 655f 6964 203d 2063 6c69 656e 745f 696e  e_id = client_in
+0000f600: 7374 616e 6365 5f69 640a 2020 2020 2020  stance_id.      
+0000f610: 2020 7365 6c66 2e65 6c61 7374 6963 5f61    self.elastic_a
+0000f620: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
+0000f630: 6e63 655f 6964 203d 2065 6c61 7374 6963  nce_id = elastic
+0000f640: 5f61 6363 656c 6572 6174 6564 5f69 6e73  _accelerated_ins
+0000f650: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+0000f660: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+0000f670: 3d20 7265 6769 6f6e 5f69 640a 0a20 2020  = region_id..   
+0000f680: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+0000f690: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+0000f6a0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+0000f6b0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0000f6c0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+0000f6d0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0000f6e0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0000f6f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000f700: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0000f710: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000f720: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0000f730: 6620 7365 6c66 2e63 6c69 656e 745f 696e  f self.client_in
+0000f740: 7374 616e 6365 5f69 6420 6973 206e 6f74  stance_id is not
+0000f750: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000f760: 2020 2072 6573 756c 745b 2743 6c69 656e     result['Clien
+0000f770: 7449 6e73 7461 6e63 6549 6427 5d20 3d20  tInstanceId'] = 
+0000f780: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
+0000f790: 616e 6365 5f69 640a 2020 2020 2020 2020  ance_id.        
+0000f7a0: 6966 2073 656c 662e 656c 6173 7469 635f  if self.elastic_
+0000f7b0: 6163 6365 6c65 7261 7465 645f 696e 7374  accelerated_inst
+0000f7c0: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
+0000f7d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000f7e0: 2072 6573 756c 745b 2745 6c61 7374 6963   result['Elastic
+0000f7f0: 4163 6365 6c65 7261 7465 6449 6e73 7461  AcceleratedInsta
+0000f800: 6e63 6549 6427 5d20 3d20 7365 6c66 2e65  nceId'] = self.e
+0000f810: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+0000f820: 6564 5f69 6e73 7461 6e63 655f 6964 0a20  ed_instance_id. 
+0000f830: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000f840: 6567 696f 6e5f 6964 2069 7320 6e6f 7420  egion_id is not 
+0000f850: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000f860: 2020 7265 7375 6c74 5b27 5265 6769 6f6e    result['Region
+0000f870: 4964 275d 203d 2073 656c 662e 7265 6769  Id'] = self.regi
+0000f880: 6f6e 5f69 640a 2020 2020 2020 2020 7265  on_id.        re
+0000f890: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+0000f8a0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+0000f8b0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+0000f8c0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+0000f8d0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+0000f8e0: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
+0000f8f0: 6c69 656e 7449 6e73 7461 6e63 6549 6427  lientInstanceId'
+0000f900: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0000f910: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f920: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
+0000f930: 6964 203d 206d 2e67 6574 2827 436c 6965  id = m.get('Clie
+0000f940: 6e74 496e 7374 616e 6365 4964 2729 0a20  ntInstanceId'). 
+0000f950: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0000f960: 2745 6c61 7374 6963 4163 6365 6c65 7261  'ElasticAccelera
+0000f970: 7465 6449 6e73 7461 6e63 6549 6427 2920  tedInstanceId') 
+0000f980: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000f990: 2020 2020 2020 2020 2073 656c 662e 656c           self.el
+0000f9a0: 6173 7469 635f 6163 6365 6c65 7261 7465  astic_accelerate
+0000f9b0: 645f 696e 7374 616e 6365 5f69 6420 3d20  d_instance_id = 
+0000f9c0: 6d2e 6765 7428 2745 6c61 7374 6963 4163  m.get('ElasticAc
+0000f9d0: 6365 6c65 7261 7465 6449 6e73 7461 6e63  celeratedInstanc
+0000f9e0: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
+0000f9f0: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
+0000fa00: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0000fa10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fa20: 2e72 6567 696f 6e5f 6964 203d 206d 2e67  .region_id = m.g
+0000fa30: 6574 2827 5265 6769 6f6e 4964 2729 0a20  et('RegionId'). 
+0000fa40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000fa50: 6c66 0a0a 0a63 6c61 7373 2044 656c 6574  lf...class Delet
+0000fa60: 6545 6169 416c 6c52 6573 706f 6e73 6542  eEaiAllResponseB
+0000fa70: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
+0000fa80: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000fa90: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000faa0: 2020 2020 2020 2072 6571 7565 7374 5f69         request_i
+0000fab0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0000fac0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+0000fad0: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+0000fae0: 7265 7175 6573 745f 6964 0a0a 2020 2020  request_id..    
+0000faf0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0000fb00: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0000fb10: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0000fb20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000fb30: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+0000fb40: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0000fb50: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+0000fb60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000fb70: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+0000fb80: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+0000fb90: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0000fba0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+0000fbb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000fbc0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000fbd0: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
+0000fbe0: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
+0000fbf0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000fc00: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0000fc10: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0000fc20: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0000fc30: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0000fc40: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0000fc50: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
+0000fc60: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+0000fc70: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000fc80: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+0000fc90: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+0000fca0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+0000fcb0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2044  n self...class D
+0000fcc0: 656c 6574 6545 6169 416c 6c52 6573 706f  eleteEaiAllRespo
+0000fcd0: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
+0000fce0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0000fcf0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+0000fd00: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
+0000fd10: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
+0000fd20: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+0000fd30: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
+0000fd40: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000fd50: 626f 6479 3a20 4465 6c65 7465 4561 6941  body: DeleteEaiA
+0000fd60: 6c6c 5265 7370 6f6e 7365 426f 6479 203d  llResponseBody =
+0000fd70: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+0000fd80: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+0000fd90: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
+0000fda0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+0000fdb0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+0000fdc0: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
+0000fdd0: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
+0000fde0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+0000fdf0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+0000fe00: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+0000fe10: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
+0000fe20: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
+0000fe30: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+0000fe40: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+0000fe50: 662e 7374 6174 7573 5f63 6f64 652c 2027  f.status_code, '
+0000fe60: 7374 6174 7573 5f63 6f64 6527 290a 2020  status_code').  
+0000fe70: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+0000fe80: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+0000fe90: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
+0000fea0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000feb0: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+0000fec0: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+0000fed0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+0000fee0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+0000fef0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+0000ff00: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+0000ff10: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+0000ff20: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000ff30: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+0000ff40: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+0000ff50: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+0000ff60: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
+0000ff70: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
+0000ff80: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000ff90: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
+0000ffa0: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
+0000ffb0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+0000ffc0: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
+0000ffd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000ffe0: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
+0000fff0: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
+00010000: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+00010010: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
+00010020: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00010030: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00010040: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
+00010050: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
+00010060: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00010070: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00010080: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+00010090: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+000100a0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+000100b0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+000100c0: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
+000100d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000100e0: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+000100f0: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
+00010100: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+00010110: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
+00010120: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
+00010130: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00010140: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00010150: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
+00010160: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
+00010170: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
+00010180: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00010190: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+000101a0: 6f64 656c 203d 2044 656c 6574 6545 6169  odel = DeleteEai
+000101b0: 416c 6c52 6573 706f 6e73 6542 6f64 7928  AllResponseBody(
+000101c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000101d0: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
+000101e0: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
+000101f0: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
+00010200: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00010210: 6c61 7373 2044 656c 6574 6545 6169 7345  lass DeleteEaisE
+00010220: 6952 6571 7565 7374 2854 6561 4d6f 6465  iRequest(TeaMode
+00010230: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00010240: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00010250: 6c66 2c0a 2020 2020 2020 2020 6569 5f69  lf,.        ei_i
+00010260: 6e73 7461 6e63 655f 6964 3a20 7374 7220  nstance_id: str 
+00010270: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00010280: 666f 7263 653a 2062 6f6f 6c20 3d20 4e6f  force: bool = No
+00010290: 6e65 2c0a 2020 2020 2020 2020 7265 6769  ne,.        regi
+000102a0: 6f6e 5f69 643a 2073 7472 203d 204e 6f6e  on_id: str = Non
+000102b0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000102c0: 2020 7365 6c66 2e65 695f 696e 7374 616e    self.ei_instan
+000102d0: 6365 5f69 6420 3d20 6569 5f69 6e73 7461  ce_id = ei_insta
+000102e0: 6e63 655f 6964 0a20 2020 2020 2020 2073  nce_id.        s
+000102f0: 656c 662e 666f 7263 6520 3d20 666f 7263  elf.force = forc
+00010300: 650a 2020 2020 2020 2020 7365 6c66 2e72  e.        self.r
+00010310: 6567 696f 6e5f 6964 203d 2072 6567 696f  egion_id = regio
+00010320: 6e5f 6964 0a0a 2020 2020 6465 6620 7661  n_id..    def va
+00010330: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00010340: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00010350: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00010360: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00010370: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00010380: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00010390: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000103a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000103b0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+000103c0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+000103d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000103e0: 6569 5f69 6e73 7461 6e63 655f 6964 2069  ei_instance_id i
+000103f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00010400: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00010410: 4569 496e 7374 616e 6365 4964 275d 203d  EiInstanceId'] =
+00010420: 2073 656c 662e 6569 5f69 6e73 7461 6e63   self.ei_instanc
+00010430: 655f 6964 0a20 2020 2020 2020 2069 6620  e_id.        if 
+00010440: 7365 6c66 2e66 6f72 6365 2069 7320 6e6f  self.force is no
+00010450: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00010460: 2020 2020 7265 7375 6c74 5b27 466f 7263      result['Forc
+00010470: 6527 5d20 3d20 7365 6c66 2e66 6f72 6365  e'] = self.force
+00010480: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00010490: 2e72 6567 696f 6e5f 6964 2069 7320 6e6f  .region_id is no
+000104a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000104b0: 2020 2020 7265 7375 6c74 5b27 5265 6769      result['Regi
+000104c0: 6f6e 4964 275d 203d 2073 656c 662e 7265  onId'] = self.re
+000104d0: 6769 6f6e 5f69 640a 2020 2020 2020 2020  gion_id.        
+000104e0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+000104f0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00010500: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00010510: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00010520: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00010530: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00010540: 2745 6949 6e73 7461 6e63 6549 6427 2920  'EiInstanceId') 
+00010550: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00010560: 2020 2020 2020 2020 2073 656c 662e 6569           self.ei
+00010570: 5f69 6e73 7461 6e63 655f 6964 203d 206d  _instance_id = m
+00010580: 2e67 6574 2827 4569 496e 7374 616e 6365  .get('EiInstance
+00010590: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+000105a0: 6d2e 6765 7428 2746 6f72 6365 2729 2069  m.get('Force') i
+000105b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000105c0: 2020 2020 2020 2020 7365 6c66 2e66 6f72          self.for
+000105d0: 6365 203d 206d 2e67 6574 2827 466f 7263  ce = m.get('Forc
+000105e0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+000105f0: 2e67 6574 2827 5265 6769 6f6e 4964 2729  .get('RegionId')
+00010600: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00010610: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00010620: 6567 696f 6e5f 6964 203d 206d 2e67 6574  egion_id = m.get
+00010630: 2827 5265 6769 6f6e 4964 2729 0a20 2020  ('RegionId').   
+00010640: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00010650: 0a0a 0a63 6c61 7373 2044 656c 6574 6545  ...class DeleteE
+00010660: 6169 7345 6952 6573 706f 6e73 6542 6f64  aisEiResponseBod
+00010670: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+00010680: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00010690: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000106a0: 2020 2020 2072 6571 7565 7374 5f69 643a       request_id:
+000106b0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000106c0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+000106d0: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
+000106e0: 7175 6573 745f 6964 0a0a 2020 2020 6465  quest_id..    de
+000106f0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00010700: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00010710: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00010720: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00010730: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00010740: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00010750: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00010760: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00010770: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00010780: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00010790: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+000107a0: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
+000107b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000107c0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000107d0: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
+000107e0: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
+000107f0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00010800: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00010810: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00010820: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+00010830: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00010840: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00010850: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+00010860: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00010870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010880: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
+00010890: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+000108a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000108b0: 7365 6c66 0a0a 0a63 6c61 7373 2044 656c  self...class Del
+000108c0: 6574 6545 6169 7345 6952 6573 706f 6e73  eteEaisEiRespons
+000108d0: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+000108e0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+000108f0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00010900: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
+00010910: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
+00010920: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
+00010930: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
+00010940: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
+00010950: 6479 3a20 4465 6c65 7465 4561 6973 4569  dy: DeleteEaisEi
+00010960: 5265 7370 6f6e 7365 426f 6479 203d 204e  ResponseBody = N
+00010970: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+00010980: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+00010990: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
+000109a0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+000109b0: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+000109c0: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
+000109d0: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
+000109e0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+000109f0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00010a00: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+00010a10: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
+00010a20: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
+00010a30: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+00010a40: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+00010a50: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
+00010a60: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
+00010a70: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+00010a80: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+00010a90: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
+00010aa0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00010ab0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
+00010ac0: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
+00010ad0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+00010ae0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00010af0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00010b00: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+00010b10: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00010b20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00010b30: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00010b40: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00010b50: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00010b60: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+00010b70: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00010b80: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00010b90: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+00010ba0: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+00010bb0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00010bc0: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+00010bd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00010be0: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+00010bf0: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+00010c00: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+00010c10: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+00010c20: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00010c30: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+00010c40: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+00010c50: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+00010c60: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00010c70: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00010c80: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+00010c90: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00010ca0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+00010cb0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00010cc0: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
+00010cd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00010ce0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+00010cf0: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
+00010d00: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
+00010d10: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
+00010d20: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
+00010d30: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00010d40: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00010d50: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
+00010d60: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
+00010d70: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
+00010d80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00010d90: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+00010da0: 656c 203d 2044 656c 6574 6545 6169 7345  el = DeleteEaisE
+00010db0: 6952 6573 706f 6e73 6542 6f64 7928 290a  iResponseBody().
+00010dc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010dd0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+00010de0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+00010df0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+00010e00: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00010e10: 7373 2044 6573 6372 6962 6545 6169 7352  ss DescribeEaisR
+00010e20: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+00010e30: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00010e40: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00010e50: 2c0a 2020 2020 2020 2020 656c 6173 7469  ,.        elasti
+00010e60: 635f 6163 6365 6c65 7261 7465 645f 696e  c_accelerated_in
+00010e70: 7374 616e 6365 5f69 6473 3a20 7374 7220  stance_ids: str 
+00010e80: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00010e90: 696e 7374 616e 6365 5f6e 616d 653a 2073  instance_name: s
+00010ea0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+00010eb0: 2020 2069 6e73 7461 6e63 655f 7479 7065     instance_type
+00010ec0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00010ed0: 2020 2020 2020 7061 6765 5f6e 756d 6265        page_numbe
+00010ee0: 723a 2069 6e74 203d 204e 6f6e 652c 0a20  r: int = None,. 
+00010ef0: 2020 2020 2020 2070 6167 655f 7369 7a65         page_size
+00010f00: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+00010f10: 2020 2020 2020 7265 6769 6f6e 5f69 643a        region_id:
+00010f20: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00010f30: 2020 2020 2072 6573 6f75 7263 655f 6772       resource_gr
+00010f40: 6f75 705f 6964 3a20 7374 7220 3d20 4e6f  oup_id: str = No
+00010f50: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+00010f60: 7573 3a20 7374 7220 3d20 4e6f 6e65 2c0a  us: str = None,.
+00010f70: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00010f80: 656c 662e 656c 6173 7469 635f 6163 6365  elf.elastic_acce
+00010f90: 6c65 7261 7465 645f 696e 7374 616e 6365  lerated_instance
+00010fa0: 5f69 6473 203d 2065 6c61 7374 6963 5f61  _ids = elastic_a
+00010fb0: 6363 656c 6572 6174 6564 5f69 6e73 7461  ccelerated_insta
+00010fc0: 6e63 655f 6964 730a 2020 2020 2020 2020  nce_ids.        
+00010fd0: 7365 6c66 2e69 6e73 7461 6e63 655f 6e61  self.instance_na
+00010fe0: 6d65 203d 2069 6e73 7461 6e63 655f 6e61  me = instance_na
+00010ff0: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
+00011000: 696e 7374 616e 6365 5f74 7970 6520 3d20  instance_type = 
+00011010: 696e 7374 616e 6365 5f74 7970 650a 2020  instance_type.  
+00011020: 2020 2020 2020 7365 6c66 2e70 6167 655f        self.page_
+00011030: 6e75 6d62 6572 203d 2070 6167 655f 6e75  number = page_nu
+00011040: 6d62 6572 0a20 2020 2020 2020 2073 656c  mber.        sel
+00011050: 662e 7061 6765 5f73 697a 6520 3d20 7061  f.page_size = pa
+00011060: 6765 5f73 697a 650a 2020 2020 2020 2020  ge_size.        
+00011070: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
+00011080: 2072 6567 696f 6e5f 6964 0a20 2020 2020   region_id.     
+00011090: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
+000110a0: 5f67 726f 7570 5f69 6420 3d20 7265 736f  _group_id = reso
+000110b0: 7572 6365 5f67 726f 7570 5f69 640a 2020  urce_group_id.  
+000110c0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+000110d0: 7320 3d20 7374 6174 7573 0a0a 2020 2020  s = status..    
+000110e0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+000110f0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00011100: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00011110: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00011120: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+00011130: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00011140: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00011150: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00011160: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00011170: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00011180: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00011190: 2073 656c 662e 656c 6173 7469 635f 6163   self.elastic_ac
+000111a0: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+000111b0: 6365 5f69 6473 2069 7320 6e6f 7420 4e6f  ce_ids is not No
+000111c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000111d0: 7265 7375 6c74 5b27 456c 6173 7469 6341  result['ElasticA
+000111e0: 6363 656c 6572 6174 6564 496e 7374 616e  cceleratedInstan
+000111f0: 6365 4964 7327 5d20 3d20 7365 6c66 2e65  ceIds'] = self.e
+00011200: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+00011210: 6564 5f69 6e73 7461 6e63 655f 6964 730a  ed_instance_ids.
+00011220: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011230: 696e 7374 616e 6365 5f6e 616d 6520 6973  instance_name is
+00011240: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00011250: 2020 2020 2020 2072 6573 756c 745b 2749         result['I
+00011260: 6e73 7461 6e63 654e 616d 6527 5d20 3d20  nstanceName'] = 
+00011270: 7365 6c66 2e69 6e73 7461 6e63 655f 6e61  self.instance_na
+00011280: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
+00011290: 6c66 2e69 6e73 7461 6e63 655f 7479 7065  lf.instance_type
+000112a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000112b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000112c0: 5b27 496e 7374 616e 6365 5479 7065 275d  ['InstanceType']
+000112d0: 203d 2073 656c 662e 696e 7374 616e 6365   = self.instance
+000112e0: 5f74 7970 650a 2020 2020 2020 2020 6966  _type.        if
+000112f0: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
+00011300: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+00011310: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00011320: 745b 2750 6167 654e 756d 6265 7227 5d20  t['PageNumber'] 
+00011330: 3d20 7365 6c66 2e70 6167 655f 6e75 6d62  = self.page_numb
+00011340: 6572 0a20 2020 2020 2020 2069 6620 7365  er.        if se
+00011350: 6c66 2e70 6167 655f 7369 7a65 2069 7320  lf.page_size is 
+00011360: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00011370: 2020 2020 2020 7265 7375 6c74 5b27 5061        result['Pa
+00011380: 6765 5369 7a65 275d 203d 2073 656c 662e  geSize'] = self.
+00011390: 7061 6765 5f73 697a 650a 2020 2020 2020  page_size.      
+000113a0: 2020 6966 2073 656c 662e 7265 6769 6f6e    if self.region
+000113b0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+000113c0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000113d0: 756c 745b 2752 6567 696f 6e49 6427 5d20  ult['RegionId'] 
+000113e0: 3d20 7365 6c66 2e72 6567 696f 6e5f 6964  = self.region_id
+000113f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00011400: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
+00011410: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00011420: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00011430: 6c74 5b27 5265 736f 7572 6365 4772 6f75  lt['ResourceGrou
+00011440: 7049 6427 5d20 3d20 7365 6c66 2e72 6573  pId'] = self.res
+00011450: 6f75 7263 655f 6772 6f75 705f 6964 0a20  ource_group_id. 
+00011460: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00011470: 7461 7475 7320 6973 206e 6f74 204e 6f6e  tatus is not Non
+00011480: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00011490: 6573 756c 745b 2753 7461 7475 7327 5d20  esult['Status'] 
+000114a0: 3d20 7365 6c66 2e73 7461 7475 730a 2020  = self.status.  
+000114b0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+000114c0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+000114d0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+000114e0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+000114f0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00011500: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00011510: 6d2e 6765 7428 2745 6c61 7374 6963 4163  m.get('ElasticAc
+00011520: 6365 6c65 7261 7465 6449 6e73 7461 6e63  celeratedInstanc
+00011530: 6549 6473 2729 2069 7320 6e6f 7420 4e6f  eIds') is not No
+00011540: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00011550: 7365 6c66 2e65 6c61 7374 6963 5f61 6363  self.elastic_acc
+00011560: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
+00011570: 655f 6964 7320 3d20 6d2e 6765 7428 2745  e_ids = m.get('E
+00011580: 6c61 7374 6963 4163 6365 6c65 7261 7465  lasticAccelerate
+00011590: 6449 6e73 7461 6e63 6549 6473 2729 0a20  dInstanceIds'). 
+000115a0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000115b0: 2749 6e73 7461 6e63 654e 616d 6527 2920  'InstanceName') 
+000115c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000115d0: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
+000115e0: 7374 616e 6365 5f6e 616d 6520 3d20 6d2e  stance_name = m.
+000115f0: 6765 7428 2749 6e73 7461 6e63 654e 616d  get('InstanceNam
+00011600: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00011610: 2e67 6574 2827 496e 7374 616e 6365 5479  .get('InstanceTy
+00011620: 7065 2729 2069 7320 6e6f 7420 4e6f 6e65  pe') is not None
+00011630: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00011640: 6c66 2e69 6e73 7461 6e63 655f 7479 7065  lf.instance_type
+00011650: 203d 206d 2e67 6574 2827 496e 7374 616e   = m.get('Instan
+00011660: 6365 5479 7065 2729 0a20 2020 2020 2020  ceType').       
+00011670: 2069 6620 6d2e 6765 7428 2750 6167 654e   if m.get('PageN
+00011680: 756d 6265 7227 2920 6973 206e 6f74 204e  umber') is not N
+00011690: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000116a0: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
+000116b0: 7220 3d20 6d2e 6765 7428 2750 6167 654e  r = m.get('PageN
+000116c0: 756d 6265 7227 290a 2020 2020 2020 2020  umber').        
+000116d0: 6966 206d 2e67 6574 2827 5061 6765 5369  if m.get('PageSi
+000116e0: 7a65 2729 2069 7320 6e6f 7420 4e6f 6e65  ze') is not None
+000116f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00011700: 6c66 2e70 6167 655f 7369 7a65 203d 206d  lf.page_size = m
+00011710: 2e67 6574 2827 5061 6765 5369 7a65 2729  .get('PageSize')
+00011720: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00011730: 7428 2752 6567 696f 6e49 6427 2920 6973  t('RegionId') is
+00011740: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00011750: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
+00011760: 6f6e 5f69 6420 3d20 6d2e 6765 7428 2752  on_id = m.get('R
+00011770: 6567 696f 6e49 6427 290a 2020 2020 2020  egionId').      
+00011780: 2020 6966 206d 2e67 6574 2827 5265 736f    if m.get('Reso
+00011790: 7572 6365 4772 6f75 7049 6427 2920 6973  urceGroupId') is
+000117a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000117b0: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
+000117c0: 7572 6365 5f67 726f 7570 5f69 6420 3d20  urce_group_id = 
+000117d0: 6d2e 6765 7428 2752 6573 6f75 7263 6547  m.get('ResourceG
+000117e0: 726f 7570 4964 2729 0a20 2020 2020 2020  roupId').       
+000117f0: 2069 6620 6d2e 6765 7428 2753 7461 7475   if m.get('Statu
+00011800: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00011810: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011820: 662e 7374 6174 7573 203d 206d 2e67 6574  f.status = m.get
+00011830: 2827 5374 6174 7573 2729 0a20 2020 2020  ('Status').     
+00011840: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00011850: 0a63 6c61 7373 2044 6573 6372 6962 6545  .class DescribeE
+00011860: 6169 7352 6573 706f 6e73 6542 6f64 7949  aisResponseBodyI
+00011870: 6e73 7461 6e63 6573 496e 7374 616e 6365  nstancesInstance
+00011880: 5461 6773 5461 6728 5465 614d 6f64 656c  TagsTag(TeaModel
+00011890: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+000118a0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000118b0: 662c 0a20 2020 2020 2020 2074 6167 5f6b  f,.        tag_k
+000118c0: 6579 3a20 7374 7220 3d20 4e6f 6e65 2c0a  ey: str = None,.
+000118d0: 2020 2020 2020 2020 7461 675f 7661 6c75          tag_valu
+000118e0: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+000118f0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+00011900: 6c66 2e74 6167 5f6b 6579 203d 2074 6167  lf.tag_key = tag
+00011910: 5f6b 6579 0a20 2020 2020 2020 2073 656c  _key.        sel
+00011920: 662e 7461 675f 7661 6c75 6520 3d20 7461  f.tag_value = ta
+00011930: 675f 7661 6c75 650a 0a20 2020 2064 6566  g_value..    def
+00011940: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00011950: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00011960: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00011970: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00011980: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+00011990: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+000119a0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+000119b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000119c0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+000119d0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+000119e0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+000119f0: 6c66 2e74 6167 5f6b 6579 2069 7320 6e6f  lf.tag_key is no
+00011a00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00011a10: 2020 2020 7265 7375 6c74 5b27 5461 674b      result['TagK
+00011a20: 6579 275d 203d 2073 656c 662e 7461 675f  ey'] = self.tag_
+00011a30: 6b65 790a 2020 2020 2020 2020 6966 2073  key.        if s
+00011a40: 656c 662e 7461 675f 7661 6c75 6520 6973  elf.tag_value is
+00011a50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00011a60: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
+00011a70: 6167 5661 6c75 6527 5d20 3d20 7365 6c66  agValue'] = self
+00011a80: 2e74 6167 5f76 616c 7565 0a20 2020 2020  .tag_value.     
+00011a90: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00011aa0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00011ab0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+00011ac0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00011ad0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+00011ae0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00011af0: 6574 2827 5461 674b 6579 2729 2069 7320  et('TagKey') is 
+00011b00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00011b10: 2020 2020 2020 7365 6c66 2e74 6167 5f6b        self.tag_k
+00011b20: 6579 203d 206d 2e67 6574 2827 5461 674b  ey = m.get('TagK
+00011b30: 6579 2729 0a20 2020 2020 2020 2069 6620  ey').        if 
+00011b40: 6d2e 6765 7428 2754 6167 5661 6c75 6527  m.get('TagValue'
+00011b50: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00011b60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011b70: 7461 675f 7661 6c75 6520 3d20 6d2e 6765  tag_value = m.ge
+00011b80: 7428 2754 6167 5661 6c75 6527 290a 2020  t('TagValue').  
+00011b90: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00011ba0: 660a 0a0a 636c 6173 7320 4465 7363 7269  f...class Descri
+00011bb0: 6265 4561 6973 5265 7370 6f6e 7365 426f  beEaisResponseBo
+00011bc0: 6479 496e 7374 616e 6365 7349 6e73 7461  dyInstancesInsta
+00011bd0: 6e63 6554 6167 7328 5465 614d 6f64 656c  nceTags(TeaModel
+00011be0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00011bf0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00011c00: 662c 0a20 2020 2020 2020 2074 6167 3a20  f,.        tag: 
+00011c10: 4c69 7374 5b44 6573 6372 6962 6545 6169  List[DescribeEai
+00011c20: 7352 6573 706f 6e73 6542 6f64 7949 6e73  sResponseBodyIns
+00011c30: 7461 6e63 6573 496e 7374 616e 6365 5461  tancesInstanceTa
+00011c40: 6773 5461 675d 203d 204e 6f6e 652c 0a20  gsTag] = None,. 
+00011c50: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+00011c60: 6c66 2e74 6167 203d 2074 6167 0a0a 2020  lf.tag = tag..  
+00011c70: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00011c80: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+00011c90: 2073 656c 662e 7461 673a 0a20 2020 2020   self.tag:.     
+00011ca0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00011cb0: 7365 6c66 2e74 6167 3a0a 2020 2020 2020  self.tag:.      
+00011cc0: 2020 2020 2020 2020 2020 6966 206b 3a0a            if k:.
+00011cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ce0: 2020 2020 6b2e 7661 6c69 6461 7465 2829      k.validate()
+00011cf0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00011d00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00011d10: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+00011d20: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00011d30: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00011d40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00011d50: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00011d60: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00011d70: 6963 7428 290a 2020 2020 2020 2020 7265  ict().        re
+00011d80: 7375 6c74 5b27 5461 6727 5d20 3d20 5b5d  sult['Tag'] = []
+00011d90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00011da0: 2e74 6167 2069 7320 6e6f 7420 4e6f 6e65  .tag is not None
+00011db0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00011dc0: 7220 6b20 696e 2073 656c 662e 7461 673a  r k in self.tag:
+00011dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011de0: 2072 6573 756c 745b 2754 6167 275d 2e61   result['Tag'].a
+00011df0: 7070 656e 6428 6b2e 746f 5f6d 6170 2829  ppend(k.to_map()
+00011e00: 2069 6620 6b20 656c 7365 204e 6f6e 6529   if k else None)
+00011e10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011e20: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00011e30: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00011e40: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+00011e50: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00011e60: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00011e70: 7365 6c66 2e74 6167 203d 205b 5d0a 2020  self.tag = [].  
+00011e80: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00011e90: 5461 6727 2920 6973 206e 6f74 204e 6f6e  Tag') is not Non
+00011ea0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+00011eb0: 6f72 206b 2069 6e20 6d2e 6765 7428 2754  or k in m.get('T
+00011ec0: 6167 2729 3a0a 2020 2020 2020 2020 2020  ag'):.          
+00011ed0: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00011ee0: 203d 2044 6573 6372 6962 6545 6169 7352   = DescribeEaisR
+00011ef0: 6573 706f 6e73 6542 6f64 7949 6e73 7461  esponseBodyInsta
+00011f00: 6e63 6573 496e 7374 616e 6365 5461 6773  ncesInstanceTags
+00011f10: 5461 6728 290a 2020 2020 2020 2020 2020  Tag().          
+00011f20: 2020 2020 2020 7365 6c66 2e74 6167 2e61        self.tag.a
+00011f30: 7070 656e 6428 7465 6d70 5f6d 6f64 656c  ppend(temp_model
+00011f40: 2e66 726f 6d5f 6d61 7028 6b29 290a 2020  .from_map(k)).  
+00011f50: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00011f60: 660a 0a0a 636c 6173 7320 4465 7363 7269  f...class Descri
+00011f70: 6265 4561 6973 5265 7370 6f6e 7365 426f  beEaisResponseBo
+00011f80: 6479 496e 7374 616e 6365 7349 6e73 7461  dyInstancesInsta
+00011f90: 6e63 6528 5465 614d 6f64 656c 293a 0a20  nce(TeaModel):. 
+00011fa0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00011fb0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00011fc0: 2020 2020 2020 2063 6174 6567 6f72 793a         category:
+00011fd0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00011fe0: 2020 2020 2063 6c69 656e 745f 696e 7374       client_inst
+00011ff0: 616e 6365 5f69 643a 2073 7472 203d 204e  ance_id: str = N
+00012000: 6f6e 652c 0a20 2020 2020 2020 2063 6c69  one,.        cli
+00012010: 656e 745f 696e 7374 616e 6365 5f6e 616d  ent_instance_nam
+00012020: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+00012030: 2020 2020 2020 2063 6c69 656e 745f 696e         client_in
+00012040: 7374 616e 6365 5f74 7970 653a 2073 7472  stance_type: str
+00012050: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00012060: 2063 7265 6174 696f 6e5f 7469 6d65 3a20   creation_time: 
+00012070: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00012080: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00012090: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+000120a0: 2020 2020 2065 6c61 7374 6963 5f61 6363       elastic_acc
+000120b0: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
+000120c0: 655f 6964 3a20 7374 7220 3d20 4e6f 6e65  e_id: str = None
+000120d0: 2c0a 2020 2020 2020 2020 696e 7374 616e  ,.        instan
+000120e0: 6365 5f6e 616d 653a 2073 7472 203d 204e  ce_name: str = N
+000120f0: 6f6e 652c 0a20 2020 2020 2020 2069 6e73  one,.        ins
+00012100: 7461 6e63 655f 7479 7065 3a20 7374 7220  tance_type: str 
+00012110: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00012120: 6a75 7079 7465 725f 7572 6c3a 2073 7472  jupyter_url: str
+00012130: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00012140: 2072 6567 696f 6e5f 6964 3a20 7374 7220   region_id: str 
+00012150: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00012160: 7265 736f 7572 6365 5f67 726f 7570 5f69  resource_group_i
+00012170: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+00012180: 2020 2020 2020 2073 6563 7572 6974 795f         security_
+00012190: 6772 6f75 705f 6964 3a20 7374 7220 3d20  group_id: str = 
+000121a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+000121b0: 6172 745f 7469 6d65 3a20 7374 7220 3d20  art_time: str = 
+000121c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+000121d0: 6174 7573 3a20 7374 7220 3d20 4e6f 6e65  atus: str = None
+000121e0: 2c0a 2020 2020 2020 2020 7461 6773 3a20  ,.        tags: 
+000121f0: 4465 7363 7269 6265 4561 6973 5265 7370  DescribeEaisResp
+00012200: 6f6e 7365 426f 6479 496e 7374 616e 6365  onseBodyInstance
+00012210: 7349 6e73 7461 6e63 6554 6167 7320 3d20  sInstanceTags = 
+00012220: 4e6f 6e65 2c0a 2020 2020 2020 2020 765f  None,.        v_
+00012230: 7377 6974 6368 5f69 643a 2073 7472 203d  switch_id: str =
+00012240: 204e 6f6e 652c 0a20 2020 2020 2020 207a   None,.        z
+00012250: 6f6e 655f 6964 3a20 7374 7220 3d20 4e6f  one_id: str = No
+00012260: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+00012270: 2020 2073 656c 662e 6361 7465 676f 7279     self.category
+00012280: 203d 2063 6174 6567 6f72 790a 2020 2020   = category.    
+00012290: 2020 2020 7365 6c66 2e63 6c69 656e 745f      self.client_
+000122a0: 696e 7374 616e 6365 5f69 6420 3d20 636c  instance_id = cl
+000122b0: 6965 6e74 5f69 6e73 7461 6e63 655f 6964  ient_instance_id
+000122c0: 0a20 2020 2020 2020 2073 656c 662e 636c  .        self.cl
+000122d0: 6965 6e74 5f69 6e73 7461 6e63 655f 6e61  ient_instance_na
+000122e0: 6d65 203d 2063 6c69 656e 745f 696e 7374  me = client_inst
+000122f0: 616e 6365 5f6e 616d 650a 2020 2020 2020  ance_name.      
+00012300: 2020 7365 6c66 2e63 6c69 656e 745f 696e    self.client_in
+00012310: 7374 616e 6365 5f74 7970 6520 3d20 636c  stance_type = cl
+00012320: 6965 6e74 5f69 6e73 7461 6e63 655f 7479  ient_instance_ty
+00012330: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
+00012340: 6372 6561 7469 6f6e 5f74 696d 6520 3d20  creation_time = 
+00012350: 6372 6561 7469 6f6e 5f74 696d 650a 2020  creation_time.  
+00012360: 2020 2020 2020 7365 6c66 2e64 6573 6372        self.descr
+00012370: 6970 7469 6f6e 203d 2064 6573 6372 6970  iption = descrip
+00012380: 7469 6f6e 0a20 2020 2020 2020 2073 656c  tion.        sel
+00012390: 662e 656c 6173 7469 635f 6163 6365 6c65  f.elastic_accele
+000123a0: 7261 7465 645f 696e 7374 616e 6365 5f69  rated_instance_i
+000123b0: 6420 3d20 656c 6173 7469 635f 6163 6365  d = elastic_acce
+000123c0: 6c65 7261 7465 645f 696e 7374 616e 6365  lerated_instance
+000123d0: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+000123e0: 2e69 6e73 7461 6e63 655f 6e61 6d65 203d  .instance_name =
+000123f0: 2069 6e73 7461 6e63 655f 6e61 6d65 0a20   instance_name. 
+00012400: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
+00012410: 616e 6365 5f74 7970 6520 3d20 696e 7374  ance_type = inst
+00012420: 616e 6365 5f74 7970 650a 2020 2020 2020  ance_type.      
+00012430: 2020 7365 6c66 2e6a 7570 7974 6572 5f75    self.jupyter_u
+00012440: 726c 203d 206a 7570 7974 6572 5f75 726c  rl = jupyter_url
+00012450: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00012460: 6769 6f6e 5f69 6420 3d20 7265 6769 6f6e  gion_id = region
+00012470: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+00012480: 2e72 6573 6f75 7263 655f 6772 6f75 705f  .resource_group_
+00012490: 6964 203d 2072 6573 6f75 7263 655f 6772  id = resource_gr
+000124a0: 6f75 705f 6964 0a20 2020 2020 2020 2073  oup_id.        s
+000124b0: 656c 662e 7365 6375 7269 7479 5f67 726f  elf.security_gro
+000124c0: 7570 5f69 6420 3d20 7365 6375 7269 7479  up_id = security
+000124d0: 5f67 726f 7570 5f69 640a 2020 2020 2020  _group_id.      
+000124e0: 2020 7365 6c66 2e73 7461 7274 5f74 696d    self.start_tim
+000124f0: 6520 3d20 7374 6172 745f 7469 6d65 0a20  e = start_time. 
+00012500: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00012510: 7573 203d 2073 7461 7475 730a 2020 2020  us = status.    
+00012520: 2020 2020 7365 6c66 2e74 6167 7320 3d20      self.tags = 
+00012530: 7461 6773 0a20 2020 2020 2020 2073 656c  tags.        sel
+00012540: 662e 765f 7377 6974 6368 5f69 6420 3d20  f.v_switch_id = 
+00012550: 765f 7377 6974 6368 5f69 640a 2020 2020  v_switch_id.    
+00012560: 2020 2020 7365 6c66 2e7a 6f6e 655f 6964      self.zone_id
+00012570: 203d 207a 6f6e 655f 6964 0a0a 2020 2020   = zone_id..    
+00012580: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00012590: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
+000125a0: 656c 662e 7461 6773 3a0a 2020 2020 2020  elf.tags:.      
+000125b0: 2020 2020 2020 7365 6c66 2e74 6167 732e        self.tags.
+000125c0: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+000125d0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+000125e0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+000125f0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00012600: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00012610: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00012620: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00012630: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00012640: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00012650: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00012660: 6361 7465 676f 7279 2069 7320 6e6f 7420  category is not 
+00012670: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00012680: 2020 7265 7375 6c74 5b27 4361 7465 676f    result['Catego
+00012690: 7279 275d 203d 2073 656c 662e 6361 7465  ry'] = self.cate
+000126a0: 676f 7279 0a20 2020 2020 2020 2069 6620  gory.        if 
+000126b0: 7365 6c66 2e63 6c69 656e 745f 696e 7374  self.client_inst
+000126c0: 616e 6365 5f69 6420 6973 206e 6f74 204e  ance_id is not N
+000126d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000126e0: 2072 6573 756c 745b 2743 6c69 656e 7449   result['ClientI
+000126f0: 6e73 7461 6e63 6549 6427 5d20 3d20 7365  nstanceId'] = se
+00012700: 6c66 2e63 6c69 656e 745f 696e 7374 616e  lf.client_instan
+00012710: 6365 5f69 640a 2020 2020 2020 2020 6966  ce_id.        if
+00012720: 2073 656c 662e 636c 6965 6e74 5f69 6e73   self.client_ins
+00012730: 7461 6e63 655f 6e61 6d65 2069 7320 6e6f  tance_name is no
+00012740: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00012750: 2020 2020 7265 7375 6c74 5b27 436c 6965      result['Clie
+00012760: 6e74 496e 7374 616e 6365 4e61 6d65 275d  ntInstanceName']
+00012770: 203d 2073 656c 662e 636c 6965 6e74 5f69   = self.client_i
+00012780: 6e73 7461 6e63 655f 6e61 6d65 0a20 2020  nstance_name.   
+00012790: 2020 2020 2069 6620 7365 6c66 2e63 6c69       if self.cli
+000127a0: 656e 745f 696e 7374 616e 6365 5f74 7970  ent_instance_typ
+000127b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000127c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000127d0: 745b 2743 6c69 656e 7449 6e73 7461 6e63  t['ClientInstanc
+000127e0: 6554 7970 6527 5d20 3d20 7365 6c66 2e63  eType'] = self.c
+000127f0: 6c69 656e 745f 696e 7374 616e 6365 5f74  lient_instance_t
+00012800: 7970 650a 2020 2020 2020 2020 6966 2073  ype.        if s
+00012810: 656c 662e 6372 6561 7469 6f6e 5f74 696d  elf.creation_tim
+00012820: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00012830: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00012840: 745b 2743 7265 6174 696f 6e54 696d 6527  t['CreationTime'
+00012850: 5d20 3d20 7365 6c66 2e63 7265 6174 696f  ] = self.creatio
+00012860: 6e5f 7469 6d65 0a20 2020 2020 2020 2069  n_time.        i
+00012870: 6620 7365 6c66 2e64 6573 6372 6970 7469  f self.descripti
+00012880: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0a  on is not None:.
+00012890: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000128a0: 6c74 5b27 4465 7363 7269 7074 696f 6e27  lt['Description'
+000128b0: 5d20 3d20 7365 6c66 2e64 6573 6372 6970  ] = self.descrip
+000128c0: 7469 6f6e 0a20 2020 2020 2020 2069 6620  tion.        if 
+000128d0: 7365 6c66 2e65 6c61 7374 6963 5f61 6363  self.elastic_acc
+000128e0: 656c 6572 6174 6564 5f69 6e73 7461 6e63  elerated_instanc
+000128f0: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+00012900: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00012910: 7375 6c74 5b27 456c 6173 7469 6341 6363  sult['ElasticAcc
+00012920: 656c 6572 6174 6564 496e 7374 616e 6365  eleratedInstance
+00012930: 4964 275d 203d 2073 656c 662e 656c 6173  Id'] = self.elas
+00012940: 7469 635f 6163 6365 6c65 7261 7465 645f  tic_accelerated_
+00012950: 696e 7374 616e 6365 5f69 640a 2020 2020  instance_id.    
+00012960: 2020 2020 6966 2073 656c 662e 696e 7374      if self.inst
+00012970: 616e 6365 5f6e 616d 6520 6973 206e 6f74  ance_name is not
+00012980: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00012990: 2020 2072 6573 756c 745b 2749 6e73 7461     result['Insta
+000129a0: 6e63 654e 616d 6527 5d20 3d20 7365 6c66  nceName'] = self
+000129b0: 2e69 6e73 7461 6e63 655f 6e61 6d65 0a20  .instance_name. 
+000129c0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+000129d0: 6e73 7461 6e63 655f 7479 7065 2069 7320  nstance_type is 
+000129e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000129f0: 2020 2020 2020 7265 7375 6c74 5b27 496e        result['In
+00012a00: 7374 616e 6365 5479 7065 275d 203d 2073  stanceType'] = s
+00012a10: 656c 662e 696e 7374 616e 6365 5f74 7970  elf.instance_typ
+00012a20: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00012a30: 662e 6a75 7079 7465 725f 7572 6c20 6973  f.jupyter_url is
+00012a40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00012a50: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
+00012a60: 7570 7974 6572 5572 6c27 5d20 3d20 7365  upyterUrl'] = se
+00012a70: 6c66 2e6a 7570 7974 6572 5f75 726c 0a20  lf.jupyter_url. 
+00012a80: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00012a90: 6567 696f 6e5f 6964 2069 7320 6e6f 7420  egion_id is not 
+00012aa0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00012ab0: 2020 7265 7375 6c74 5b27 5265 6769 6f6e    result['Region
+00012ac0: 4964 275d 203d 2073 656c 662e 7265 6769  Id'] = self.regi
+00012ad0: 6f6e 5f69 640a 2020 2020 2020 2020 6966  on_id.        if
+00012ae0: 2073 656c 662e 7265 736f 7572 6365 5f67   self.resource_g
+00012af0: 726f 7570 5f69 6420 6973 206e 6f74 204e  roup_id is not N
+00012b00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00012b10: 2072 6573 756c 745b 2752 6573 6f75 7263   result['Resourc
+00012b20: 6547 726f 7570 4964 275d 203d 2073 656c  eGroupId'] = sel
+00012b30: 662e 7265 736f 7572 6365 5f67 726f 7570  f.resource_group
+00012b40: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00012b50: 656c 662e 7365 6375 7269 7479 5f67 726f  elf.security_gro
+00012b60: 7570 5f69 6420 6973 206e 6f74 204e 6f6e  up_id is not Non
+00012b70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00012b80: 6573 756c 745b 2753 6563 7572 6974 7947  esult['SecurityG
+00012b90: 726f 7570 4964 275d 203d 2073 656c 662e  roupId'] = self.
+00012ba0: 7365 6375 7269 7479 5f67 726f 7570 5f69  security_group_i
+00012bb0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+00012bc0: 662e 7374 6172 745f 7469 6d65 2069 7320  f.start_time is 
+00012bd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00012be0: 2020 2020 2020 7265 7375 6c74 5b27 5374        result['St
+00012bf0: 6172 7454 696d 6527 5d20 3d20 7365 6c66  artTime'] = self
+00012c00: 2e73 7461 7274 5f74 696d 650a 2020 2020  .start_time.    
+00012c10: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00012c20: 7573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  us is not None:.
+00012c30: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00012c40: 6c74 5b27 5374 6174 7573 275d 203d 2073  lt['Status'] = s
+00012c50: 656c 662e 7374 6174 7573 0a20 2020 2020  elf.status.     
+00012c60: 2020 2069 6620 7365 6c66 2e74 6167 7320     if self.tags 
+00012c70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00012c80: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00012c90: 2754 6167 7327 5d20 3d20 7365 6c66 2e74  'Tags'] = self.t
+00012ca0: 6167 732e 746f 5f6d 6170 2829 0a20 2020  ags.to_map().   
+00012cb0: 2020 2020 2069 6620 7365 6c66 2e76 5f73       if self.v_s
+00012cc0: 7769 7463 685f 6964 2069 7320 6e6f 7420  witch_id is not 
+00012cd0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00012ce0: 2020 7265 7375 6c74 5b27 5653 7769 7463    result['VSwitc
+00012cf0: 6849 6427 5d20 3d20 7365 6c66 2e76 5f73  hId'] = self.v_s
+00012d00: 7769 7463 685f 6964 0a20 2020 2020 2020  witch_id.       
+00012d10: 2069 6620 7365 6c66 2e7a 6f6e 655f 6964   if self.zone_id
+00012d20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00012d30: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00012d40: 5b27 5a6f 6e65 4964 275d 203d 2073 656c  ['ZoneId'] = sel
+00012d50: 662e 7a6f 6e65 5f69 640a 2020 2020 2020  f.zone_id.      
+00012d60: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00012d70: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00012d80: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+00012d90: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+00012da0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00012db0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00012dc0: 7428 2743 6174 6567 6f72 7927 2920 6973  t('Category') is
+00012dd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00012de0: 2020 2020 2020 2073 656c 662e 6361 7465         self.cate
+00012df0: 676f 7279 203d 206d 2e67 6574 2827 4361  gory = m.get('Ca
+00012e00: 7465 676f 7279 2729 0a20 2020 2020 2020  tegory').       
+00012e10: 2069 6620 6d2e 6765 7428 2743 6c69 656e   if m.get('Clien
+00012e20: 7449 6e73 7461 6e63 6549 6427 2920 6973  tInstanceId') is
+00012e30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00012e40: 2020 2020 2020 2073 656c 662e 636c 6965         self.clie
+00012e50: 6e74 5f69 6e73 7461 6e63 655f 6964 203d  nt_instance_id =
+00012e60: 206d 2e67 6574 2827 436c 6965 6e74 496e   m.get('ClientIn
+00012e70: 7374 616e 6365 4964 2729 0a20 2020 2020  stanceId').     
+00012e80: 2020 2069 6620 6d2e 6765 7428 2743 6c69     if m.get('Cli
+00012e90: 656e 7449 6e73 7461 6e63 654e 616d 6527  entInstanceName'
+00012ea0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00012eb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012ec0: 636c 6965 6e74 5f69 6e73 7461 6e63 655f  client_instance_
+00012ed0: 6e61 6d65 203d 206d 2e67 6574 2827 436c  name = m.get('Cl
+00012ee0: 6965 6e74 496e 7374 616e 6365 4e61 6d65  ientInstanceName
+00012ef0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00012f00: 6765 7428 2743 6c69 656e 7449 6e73 7461  get('ClientInsta
+00012f10: 6e63 6554 7970 6527 2920 6973 206e 6f74  nceType') is not
+00012f20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00012f30: 2020 2073 656c 662e 636c 6965 6e74 5f69     self.client_i
+00012f40: 6e73 7461 6e63 655f 7479 7065 203d 206d  nstance_type = m
+00012f50: 2e67 6574 2827 436c 6965 6e74 496e 7374  .get('ClientInst
+00012f60: 616e 6365 5479 7065 2729 0a20 2020 2020  anceType').     
+00012f70: 2020 2069 6620 6d2e 6765 7428 2743 7265     if m.get('Cre
+00012f80: 6174 696f 6e54 696d 6527 2920 6973 206e  ationTime') is n
+00012f90: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00012fa0: 2020 2020 2073 656c 662e 6372 6561 7469       self.creati
+00012fb0: 6f6e 5f74 696d 6520 3d20 6d2e 6765 7428  on_time = m.get(
+00012fc0: 2743 7265 6174 696f 6e54 696d 6527 290a  'CreationTime').
+00012fd0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00012fe0: 2827 4465 7363 7269 7074 696f 6e27 2920  ('Description') 
+00012ff0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00013000: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00013010: 7363 7269 7074 696f 6e20 3d20 6d2e 6765  scription = m.ge
+00013020: 7428 2744 6573 6372 6970 7469 6f6e 2729  t('Description')
+00013030: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00013040: 7428 2745 6c61 7374 6963 4163 6365 6c65  t('ElasticAccele
+00013050: 7261 7465 6449 6e73 7461 6e63 6549 6427  ratedInstanceId'
+00013060: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00013070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013080: 656c 6173 7469 635f 6163 6365 6c65 7261  elastic_accelera
+00013090: 7465 645f 696e 7374 616e 6365 5f69 6420  ted_instance_id 
+000130a0: 3d20 6d2e 6765 7428 2745 6c61 7374 6963  = m.get('Elastic
+000130b0: 4163 6365 6c65 7261 7465 6449 6e73 7461  AcceleratedInsta
+000130c0: 6e63 6549 6427 290a 2020 2020 2020 2020  nceId').        
+000130d0: 6966 206d 2e67 6574 2827 496e 7374 616e  if m.get('Instan
+000130e0: 6365 4e61 6d65 2729 2069 7320 6e6f 7420  ceName') is not 
+000130f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00013100: 2020 7365 6c66 2e69 6e73 7461 6e63 655f    self.instance_
+00013110: 6e61 6d65 203d 206d 2e67 6574 2827 496e  name = m.get('In
+00013120: 7374 616e 6365 4e61 6d65 2729 0a20 2020  stanceName').   
+00013130: 2020 2020 2069 6620 6d2e 6765 7428 2749       if m.get('I
+00013140: 6e73 7461 6e63 6554 7970 6527 2920 6973  nstanceType') is
+00013150: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00013160: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
+00013170: 616e 6365 5f74 7970 6520 3d20 6d2e 6765  ance_type = m.ge
+00013180: 7428 2749 6e73 7461 6e63 6554 7970 6527  t('InstanceType'
+00013190: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000131a0: 6574 2827 4a75 7079 7465 7255 726c 2729  et('JupyterUrl')
+000131b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000131c0: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
+000131d0: 7570 7974 6572 5f75 726c 203d 206d 2e67  upyter_url = m.g
+000131e0: 6574 2827 4a75 7079 7465 7255 726c 2729  et('JupyterUrl')
+000131f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00013200: 7428 2752 6567 696f 6e49 6427 2920 6973  t('RegionId') is
+00013210: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00013220: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
+00013230: 6f6e 5f69 6420 3d20 6d2e 6765 7428 2752  on_id = m.get('R
+00013240: 6567 696f 6e49 6427 290a 2020 2020 2020  egionId').      
+00013250: 2020 6966 206d 2e67 6574 2827 5265 736f    if m.get('Reso
+00013260: 7572 6365 4772 6f75 7049 6427 2920 6973  urceGroupId') is
+00013270: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00013280: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
+00013290: 7572 6365 5f67 726f 7570 5f69 6420 3d20  urce_group_id = 
+000132a0: 6d2e 6765 7428 2752 6573 6f75 7263 6547  m.get('ResourceG
+000132b0: 726f 7570 4964 2729 0a20 2020 2020 2020  roupId').       
+000132c0: 2069 6620 6d2e 6765 7428 2753 6563 7572   if m.get('Secur
+000132d0: 6974 7947 726f 7570 4964 2729 2069 7320  ityGroupId') is 
+000132e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000132f0: 2020 2020 2020 7365 6c66 2e73 6563 7572        self.secur
+00013300: 6974 795f 6772 6f75 705f 6964 203d 206d  ity_group_id = m
+00013310: 2e67 6574 2827 5365 6375 7269 7479 4772  .get('SecurityGr
+00013320: 6f75 7049 6427 290a 2020 2020 2020 2020  oupId').        
+00013330: 6966 206d 2e67 6574 2827 5374 6172 7454  if m.get('StartT
+00013340: 696d 6527 2920 6973 206e 6f74 204e 6f6e  ime') is not Non
+00013350: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00013360: 656c 662e 7374 6172 745f 7469 6d65 203d  elf.start_time =
+00013370: 206d 2e67 6574 2827 5374 6172 7454 696d   m.get('StartTim
+00013380: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00013390: 2e67 6574 2827 5374 6174 7573 2729 2069  .get('Status') i
+000133a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000133b0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+000133c0: 7475 7320 3d20 6d2e 6765 7428 2753 7461  tus = m.get('Sta
+000133d0: 7475 7327 290a 2020 2020 2020 2020 6966  tus').        if
+000133e0: 206d 2e67 6574 2827 5461 6773 2729 2069   m.get('Tags') i
+000133f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00013400: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+00013410: 656c 203d 2044 6573 6372 6962 6545 6169  el = DescribeEai
+00013420: 7352 6573 706f 6e73 6542 6f64 7949 6e73  sResponseBodyIns
+00013430: 7461 6e63 6573 496e 7374 616e 6365 5461  tancesInstanceTa
+00013440: 6773 2829 0a20 2020 2020 2020 2020 2020  gs().           
+00013450: 2073 656c 662e 7461 6773 203d 2074 656d   self.tags = tem
+00013460: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00013470: 286d 5b27 5461 6773 275d 290a 2020 2020  (m['Tags']).    
+00013480: 2020 2020 6966 206d 2e67 6574 2827 5653      if m.get('VS
+00013490: 7769 7463 6849 6427 2920 6973 206e 6f74  witchId') is not
+000134a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000134b0: 2020 2073 656c 662e 765f 7377 6974 6368     self.v_switch
+000134c0: 5f69 6420 3d20 6d2e 6765 7428 2756 5377  _id = m.get('VSw
+000134d0: 6974 6368 4964 2729 0a20 2020 2020 2020  itchId').       
+000134e0: 2069 6620 6d2e 6765 7428 275a 6f6e 6549   if m.get('ZoneI
+000134f0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00013500: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013510: 662e 7a6f 6e65 5f69 6420 3d20 6d2e 6765  f.zone_id = m.ge
+00013520: 7428 275a 6f6e 6549 6427 290a 2020 2020  t('ZoneId').    
+00013530: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00013540: 0a0a 636c 6173 7320 4465 7363 7269 6265  ..class Describe
+00013550: 4561 6973 5265 7370 6f6e 7365 426f 6479  EaisResponseBody
+00013560: 496e 7374 616e 6365 7328 5465 614d 6f64  Instances(TeaMod
+00013570: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00013580: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00013590: 656c 662c 0a20 2020 2020 2020 2069 6e73  elf,.        ins
+000135a0: 7461 6e63 653a 204c 6973 745b 4465 7363  tance: List[Desc
+000135b0: 7269 6265 4561 6973 5265 7370 6f6e 7365  ribeEaisResponse
+000135c0: 426f 6479 496e 7374 616e 6365 7349 6e73  BodyInstancesIns
+000135d0: 7461 6e63 655d 203d 204e 6f6e 652c 0a20  tance] = None,. 
+000135e0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+000135f0: 6c66 2e69 6e73 7461 6e63 6520 3d20 696e  lf.instance = in
+00013600: 7374 616e 6365 0a0a 2020 2020 6465 6620  stance..    def 
+00013610: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00013620: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00013630: 696e 7374 616e 6365 3a0a 2020 2020 2020  instance:.      
+00013640: 2020 2020 2020 666f 7220 6b20 696e 2073        for k in s
+00013650: 656c 662e 696e 7374 616e 6365 3a0a 2020  elf.instance:.  
+00013660: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00013670: 206b 3a0a 2020 2020 2020 2020 2020 2020   k:.            
+00013680: 2020 2020 2020 2020 6b2e 7661 6c69 6461          k.valida
+00013690: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+000136a0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+000136b0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+000136c0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+000136d0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+000136e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000136f0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00013700: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00013710: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00013720: 2020 7265 7375 6c74 5b27 496e 7374 616e    result['Instan
+00013730: 6365 275d 203d 205b 5d0a 2020 2020 2020  ce'] = [].      
+00013740: 2020 6966 2073 656c 662e 696e 7374 616e    if self.instan
+00013750: 6365 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ce is not None:.
+00013760: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00013770: 6b20 696e 2073 656c 662e 696e 7374 616e  k in self.instan
+00013780: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
+00013790: 2020 2020 7265 7375 6c74 5b27 496e 7374      result['Inst
+000137a0: 616e 6365 275d 2e61 7070 656e 6428 6b2e  ance'].append(k.
+000137b0: 746f 5f6d 6170 2829 2069 6620 6b20 656c  to_map() if k el
+000137c0: 7365 204e 6f6e 6529 0a20 2020 2020 2020  se None).       
+000137d0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000137e0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000137f0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00013800: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00013810: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00013820: 2020 2020 2020 2020 7365 6c66 2e69 6e73          self.ins
+00013830: 7461 6e63 6520 3d20 5b5d 0a20 2020 2020  tance = [].     
+00013840: 2020 2069 6620 6d2e 6765 7428 2749 6e73     if m.get('Ins
+00013850: 7461 6e63 6527 2920 6973 206e 6f74 204e  tance') is not N
+00013860: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013870: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
+00013880: 2749 6e73 7461 6e63 6527 293a 0a20 2020  'Instance'):.   
+00013890: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+000138a0: 705f 6d6f 6465 6c20 3d20 4465 7363 7269  p_model = Descri
+000138b0: 6265 4561 6973 5265 7370 6f6e 7365 426f  beEaisResponseBo
+000138c0: 6479 496e 7374 616e 6365 7349 6e73 7461  dyInstancesInsta
+000138d0: 6e63 6528 290a 2020 2020 2020 2020 2020  nce().          
+000138e0: 2020 2020 2020 7365 6c66 2e69 6e73 7461        self.insta
+000138f0: 6e63 652e 6170 7065 6e64 2874 656d 705f  nce.append(temp_
+00013900: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286b  model.from_map(k
+00013910: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
+00013920: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2044  n self...class D
+00013930: 6573 6372 6962 6545 6169 7352 6573 706f  escribeEaisRespo
+00013940: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
+00013950: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00013960: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00013970: 662c 0a20 2020 2020 2020 2069 6e73 7461  f,.        insta
+00013980: 6e63 6573 3a20 4465 7363 7269 6265 4561  nces: DescribeEa
+00013990: 6973 5265 7370 6f6e 7365 426f 6479 496e  isResponseBodyIn
+000139a0: 7374 616e 6365 7320 3d20 4e6f 6e65 2c0a  stances = None,.
+000139b0: 2020 2020 2020 2020 7061 6765 5f6e 756d          page_num
+000139c0: 6265 723a 2069 6e74 203d 204e 6f6e 652c  ber: int = None,
+000139d0: 0a20 2020 2020 2020 2070 6167 655f 7369  .        page_si
+000139e0: 7a65 3a20 696e 7420 3d20 4e6f 6e65 2c0a  ze: int = None,.
+000139f0: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+00013a00: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+00013a10: 2020 2020 2020 2020 746f 7461 6c5f 636f          total_co
+00013a20: 756e 743a 2069 6e74 203d 204e 6f6e 652c  unt: int = None,
+00013a30: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00013a40: 7365 6c66 2e69 6e73 7461 6e63 6573 203d  self.instances =
+00013a50: 2069 6e73 7461 6e63 6573 0a20 2020 2020   instances.     
+00013a60: 2020 2073 656c 662e 7061 6765 5f6e 756d     self.page_num
+00013a70: 6265 7220 3d20 7061 6765 5f6e 756d 6265  ber = page_numbe
+00013a80: 720a 2020 2020 2020 2020 7365 6c66 2e70  r.        self.p
+00013a90: 6167 655f 7369 7a65 203d 2070 6167 655f  age_size = page_
+00013aa0: 7369 7a65 0a20 2020 2020 2020 2073 656c  size.        sel
+00013ab0: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
+00013ac0: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
+00013ad0: 2020 7365 6c66 2e74 6f74 616c 5f63 6f75    self.total_cou
+00013ae0: 6e74 203d 2074 6f74 616c 5f63 6f75 6e74  nt = total_count
+00013af0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00013b00: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00013b10: 2020 6966 2073 656c 662e 696e 7374 616e    if self.instan
+00013b20: 6365 733a 0a20 2020 2020 2020 2020 2020  ces:.           
+00013b30: 2073 656c 662e 696e 7374 616e 6365 732e   self.instances.
+00013b40: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+00013b50: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00013b60: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00013b70: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00013b80: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00013b90: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00013ba0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00013bb0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00013bc0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00013bd0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00013be0: 696e 7374 616e 6365 7320 6973 206e 6f74  instances is not
+00013bf0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00013c00: 2020 2072 6573 756c 745b 2749 6e73 7461     result['Insta
+00013c10: 6e63 6573 275d 203d 2073 656c 662e 696e  nces'] = self.in
+00013c20: 7374 616e 6365 732e 746f 5f6d 6170 2829  stances.to_map()
+00013c30: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00013c40: 2e70 6167 655f 6e75 6d62 6572 2069 7320  .page_number is 
+00013c50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00013c60: 2020 2020 2020 7265 7375 6c74 5b27 5061        result['Pa
+00013c70: 6765 4e75 6d62 6572 275d 203d 2073 656c  geNumber'] = sel
+00013c80: 662e 7061 6765 5f6e 756d 6265 720a 2020  f.page_number.  
+00013c90: 2020 2020 2020 6966 2073 656c 662e 7061        if self.pa
+00013ca0: 6765 5f73 697a 6520 6973 206e 6f74 204e  ge_size is not N
+00013cb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013cc0: 2072 6573 756c 745b 2750 6167 6553 697a   result['PageSiz
+00013cd0: 6527 5d20 3d20 7365 6c66 2e70 6167 655f  e'] = self.page_
+00013ce0: 7369 7a65 0a20 2020 2020 2020 2069 6620  size.        if 
+00013cf0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00013d00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00013d10: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00013d20: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+00013d30: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+00013d40: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00013d50: 6f74 616c 5f63 6f75 6e74 2069 7320 6e6f  otal_count is no
+00013d60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00013d70: 2020 2020 7265 7375 6c74 5b27 546f 7461      result['Tota
+00013d80: 6c43 6f75 6e74 275d 203d 2073 656c 662e  lCount'] = self.
+00013d90: 746f 7461 6c5f 636f 756e 740a 2020 2020  total_count.    
+00013da0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00013db0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+00013dc0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+00013dd0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+00013de0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00013df0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00013e00: 6765 7428 2749 6e73 7461 6e63 6573 2729  get('Instances')
+00013e10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00013e20: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+00013e30: 6f64 656c 203d 2044 6573 6372 6962 6545  odel = DescribeE
+00013e40: 6169 7352 6573 706f 6e73 6542 6f64 7949  aisResponseBodyI
+00013e50: 6e73 7461 6e63 6573 2829 0a20 2020 2020  nstances().     
+00013e60: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
+00013e70: 616e 6365 7320 3d20 7465 6d70 5f6d 6f64  ances = temp_mod
+00013e80: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2749  el.from_map(m['I
+00013e90: 6e73 7461 6e63 6573 275d 290a 2020 2020  nstances']).    
+00013ea0: 2020 2020 6966 206d 2e67 6574 2827 5061      if m.get('Pa
+00013eb0: 6765 4e75 6d62 6572 2729 2069 7320 6e6f  geNumber') is no
+00013ec0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00013ed0: 2020 2020 7365 6c66 2e70 6167 655f 6e75      self.page_nu
+00013ee0: 6d62 6572 203d 206d 2e67 6574 2827 5061  mber = m.get('Pa
+00013ef0: 6765 4e75 6d62 6572 2729 0a20 2020 2020  geNumber').     
+00013f00: 2020 2069 6620 6d2e 6765 7428 2750 6167     if m.get('Pag
+00013f10: 6553 697a 6527 2920 6973 206e 6f74 204e  eSize') is not N
+00013f20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013f30: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
+00013f40: 3d20 6d2e 6765 7428 2750 6167 6553 697a  = m.get('PageSiz
+00013f50: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00013f60: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+00013f70: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00013f80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013f90: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
+00013fa0: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
+00013fb0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00013fc0: 2827 546f 7461 6c43 6f75 6e74 2729 2069  ('TotalCount') i
+00013fd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00013fe0: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
+00013ff0: 616c 5f63 6f75 6e74 203d 206d 2e67 6574  al_count = m.get
+00014000: 2827 546f 7461 6c43 6f75 6e74 2729 0a20  ('TotalCount'). 
+00014010: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00014020: 6c66 0a0a 0a63 6c61 7373 2044 6573 6372  lf...class Descr
+00014030: 6962 6545 6169 7352 6573 706f 6e73 6528  ibeEaisResponse(
+00014040: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00014050: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00014060: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00014070: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
+00014080: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
+00014090: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
+000140a0: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
+000140b0: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
+000140c0: 3a20 4465 7363 7269 6265 4561 6973 5265  : DescribeEaisRe
+000140d0: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
+000140e0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000140f0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00014100: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
+00014110: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00014120: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
+00014130: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00014140: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
+00014150: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00014160: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
+00014170: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00014180: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
+00014190: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+000141a0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+000141b0: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
+000141c0: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
+000141d0: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
+000141e0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+000141f0: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
+00014200: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
+00014210: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00014220: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00014230: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00014240: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00014250: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00014260: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+00014270: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00014280: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00014290: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000142a0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+000142b0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000142c0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000142d0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+000142e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000142f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00014300: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+00014310: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+00014320: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00014330: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00014340: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00014350: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00014360: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00014370: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00014380: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00014390: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000143a0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+000143b0: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+000143c0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000143d0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000143e0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000143f0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00014400: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00014410: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00014420: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00014430: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+00014440: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00014450: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00014460: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+00014470: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+00014480: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00014490: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+000144a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000144b0: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+000144c0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+000144d0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+000144e0: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+000144f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00014500: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00014510: 203d 2044 6573 6372 6962 6545 6169 7352   = DescribeEaisR
+00014520: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
+00014530: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00014540: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+00014550: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+00014560: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+00014570: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00014580: 2044 6573 6372 6962 6552 6567 696f 6e73   DescribeRegions
+00014590: 5265 7370 6f6e 7365 426f 6479 5265 6769  ResponseBodyRegi
+000145a0: 6f6e 7352 6567 696f 6e28 5465 614d 6f64  onsRegion(TeaMod
+000145b0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000145c0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+000145d0: 656c 662c 0a20 2020 2020 2020 206c 6f63  elf,.        loc
+000145e0: 616c 5f6e 616d 653a 2073 7472 203d 204e  al_name: str = N
+000145f0: 6f6e 652c 0a20 2020 2020 2020 2072 6567  one,.        reg
+00014600: 696f 6e5f 656e 6470 6f69 6e74 3a20 7374  ion_endpoint: st
+00014610: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00014620: 2020 7265 6769 6f6e 5f69 643a 2073 7472    region_id: str
+00014630: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00014640: 2020 2020 2020 2020 7365 6c66 2e6c 6f63          self.loc
+00014650: 616c 5f6e 616d 6520 3d20 6c6f 6361 6c5f  al_name = local_
+00014660: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
+00014670: 662e 7265 6769 6f6e 5f65 6e64 706f 696e  f.region_endpoin
+00014680: 7420 3d20 7265 6769 6f6e 5f65 6e64 706f  t = region_endpo
+00014690: 696e 740a 2020 2020 2020 2020 7365 6c66  int.        self
+000146a0: 2e72 6567 696f 6e5f 6964 203d 2072 6567  .region_id = reg
+000146b0: 696f 6e5f 6964 0a0a 2020 2020 6465 6620  ion_id..    def 
+000146c0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000146d0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000146e0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000146f0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00014700: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+00014710: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00014720: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00014730: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00014740: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+00014750: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00014760: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00014770: 662e 6c6f 6361 6c5f 6e61 6d65 2069 7320  f.local_name is 
+00014780: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00014790: 2020 2020 2020 7265 7375 6c74 5b27 4c6f        result['Lo
+000147a0: 6361 6c4e 616d 6527 5d20 3d20 7365 6c66  calName'] = self
+000147b0: 2e6c 6f63 616c 5f6e 616d 650a 2020 2020  .local_name.    
+000147c0: 2020 2020 6966 2073 656c 662e 7265 6769      if self.regi
+000147d0: 6f6e 5f65 6e64 706f 696e 7420 6973 206e  on_endpoint is n
+000147e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000147f0: 2020 2020 2072 6573 756c 745b 2752 6567       result['Reg
+00014800: 696f 6e45 6e64 706f 696e 7427 5d20 3d20  ionEndpoint'] = 
+00014810: 7365 6c66 2e72 6567 696f 6e5f 656e 6470  self.region_endp
+00014820: 6f69 6e74 0a20 2020 2020 2020 2069 6620  oint.        if 
+00014830: 7365 6c66 2e72 6567 696f 6e5f 6964 2069  self.region_id i
+00014840: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00014850: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00014860: 5265 6769 6f6e 4964 275d 203d 2073 656c  RegionId'] = sel
+00014870: 662e 7265 6769 6f6e 5f69 640a 2020 2020  f.region_id.    
+00014880: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00014890: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+000148a0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+000148b0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+000148c0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+000148d0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+000148e0: 6765 7428 274c 6f63 616c 4e61 6d65 2729  get('LocalName')
+000148f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00014900: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00014910: 6f63 616c 5f6e 616d 6520 3d20 6d2e 6765  ocal_name = m.ge
+00014920: 7428 274c 6f63 616c 4e61 6d65 2729 0a20  t('LocalName'). 
+00014930: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00014940: 2752 6567 696f 6e45 6e64 706f 696e 7427  'RegionEndpoint'
+00014950: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00014960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014970: 7265 6769 6f6e 5f65 6e64 706f 696e 7420  region_endpoint 
+00014980: 3d20 6d2e 6765 7428 2752 6567 696f 6e45  = m.get('RegionE
+00014990: 6e64 706f 696e 7427 290a 2020 2020 2020  ndpoint').      
+000149a0: 2020 6966 206d 2e67 6574 2827 5265 6769    if m.get('Regi
+000149b0: 6f6e 4964 2729 2069 7320 6e6f 7420 4e6f  onId') is not No
+000149c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000149d0: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
+000149e0: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
+000149f0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+00014a00: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2044  n self...class D
+00014a10: 6573 6372 6962 6552 6567 696f 6e73 5265  escribeRegionsRe
+00014a20: 7370 6f6e 7365 426f 6479 5265 6769 6f6e  sponseBodyRegion
+00014a30: 7328 5465 614d 6f64 656c 293a 0a20 2020  s(TeaModel):.   
+00014a40: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00014a50: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00014a60: 2020 2020 2072 6567 696f 6e3a 204c 6973       region: Lis
+00014a70: 745b 4465 7363 7269 6265 5265 6769 6f6e  t[DescribeRegion
+00014a80: 7352 6573 706f 6e73 6542 6f64 7952 6567  sResponseBodyReg
+00014a90: 696f 6e73 5265 6769 6f6e 5d20 3d20 4e6f  ionsRegion] = No
+00014aa0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+00014ab0: 2020 2073 656c 662e 7265 6769 6f6e 203d     self.region =
+00014ac0: 2072 6567 696f 6e0a 0a20 2020 2064 6566   region..    def
+00014ad0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00014ae0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00014af0: 2e72 6567 696f 6e3a 0a20 2020 2020 2020  .region:.       
+00014b00: 2020 2020 2066 6f72 206b 2069 6e20 7365       for k in se
+00014b10: 6c66 2e72 6567 696f 6e3a 0a20 2020 2020  lf.region:.     
+00014b20: 2020 2020 2020 2020 2020 2069 6620 6b3a             if k:
+00014b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014b40: 2020 2020 206b 2e76 616c 6964 6174 6528       k.validate(
+00014b50: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+00014b60: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00014b70: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+00014b80: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00014b90: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00014ba0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00014bb0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00014bc0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00014bd0: 6469 6374 2829 0a20 2020 2020 2020 2072  dict().        r
+00014be0: 6573 756c 745b 2752 6567 696f 6e27 5d20  esult['Region'] 
+00014bf0: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
+00014c00: 7365 6c66 2e72 6567 696f 6e20 6973 206e  self.region is n
+00014c10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00014c20: 2020 2020 2066 6f72 206b 2069 6e20 7365       for k in se
+00014c30: 6c66 2e72 6567 696f 6e3a 0a20 2020 2020  lf.region:.     
+00014c40: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00014c50: 745b 2752 6567 696f 6e27 5d2e 6170 7065  t['Region'].appe
+00014c60: 6e64 286b 2e74 6f5f 6d61 7028 2920 6966  nd(k.to_map() if
+00014c70: 206b 2065 6c73 6520 4e6f 6e65 290a 2020   k else None).  
+00014c80: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00014c90: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00014ca0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00014cb0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+00014cc0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00014cd0: 6374 2829 0a20 2020 2020 2020 2073 656c  ct().        sel
+00014ce0: 662e 7265 6769 6f6e 203d 205b 5d0a 2020  f.region = [].  
+00014cf0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00014d00: 5265 6769 6f6e 2729 2069 7320 6e6f 7420  Region') is not 
+00014d10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00014d20: 2020 666f 7220 6b20 696e 206d 2e67 6574    for k in m.get
+00014d30: 2827 5265 6769 6f6e 2729 3a0a 2020 2020  ('Region'):.    
+00014d40: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+00014d50: 5f6d 6f64 656c 203d 2044 6573 6372 6962  _model = Describ
+00014d60: 6552 6567 696f 6e73 5265 7370 6f6e 7365  eRegionsResponse
+00014d70: 426f 6479 5265 6769 6f6e 7352 6567 696f  BodyRegionsRegio
+00014d80: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
+00014d90: 2020 2020 7365 6c66 2e72 6567 696f 6e2e      self.region.
+00014da0: 6170 7065 6e64 2874 656d 705f 6d6f 6465  append(temp_mode
+00014db0: 6c2e 6672 6f6d 5f6d 6170 286b 2929 0a20  l.from_map(k)). 
+00014dc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00014dd0: 6c66 0a0a 0a63 6c61 7373 2044 6573 6372  lf...class Descr
+00014de0: 6962 6552 6567 696f 6e73 5265 7370 6f6e  ibeRegionsRespon
+00014df0: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
+00014e00: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00014e10: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00014e20: 2c0a 2020 2020 2020 2020 7265 6769 6f6e  ,.        region
+00014e30: 733a 2044 6573 6372 6962 6552 6567 696f  s: DescribeRegio
+00014e40: 6e73 5265 7370 6f6e 7365 426f 6479 5265  nsResponseBodyRe
+00014e50: 6769 6f6e 7320 3d20 4e6f 6e65 2c0a 2020  gions = None,.  
+00014e60: 2020 2020 2020 7265 7175 6573 745f 6964        request_id
+00014e70: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00014e80: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00014e90: 662e 7265 6769 6f6e 7320 3d20 7265 6769  f.regions = regi
+00014ea0: 6f6e 730a 2020 2020 2020 2020 7365 6c66  ons.        self
+00014eb0: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
+00014ec0: 7175 6573 745f 6964 0a0a 2020 2020 6465  quest_id..    de
+00014ed0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00014ee0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
+00014ef0: 662e 7265 6769 6f6e 733a 0a20 2020 2020  f.regions:.     
+00014f00: 2020 2020 2020 2073 656c 662e 7265 6769         self.regi
+00014f10: 6f6e 732e 7661 6c69 6461 7465 2829 0a0a  ons.validate()..
+00014f20: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00014f30: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00014f40: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00014f50: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00014f60: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00014f70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00014f80: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00014f90: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00014fa0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00014fb0: 656c 662e 7265 6769 6f6e 7320 6973 206e  elf.regions is n
+00014fc0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00014fd0: 2020 2020 2072 6573 756c 745b 2752 6567       result['Reg
+00014fe0: 696f 6e73 275d 203d 2073 656c 662e 7265  ions'] = self.re
+00014ff0: 6769 6f6e 732e 746f 5f6d 6170 2829 0a20  gions.to_map(). 
+00015000: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00015010: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
+00015020: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00015030: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
+00015040: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
+00015050: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+00015060: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00015070: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00015080: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00015090: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+000150a0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+000150b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000150c0: 2827 5265 6769 6f6e 7327 2920 6973 206e  ('Regions') is n
+000150d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000150e0: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+000150f0: 3d20 4465 7363 7269 6265 5265 6769 6f6e  = DescribeRegion
+00015100: 7352 6573 706f 6e73 6542 6f64 7952 6567  sResponseBodyReg
+00015110: 696f 6e73 2829 0a20 2020 2020 2020 2020  ions().         
+00015120: 2020 2073 656c 662e 7265 6769 6f6e 7320     self.regions 
+00015130: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+00015140: 6d5f 6d61 7028 6d5b 2752 6567 696f 6e73  m_map(m['Regions
+00015150: 275d 290a 2020 2020 2020 2020 6966 206d  ']).        if m
+00015160: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+00015170: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00015180: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015190: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
+000151a0: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
+000151b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000151c0: 656c 660a 0a0a 636c 6173 7320 4465 7363  elf...class Desc
+000151d0: 7269 6265 5265 6769 6f6e 7352 6573 706f  ribeRegionsRespo
+000151e0: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
+000151f0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00015200: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00015210: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
+00015220: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
+00015230: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+00015240: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
+00015250: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00015260: 626f 6479 3a20 4465 7363 7269 6265 5265  body: DescribeRe
+00015270: 6769 6f6e 7352 6573 706f 6e73 6542 6f64  gionsResponseBod
+00015280: 7920 3d20 4e6f 6e65 2c0a 2020 2020 293a  y = None,.    ):
+00015290: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+000152a0: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
+000152b0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+000152c0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+000152d0: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
+000152e0: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+000152f0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00015300: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00015310: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+00015320: 6571 7569 7265 6428 7365 6c66 2e68 6561  equired(self.hea
+00015330: 6465 7273 2c20 2768 6561 6465 7273 2729  ders, 'headers')
+00015340: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00015350: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+00015360: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00015370: 2c20 2773 7461 7475 735f 636f 6465 2729  , 'status_code')
+00015380: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00015390: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+000153a0: 7365 6c66 2e62 6f64 792c 2027 626f 6479  self.body, 'body
+000153b0: 2729 0a20 2020 2020 2020 2069 6620 7365  ').        if se
+000153c0: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+000153d0: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+000153e0: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+000153f0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00015400: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00015410: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+00015420: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00015430: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00015440: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00015450: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00015460: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00015470: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+00015480: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+00015490: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000154a0: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+000154b0: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+000154c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000154d0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+000154e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000154f0: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+00015500: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+00015510: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+00015520: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00015530: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+00015540: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00015550: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+00015560: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+00015570: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00015580: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00015590: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+000155a0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+000155b0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+000155c0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000155d0: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+000155e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000155f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015600: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+00015610: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+00015620: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+00015630: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+00015640: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00015650: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00015660: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+00015670: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+00015680: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+00015690: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+000156a0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+000156b0: 705f 6d6f 6465 6c20 3d20 4465 7363 7269  p_model = Descri
+000156c0: 6265 5265 6769 6f6e 7352 6573 706f 6e73  beRegionsRespons
+000156d0: 6542 6f64 7928 290a 2020 2020 2020 2020  eBody().        
+000156e0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+000156f0: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
+00015700: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
+00015710: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00015720: 6c66 0a0a 0a63 6c61 7373 2044 6574 6163  lf...class Detac
+00015730: 6845 6169 5265 7175 6573 7428 5465 614d  hEaiRequest(TeaM
+00015740: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00015750: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00015760: 2073 656c 662c 0a20 2020 2020 2020 2065   self,.        e
+00015770: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+00015780: 6564 5f69 6e73 7461 6e63 655f 6964 3a20  ed_instance_id: 
+00015790: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+000157a0: 2020 2020 7265 6769 6f6e 5f69 643a 2073      region_id: s
+000157b0: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+000157c0: 3a0a 2020 2020 2020 2020 7365 6c66 2e65  :.        self.e
+000157d0: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+000157e0: 6564 5f69 6e73 7461 6e63 655f 6964 203d  ed_instance_id =
+000157f0: 2065 6c61 7374 6963 5f61 6363 656c 6572   elastic_acceler
+00015800: 6174 6564 5f69 6e73 7461 6e63 655f 6964  ated_instance_id
+00015810: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00015820: 6769 6f6e 5f69 6420 3d20 7265 6769 6f6e  gion_id = region
+00015830: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
+00015840: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00015850: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00015860: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00015870: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00015880: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+00015890: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+000158a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000158b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000158c0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+000158d0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+000158e0: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+000158f0: 6c61 7374 6963 5f61 6363 656c 6572 6174  lastic_accelerat
+00015900: 6564 5f69 6e73 7461 6e63 655f 6964 2069  ed_instance_id i
+00015910: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00015920: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00015930: 456c 6173 7469 6341 6363 656c 6572 6174  ElasticAccelerat
+00015940: 6564 496e 7374 616e 6365 4964 275d 203d  edInstanceId'] =
+00015950: 2073 656c 662e 656c 6173 7469 635f 6163   self.elastic_ac
+00015960: 6365 6c65 7261 7465 645f 696e 7374 616e  celerated_instan
+00015970: 6365 5f69 640a 2020 2020 2020 2020 6966  ce_id.        if
+00015980: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+00015990: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000159a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000159b0: 2752 6567 696f 6e49 6427 5d20 3d20 7365  'RegionId'] = se
+000159c0: 6c66 2e72 6567 696f 6e5f 6964 0a20 2020  lf.region_id.   
+000159d0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000159e0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+000159f0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+00015a00: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+00015a10: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00015a20: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00015a30: 2e67 6574 2827 456c 6173 7469 6341 6363  .get('ElasticAcc
+00015a40: 656c 6572 6174 6564 496e 7374 616e 6365  eleratedInstance
+00015a50: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00015a60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00015a70: 6c66 2e65 6c61 7374 6963 5f61 6363 656c  lf.elastic_accel
+00015a80: 6572 6174 6564 5f69 6e73 7461 6e63 655f  erated_instance_
+00015a90: 6964 203d 206d 2e67 6574 2827 456c 6173  id = m.get('Elas
+00015aa0: 7469 6341 6363 656c 6572 6174 6564 496e  ticAcceleratedIn
+00015ab0: 7374 616e 6365 4964 2729 0a20 2020 2020  stanceId').     
+00015ac0: 2020 2069 6620 6d2e 6765 7428 2752 6567     if m.get('Reg
+00015ad0: 696f 6e49 6427 2920 6973 206e 6f74 204e  ionId') is not N
+00015ae0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00015af0: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+00015b00: 3d20 6d2e 6765 7428 2752 6567 696f 6e49  = m.get('RegionI
+00015b10: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
+00015b20: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00015b30: 4465 7461 6368 4561 6952 6573 706f 6e73  DetachEaiRespons
+00015b40: 6542 6f64 7928 5465 614d 6f64 656c 293a  eBody(TeaModel):
+00015b50: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00015b60: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00015b70: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+00015b80: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00015b90: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00015ba0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00015bb0: 3d20 7265 7175 6573 745f 6964 0a0a 2020  = request_id..  
+00015bc0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00015bd0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+00015be0: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+00015bf0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00015c00: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+00015c10: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00015c20: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00015c30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00015c40: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00015c50: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00015c60: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00015c70: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+00015c80: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00015c90: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00015ca0: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
+00015cb0: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
+00015cc0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+00015cd0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00015ce0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00015cf0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+00015d00: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00015d10: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00015d20: 2069 6620 6d2e 6765 7428 2752 6571 7565   if m.get('Reque
+00015d30: 7374 4964 2729 2069 7320 6e6f 7420 4e6f  stId') is not No
+00015d40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00015d50: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00015d60: 3d20 6d2e 6765 7428 2752 6571 7565 7374  = m.get('Request
+00015d70: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
+00015d80: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00015d90: 2044 6574 6163 6845 6169 5265 7370 6f6e   DetachEaiRespon
+00015da0: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+00015db0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00015dc0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00015dd0: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
+00015de0: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
+00015df0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+00015e00: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
+00015e10: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
+00015e20: 6f64 793a 2044 6574 6163 6845 6169 5265  ody: DetachEaiRe
+00015e30: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
+00015e40: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00015e50: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00015e60: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
+00015e70: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00015e80: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
+00015e90: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00015ea0: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
+00015eb0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00015ec0: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
+00015ed0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00015ee0: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
+00015ef0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+00015f00: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00015f10: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
+00015f20: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
+00015f30: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
+00015f40: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00015f50: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
+00015f60: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
+00015f70: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00015f80: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00015f90: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00015fa0: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00015fb0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00015fc0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+00015fd0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00015fe0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00015ff0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00016000: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00016010: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00016020: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00016030: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+00016040: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00016050: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00016060: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+00016070: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+00016080: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00016090: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+000160a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000160b0: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+000160c0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+000160d0: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+000160e0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+000160f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00016100: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+00016110: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+00016120: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00016130: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00016140: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00016150: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00016160: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00016170: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00016180: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00016190: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+000161a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000161b0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+000161c0: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+000161d0: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+000161e0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+000161f0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00016200: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00016210: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00016220: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00016230: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00016240: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+00016250: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00016260: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00016270: 203d 2044 6574 6163 6845 6169 5265 7370   = DetachEaiResp
+00016280: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+00016290: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+000162a0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+000162b0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+000162c0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000162d0: 2073 656c 660a 0a0a 636c 6173 7320 4465   self...class De
+000162e0: 7461 6368 4561 6973 4569 5265 7175 6573  tachEaisEiReques
+000162f0: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+00016300: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00016310: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00016320: 2020 2020 2065 695f 696e 7374 616e 6365       ei_instance
+00016330: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00016340: 0a20 2020 2020 2020 2072 6567 696f 6e5f  .        region_
+00016350: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+00016360: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00016370: 656c 662e 6569 5f69 6e73 7461 6e63 655f  elf.ei_instance_
+00016380: 6964 203d 2065 695f 696e 7374 616e 6365  id = ei_instance
+00016390: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+000163a0: 2e72 6567 696f 6e5f 6964 203d 2072 6567  .region_id = reg
+000163b0: 696f 6e5f 6964 0a0a 2020 2020 6465 6620  ion_id..    def 
+000163c0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+000163d0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000163e0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+000163f0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00016400: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+00016410: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00016420: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00016430: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00016440: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+00016450: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00016460: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00016470: 662e 6569 5f69 6e73 7461 6e63 655f 6964  f.ei_instance_id
+00016480: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00016490: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000164a0: 5b27 4569 496e 7374 616e 6365 4964 275d  ['EiInstanceId']
+000164b0: 203d 2073 656c 662e 6569 5f69 6e73 7461   = self.ei_insta
+000164c0: 6e63 655f 6964 0a20 2020 2020 2020 2069  nce_id.        i
+000164d0: 6620 7365 6c66 2e72 6567 696f 6e5f 6964  f self.region_id
+000164e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000164f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00016500: 5b27 5265 6769 6f6e 4964 275d 203d 2073  ['RegionId'] = s
+00016510: 656c 662e 7265 6769 6f6e 5f69 640a 2020  elf.region_id.  
+00016520: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00016530: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00016540: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00016550: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+00016560: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00016570: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00016580: 6d2e 6765 7428 2745 6949 6e73 7461 6e63  m.get('EiInstanc
+00016590: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+000165a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000165b0: 656c 662e 6569 5f69 6e73 7461 6e63 655f  elf.ei_instance_
+000165c0: 6964 203d 206d 2e67 6574 2827 4569 496e  id = m.get('EiIn
+000165d0: 7374 616e 6365 4964 2729 0a20 2020 2020  stanceId').     
+000165e0: 2020 2069 6620 6d2e 6765 7428 2752 6567     if m.get('Reg
+000165f0: 696f 6e49 6427 2920 6973 206e 6f74 204e  ionId') is not N
+00016600: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00016610: 2073 656c 662e 7265 6769 6f6e 5f69 6420   self.region_id 
+00016620: 3d20 6d2e 6765 7428 2752 6567 696f 6e49  = m.get('RegionI
+00016630: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
+00016640: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00016650: 4465 7461 6368 4561 6973 4569 5265 7370  DetachEaisEiResp
+00016660: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
+00016670: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00016680: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00016690: 6c66 2c0a 2020 2020 2020 2020 7265 7175  lf,.        requ
+000166a0: 6573 745f 6964 3a20 7374 7220 3d20 4e6f  est_id: str = No
+000166b0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000166c0: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+000166d0: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
+000166e0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000166f0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00016700: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+00016710: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00016720: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00016730: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00016740: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00016750: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00016760: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00016770: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00016780: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00016790: 2020 2069 6620 7365 6c66 2e72 6571 7565     if self.reque
+000167a0: 7374 5f69 6420 6973 206e 6f74 204e 6f6e  st_id is not Non
+000167b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000167c0: 6573 756c 745b 2752 6571 7565 7374 4964  esult['RequestId
+000167d0: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
+000167e0: 745f 6964 0a20 2020 2020 2020 2072 6574  t_id.        ret
+000167f0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00016800: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00016810: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+00016820: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00016830: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00016840: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+00016850: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
+00016860: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00016870: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+00016880: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
+00016890: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
+000168a0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+000168b0: 6173 7320 4465 7461 6368 4561 6973 4569  ass DetachEaisEi
+000168c0: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
+000168d0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+000168e0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+000168f0: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
+00016900: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
+00016910: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00016920: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
+00016930: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+00016940: 2020 2020 2062 6f64 793a 2044 6574 6163       body: Detac
+00016950: 6845 6169 7345 6952 6573 706f 6e73 6542  hEaisEiResponseB
+00016960: 6f64 7920 3d20 4e6f 6e65 2c0a 2020 2020  ody = None,.    
+00016970: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00016980: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+00016990: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+000169a0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+000169b0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+000169c0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+000169d0: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+000169e0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+000169f0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+00016a00: 5f72 6571 7569 7265 6428 7365 6c66 2e68  _required(self.h
+00016a10: 6561 6465 7273 2c20 2768 6561 6465 7273  eaders, 'headers
+00016a20: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+00016a30: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+00016a40: 6428 7365 6c66 2e73 7461 7475 735f 636f  d(self.status_co
+00016a50: 6465 2c20 2773 7461 7475 735f 636f 6465  de, 'status_code
+00016a60: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+00016a70: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+00016a80: 6428 7365 6c66 2e62 6f64 792c 2027 626f  d(self.body, 'bo
+00016a90: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
+00016aa0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+00016ab0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+00016ac0: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+00016ad0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+00016ae0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+00016af0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+00016b00: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00016b10: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00016b20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00016b30: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00016b40: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00016b50: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00016b60: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+00016b70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00016b80: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+00016b90: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+00016ba0: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+00016bb0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+00016bc0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00016bd0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00016be0: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+00016bf0: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+00016c00: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00016c10: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+00016c20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00016c30: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+00016c40: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+00016c50: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00016c60: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00016c70: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00016c80: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+00016c90: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00016ca0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00016cb0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+00016cc0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+00016cd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00016ce0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+00016cf0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+00016d00: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00016d10: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+00016d20: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00016d30: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00016d40: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+00016d50: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+00016d60: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+00016d70: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+00016d80: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+00016d90: 656d 705f 6d6f 6465 6c20 3d20 4465 7461  emp_model = Deta
+00016da0: 6368 4561 6973 4569 5265 7370 6f6e 7365  chEaisEiResponse
+00016db0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
+00016dc0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+00016dd0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+00016de0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+00016df0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00016e00: 660a 0a0a 636c 6173 7320 4765 7449 6e73  f...class GetIns
+00016e10: 7461 6e63 654d 6574 7269 6373 5265 7175  tanceMetricsRequ
+00016e20: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+00016e30: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00016e40: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00016e50: 2020 2020 2020 2065 6e64 5f74 696d 653a         end_time:
+00016e60: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00016e70: 2020 2020 2069 6e73 7461 6e63 655f 6964       instance_id
+00016e80: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00016e90: 2020 2020 2020 6d65 7472 6963 5f74 7970        metric_typ
+00016ea0: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+00016eb0: 2020 2020 2020 2072 6567 696f 6e5f 6964         region_id
+00016ec0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00016ed0: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
+00016ee0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00016ef0: 2020 2020 2020 7469 6d65 5f73 7465 703a        time_step:
+00016f00: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00016f10: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+00016f20: 2e65 6e64 5f74 696d 6520 3d20 656e 645f  .end_time = end_
+00016f30: 7469 6d65 0a20 2020 2020 2020 2073 656c  time.        sel
+00016f40: 662e 696e 7374 616e 6365 5f69 6420 3d20  f.instance_id = 
+00016f50: 696e 7374 616e 6365 5f69 640a 2020 2020  instance_id.    
+00016f60: 2020 2020 7365 6c66 2e6d 6574 7269 635f      self.metric_
+00016f70: 7479 7065 203d 206d 6574 7269 635f 7479  type = metric_ty
+00016f80: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
+00016f90: 7265 6769 6f6e 5f69 6420 3d20 7265 6769  region_id = regi
+00016fa0: 6f6e 5f69 640a 2020 2020 2020 2020 7365  on_id.        se
+00016fb0: 6c66 2e73 7461 7274 5f74 696d 6520 3d20  lf.start_time = 
+00016fc0: 7374 6172 745f 7469 6d65 0a20 2020 2020  start_time.     
+00016fd0: 2020 2073 656c 662e 7469 6d65 5f73 7465     self.time_ste
+00016fe0: 7020 3d20 7469 6d65 5f73 7465 700a 0a20  p = time_step.. 
+00016ff0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+00017000: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+00017010: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+00017020: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00017030: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00017040: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00017050: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00017060: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00017070: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00017080: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00017090: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000170a0: 2069 6620 7365 6c66 2e65 6e64 5f74 696d   if self.end_tim
+000170b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000170c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000170d0: 745b 2745 6e64 5469 6d65 275d 203d 2073  t['EndTime'] = s
+000170e0: 656c 662e 656e 645f 7469 6d65 0a20 2020  elf.end_time.   
+000170f0: 2020 2020 2069 6620 7365 6c66 2e69 6e73       if self.ins
+00017100: 7461 6e63 655f 6964 2069 7320 6e6f 7420  tance_id is not 
+00017110: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00017120: 2020 7265 7375 6c74 5b27 496e 7374 616e    result['Instan
+00017130: 6365 4964 275d 203d 2073 656c 662e 696e  ceId'] = self.in
+00017140: 7374 616e 6365 5f69 640a 2020 2020 2020  stance_id.      
+00017150: 2020 6966 2073 656c 662e 6d65 7472 6963    if self.metric
+00017160: 5f74 7970 6520 6973 206e 6f74 204e 6f6e  _type is not Non
+00017170: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00017180: 6573 756c 745b 274d 6574 7269 6354 7970  esult['MetricTyp
+00017190: 6527 5d20 3d20 7365 6c66 2e6d 6574 7269  e'] = self.metri
+000171a0: 635f 7479 7065 0a20 2020 2020 2020 2069  c_type.        i
+000171b0: 6620 7365 6c66 2e72 6567 696f 6e5f 6964  f self.region_id
+000171c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000171d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000171e0: 5b27 5265 6769 6f6e 4964 275d 203d 2073  ['RegionId'] = s
+000171f0: 656c 662e 7265 6769 6f6e 5f69 640a 2020  elf.region_id.  
+00017200: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+00017210: 6172 745f 7469 6d65 2069 7320 6e6f 7420  art_time is not 
+00017220: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00017230: 2020 7265 7375 6c74 5b27 5374 6172 7454    result['StartT
+00017240: 696d 6527 5d20 3d20 7365 6c66 2e73 7461  ime'] = self.sta
+00017250: 7274 5f74 696d 650a 2020 2020 2020 2020  rt_time.        
+00017260: 6966 2073 656c 662e 7469 6d65 5f73 7465  if self.time_ste
+00017270: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00017280: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00017290: 745b 2754 696d 6553 7465 7027 5d20 3d20  t['TimeStep'] = 
+000172a0: 7365 6c66 2e74 696d 655f 7374 6570 0a20  self.time_step. 
+000172b0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000172c0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+000172d0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+000172e0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+000172f0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00017300: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00017310: 206d 2e67 6574 2827 456e 6454 696d 6527   m.get('EndTime'
+00017320: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00017330: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017340: 656e 645f 7469 6d65 203d 206d 2e67 6574  end_time = m.get
+00017350: 2827 456e 6454 696d 6527 290a 2020 2020  ('EndTime').    
+00017360: 2020 2020 6966 206d 2e67 6574 2827 496e      if m.get('In
+00017370: 7374 616e 6365 4964 2729 2069 7320 6e6f  stanceId') is no
+00017380: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00017390: 2020 2020 7365 6c66 2e69 6e73 7461 6e63      self.instanc
+000173a0: 655f 6964 203d 206d 2e67 6574 2827 496e  e_id = m.get('In
+000173b0: 7374 616e 6365 4964 2729 0a20 2020 2020  stanceId').     
+000173c0: 2020 2069 6620 6d2e 6765 7428 274d 6574     if m.get('Met
+000173d0: 7269 6354 7970 6527 2920 6973 206e 6f74  ricType') is not
+000173e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000173f0: 2020 2073 656c 662e 6d65 7472 6963 5f74     self.metric_t
+00017400: 7970 6520 3d20 6d2e 6765 7428 274d 6574  ype = m.get('Met
+00017410: 7269 6354 7970 6527 290a 2020 2020 2020  ricType').      
+00017420: 2020 6966 206d 2e67 6574 2827 5265 6769    if m.get('Regi
+00017430: 6f6e 4964 2729 2069 7320 6e6f 7420 4e6f  onId') is not No
+00017440: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00017450: 7365 6c66 2e72 6567 696f 6e5f 6964 203d  self.region_id =
+00017460: 206d 2e67 6574 2827 5265 6769 6f6e 4964   m.get('RegionId
+00017470: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00017480: 6765 7428 2753 7461 7274 5469 6d65 2729  get('StartTime')
+00017490: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000174a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000174b0: 7461 7274 5f74 696d 6520 3d20 6d2e 6765  tart_time = m.ge
+000174c0: 7428 2753 7461 7274 5469 6d65 2729 0a20  t('StartTime'). 
+000174d0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000174e0: 2754 696d 6553 7465 7027 2920 6973 206e  'TimeStep') is n
+000174f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00017500: 2020 2020 2073 656c 662e 7469 6d65 5f73       self.time_s
+00017510: 7465 7020 3d20 6d2e 6765 7428 2754 696d  tep = m.get('Tim
+00017520: 6553 7465 7027 290a 2020 2020 2020 2020  eStep').        
+00017530: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00017540: 6173 7320 4765 7449 6e73 7461 6e63 654d  ass GetInstanceM
+00017550: 6574 7269 6373 5265 7370 6f6e 7365 426f  etricsResponseBo
+00017560: 6479 506f 644d 6574 7269 6373 4d65 7472  dyPodMetricsMetr
+00017570: 6963 7328 5465 614d 6f64 656c 293a 0a20  ics(TeaModel):. 
+00017580: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00017590: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000175a0: 2020 2020 2020 2074 696d 653a 2073 7472         time: str
+000175b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000175c0: 2076 616c 7565 3a20 7374 7220 3d20 4e6f   value: str = No
+000175d0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000175e0: 2020 2073 656c 662e 7469 6d65 203d 2074     self.time = t
+000175f0: 696d 650a 2020 2020 2020 2020 7365 6c66  ime.        self
+00017600: 2e76 616c 7565 203d 2076 616c 7565 0a0a  .value = value..
+00017610: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00017620: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00017630: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+00017640: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00017650: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00017660: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+00017670: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00017680: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00017690: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+000176a0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+000176b0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+000176c0: 2020 6966 2073 656c 662e 7469 6d65 2069    if self.time i
+000176d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000176e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000176f0: 5469 6d65 275d 203d 2073 656c 662e 7469  Time'] = self.ti
+00017700: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
+00017710: 6c66 2e76 616c 7565 2069 7320 6e6f 7420  lf.value is not 
+00017720: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00017730: 2020 7265 7375 6c74 5b27 5661 6c75 6527    result['Value'
+00017740: 5d20 3d20 7365 6c66 2e76 616c 7565 0a20  ] = self.value. 
+00017750: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00017760: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00017770: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+00017780: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+00017790: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+000177a0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+000177b0: 206d 2e67 6574 2827 5469 6d65 2729 2069   m.get('Time') i
+000177c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000177d0: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+000177e0: 6520 3d20 6d2e 6765 7428 2754 696d 6527  e = m.get('Time'
+000177f0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00017800: 6574 2827 5661 6c75 6527 2920 6973 206e  et('Value') is n
+00017810: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00017820: 2020 2020 2073 656c 662e 7661 6c75 6520       self.value 
+00017830: 3d20 6d2e 6765 7428 2756 616c 7565 2729  = m.get('Value')
+00017840: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00017850: 7365 6c66 0a0a 0a63 6c61 7373 2047 6574  self...class Get
+00017860: 496e 7374 616e 6365 4d65 7472 6963 7352  InstanceMetricsR
+00017870: 6573 706f 6e73 6542 6f64 7950 6f64 4d65  esponseBodyPodMe
+00017880: 7472 6963 7328 5465 614d 6f64 656c 293a  trics(TeaModel):
+00017890: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000178a0: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+000178b0: 0a20 2020 2020 2020 206d 6574 7269 6373  .        metrics
+000178c0: 3a20 4c69 7374 5b47 6574 496e 7374 616e  : List[GetInstan
+000178d0: 6365 4d65 7472 6963 7352 6573 706f 6e73  ceMetricsRespons
+000178e0: 6542 6f64 7950 6f64 4d65 7472 6963 734d  eBodyPodMetricsM
+000178f0: 6574 7269 6373 5d20 3d20 4e6f 6e65 2c0a  etrics] = None,.
+00017900: 2020 2020 2020 2020 706f 645f 6964 3a20          pod_id: 
+00017910: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00017920: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00017930: 6d65 7472 6963 7320 3d20 6d65 7472 6963  metrics = metric
+00017940: 730a 2020 2020 2020 2020 2320 506f 6420  s.        # Pod 
+00017950: 4944 e380 820a 2020 2020 2020 2020 7365  ID....        se
+00017960: 6c66 2e70 6f64 5f69 6420 3d20 706f 645f  lf.pod_id = pod_
+00017970: 6964 0a0a 2020 2020 6465 6620 7661 6c69  id..    def vali
+00017980: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00017990: 2020 2020 6966 2073 656c 662e 6d65 7472      if self.metr
+000179a0: 6963 733a 0a20 2020 2020 2020 2020 2020  ics:.           
+000179b0: 2066 6f72 206b 2069 6e20 7365 6c66 2e6d   for k in self.m
+000179c0: 6574 7269 6373 3a0a 2020 2020 2020 2020  etrics:.        
+000179d0: 2020 2020 2020 2020 6966 206b 3a0a 2020          if k:.  
+000179e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179f0: 2020 6b2e 7661 6c69 6461 7465 2829 0a0a    k.validate()..
+00017a00: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00017a10: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00017a20: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+00017a30: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00017a40: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00017a50: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00017a60: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00017a70: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00017a80: 7428 290a 2020 2020 2020 2020 7265 7375  t().        resu
+00017a90: 6c74 5b27 4d65 7472 6963 7327 5d20 3d20  lt['Metrics'] = 
+00017aa0: 5b5d 0a20 2020 2020 2020 2069 6620 7365  [].        if se
+00017ab0: 6c66 2e6d 6574 7269 6373 2069 7320 6e6f  lf.metrics is no
+00017ac0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00017ad0: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
+00017ae0: 662e 6d65 7472 6963 733a 0a20 2020 2020  f.metrics:.     
+00017af0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00017b00: 745b 274d 6574 7269 6373 275d 2e61 7070  t['Metrics'].app
+00017b10: 656e 6428 6b2e 746f 5f6d 6170 2829 2069  end(k.to_map() i
+00017b20: 6620 6b20 656c 7365 204e 6f6e 6529 0a20  f k else None). 
+00017b30: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00017b40: 6f64 5f69 6420 6973 206e 6f74 204e 6f6e  od_id is not Non
+00017b50: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00017b60: 6573 756c 745b 2750 6f64 4964 275d 203d  esult['PodId'] =
+00017b70: 2073 656c 662e 706f 645f 6964 0a20 2020   self.pod_id.   
+00017b80: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00017b90: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00017ba0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+00017bb0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+00017bc0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00017bd0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+00017be0: 2e6d 6574 7269 6373 203d 205b 5d0a 2020  .metrics = [].  
+00017bf0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00017c00: 4d65 7472 6963 7327 2920 6973 206e 6f74  Metrics') is not
+00017c10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00017c20: 2020 2066 6f72 206b 2069 6e20 6d2e 6765     for k in m.ge
+00017c30: 7428 274d 6574 7269 6373 2729 3a0a 2020  t('Metrics'):.  
+00017c40: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00017c50: 6d70 5f6d 6f64 656c 203d 2047 6574 496e  mp_model = GetIn
+00017c60: 7374 616e 6365 4d65 7472 6963 7352 6573  stanceMetricsRes
+00017c70: 706f 6e73 6542 6f64 7950 6f64 4d65 7472  ponseBodyPodMetr
+00017c80: 6963 734d 6574 7269 6373 2829 0a20 2020  icsMetrics().   
+00017c90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017ca0: 662e 6d65 7472 6963 732e 6170 7065 6e64  f.metrics.append
+00017cb0: 2874 656d 705f 6d6f 6465 6c2e 6672 6f6d  (temp_model.from
+00017cc0: 5f6d 6170 286b 2929 0a20 2020 2020 2020  _map(k)).       
+00017cd0: 2069 6620 6d2e 6765 7428 2750 6f64 4964   if m.get('PodId
+00017ce0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00017cf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017d00: 2e70 6f64 5f69 6420 3d20 6d2e 6765 7428  .pod_id = m.get(
+00017d10: 2750 6f64 4964 2729 0a20 2020 2020 2020  'PodId').       
+00017d20: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00017d30: 6c61 7373 2047 6574 496e 7374 616e 6365  lass GetInstance
+00017d40: 4d65 7472 6963 7352 6573 706f 6e73 6542  MetricsResponseB
+00017d50: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
+00017d60: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00017d70: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00017d80: 2020 2020 2020 2069 6e73 7461 6e63 655f         instance_
+00017d90: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+00017da0: 2020 2020 2020 2020 706f 645f 6d65 7472          pod_metr
+00017db0: 6963 733a 204c 6973 745b 4765 7449 6e73  ics: List[GetIns
+00017dc0: 7461 6e63 654d 6574 7269 6373 5265 7370  tanceMetricsResp
+00017dd0: 6f6e 7365 426f 6479 506f 644d 6574 7269  onseBodyPodMetri
+00017de0: 6373 5d20 3d20 4e6f 6e65 2c0a 2020 2020  cs] = None,.    
+00017df0: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
+00017e00: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+00017e10: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00017e20: 696e 7374 616e 6365 5f69 6420 3d20 696e  instance_id = in
+00017e30: 7374 616e 6365 5f69 640a 2020 2020 2020  stance_id.      
+00017e40: 2020 7365 6c66 2e70 6f64 5f6d 6574 7269    self.pod_metri
+00017e50: 6373 203d 2070 6f64 5f6d 6574 7269 6373  cs = pod_metrics
+00017e60: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00017e70: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
+00017e80: 7374 5f69 640a 0a20 2020 2064 6566 2076  st_id..    def v
+00017e90: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00017ea0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00017eb0: 6f64 5f6d 6574 7269 6373 3a0a 2020 2020  od_metrics:.    
+00017ec0: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
+00017ed0: 2073 656c 662e 706f 645f 6d65 7472 6963   self.pod_metric
+00017ee0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00017ef0: 2020 2069 6620 6b3a 0a20 2020 2020 2020     if k:.       
+00017f00: 2020 2020 2020 2020 2020 2020 206b 2e76               k.v
+00017f10: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+00017f20: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00017f30: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00017f40: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+00017f50: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00017f60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00017f70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00017f80: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00017f90: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00017fa0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+00017fb0: 6e73 7461 6e63 655f 6964 2069 7320 6e6f  nstance_id is no
+00017fc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00017fd0: 2020 2020 7265 7375 6c74 5b27 496e 7374      result['Inst
+00017fe0: 616e 6365 4964 275d 203d 2073 656c 662e  anceId'] = self.
+00017ff0: 696e 7374 616e 6365 5f69 640a 2020 2020  instance_id.    
+00018000: 2020 2020 7265 7375 6c74 5b27 506f 644d      result['PodM
+00018010: 6574 7269 6373 275d 203d 205b 5d0a 2020  etrics'] = [].  
+00018020: 2020 2020 2020 6966 2073 656c 662e 706f        if self.po
+00018030: 645f 6d65 7472 6963 7320 6973 206e 6f74  d_metrics is not
+00018040: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00018050: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
+00018060: 2e70 6f64 5f6d 6574 7269 6373 3a0a 2020  .pod_metrics:.  
+00018070: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00018080: 7375 6c74 5b27 506f 644d 6574 7269 6373  sult['PodMetrics
+00018090: 275d 2e61 7070 656e 6428 6b2e 746f 5f6d  '].append(k.to_m
+000180a0: 6170 2829 2069 6620 6b20 656c 7365 204e  ap() if k else N
+000180b0: 6f6e 6529 0a20 2020 2020 2020 2069 6620  one).        if 
+000180c0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+000180d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000180e0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000180f0: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+00018100: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+00018110: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00018120: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00018130: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+00018140: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+00018150: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+00018160: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00018170: 206d 2e67 6574 2827 496e 7374 616e 6365   m.get('Instance
+00018180: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00018190: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000181a0: 6c66 2e69 6e73 7461 6e63 655f 6964 203d  lf.instance_id =
+000181b0: 206d 2e67 6574 2827 496e 7374 616e 6365   m.get('Instance
+000181c0: 4964 2729 0a20 2020 2020 2020 2073 656c  Id').        sel
+000181d0: 662e 706f 645f 6d65 7472 6963 7320 3d20  f.pod_metrics = 
+000181e0: 5b5d 0a20 2020 2020 2020 2069 6620 6d2e  [].        if m.
+000181f0: 6765 7428 2750 6f64 4d65 7472 6963 7327  get('PodMetrics'
+00018200: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00018210: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+00018220: 2069 6e20 6d2e 6765 7428 2750 6f64 4d65   in m.get('PodMe
+00018230: 7472 6963 7327 293a 0a20 2020 2020 2020  trics'):.       
+00018240: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+00018250: 6465 6c20 3d20 4765 7449 6e73 7461 6e63  del = GetInstanc
+00018260: 654d 6574 7269 6373 5265 7370 6f6e 7365  eMetricsResponse
+00018270: 426f 6479 506f 644d 6574 7269 6373 2829  BodyPodMetrics()
+00018280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018290: 2073 656c 662e 706f 645f 6d65 7472 6963   self.pod_metric
+000182a0: 732e 6170 7065 6e64 2874 656d 705f 6d6f  s.append(temp_mo
+000182b0: 6465 6c2e 6672 6f6d 5f6d 6170 286b 2929  del.from_map(k))
+000182c0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000182d0: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
+000182e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000182f0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+00018300: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
+00018310: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
+00018320: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00018330: 0a0a 0a63 6c61 7373 2047 6574 496e 7374  ...class GetInst
+00018340: 616e 6365 4d65 7472 6963 7352 6573 706f  anceMetricsRespo
+00018350: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
+00018360: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00018370: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00018380: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
+00018390: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
+000183a0: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+000183b0: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
+000183c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000183d0: 626f 6479 3a20 4765 7449 6e73 7461 6e63  body: GetInstanc
+000183e0: 654d 6574 7269 6373 5265 7370 6f6e 7365  eMetricsResponse
+000183f0: 426f 6479 203d 204e 6f6e 652c 0a20 2020  Body = None,.   
+00018400: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+00018410: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
+00018420: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
+00018430: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+00018440: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+00018450: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
+00018460: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
+00018470: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00018480: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+00018490: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+000184a0: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
+000184b0: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
+000184c0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+000184d0: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
+000184e0: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
+000184f0: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
+00018500: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+00018510: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
+00018520: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
+00018530: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+00018540: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00018550: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+00018560: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00018570: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00018580: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+00018590: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+000185a0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+000185b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000185c0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000185d0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000185e0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000185f0: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+00018600: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00018610: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+00018620: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+00018630: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+00018640: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00018650: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00018660: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00018670: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+00018680: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00018690: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000186a0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+000186b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000186c0: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+000186d0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+000186e0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+000186f0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00018700: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00018710: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+00018720: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00018730: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00018740: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+00018750: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+00018760: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00018770: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+00018780: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+00018790: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000187a0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+000187b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000187c0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000187d0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+000187e0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+000187f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00018800: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+00018810: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00018820: 7465 6d70 5f6d 6f64 656c 203d 2047 6574  temp_model = Get
+00018830: 496e 7374 616e 6365 4d65 7472 6963 7352  InstanceMetricsR
+00018840: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
+00018850: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00018860: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+00018870: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+00018880: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+00018890: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+000188a0: 2053 7461 7274 4561 6973 4569 5265 7175   StartEaisEiRequ
+000188b0: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+000188c0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000188d0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000188e0: 2020 2020 2020 2065 695f 696e 7374 616e         ei_instan
+000188f0: 6365 5f69 643a 2073 7472 203d 204e 6f6e  ce_id: str = Non
+00018900: 652c 0a20 2020 2020 2020 2072 6567 696f  e,.        regio
+00018910: 6e5f 6964 3a20 7374 7220 3d20 4e6f 6e65  n_id: str = None
+00018920: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00018930: 2073 656c 662e 6569 5f69 6e73 7461 6e63   self.ei_instanc
+00018940: 655f 6964 203d 2065 695f 696e 7374 616e  e_id = ei_instan
+00018950: 6365 5f69 640a 2020 2020 2020 2020 7365  ce_id.        se
+00018960: 6c66 2e72 6567 696f 6e5f 6964 203d 2072  lf.region_id = r
+00018970: 6567 696f 6e5f 6964 0a0a 2020 2020 6465  egion_id..    de
+00018980: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00018990: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+000189a0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+000189b0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000189c0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000189d0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000189e0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000189f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00018a00: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00018a10: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00018a20: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00018a30: 656c 662e 6569 5f69 6e73 7461 6e63 655f  elf.ei_instance_
+00018a40: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00018a50: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00018a60: 6c74 5b27 4569 496e 7374 616e 6365 4964  lt['EiInstanceId
+00018a70: 275d 203d 2073 656c 662e 6569 5f69 6e73  '] = self.ei_ins
+00018a80: 7461 6e63 655f 6964 0a20 2020 2020 2020  tance_id.       
+00018a90: 2069 6620 7365 6c66 2e72 6567 696f 6e5f   if self.region_
+00018aa0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00018ab0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00018ac0: 6c74 5b27 5265 6769 6f6e 4964 275d 203d  lt['RegionId'] =
+00018ad0: 2073 656c 662e 7265 6769 6f6e 5f69 640a   self.region_id.
+00018ae0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00018af0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00018b00: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00018b10: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00018b20: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00018b30: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00018b40: 6620 6d2e 6765 7428 2745 6949 6e73 7461  f m.get('EiInsta
+00018b50: 6e63 6549 6427 2920 6973 206e 6f74 204e  nceId') is not N
+00018b60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00018b70: 2073 656c 662e 6569 5f69 6e73 7461 6e63   self.ei_instanc
+00018b80: 655f 6964 203d 206d 2e67 6574 2827 4569  e_id = m.get('Ei
+00018b90: 496e 7374 616e 6365 4964 2729 0a20 2020  InstanceId').   
+00018ba0: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+00018bb0: 6567 696f 6e49 6427 2920 6973 206e 6f74  egionId') is not
+00018bc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00018bd0: 2020 2073 656c 662e 7265 6769 6f6e 5f69     self.region_i
+00018be0: 6420 3d20 6d2e 6765 7428 2752 6567 696f  d = m.get('Regio
+00018bf0: 6e49 6427 290a 2020 2020 2020 2020 7265  nId').        re
+00018c00: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00018c10: 7320 5374 6172 7445 6169 7345 6952 6573  s StartEaisEiRes
+00018c20: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+00018c30: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00018c40: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00018c50: 656c 662c 0a20 2020 2020 2020 2072 6571  elf,.        req
+00018c60: 7565 7374 5f69 643a 2073 7472 203d 204e  uest_id: str = N
+00018c70: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+00018c80: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+00018c90: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
+00018ca0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00018cb0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00018cc0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00018cd0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+00018ce0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+00018cf0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+00018d00: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00018d10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00018d20: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00018d30: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00018d40: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00018d50: 2020 2020 6966 2073 656c 662e 7265 7175      if self.requ
+00018d60: 6573 745f 6964 2069 7320 6e6f 7420 4e6f  est_id is not No
+00018d70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00018d80: 7265 7375 6c74 5b27 5265 7175 6573 7449  result['RequestI
+00018d90: 6427 5d20 3d20 7365 6c66 2e72 6571 7565  d'] = self.reque
+00018da0: 7374 5f69 640a 2020 2020 2020 2020 7265  st_id.        re
+00018db0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00018dc0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00018dd0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00018de0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00018df0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00018e00: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+00018e10: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
+00018e20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00018e30: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+00018e40: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
+00018e50: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
+00018e60: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00018e70: 6c61 7373 2053 7461 7274 4561 6973 4569  lass StartEaisEi
+00018e80: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
+00018e90: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00018ea0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00018eb0: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
+00018ec0: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
+00018ed0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+00018ee0: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
+00018ef0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
+00018f00: 2020 2020 2062 6f64 793a 2053 7461 7274       body: Start
+00018f10: 4561 6973 4569 5265 7370 6f6e 7365 426f  EaisEiResponseBo
+00018f20: 6479 203d 204e 6f6e 652c 0a20 2020 2029  dy = None,.    )
+00018f30: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
+00018f40: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
+00018f50: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00018f60: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
+00018f70: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+00018f80: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+00018f90: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00018fa0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00018fb0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00018fc0: 7265 7175 6972 6564 2873 656c 662e 6865  required(self.he
+00018fd0: 6164 6572 732c 2027 6865 6164 6572 7327  aders, 'headers'
+00018fe0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00018ff0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00019000: 2873 656c 662e 7374 6174 7573 5f63 6f64  (self.status_cod
+00019010: 652c 2027 7374 6174 7573 5f63 6f64 6527  e, 'status_code'
+00019020: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+00019030: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00019040: 2873 656c 662e 626f 6479 2c20 2762 6f64  (self.body, 'bod
+00019050: 7927 290a 2020 2020 2020 2020 6966 2073  y').        if s
+00019060: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+00019070: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+00019080: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+00019090: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+000190a0: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+000190b0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+000190c0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+000190d0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+000190e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000190f0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00019100: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00019110: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00019120: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+00019130: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00019140: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
+00019150: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
+00019160: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00019170: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
+00019180: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00019190: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+000191a0: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
+000191b0: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
+000191c0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+000191d0: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+000191e0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000191f0: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
+00019200: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
+00019210: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019220: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00019230: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00019240: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+00019250: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00019260: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00019270: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
+00019280: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00019290: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000192a0: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
+000192b0: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
+000192c0: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
+000192d0: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
+000192e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000192f0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+00019300: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
+00019310: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
+00019320: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
+00019330: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
+00019340: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00019350: 6d70 5f6d 6f64 656c 203d 2053 7461 7274  mp_model = Start
+00019360: 4561 6973 4569 5265 7370 6f6e 7365 426f  EaisEiResponseBo
+00019370: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+00019380: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+00019390: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+000193a0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+000193b0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000193c0: 0a0a 636c 6173 7320 5374 6f70 4561 6973  ..class StopEais
+000193d0: 4569 5265 7175 6573 7428 5465 614d 6f64  EiRequest(TeaMod
+000193e0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000193f0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00019400: 656c 662c 0a20 2020 2020 2020 2065 695f  elf,.        ei_
+00019410: 696e 7374 616e 6365 5f69 643a 2073 7472  instance_id: str
+00019420: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00019430: 2072 6567 696f 6e5f 6964 3a20 7374 7220   region_id: str 
+00019440: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+00019450: 2020 2020 2020 2073 656c 662e 6569 5f69         self.ei_i
+00019460: 6e73 7461 6e63 655f 6964 203d 2065 695f  nstance_id = ei_
+00019470: 696e 7374 616e 6365 5f69 640a 2020 2020  instance_id.    
+00019480: 2020 2020 7365 6c66 2e72 6567 696f 6e5f      self.region_
+00019490: 6964 203d 2072 6567 696f 6e5f 6964 0a0a  id = region_id..
+000194a0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000194b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000194c0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+000194d0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+000194e0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+000194f0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+00019500: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00019510: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00019520: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00019530: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00019540: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00019550: 2020 6966 2073 656c 662e 6569 5f69 6e73    if self.ei_ins
+00019560: 7461 6e63 655f 6964 2069 7320 6e6f 7420  tance_id is not 
+00019570: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00019580: 2020 7265 7375 6c74 5b27 4569 496e 7374    result['EiInst
+00019590: 616e 6365 4964 275d 203d 2073 656c 662e  anceId'] = self.
+000195a0: 6569 5f69 6e73 7461 6e63 655f 6964 0a20  ei_instance_id. 
+000195b0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+000195c0: 6567 696f 6e5f 6964 2069 7320 6e6f 7420  egion_id is not 
+000195d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000195e0: 2020 7265 7375 6c74 5b27 5265 6769 6f6e    result['Region
+000195f0: 4964 275d 203d 2073 656c 662e 7265 6769  Id'] = self.regi
+00019600: 6f6e 5f69 640a 2020 2020 2020 2020 7265  on_id.        re
+00019610: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00019620: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00019630: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00019640: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00019650: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00019660: 2020 2020 2069 6620 6d2e 6765 7428 2745       if m.get('E
+00019670: 6949 6e73 7461 6e63 6549 6427 2920 6973  iInstanceId') is
+00019680: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00019690: 2020 2020 2020 2073 656c 662e 6569 5f69         self.ei_i
+000196a0: 6e73 7461 6e63 655f 6964 203d 206d 2e67  nstance_id = m.g
+000196b0: 6574 2827 4569 496e 7374 616e 6365 4964  et('EiInstanceId
+000196c0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000196d0: 6765 7428 2752 6567 696f 6e49 6427 2920  get('RegionId') 
+000196e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000196f0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00019700: 6769 6f6e 5f69 6420 3d20 6d2e 6765 7428  gion_id = m.get(
+00019710: 2752 6567 696f 6e49 6427 290a 2020 2020  'RegionId').    
+00019720: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00019730: 0a0a 636c 6173 7320 5374 6f70 4561 6973  ..class StopEais
+00019740: 4569 5265 7370 6f6e 7365 426f 6479 2854  EiResponseBody(T
+00019750: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00019760: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00019770: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00019780: 2020 7265 7175 6573 745f 6964 3a20 7374    request_id: st
+00019790: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
+000197a0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+000197b0: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
+000197c0: 7374 5f69 640a 0a20 2020 2064 6566 2076  st_id..    def v
+000197d0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+000197e0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+000197f0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+00019800: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+00019810: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+00019820: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00019830: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00019840: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00019850: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00019860: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00019870: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00019880: 2e72 6571 7565 7374 5f69 6420 6973 206e  .request_id is n
+00019890: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000198a0: 2020 2020 2072 6573 756c 745b 2752 6571       result['Req
+000198b0: 7565 7374 4964 275d 203d 2073 656c 662e  uestId'] = self.
+000198c0: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
+000198d0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+000198e0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+000198f0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+00019900: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+00019910: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+00019920: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00019930: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
+00019940: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00019950: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+00019960: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
+00019970: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
+00019980: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00019990: 660a 0a0a 636c 6173 7320 5374 6f70 4561  f...class StopEa
+000199a0: 6973 4569 5265 7370 6f6e 7365 2854 6561  isEiResponse(Tea
+000199b0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+000199c0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000199d0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000199e0: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
+000199f0: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+00019a00: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+00019a10: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
+00019a20: 0a20 2020 2020 2020 2062 6f64 793a 2053  .        body: S
+00019a30: 746f 7045 6169 7345 6952 6573 706f 6e73  topEaisEiRespons
+00019a40: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
+00019a50: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00019a60: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00019a70: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+00019a80: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+00019a90: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+00019aa0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+00019ab0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+00019ac0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00019ad0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+00019ae0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+00019af0: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
+00019b00: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
+00019b10: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00019b20: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
+00019b30: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
+00019b40: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
+00019b50: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00019b60: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
+00019b70: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
+00019b80: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
+00019b90: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+00019ba0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
+00019bb0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+00019bc0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+00019bd0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+00019be0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00019bf0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00019c00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00019c10: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00019c20: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00019c30: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00019c40: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+00019c50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00019c60: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+00019c70: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+00019c80: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+00019c90: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00019ca0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00019cb0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00019cc0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+00019cd0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00019ce0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00019cf0: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+00019d00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00019d10: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+00019d20: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+00019d30: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+00019d40: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00019d50: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00019d60: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+00019d70: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+00019d80: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+00019d90: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
+00019da0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
+00019db0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00019dc0: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
+00019dd0: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
+00019de0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00019df0: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
+00019e00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00019e10: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00019e20: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
+00019e30: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
+00019e40: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00019e50: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+00019e60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00019e70: 2074 656d 705f 6d6f 6465 6c20 3d20 5374   temp_model = St
+00019e80: 6f70 4561 6973 4569 5265 7370 6f6e 7365  opEaisEiResponse
+00019e90: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
+00019ea0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+00019eb0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+00019ec0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+00019ed0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00019ee0: 660a 0a0a                                f...
```

### Comparing `alibabacloud_eais20190624-2.1.2/alibabacloud_eais20190624.egg-info/PKG-INFO` & `alibabacloud_eais20190624-2.1.3/alibabacloud_eais20190624.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eais20190624
-Version: 2.1.2
+Version: 2.1.3
 Summary: Alibaba Cloud eais (20190624) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eais20190624-2.1.2/setup.py` & `alibabacloud_eais20190624-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eais20190624.
 
-Created on 10/01/2023
+Created on 12/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eais20190624"
 NAME = "alibabacloud_eais20190624" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eais (20190624) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

