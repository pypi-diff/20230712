# Comparing `tmp/tencentcloud-sdk-python-autoscaling-3.0.931.tar.gz` & `tmp/tencentcloud-sdk-python-autoscaling-3.0.932.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.931.tar", last modified: Mon Jul 10 00:30:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-autoscaling-3.0.932.tar", last modified: Tue Jul 11 00:30:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-autoscaling-3.0.931.tar` & `tencentcloud-sdk-python-autoscaling-3.0.932.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud_sdk_python_autoscaling.egg-info/
--rw-r--r--   0 root         (0) root         (0)      525 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/setup.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/autoscaling/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/autoscaling/v20180419/
--rw-r--r--   0 root         (0) root         (0)    19989 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/autoscaling/v20180419/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   389842 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/autoscaling/v20180419/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/autoscaling/v20180419/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60526 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/autoscaling/v20180419/autoscaling_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/autoscaling/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-10 00:30:24.000000 tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud_sdk_python_autoscaling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      525 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud_sdk_python_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud_sdk_python_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/autoscaling/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/autoscaling/v20180419/
+-rw-r--r--   0 root         (0) root         (0)    19989 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/autoscaling/v20180419/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   389762 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/autoscaling/v20180419/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/autoscaling/v20180419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60526 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/autoscaling/v20180419/autoscaling_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/autoscaling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:30:49.000000 tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/__init__.py
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud_sdk_python_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud_sdk_python_autoscaling.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.931/setup.py` & `tencentcloud-sdk-python-autoscaling-3.0.932/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.931/PKG-INFO` & `tencentcloud-sdk-python-autoscaling-3.0.932/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-autoscaling
-Version: 3.0.931
+Version: 3.0.932
 Summary: Tencent Cloud Autoscaling SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.931/README.rst` & `tencentcloud-sdk-python-autoscaling-3.0.932/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/autoscaling/v20180419/errorcodes.py` & `tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/autoscaling/v20180419/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/autoscaling/v20180419/models.py` & `tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/autoscaling/v20180419/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8452,16 +8452,16 @@
         :type PredefinedMetricType: str
         :param _TargetValue: 目标值，仅适用于目标追踪策略。<br><li>ASG_AVG_CPU_UTILIZATION：[1, 100)，单位：%</li><li>ASG_AVG_LAN_TRAFFIC_OUT：>0，单位：Mbps</li><li>ASG_AVG_LAN_TRAFFIC_IN：>0，单位：Mbps</li><li>ASG_AVG_WAN_TRAFFIC_OUT：>0，单位：Mbps</li><li>ASG_AVG_WAN_TRAFFIC_IN：>0，单位：Mbps</li>
         :type TargetValue: int
         :param _EstimatedInstanceWarmup: 实例预热时间，单位为秒，仅适用于目标追踪策略。取值范围为0-3600。
         :type EstimatedInstanceWarmup: int
         :param _DisableScaleIn: 是否禁用缩容，仅适用于目标追踪策略。取值范围：<br><li>true：目标追踪策略仅触发扩容</li><li>false：目标追踪策略触发扩容和缩容</li>
         :type DisableScaleIn: bool
-        :param _NotificationUserGroupIds: 通知组ID，即为用户组ID集合，用户组ID可以通过[ListGroups](https://cloud.tencent.com/document/product/598/34589)查询。
-如果需要清空通知用户组，需要在列表中传入特定字符串 "NULL"。
+        :param _NotificationUserGroupIds: 此参数已不再生效，请使用[创建通知](https://cloud.tencent.com/document/api/377/33185)。
+通知组ID，即为用户组ID集合。
         :type NotificationUserGroupIds: list of str
         """
         self._AutoScalingPolicyId = None
         self._ScalingPolicyName = None
         self._AdjustmentType = None
         self._AdjustmentValue = None
         self._Cooldown = None
```

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/autoscaling/v20180419/autoscaling_client.py` & `tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/autoscaling/v20180419/autoscaling_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-autoscaling-3.0.931/tencentcloud/__init__.py` & `tencentcloud-sdk-python-autoscaling-3.0.932/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.931'
+__version__ = '3.0.932'
```

