# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.932.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.932.tar", last modified: Tue Jul 11 01:04:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.933.tar", last modified: Wed Jul 12 00:45:47 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.932.tar` & `tencentcloud-sdk-python-vpc-3.0.933.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)    42398 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1311253 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   332400 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 01:04:30.000000 tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332400 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42398 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1312049 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:45:47.000000 tencentcloud-sdk-python-vpc-3.0.933/README.rst
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.932/setup.py` & `tencentcloud-sdk-python-vpc-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.932/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.933/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.932/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.933/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.932/README.rst` & `tencentcloud-sdk-python-vpc-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -19911,32 +19911,38 @@
 class DescribeSecurityGroupsRequest(AbstractModel):
     """DescribeSecurityGroups请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _SecurityGroupIds: 安全组实例ID，例如：sg-33ocnj9n，可通过DescribeSecurityGroups获取。每次请求的实例的上限为100。参数不支持同时指定SecurityGroupIds和Filters。
+        :param _SecurityGroupIds: 安全组实例ID，例如：sg-33ocnj9n。每次请求的实例的上限为100。参数不支持同时指定SecurityGroupIds和Filters。
         :type SecurityGroupIds: list of str
         :param _Filters: 过滤条件，参数不支持同时指定SecurityGroupIds和Filters。
 <li>security-group-id - String - （过滤条件）安全组ID。</li>
 <li>project-id - Integer - （过滤条件）项目ID。</li>
 <li>security-group-name - String - （过滤条件）安全组名称。</li>
 <li>tag-key - String -是否必填：否- （过滤条件）按照标签键进行过滤。使用请参考示例2。</li>
 <li>tag:tag-key - String - 是否必填：否 - （过滤条件）按照标签键值对进行过滤。 tag-key使用具体的标签键进行替换。使用请参考示例3。</li>
         :type Filters: list of Filter
         :param _Offset: 偏移量，默认为0。
         :type Offset: str
         :param _Limit: 返回数量，默认为20，最大值为100。
         :type Limit: str
+        :param _OrderField: 排序字段。支持：`CreatedTime` `UpdateTime`。注意：该字段没有默认值。
+        :type OrderField: str
+        :param _OrderDirection: 排序方法。升序：`ASC`，倒序：`DESC`。默认值：`ASC`
+        :type OrderDirection: str
         """
         self._SecurityGroupIds = None
         self._Filters = None
         self._Offset = None
         self._Limit = None
+        self._OrderField = None
+        self._OrderDirection = None
 
     @property
     def SecurityGroupIds(self):
         return self._SecurityGroupIds
 
     @SecurityGroupIds.setter
     def SecurityGroupIds(self, SecurityGroupIds):
@@ -19962,25 +19968,43 @@
     def Limit(self):
         return self._Limit
 
     @Limit.setter
     def Limit(self, Limit):
         self._Limit = Limit
 
+    @property
+    def OrderField(self):
+        return self._OrderField
+
+    @OrderField.setter
+    def OrderField(self, OrderField):
+        self._OrderField = OrderField
+
+    @property
+    def OrderDirection(self):
+        return self._OrderDirection
+
+    @OrderDirection.setter
+    def OrderDirection(self, OrderDirection):
+        self._OrderDirection = OrderDirection
+
 
     def _deserialize(self, params):
         self._SecurityGroupIds = params.get("SecurityGroupIds")
         if params.get("Filters") is not None:
             self._Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self._Filters.append(obj)
         self._Offset = params.get("Offset")
         self._Limit = params.get("Limit")
+        self._OrderField = params.get("OrderField")
+        self._OrderDirection = params.get("OrderDirection")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.932/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.933/tencentcloud/__init__.py`

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

