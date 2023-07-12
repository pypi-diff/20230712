# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.932.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.932.tar", last modified: Tue Jul 11 00:43:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.933.tar", last modified: Wed Jul 12 00:29:46 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.932.tar` & `tencentcloud-sdk-python-ess-3.0.933.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    61652 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24834 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   428631 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:30.000000 tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    61652 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24834 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   428668 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud/ess/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:29:46.000000 tencentcloud-sdk-python-ess-3.0.933/README.rst
```

### Comparing `tencentcloud-sdk-python-ess-3.0.932/setup.py` & `tencentcloud-sdk-python-ess-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.932/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.933/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.932/README.rst` & `tencentcloud-sdk-python-ess-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.932/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.933/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.932/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.933/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.933/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.933/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.932/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.933/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3526,17 +3526,21 @@
         :param _ReviewMessage: 审核原因 
 当ReviewType 是REJECT 时此字段必填,字符串长度不超过200
         :type ReviewMessage: str
         :param _Agent: 代理相关应用信息，如集团主企业代子企业操作的场景中ProxyOrganizationId必填
         :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
         :param _RecipientId: 审核签署节点使用 非必填 如果填写则审核该签署节点。给个人审核时必填。
         :type RecipientId: str
-        :param _OperateType: 操作类型：
-操作类型，默认：SignReview；SignReview:签署审核
-注：接口通过该字段区分操作类型
+        :param _OperateType: 操作类型：（接口通过该字段区分操作类型）
+
+SignReview:签署审核
+CreateReview:发起审核
+
+默认：SignReview；SignReview:签署审核
+
 该字段不传或者为空，则默认为SignReview签署审核，走签署审核流程
 若发起个人审核，则指定该字段为：SignReview（注意，给个人审核时，需联系客户经理开白使用）
         :type OperateType: str
         """
         self._Operator = None
         self._FlowId = None
         self._ReviewType = None
```

