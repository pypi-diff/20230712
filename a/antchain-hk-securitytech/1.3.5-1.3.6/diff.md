# Comparing `tmp/antchain_hk_securitytech-1.3.5.tar.gz` & `tmp/antchain_hk_securitytech-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_hk_securitytech-1.3.5.tar", last modified: Mon Jul 10 08:18:52 2023, max compression
+gzip compressed data, was "dist/antchain_hk_securitytech-1.3.6.tar", last modified: Wed Jul 12 09:37:38 2023, max compression
```

## Comparing `antchain_hk_securitytech-1.3.5.tar` & `antchain_hk_securitytech-1.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2234 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      840 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2234 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29160 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/client.py
--rw-r--r--   0 root         (0) root         (0)    56622 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 08:18:52.000000 antchain_hk_securitytech-1.3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2550 2023-07-10 08:18:51.000000 antchain_hk_securitytech-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:37:38.000000 antchain_hk_securitytech-1.3.6/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-07-12 09:37:38.000000 antchain_hk_securitytech-1.3.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      840 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:37:38.000000 antchain_hk_securitytech-1.3.6/antchain_hk_securitytech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/antchain_hk_securitytech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-12 09:37:38.000000 antchain_hk_securitytech-1.3.6/antchain_hk_securitytech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/antchain_hk_securitytech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/antchain_hk_securitytech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/antchain_hk_securitytech.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:37:38.000000 antchain_hk_securitytech-1.3.6/antchain_sdk_hk_securitytech/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/antchain_sdk_hk_securitytech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31532 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/antchain_sdk_hk_securitytech/client.py
+-rw-r--r--   0 root         (0) root         (0)    64544 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/antchain_sdk_hk_securitytech/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 09:37:38.000000 antchain_hk_securitytech-1.3.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2550 2023-07-12 09:37:37.000000 antchain_hk_securitytech-1.3.6/setup.py
```

### Comparing `antchain_hk_securitytech-1.3.5/LICENSE` & `antchain_hk_securitytech-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_hk_securitytech-1.3.5/PKG-INFO` & `antchain_hk_securitytech-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_hk_securitytech
-Version: 1.3.5
+Version: 1.3.6
 Summary: Ant Chain HK_SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_hk_securitytech-1.3.5/README-CN.md` & `antchain_hk_securitytech-1.3.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_hk_securitytech-1.3.5/README.md` & `antchain_hk_securitytech-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `antchain_hk_securitytech-1.3.5/antchain_hk_securitytech.egg-info/PKG-INFO` & `antchain_hk_securitytech-1.3.6/antchain_hk_securitytech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-hk-securitytech
-Version: 1.3.5
+Version: 1.3.6
 Summary: Ant Chain HK_SECURITYTECH SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/client.py` & `antchain_hk_securitytech-1.3.6/antchain_sdk_hk_securitytech/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.3.5',
+                    'sdk_version': '1.3.6',
                     '_prod_code': 'HK_SECURITYTECH',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.3.5',
+                    'sdk_version': '1.3.6',
                     '_prod_code': 'HK_SECURITYTECH',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -662,7 +662,63 @@
         Summary: 设备信息上报
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             hk__securitytech_models.SubmitDeviceriskReportResponse(),
             await self.do_request_async('1.0', 'hksecuritytech.gateway.devicerisk.report.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def query_eaglepromo_marketingrisk(
+        self,
+        request: hk__securitytech_models.QueryEaglepromoMarketingriskRequest,
+    ) -> hk__securitytech_models.QueryEaglepromoMarketingriskResponse:
+        """
+        Description: 终端安全 EaglePromo
+        Summary: EaglePromo
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_eaglepromo_marketingrisk_ex(request, headers, runtime)
+
+    async def query_eaglepromo_marketingrisk_async(
+        self,
+        request: hk__securitytech_models.QueryEaglepromoMarketingriskRequest,
+    ) -> hk__securitytech_models.QueryEaglepromoMarketingriskResponse:
+        """
+        Description: 终端安全 EaglePromo
+        Summary: EaglePromo
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_eaglepromo_marketingrisk_ex_async(request, headers, runtime)
+
+    def query_eaglepromo_marketingrisk_ex(
+        self,
+        request: hk__securitytech_models.QueryEaglepromoMarketingriskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> hk__securitytech_models.QueryEaglepromoMarketingriskResponse:
+        """
+        Description: 终端安全 EaglePromo
+        Summary: EaglePromo
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            hk__securitytech_models.QueryEaglepromoMarketingriskResponse(),
+            self.do_request('1.0', 'hksecuritytech.gateway.eaglepromo.marketingrisk.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_eaglepromo_marketingrisk_ex_async(
+        self,
+        request: hk__securitytech_models.QueryEaglepromoMarketingriskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> hk__securitytech_models.QueryEaglepromoMarketingriskResponse:
+        """
+        Description: 终端安全 EaglePromo
+        Summary: EaglePromo
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            hk__securitytech_models.QueryEaglepromoMarketingriskResponse(),
+            await self.do_request_async('1.0', 'hksecuritytech.gateway.eaglepromo.marketingrisk.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_hk_securitytech-1.3.5/antchain_sdk_hk_securitytech/models.py` & `antchain_hk_securitytech-1.3.6/antchain_sdk_hk_securitytech/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -512,14 +512,50 @@
         if m.get('after_md_five') is not None:
             self.after_md_five = m.get('after_md_five')
         if m.get('after_size') is not None:
             self.after_size = m.get('after_size')
         return self
 
 
+class MarketingRiskData(TeaModel):
+    def __init__(
+        self,
+        risk_level: int = None,
+        sug_action: str = None,
+    ):
+        # risk_level
+        self.risk_level = risk_level
+        # sug_action
+        self.sug_action = sug_action
+
+    def validate(self):
+        self.validate_required(self.risk_level, 'risk_level')
+        self.validate_required(self.sug_action, 'sug_action')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.risk_level is not None:
+            result['risk_level'] = self.risk_level
+        if self.sug_action is not None:
+            result['sug_action'] = self.sug_action
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('risk_level') is not None:
+            self.risk_level = m.get('risk_level')
+        if m.get('sug_action') is not None:
+            self.sug_action = m.get('sug_action')
+        return self
+
+
 class DeviceRiskResp(TeaModel):
     def __init__(
         self,
         apdid: str = None,
         apdid_token: str = None,
         risk_level: int = None,
         risk_desc: str = None,
@@ -580,14 +616,58 @@
         if m.get('sug_action') is not None:
             self.sug_action = m.get('sug_action')
         if m.get('risk_labels') is not None:
             self.risk_labels = m.get('risk_labels')
         return self
 
 
+class MarketingRiskSecurityData(TeaModel):
+    def __init__(
+        self,
+        apdid_token: str = None,
+        signature: str = None,
+        solution_risk_code: str = None,
+    ):
+        # apdid_token
+        self.apdid_token = apdid_token
+        # signature
+        self.signature = signature
+        # solution_risk_code
+        self.solution_risk_code = solution_risk_code
+
+    def validate(self):
+        self.validate_required(self.apdid_token, 'apdid_token')
+        self.validate_required(self.signature, 'signature')
+        self.validate_required(self.solution_risk_code, 'solution_risk_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.apdid_token is not None:
+            result['apdid_token'] = self.apdid_token
+        if self.signature is not None:
+            result['signature'] = self.signature
+        if self.solution_risk_code is not None:
+            result['solution_risk_code'] = self.solution_risk_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('apdid_token') is not None:
+            self.apdid_token = m.get('apdid_token')
+        if m.get('signature') is not None:
+            self.signature = m.get('signature')
+        if m.get('solution_risk_code') is not None:
+            self.solution_risk_code = m.get('solution_risk_code')
+        return self
+
+
 class CreateBlueshieldSecuritypictureRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         app_name: str = None,
         client_name: str = None,
@@ -1601,7 +1681,161 @@
             self.dynamic_key = m.get('dynamic_key')
         if m.get('result_data') is not None:
             temp_model = DeviceRiskReportResultData()
             self.result_data = temp_model.from_map(m['result_data'])
         return self
 
 
+class QueryEaglepromoMarketingriskRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        security_data: MarketingRiskSecurityData = None,
+        sign_factor: str = None,
+        client_id: str = None,
+        request_id: str = None,
+        biz_code: str = None,
+        terminal_type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # security_data
+        self.security_data = security_data
+        # sign_factor
+        self.sign_factor = sign_factor
+        # client_id
+        self.client_id = client_id
+        # request_id
+        self.request_id = request_id
+        # biz_code
+        self.biz_code = biz_code
+        # terminal_type
+        self.terminal_type = terminal_type
+
+    def validate(self):
+        self.validate_required(self.security_data, 'security_data')
+        if self.security_data:
+            self.security_data.validate()
+        self.validate_required(self.sign_factor, 'sign_factor')
+        self.validate_required(self.client_id, 'client_id')
+        self.validate_required(self.terminal_type, 'terminal_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.security_data is not None:
+            result['security_data'] = self.security_data.to_map()
+        if self.sign_factor is not None:
+            result['sign_factor'] = self.sign_factor
+        if self.client_id is not None:
+            result['client_id'] = self.client_id
+        if self.request_id is not None:
+            result['request_id'] = self.request_id
+        if self.biz_code is not None:
+            result['biz_code'] = self.biz_code
+        if self.terminal_type is not None:
+            result['terminal_type'] = self.terminal_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('security_data') is not None:
+            temp_model = MarketingRiskSecurityData()
+            self.security_data = temp_model.from_map(m['security_data'])
+        if m.get('sign_factor') is not None:
+            self.sign_factor = m.get('sign_factor')
+        if m.get('client_id') is not None:
+            self.client_id = m.get('client_id')
+        if m.get('request_id') is not None:
+            self.request_id = m.get('request_id')
+        if m.get('biz_code') is not None:
+            self.biz_code = m.get('biz_code')
+        if m.get('terminal_type') is not None:
+            self.terminal_type = m.get('terminal_type')
+        return self
+
+
+class QueryEaglepromoMarketingriskResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        message: str = None,
+        code: int = None,
+        data: MarketingRiskData = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # success
+        self.success = success
+        # message
+        self.message = message
+        # code
+        self.code = code
+        # data
+        self.data = data
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.message is not None:
+            result['message'] = self.message
+        if self.code is not None:
+            result['code'] = self.code
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('data') is not None:
+            temp_model = MarketingRiskData()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
```

### Comparing `antchain_hk_securitytech-1.3.5/setup.py` & `antchain_hk_securitytech-1.3.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_hk_securitytech.
 
-Created on 10/07/2023
+Created on 12/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_hk_securitytech"
 NAME = "antchain_hk_securitytech" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain HK_SECURITYTECH SDK Library for Python"
```

