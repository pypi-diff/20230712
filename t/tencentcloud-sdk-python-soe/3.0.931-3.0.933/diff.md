# Comparing `tmp/tencentcloud-sdk-python-soe-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-soe-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-soe-3.0.931.tar", last modified: Mon Jul 10 00:51:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-soe-3.0.933.tar", last modified: Wed Jul 12 00:36:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-soe-3.0.931.tar` & `tencentcloud-sdk-python-soe-3.0.933.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/
--rw-r--r--   0 root         (0) root         (0)    14652 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    67959 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)     5903 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/soe_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:51:11.000000 tencentcloud-sdk-python-soe-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud/soe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud/soe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud/soe/v20180724/
+-rw-r--r--   0 root         (0) root         (0)     5903 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud/soe/v20180724/soe_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud/soe/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud/soe/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    67959 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud/soe/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud_sdk_python_soe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud_sdk_python_soe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud_sdk_python_soe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud_sdk_python_soe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/tencentcloud_sdk_python_soe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:36:24.000000 tencentcloud-sdk-python-soe-3.0.933/README.rst
```

### Comparing `tencentcloud-sdk-python-soe-3.0.931/setup.py` & `tencentcloud-sdk-python-soe-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-soe-3.0.933/tencentcloud_sdk_python_soe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-soe
-Version: 3.0.931
+Version: 3.0.933
 Summary: Tencent Cloud Soe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-soe-3.0.931/README.rst` & `tencentcloud-sdk-python-soe-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.931/tencentcloud_sdk_python_soe.egg-info/PKG-INFO` & `tencentcloud-sdk-python-soe-3.0.933/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-soe
-Version: 3.0.931
+Version: 3.0.933
 Summary: Tencent Cloud Soe SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/errorcodes.py` & `tencentcloud-sdk-python-soe-3.0.933/tencentcloud/soe/v20180724/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,14 +247,17 @@
 
 # 输入音频异常，音频数据指针或音频⻓度必须为偶数，请参考API文档检查音频数据是否正确后重新传输数据。
 INVALIDPARAMETERVALUE_AUDIOSIZEMUSTBEEVEN = 'InvalidParameterValue.AudioSizeMustBeEven'
 
 # BASE64解码错误。
 INVALIDPARAMETERVALUE_BASEDECODEFAILED = 'InvalidParameterValue.BASEDecodeFailed'
 
+# 该评测功能暂不支持，请参考API文档检查评测参数。
+INVALIDPARAMETERVALUE_FUNCTIONNOTSUPPORT = 'InvalidParameterValue.FunctionNotSupport'
+
 # 分片序号错误。
 INVALIDPARAMETERVALUE_INVALIDSEQID = 'InvalidParameterValue.InvalidSeqId'
 
 # WAV头部格式非法或不在同一分片内。
 INVALIDPARAMETERVALUE_INVALIDWAVHEADER = 'InvalidParameterValue.InvalidWAVHeader'
 
 # 表单中没有文件。
```

### Comparing `tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/models.py` & `tencentcloud-sdk-python-soe-3.0.933/tencentcloud/soe/v20180724/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.931/tencentcloud/soe/v20180724/soe_client.py` & `tencentcloud-sdk-python-soe-3.0.933/tencentcloud/soe/v20180724/soe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-soe-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-soe-3.0.933/tencentcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.931'
+__version__ = '3.0.933'
```

