# Comparing `tmp/alibabacloud_dms-enterprise20181101-1.52.0.tar.gz` & `tmp/alibabacloud_dms-enterprise20181101-1.53.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101-1.52.0.tar", last modified: Thu Jul  6 07:23:22 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101-1.53.0.tar", last modified: Wed Jul 12 03:00:20 2023, max compression
```

## Comparing `alibabacloud_dms-enterprise20181101-1.52.0.tar` & `alibabacloud_dms-enterprise20181101-1.53.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/
--rw-r--r--   0 root         (0) root         (0)     5958 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2395 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   809475 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101/client.py
--rw-r--r--   0 root         (0) root         (0)  1889703 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2395 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2667 2023-07-06 07:23:22.000000 alibabacloud_dms-enterprise20181101-1.52.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:00:20.000000 alibabacloud_dms-enterprise20181101-1.53.0/
+-rw-r--r--   0 root         (0) root         (0)     6066 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-07-12 03:00:20.000000 alibabacloud_dms-enterprise20181101-1.53.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:00:20.000000 alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   817799 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1906586 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 03:00:20.000000 alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 03:00:20.000000 alibabacloud_dms-enterprise20181101-1.53.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-07-12 03:00:19.000000 alibabacloud_dms-enterprise20181101-1.53.0/setup.py
```

### Comparing `alibabacloud_dms-enterprise20181101-1.52.0/ChangeLog.md` & `alibabacloud_dms-enterprise20181101-1.53.0/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-06 Version: 1.52.0
+- Modify GetDataArchiveOrderDetail API. Add output parameter: TempTableNameMap.
+
 2023-06-30 Version: 1.51.0
 - Modify ListTaskFlowsByPage API. Add output parameter: DagOwnerId.
 - Modify ReRunTaskFlowInstance, ReSumeTaskFlowInstance: input parameter DagVersion is not required.
 
 2023-05-25 Version: 1.50.0
 - Support AnalyzeLineage API.
 - Modify ListTaskFlowsByPage API. Add input parameters: DagIdList. Add output parameters: CronSwitch, CronStr, CronParam, TriggerType, CronType, TimeZoneId
```

### Comparing `alibabacloud_dms-enterprise20181101-1.52.0/LICENSE` & `alibabacloud_dms-enterprise20181101-1.53.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.52.0/PKG-INFO` & `alibabacloud_dms-enterprise20181101-1.53.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dms-enterprise20181101
-Version: 1.52.0
+Version: 1.53.0
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101-1.52.0/README-CN.md` & `alibabacloud_dms-enterprise20181101-1.53.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.52.0/README.md` & `alibabacloud_dms-enterprise20181101-1.53.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101/client.py` & `alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1265,14 +1265,116 @@
         
         @param request: CreateAuthorityTemplateRequest
         @return: CreateAuthorityTemplateResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_authority_template_with_options_async(request, runtime)
 
