# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.932.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.932.tar", last modified: Tue Jul 11 00:33:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.933.tar", last modified: Wed Jul 12 00:22:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.932.tar` & `tencentcloud-sdk-python-cfs-3.0.933.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1006 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/setup.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/cfs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/cfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)    15890 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   191259 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39796 2023-07-11 00:33:32.000000 tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/cfs/v20190719/cfs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)    39796 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15890 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   193044 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-07-12 00:22:23.000000 tencentcloud-sdk-python-cfs-3.0.933/README.rst
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.932/setup.py` & `tencentcloud-sdk-python-cfs-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.932/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.933/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.932/README.rst` & `tencentcloud-sdk-python-cfs-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.932/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.933/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -806,14 +806,20 @@
         :type ClientToken: str
         :param _CcnId: 云联网ID， 若网络类型选择的是CCN，该字段为必填
         :type CcnId: str
         :param _CidrBlock: 云联网中CFS使用的网段， 若网络类型选择的是Ccn，该字段为必填，且不能和Ccn中已经绑定的网段冲突
         :type CidrBlock: str
         :param _Capacity: 文件系统容量，turbo系列必填，单位为GiB。 turbo标准型单位GB，起售40TiB，即40960 GiB；扩容步长20TiB，即20480 GiB。turbo性能型起售20TiB，即20480 GiB；扩容步长10TiB，10240 GiB。
         :type Capacity: int
+        :param _SnapshotId: 文件系统快照ID
+        :type SnapshotId: str
+        :param _AutoSnapshotPolicyId: 定期快照策略ID
+        :type AutoSnapshotPolicyId: str
+        :param _EnableAutoScaleUp: 是否开启默认扩容，仅Turbo类型文件存储支持
+        :type EnableAutoScaleUp: bool
         """
         self._Zone = None
         self._NetInterface = None
         self._PGroupId = None
         self._Protocol = None
         self._StorageType = None
         self._VpcId = None
@@ -821,14 +827,17 @@
         self._MountIP = None
         self._FsName = None
         self._ResourceTags = None
         self._ClientToken = None
         self._CcnId = None
         self._CidrBlock = None
         self._Capacity = None
+        self._SnapshotId = None
+        self._AutoSnapshotPolicyId = None
+        self._EnableAutoScaleUp = None
 
     @property
     def Zone(self):
         return self._Zone
 
     @Zone.setter
     def Zone(self, Zone):
@@ -934,14 +943,38 @@
     def Capacity(self):
         return self._Capacity
 
     @Capacity.setter
     def Capacity(self, Capacity):
         self._Capacity = Capacity
 
+    @property
+    def SnapshotId(self):
+        return self._SnapshotId
+
+    @SnapshotId.setter
+    def SnapshotId(self, SnapshotId):
+        self._SnapshotId = SnapshotId
+
+    @property
+    def AutoSnapshotPolicyId(self):
+        return self._AutoSnapshotPolicyId
+
+    @AutoSnapshotPolicyId.setter
+    def AutoSnapshotPolicyId(self, AutoSnapshotPolicyId):
+        self._AutoSnapshotPolicyId = AutoSnapshotPolicyId
+
+    @property
+    def EnableAutoScaleUp(self):
+        return self._EnableAutoScaleUp
+
+    @EnableAutoScaleUp.setter
+    def EnableAutoScaleUp(self, EnableAutoScaleUp):
+        self._EnableAutoScaleUp = EnableAutoScaleUp
+
 
     def _deserialize(self, params):
         self._Zone = params.get("Zone")
         self._NetInterface = params.get("NetInterface")
         self._PGroupId = params.get("PGroupId")
         self._Protocol = params.get("Protocol")
         self._StorageType = params.get("StorageType")
@@ -955,14 +988,17 @@
                 obj = TagInfo()
                 obj._deserialize(item)
                 self._ResourceTags.append(obj)
         self._ClientToken = params.get("ClientToken")
         self._CcnId = params.get("CcnId")
         self._CidrBlock = params.get("CidrBlock")
         self._Capacity = params.get("Capacity")
+        self._SnapshotId = params.get("SnapshotId")
+        self._AutoSnapshotPolicyId = params.get("AutoSnapshotPolicyId")
+        self._EnableAutoScaleUp = params.get("EnableAutoScaleUp")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -5348,14 +5384,17 @@
         :param _FsName: 文件系统名称
         :type FsName: str
         :param _Tags: 快照标签
         :type Tags: list of TagInfo
         :param _SnapshotType: 快照类型
 注意：此字段可能返回 null，表示取不到有效值。
         :type SnapshotType: str
+        :param _SnapshotTime: 实际快照时间，这里主要是为了标识跨地域复制快照的时间快照时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SnapshotTime: str
         """
         self._CreationTime = None
         self._SnapshotName = None
         self._SnapshotId = None
         self._Status = None
         self._RegionName = None
         self._FileSystemId = None
@@ -5363,14 +5402,15 @@
         self._AliveDay = None
         self._Percent = None
         self._AppId = None
         self._DeleteTime = None
         self._FsName = None
         self._Tags = None
         self._SnapshotType = None
+        self._SnapshotTime = None
 
     @property
     def CreationTime(self):
         return self._CreationTime
 
     @CreationTime.setter
     def CreationTime(self, CreationTime):
@@ -5476,14 +5516,22 @@
     def SnapshotType(self):
         return self._SnapshotType
 
     @SnapshotType.setter
     def SnapshotType(self, SnapshotType):
         self._SnapshotType = SnapshotType
 
+    @property
+    def SnapshotTime(self):
+        return self._SnapshotTime
+
+    @SnapshotTime.setter
+    def SnapshotTime(self, SnapshotTime):
+        self._SnapshotTime = SnapshotTime
+
 
     def _deserialize(self, params):
         self._CreationTime = params.get("CreationTime")
         self._SnapshotName = params.get("SnapshotName")
         self._SnapshotId = params.get("SnapshotId")
         self._Status = params.get("Status")
         self._RegionName = params.get("RegionName")
@@ -5497,14 +5545,15 @@
         if params.get("Tags") is not None:
             self._Tags = []
             for item in params.get("Tags"):
                 obj = TagInfo()
                 obj._deserialize(item)
                 self._Tags.append(obj)
         self._SnapshotType = params.get("SnapshotType")
+        self._SnapshotTime = params.get("SnapshotTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -6323,15 +6372,15 @@
 
     def __init__(self):
         r"""
         :param _PGroupId: 权限组 ID
         :type PGroupId: str
         :param _Name: 权限组名称，1-64个字符且只能为中文，字母，数字，下划线或横线
         :type Name: str
-        :param _DescInfo: 权限组描述信息，1-255个字符
+        :param _DescInfo: 权限组描述信息，1-255个字符。 Name和Descinfo不能同时为空
         :type DescInfo: str
         """
         self._PGroupId = None
         self._Name = None
         self._DescInfo = None
 
     @property
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.932/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.933/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files identical despite different names*

