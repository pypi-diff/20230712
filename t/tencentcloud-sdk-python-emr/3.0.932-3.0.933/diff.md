# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.932.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.932.tar", last modified: Tue Jul 11 00:43:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.933.tar", last modified: Wed Jul 12 00:29:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.932.tar` & `tencentcloud-sdk-python-emr-3.0.933.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud_sdk_python_emr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud/emr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)    14329 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   455303 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30020 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud/emr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:43:15.000000 tencentcloud-sdk-python-emr-3.0.932/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud/emr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30020 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)    14329 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   455302 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud/emr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:29:34.000000 tencentcloud-sdk-python-emr-3.0.933/README.rst
```

### Comparing `tencentcloud-sdk-python-emr-3.0.932/setup.py` & `tencentcloud-sdk-python-emr-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.932/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.933/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.932/README.rst` & `tencentcloud-sdk-python-emr-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.932/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.933/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.932/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.933/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.932/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.933/tencentcloud/emr/v20190103/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6845,15 +6845,15 @@
 class InquiryPriceRenewInstanceRequest(AbstractModel):
     """InquiryPriceRenewInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TimeSpan: 实例续费的时长。需要结合TimeUnit一起使用。1表示续费1一个月
+        :param _TimeSpan: 实例续费的时长。需要结合TimeUnit一起使用。1表示续费一个月
         :type TimeSpan: int
         :param _ResourceIds: 待续费节点的资源ID列表。资源ID形如：emr-vm-xxxxxxxx。有效的资源ID可通过登录[控制台](https://console.cloud.tencent.com/emr/static/hardware)查询。
         :type ResourceIds: list of str
         :param _Placement: 实例所在的位置。通过该参数可以指定实例所属可用区，所属项目等属性。
         :type Placement: :class:`tencentcloud.emr.v20190103.models.Placement`
         :param _PayMode: 实例计费模式。此处只支持取值为1，表示包年包月。
         :type PayMode: int
```

### Comparing `tencentcloud-sdk-python-emr-3.0.932/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.933/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.932/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.933/tencentcloud/__init__.py`

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

