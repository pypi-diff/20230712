# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.932.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.932.tar", last modified: Tue Jul 11 00:43:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.933.tar", last modified: Wed Jul 12 00:29:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.932.tar` & `tencentcloud-sdk-python-essbasic-3.0.933.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)      678 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1016 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/setup.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/essbasic_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:37.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16662 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   380285 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53839 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:43:36.000000 tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53839 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   380671 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:29:51.000000 tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.933/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7650,14 +7650,17 @@
         :param _ApproverSignTypes: 签署人签署合同时的认证方式
 1-人脸认证 2-签署密码 3-运营商三要素(默认为1,2)
         :type ApproverSignTypes: list of int
         :param _SignId: 签署ID
 - 发起流程时系统自动补充
 - 创建签署链接时，可以通过查询详情接口获得签署人的SignId，然后可传入此值为该签署人创建签署链接，无需再传姓名、手机号、证件号等其他信息
         :type SignId: str
+        :param _NotifyType: SMS: 短信; NONE: 不发信息
+默认为SMS(该字段对子客无效)
+        :type NotifyType: str
         """
         self._Name = None
         self._IdCardType = None
         self._IdCardNumber = None
         self._Mobile = None
         self._OrganizationName = None
         self._NotChannelOrganization = None
@@ -7672,14 +7675,15 @@
         self._PreReadTime = None
         self._JumpUrl = None
         self._ApproverOption = None
         self._ApproverNeedSignReview = None
         self._ApproverVerifyTypes = None
         self._ApproverSignTypes = None
         self._SignId = None
+        self._NotifyType = None
 
     @property
     def Name(self):
         return self._Name
 
     @Name.setter
     def Name(self, Name):
@@ -7845,14 +7849,22 @@
     def SignId(self):
         return self._SignId
 
     @SignId.setter
     def SignId(self, SignId):
         self._SignId = SignId
 
+    @property
+    def NotifyType(self):
+        return self._NotifyType
+
+    @NotifyType.setter
+    def NotifyType(self, NotifyType):
+        self._NotifyType = NotifyType
+
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._IdCardType = params.get("IdCardType")
         self._IdCardNumber = params.get("IdCardNumber")
         self._Mobile = params.get("Mobile")
         self._OrganizationName = params.get("OrganizationName")
@@ -7875,14 +7887,15 @@
         if params.get("ApproverOption") is not None:
             self._ApproverOption = ApproverOption()
             self._ApproverOption._deserialize(params.get("ApproverOption"))
         self._ApproverNeedSignReview = params.get("ApproverNeedSignReview")
         self._ApproverVerifyTypes = params.get("ApproverVerifyTypes")
         self._ApproverSignTypes = params.get("ApproverSignTypes")
         self._SignId = params.get("SignId")
+        self._NotifyType = params.get("NotifyType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.932/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.933/tencentcloud/__init__.py`

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

