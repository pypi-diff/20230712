# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.932.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.932.tar", last modified: Tue Jul 11 01:04:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.933.tar", last modified: Wed Jul 12 00:45:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.932.tar` & `tencentcloud-sdk-python-vod-3.0.933.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)    25111 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1853920 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)   182702 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 01:04:11.000000 tencentcloud-sdk-python-vod-3.0.932/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   182690 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1853917 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:45:19.000000 tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-vod-3.0.932/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.933/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.932/setup.py` & `tencentcloud-sdk-python-vod-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.932/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.933/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.932/README.rst` & `tencentcloud-sdk-python-vod-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.932/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.932/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7888,15 +7888,15 @@
 
     def __init__(self):
         r"""
         :param _Type: 操作类型，可选值：add（添加）、delete（删除）、reset（重置）。重置操作将清空该人物已有人脸数据，并添加 FaceContents 指定人脸数据。
         :type Type: str
         :param _FaceIds: 人脸 ID 集合，当 Type为delete 时，该字段必填。
         :type FaceIds: list of str
-        :param _FaceContents: 人脸图片 [Base64](https://tools.ietf.org/html/rfc4648) 编码后的字符串集合。
+        :param _FaceContents: 人脸图片 [Base64](https://tools.ietf.org/html/rfc4648) 编码后的字符串集合，仅支持 jpeg、png 图片格式。
 <li>当 Type为add 或 reset 时，该字段必填；</li>
 <li>数组长度限制：5 张图片。</li>
 注意：图片必须是单人像正面人脸较清晰的照片，像素不低于 200*200。
         :type FaceContents: list of str
         """
         self._Type = None
         self._FaceIds = None
@@ -21699,15 +21699,15 @@
 class DescribeRebuildMediaTemplatesRequest(AbstractModel):
     """DescribeRebuildMediaTemplates请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Definitions: 音画质重生模板列表。
+        :param _Definitions: 视频重生模板列表。
         :type Definitions: list of int
         :param _SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
         :type SubAppId: int
         :param _Type: 模板类型过滤条件，可选值：
 <li>Preset：系统预置模板；</li>
 <li>Custom：用户自定义模板。</li>
         :type Type: str
@@ -21784,15 +21784,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _TotalCount: 符合过滤条件的记录总数。
         :type TotalCount: int
-        :param _RebuildMediaTemplateSet: 音画质重生模板详情列表。
+        :param _RebuildMediaTemplateSet: 视频重生模板详情列表。
         :type RebuildMediaTemplateSet: list of RebuildMediaTemplate
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._TotalCount = None
         self._RebuildMediaTemplateSet = None
         self._RequestId = None
@@ -21961,15 +21961,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param _SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
         :type SubAppId: int
-        :param _Definitions: 审核模版唯一标识过滤条件，数组长度限制：100。
+        :param _Definitions: 审核模板唯一标识过滤条件，数组长度限制：100。
         :type Definitions: list of int
         :param _Type: 模板类型过滤条件，可选值：
 <li>Preset：系统预置模板；</li>
 <li>Custom：用户自定义模板。</li>
         :type Type: str
         :param _Offset: 分页偏移量，默认值：0。
         :type Offset: int
@@ -37291,25 +37291,25 @@
 class ModifyRebuildMediaTemplateRequest(AbstractModel):
     """ModifyRebuildMediaTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Definition: 音画质重生模板号。
+        :param _Definition: 视频重生模板号。
         :type Definition: int
         :param _SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
         :type SubAppId: str
-        :param _Name: 音画质重生模板名称。
+        :param _Name: 视频重生模板名称。
         :type Name: str
-        :param _Comment: 音画质重生模板描述。
+        :param _Comment: 视频重生模板描述。
         :type Comment: str
-        :param _RebuildVideoInfo: 音画质重生视频控制信息。
+        :param _RebuildVideoInfo: 视频重生视频控制信息。
         :type RebuildVideoInfo: :class:`tencentcloud.vod.v20180717.models.RebuildVideoInfo`
-        :param _RebuildAudioInfo: 音画质重生音频控制信息。
+        :param _RebuildAudioInfo: 视频重生音频控制信息。
         :type RebuildAudioInfo: :class:`tencentcloud.vod.v20180717.models.RebuildAudioInfo`
         :param _TargetVideoInfo: 输出目标视频控制信息。
         :type TargetVideoInfo: :class:`tencentcloud.vod.v20180717.models.RebuildMediaTargetVideoStream`
         :param _TargetAudioInfo: 输出目标音频控制信息。
         :type TargetAudioInfo: :class:`tencentcloud.vod.v20180717.models.RebuildMediaTargetAudioStream`
         :param _Container: 输出文件封装格式，可选值：mp4、flv、hls。
         :type Container: str