+    def create_data_archive_order_with_options(
+        self,
+        tmp_req: dms_enterprise_20181101_models.CreateDataArchiveOrderRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.CreateDataArchiveOrderResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.CreateDataArchiveOrderShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.param):
+            request.param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.param, 'Param', 'json')
+        if not UtilClient.is_unset(tmp_req.related_user_list):
+            request.related_user_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.related_user_list, 'RelatedUserList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.param_shrink):
+            query['Param'] = request.param_shrink
+        if not UtilClient.is_unset(request.parent_id):
+            query['ParentId'] = request.parent_id
+        if not UtilClient.is_unset(request.plugin_type):
+            query['PluginType'] = request.plugin_type
+        if not UtilClient.is_unset(request.related_user_list_shrink):
+            query['RelatedUserList'] = request.related_user_list_shrink
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDataArchiveOrder',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.CreateDataArchiveOrderResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_data_archive_order_with_options_async(
+        self,
+        tmp_req: dms_enterprise_20181101_models.CreateDataArchiveOrderRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.CreateDataArchiveOrderResponse:
+        UtilClient.validate_model(tmp_req)
+        request = dms_enterprise_20181101_models.CreateDataArchiveOrderShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.param):
+            request.param_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.param, 'Param', 'json')
+        if not UtilClient.is_unset(tmp_req.related_user_list):
+            request.related_user_list_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.related_user_list, 'RelatedUserList', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.param_shrink):
+            query['Param'] = request.param_shrink
+        if not UtilClient.is_unset(request.parent_id):
+            query['ParentId'] = request.parent_id
+        if not UtilClient.is_unset(request.plugin_type):
+            query['PluginType'] = request.plugin_type
+        if not UtilClient.is_unset(request.related_user_list_shrink):
+            query['RelatedUserList'] = request.related_user_list_shrink
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDataArchiveOrder',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.CreateDataArchiveOrderResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_data_archive_order(
+        self,
+        request: dms_enterprise_20181101_models.CreateDataArchiveOrderRequest,
+    ) -> dms_enterprise_20181101_models.CreateDataArchiveOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_data_archive_order_with_options(request, runtime)
+
+    async def create_data_archive_order_async(
+        self,
+        request: dms_enterprise_20181101_models.CreateDataArchiveOrderRequest,
+    ) -> dms_enterprise_20181101_models.CreateDataArchiveOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_data_archive_order_with_options_async(request, runtime)
+
     def create_data_correct_order_with_options(
         self,
         tmp_req: dms_enterprise_20181101_models.CreateDataCorrectOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.CreateDataCorrectOrderResponse:
         """
         For more information about the Normal Data Modify feature, see [Change regular data](~~58419~~).
@@ -5821,14 +5923,96 @@
     async def get_dbtopology_async(
         self,
         request: dms_enterprise_20181101_models.GetDBTopologyRequest,
     ) -> dms_enterprise_20181101_models.GetDBTopologyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_dbtopology_with_options_async(request, runtime)
 
+    def get_data_archive_count_with_options(
+        self,
+        request: dms_enterprise_20181101_models.GetDataArchiveCountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDataArchiveCountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_result_type):
+            query['OrderResultType'] = request.order_result_type
+        if not UtilClient.is_unset(request.plugin_type):
+            query['PluginType'] = request.plugin_type
+        if not UtilClient.is_unset(request.search_date_type):
+            query['SearchDateType'] = request.search_date_type
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDataArchiveCount',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDataArchiveCountResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_data_archive_count_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDataArchiveCountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDataArchiveCountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_result_type):
+            query['OrderResultType'] = request.order_result_type
+        if not UtilClient.is_unset(request.plugin_type):
+            query['PluginType'] = request.plugin_type
+        if not UtilClient.is_unset(request.search_date_type):
+            query['SearchDateType'] = request.search_date_type
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDataArchiveCount',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDataArchiveCountResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_data_archive_count(
+        self,
+        request: dms_enterprise_20181101_models.GetDataArchiveCountRequest,
+    ) -> dms_enterprise_20181101_models.GetDataArchiveCountResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_data_archive_count_with_options(request, runtime)
+
+    async def get_data_archive_count_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDataArchiveCountRequest,
+    ) -> dms_enterprise_20181101_models.GetDataArchiveCountResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_data_archive_count_with_options_async(request, runtime)
+
     def get_data_archive_order_detail_with_options(
         self,
         request: dms_enterprise_20181101_models.GetDataArchiveOrderDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetDataArchiveOrderDetailResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101/models.py` & `alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3086,14 +3086,347 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateAuthorityTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateDataArchiveOrderRequestParamTableIncludes(TeaModel):
+    def __init__(
+        self,
+        table_name: str = None,
+        table_where: str = None,
+    ):
+        self.table_name = table_name
+        self.table_where = table_where
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.table_name is not None:
+            result['TableName'] = self.table_name
+        if self.table_where is not None:
+            result['TableWhere'] = self.table_where
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TableName') is not None:
+            self.table_name = m.get('TableName')
+        if m.get('TableWhere') is not None:
+            self.table_where = m.get('TableWhere')
+        return self
+
+
+class CreateDataArchiveOrderRequestParam(TeaModel):
+    def __init__(
+        self,
+        archive_method: str = None,
+        db_schema: str = None,
+        logic: bool = None,
+        order_after: List[str] = None,
+        run_method: str = None,
+        source_database_id: int = None,
+        table_includes: List[CreateDataArchiveOrderRequestParamTableIncludes] = None,
+        table_mapping: List[str] = None,
+        target_instance_id: str = None,
+        variables: List[str] = None,
+    ):
+        self.archive_method = archive_method
+        self.db_schema = db_schema
+        self.logic = logic
+        self.order_after = order_after
+        self.run_method = run_method
+        self.source_database_id = source_database_id
+        self.table_includes = table_includes
+        self.table_mapping = table_mapping
+        self.target_instance_id = target_instance_id
+        self.variables = variables
+
+    def validate(self):
+        if self.table_includes:
+            for k in self.table_includes:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.archive_method is not None:
+            result['ArchiveMethod'] = self.archive_method
+        if self.db_schema is not None:
+            result['DbSchema'] = self.db_schema
+        if self.logic is not None:
+            result['Logic'] = self.logic
+        if self.order_after is not None:
+            result['OrderAfter'] = self.order_after
+        if self.run_method is not None:
+            result['RunMethod'] = self.run_method
+        if self.source_database_id is not None:
+            result['SourceDatabaseId'] = self.source_database_id
+        result['TableIncludes'] = []
+        if self.table_includes is not None:
+            for k in self.table_includes:
+                result['TableIncludes'].append(k.to_map() if k else None)
+        if self.table_mapping is not None:
+            result['TableMapping'] = self.table_mapping
+        if self.target_instance_id is not None:
+            result['TargetInstanceId'] = self.target_instance_id
+        if self.variables is not None:
+            result['Variables'] = self.variables
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ArchiveMethod') is not None:
+            self.archive_method = m.get('ArchiveMethod')
+        if m.get('DbSchema') is not None:
+            self.db_schema = m.get('DbSchema')
+        if m.get('Logic') is not None:
+            self.logic = m.get('Logic')
+        if m.get('OrderAfter') is not None:
+            self.order_after = m.get('OrderAfter')
+        if m.get('RunMethod') is not None:
+            self.run_method = m.get('RunMethod')
+        if m.get('SourceDatabaseId') is not None:
+            self.source_database_id = m.get('SourceDatabaseId')
+        self.table_includes = []
+        if m.get('TableIncludes') is not None:
+            for k in m.get('TableIncludes'):
+                temp_model = CreateDataArchiveOrderRequestParamTableIncludes()
+                self.table_includes.append(temp_model.from_map(k))
+        if m.get('TableMapping') is not None:
+            self.table_mapping = m.get('TableMapping')
+        if m.get('TargetInstanceId') is not None:
+            self.target_instance_id = m.get('TargetInstanceId')
+        if m.get('Variables') is not None:
+            self.variables = m.get('Variables')
+        return self
+
+
+class CreateDataArchiveOrderRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        param: CreateDataArchiveOrderRequestParam = None,
+        parent_id: int = None,
+        plugin_type: str = None,
+        related_user_list: List[str] = None,
+        tid: int = None,
+    ):
+        self.comment = comment
+        self.param = param
+        self.parent_id = parent_id
+        self.plugin_type = plugin_type
+        self.related_user_list = related_user_list
+        self.tid = tid
+
+    def validate(self):
+        if self.param:
+            self.param.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.param is not None:
+            result['Param'] = self.param.to_map()
+        if self.parent_id is not None:
+            result['ParentId'] = self.parent_id
+        if self.plugin_type is not None:
+            result['PluginType'] = self.plugin_type
+        if self.related_user_list is not None:
+            result['RelatedUserList'] = self.related_user_list
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('Param') is not None:
+            temp_model = CreateDataArchiveOrderRequestParam()
+            self.param = temp_model.from_map(m['Param'])
+        if m.get('ParentId') is not None:
+            self.parent_id = m.get('ParentId')
+        if m.get('PluginType') is not None:
+            self.plugin_type = m.get('PluginType')
+        if m.get('RelatedUserList') is not None:
+            self.related_user_list = m.get('RelatedUserList')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class CreateDataArchiveOrderShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        param_shrink: str = None,
+        parent_id: int = None,
+        plugin_type: str = None,
+        related_user_list_shrink: str = None,
+        tid: int = None,
+    ):
+        self.comment = comment
+        self.param_shrink = param_shrink
+        self.parent_id = parent_id
+        self.plugin_type = plugin_type
+        self.related_user_list_shrink = related_user_list_shrink
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.param_shrink is not None:
+            result['Param'] = self.param_shrink
+        if self.parent_id is not None:
+            result['ParentId'] = self.parent_id
+        if self.plugin_type is not None:
+            result['PluginType'] = self.plugin_type
+        if self.related_user_list_shrink is not None:
+            result['RelatedUserList'] = self.related_user_list_shrink
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('Param') is not None:
+            self.param_shrink = m.get('Param')
+        if m.get('ParentId') is not None:
+            self.parent_id = m.get('ParentId')
+        if m.get('PluginType') is not None:
+            self.plugin_type = m.get('PluginType')
+        if m.get('RelatedUserList') is not None:
+            self.related_user_list_shrink = m.get('RelatedUserList')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class CreateDataArchiveOrderResponseBody(TeaModel):
+    def __init__(
+        self,
+        create_order_result: List[int] = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.create_order_result = create_order_result
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.create_order_result is not None:
+            result['CreateOrderResult'] = self.create_order_result
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateOrderResult') is not None:
+            self.create_order_result = m.get('CreateOrderResult')
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreateDataArchiveOrderResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateDataArchiveOrderResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateDataArchiveOrderResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateDataCorrectOrderRequestParamDbItemList(TeaModel):
     def __init__(
         self,
         db_id: int = None,
         logic: bool = None,
     ):
         # The ID of the database. The database can be a physical database or a logical database.
@@ -13442,14 +13775,189 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetDBTopologyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetDataArchiveCountRequest(TeaModel):
+    def __init__(
+        self,
+        order_result_type: str = None,
+        plugin_type: str = None,
+        search_date_type: str = None,
+        tid: int = None,
+    ):
+        self.order_result_type = order_result_type
+        self.plugin_type = plugin_type
+        self.search_date_type = search_date_type
+        self.tid = tid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.order_result_type is not None:
+            result['OrderResultType'] = self.order_result_type
+        if self.plugin_type is not None:
+            result['PluginType'] = self.plugin_type
+        if self.search_date_type is not None:
+            result['SearchDateType'] = self.search_date_type
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderResultType') is not None:
+            self.order_result_type = m.get('OrderResultType')
+        if m.get('PluginType') is not None:
+            self.plugin_type = m.get('PluginType')
+        if m.get('SearchDateType') is not None:
+            self.search_date_type = m.get('SearchDateType')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetDataArchiveCountResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        fail_count: int = None,
+        processing_count: int = None,
+        success_count: int = None,
+        total_count: int = None,
+    ):
+        self.fail_count = fail_count
+        self.processing_count = processing_count
+        self.success_count = success_count
+        self.total_count = total_count
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.fail_count is not None:
+            result['FailCount'] = self.fail_count
+        if self.processing_count is not None:
+            result['ProcessingCount'] = self.processing_count
+        if self.success_count is not None:
+            result['SuccessCount'] = self.success_count
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('FailCount') is not None:
+            self.fail_count = m.get('FailCount')
+        if m.get('ProcessingCount') is not None:
+            self.processing_count = m.get('ProcessingCount')
+        if m.get('SuccessCount') is not None:
+            self.success_count = m.get('SuccessCount')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class GetDataArchiveCountResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: GetDataArchiveCountResponseBodyData = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = GetDataArchiveCountResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetDataArchiveCountResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDataArchiveCountResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetDataArchiveCountResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetDataArchiveOrderDetailRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
         self.order_id = order_id
```

### Comparing `alibabacloud_dms-enterprise20181101-1.52.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO` & `alibabacloud_dms-enterprise20181101-1.53.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dms-enterprise20181101
-Version: 1.52.0
+Version: 1.53.0
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101-1.52.0/setup.py` & `alibabacloud_dms-enterprise20181101-1.53.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dms-enterprise20181101.
 
-Created on 06/07/2023
+Created on 12/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dms_enterprise20181101"
 NAME = "alibabacloud_dms-enterprise20181101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dms-enterprise (20181101) SDK Library for Python"
```

