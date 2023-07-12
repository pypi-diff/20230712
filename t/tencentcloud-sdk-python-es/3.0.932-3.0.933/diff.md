# Comparing `tmp/tencentcloud-sdk-python-es-3.0.932.tar.gz` & `tmp/tencentcloud-sdk-python-es-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-es-3.0.932.tar", last modified: Tue Jul 11 00:43:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-es-3.0.933.tar", last modified: Wed Jul 12 00:29:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-es-3.0.932.tar` & `tencentcloud-sdk-python-es-3.0.933.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/setup.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud_sdk_python_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)      435 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud_sdk_python_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud_sdk_python_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud_sdk_python_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud_sdk_python_es.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud/es/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud/es/v20180416/
--rw-r--r--   0 root         (0) root         (0)     3342 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud/es/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   291209 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud/es/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud/es/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35037 2023-07-11 00:43:22.000000 tencentcloud-sdk-python-es-3.0.932/tencentcloud/es/v20180416/es_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud_sdk_python_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud_sdk_python_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      435 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud_sdk_python_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud_sdk_python_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud_sdk_python_es.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud/es/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud/es/v20180416/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud/es/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud/es/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    35974 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud/es/v20180416/es_client.py
+-rw-r--r--   0 root         (0) root         (0)   293112 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/tencentcloud/es/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      734 2023-07-12 00:29:41.000000 tencentcloud-sdk-python-es-3.0.933/README.rst
```

### Comparing `tencentcloud-sdk-python-es-3.0.932/setup.py` & `tencentcloud-sdk-python-es-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.932/PKG-INFO` & `tencentcloud-sdk-python-es-3.0.933/tencentcloud_sdk_python_es.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-es
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Es SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-es-3.0.932/README.rst` & `tencentcloud-sdk-python-es-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-es-3.0.932/tencentcloud_sdk_python_es.egg-info/PKG-INFO` & `tencentcloud-sdk-python-es-3.0.933/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-es
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Es SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-es-3.0.932/tencentcloud/__init__.py` & `tencentcloud-sdk-python-es-3.0.933/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.932'
+__version__ = '3.0.933'
```

### Comparing `tencentcloud-sdk-python-es-3.0.932/tencentcloud/es/v20180416/errorcodes.py` & `tencentcloud-sdk-python-es-3.0.933/tencentcloud/es/v20180416/errorcodes.py`

 * *Files 15% similar despite different names*

```diff
@@ -55,14 +55,20 @@
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
+# 无效的InstanceId，没有找到对应资源。
+INVALIDPARAMETER_INVALIDINSTANCEID = 'InvalidParameter.InvalidInstanceId'
+
+# 安全组id列表SecurityGroupIds的取值和预期不符。
+INVALIDPARAMETER_INVALIDSECURITYGROUPIDS = 'InvalidParameter.InvalidSecurityGroupIds'
+
 # 参数取值错误。
 INVALIDPARAMETERVALUE = 'InvalidParameterValue'
 
 # 缺少参数错误。
 MISSINGPARAMETER = 'MissingParameter'
 
 # 请求的次数超过了频率限制。
@@ -82,21 +88,30 @@
 
 # 子网剩余ip数量不足。
 RESOURCEINSUFFICIENT_SUBNET = 'ResourceInsufficient.Subnet'
 
 # 资源不存在。
 RESOURCENOTFOUND = 'ResourceNotFound'
 
+# 数据库资源获取失败。
+RESOURCENOTFOUND_DBINFONOTFOUND = 'ResourceNotFound.DBInfoNotFound'
+
+# 安全组信息获取失败。
+RESOURCENOTFOUND_SECURITYGROUPNOTFOUND = 'ResourceNotFound.SecurityGroupNotFound'
+
 # 资源不可用。
 RESOURCEUNAVAILABLE = 'ResourceUnavailable'
 
 # 资源售罄。
 RESOURCESSOLDOUT = 'ResourcesSoldOut'
 
 # 未授权操作。
 UNAUTHORIZEDOPERATION = 'UnauthorizedOperation'
 
 # 未知参数错误。
 UNKNOWNPARAMETER = 'UnknownParameter'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
+
+# 不支持该操作，实例状态有误。
+UNSUPPORTEDOPERATION_STATUSNOTSUPPORT = 'UnsupportedOperation.StatusNotSupport'
```

### Comparing `tencentcloud-sdk-python-es-3.0.932/tencentcloud/es/v20180416/models.py` & `tencentcloud-sdk-python-es-3.0.933/tencentcloud/es/v20180416/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6563,14 +6563,84 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ModifyEsVipSecurityGroupRequest(AbstractModel):
+    """ModifyEsVipSecurityGroup请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: es集群的实例id
+        :type InstanceId: str
+        :param _SecurityGroupIds: 安全组id列表
+        :type SecurityGroupIds: list of str
+        """
+        self._InstanceId = None
+        self._SecurityGroupIds = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def SecurityGroupIds(self):
+        return self._SecurityGroupIds
+
+    @SecurityGroupIds.setter
+    def SecurityGroupIds(self, SecurityGroupIds):
+        self._SecurityGroupIds = SecurityGroupIds
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        self._SecurityGroupIds = params.get("SecurityGroupIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyEsVipSecurityGroupResponse(AbstractModel):
+    """ModifyEsVipSecurityGroup返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._RequestId = None
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._RequestId = params.get("RequestId")
+
+
 class NodeInfo(AbstractModel):
     """集群中一种节点类型（如热数据节点，冷数据节点，专用主节点等）的规格描述信息，包括节点类型，节点个数，节点规格，磁盘类型，磁盘大小等, Type不指定时默认为热数据节点；如果节点为master节点，则DiskType和DiskSize参数会被忽略（主节点无数据盘）
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-es-3.0.932/tencentcloud/es/v20180416/es_client.py` & `tencentcloud-sdk-python-es-3.0.933/tencentcloud/es/v20180416/es_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,14 +459,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyEsVipSecurityGroup(self, request):
+        """修改绑定VIP的安全组，传安全组id列表
+
+        :param request: Request instance for ModifyEsVipSecurityGroup.
+        :type request: :class:`tencentcloud.es.v20180416.models.ModifyEsVipSecurityGroupRequest`
+        :rtype: :class:`tencentcloud.es.v20180416.models.ModifyEsVipSecurityGroupResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyEsVipSecurityGroup", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyEsVipSecurityGroupResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def RestartInstance(self, request):
         """重启ES集群实例(用于系统版本更新等操作)
 
         :param request: Request instance for RestartInstance.
         :type request: :class:`tencentcloud.es.v20180416.models.RestartInstanceRequest`
         :rtype: :class:`tencentcloud.es.v20180416.models.RestartInstanceResponse`
```