@@ -44602,23 +44602,23 @@
 
     """
 
     def __init__(self):
         r"""
         :param _FileId: 媒体文件 ID。
         :type FileId: str
-        :param _Definition: 音画质重生模板 ID。
+        :param _Definition: 视频重生模板 ID。
         :type Definition: int
         :param _SubAppId: <b>点播[子应用](/document/product/266/14574) ID。如果要访问子应用中的资源，则将该字段填写为子应用 ID；否则无需填写该字段。</b>
         :type SubAppId: str
         :param _StartTimeOffset: 起始偏移时间，单位：秒，不填表示从视频开始截取。
         :type StartTimeOffset: float
         :param _EndTimeOffset: 结束偏移时间，单位：秒，不填表示截取到视频末尾。
         :type EndTimeOffset: float
-        :param _OutputConfig: 音画质重生后的文件配置。
+        :param _OutputConfig: 视频重生后的文件配置。
         :type OutputConfig: :class:`tencentcloud.vod.v20180717.models.RebuildMediaOutputConfig`
         :param _SessionId: 用于去重的识别码，如果三天内曾有过相同的识别码的请求，则本次的请求会返回错误。最长 50 个字符，不带或者带空字符串表示不做去重。
         :type SessionId: str
         :param _SessionContext: 来源上下文，用于透传用户请求信息，任务流状态变更回调将返回该字段值，最长 1000 个字符。
         :type SessionContext: str
         :param _TasksPriority: 任务的优先级，数值越大优先级越高，取值范围是 -10 到 10，不填代表 0。
         :type TasksPriority: int
@@ -44743,15 +44743,15 @@
 class RebuildMediaByTemplateResponse(AbstractModel):
     """RebuildMediaByTemplate返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TaskId: 音画质重生的任务 ID，可以通过该 ID 查询音画质重生任务的状态。
+        :param _TaskId: 视频重生的任务 ID，可以通过该 ID 查询视频重生任务的状态。
         :type TaskId: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._TaskId = None
         self._RequestId = None
 
@@ -45137,15 +45137,15 @@
 class RebuildMediaResponse(AbstractModel):
     """RebuildMedia返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TaskId: 音画质重生的任务 ID，可以通过该 ID 查询音画质重生任务的状态。
+        :param _TaskId: 视频重生的任务 ID，可以通过该 ID 查询视频重生任务的状态。
         :type TaskId: str
         :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._TaskId = None
         self._RequestId = None
```

### Comparing `tencentcloud-sdk-python-vod-3.0.932/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.933/tencentcloud/vod/v20180717/vod_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2074,15 +2074,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeRebuildMediaTemplates(self, request):
-        """获取音画质重生模板列表。
+        """获取视频重生模板列表。
 
         :param request: Request instance for DescribeRebuildMediaTemplates.
         :type request: :class:`tencentcloud.vod.v20180717.models.DescribeRebuildMediaTemplatesRequest`
         :rtype: :class:`tencentcloud.vod.v20180717.models.DescribeRebuildMediaTemplatesResponse`
 
         """
         try:
@@ -3090,15 +3090,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyRebuildMediaTemplate(self, request):
-        """修改音画质重生模板。
+        """修改视频重生模板。
 
         :param request: Request instance for ModifyRebuildMediaTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.ModifyRebuildMediaTemplateRequest`
         :rtype: :class:`tencentcloud.vod.v20180717.models.ModifyRebuildMediaTemplateResponse`
 
         """
         try:
@@ -3611,15 +3611,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RebuildMedia(self, request):
-        """发起音画质重生
+        """发起视频重生
 
         :param request: Request instance for RebuildMedia.
         :type request: :class:`tencentcloud.vod.v20180717.models.RebuildMediaRequest`
         :rtype: :class:`tencentcloud.vod.v20180717.models.RebuildMediaResponse`
 
         """
         try:
@@ -3634,15 +3634,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RebuildMediaByTemplate(self, request):
-        """使用模板发起音画质重生。
+        """使用模板发起视频重生。
 
         :param request: Request instance for RebuildMediaByTemplate.
         :type request: :class:`tencentcloud.vod.v20180717.models.RebuildMediaByTemplateRequest`
         :rtype: :class:`tencentcloud.vod.v20180717.models.RebuildMediaByTemplateResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-vod-3.0.932/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.933/tencentcloud/__init__.py`

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

