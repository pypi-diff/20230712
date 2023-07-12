# Comparing `tmp/tencentcloud-sdk-python-wedata-3.0.932.tar.gz` & `tmp/tencentcloud-sdk-python-wedata-3.0.933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.932.tar", last modified: Tue Jul 11 01:07:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.933.tar", last modified: Wed Jul 12 00:46:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wedata-3.0.932.tar` & `tencentcloud-sdk-python-wedata-3.0.933.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/
--rw-r--r--   0 root         (0) root         (0)       88 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1012 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/setup.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud_sdk_python_wedata.egg-info/
--rw-r--r--   0 root         (0) root         (0)      475 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/wedata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)     3451 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)  1216112 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)   186091 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/wedata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-07-11 01:07:53.000000 tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud_sdk_python_wedata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)  1253549 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)   187884 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-12 00:46:15.000000 tencentcloud-sdk-python-wedata-3.0.933/README.rst
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.932/setup.py` & `tencentcloud-sdk-python-wedata-3.0.933/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.932/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.933/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.932/README.rst` & `tencentcloud-sdk-python-wedata-3.0.933/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.932/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.933/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.932
+Version: 3.0.933
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/wedata/v20210820/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3237,14 +3237,443 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class ColumnAggregationLineage(AbstractModel):
+    """列血缘聚合信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TableName: 表名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TableName: str
+        :param _ParentId: 父节点ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParentId: str
+        :param _MetastoreType: 元数据类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MetastoreType: str
+        :param _ParentSet: 字符串类型的父节点集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParentSet: str
+        :param _ChildSet: 字符串类型的子节点集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ChildSet: str
+        :param _ColumnInfoSet: 列信息集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ColumnInfoSet: list of SimpleColumnInfo
+        """
+        self._TableName = None
+        self._ParentId = None
+        self._MetastoreType = None
+        self._ParentSet = None
+        self._ChildSet = None
+        self._ColumnInfoSet = None
+
+    @property
+    def TableName(self):
+        return self._TableName
+
+    @TableName.setter
+    def TableName(self, TableName):
+        self._TableName = TableName
+
+    @property
+    def ParentId(self):
+        return self._ParentId
+
+    @ParentId.setter
+    def ParentId(self, ParentId):
+        self._ParentId = ParentId
+
+    @property
+    def MetastoreType(self):
+        return self._MetastoreType
+
+    @MetastoreType.setter
+    def MetastoreType(self, MetastoreType):
+        self._MetastoreType = MetastoreType
+
+    @property
+    def ParentSet(self):
+        return self._ParentSet
+
+    @ParentSet.setter
+    def ParentSet(self, ParentSet):
+        self._ParentSet = ParentSet
+
+    @property
+    def ChildSet(self):
+        return self._ChildSet
+
+    @ChildSet.setter
+    def ChildSet(self, ChildSet):
+        self._ChildSet = ChildSet
+
+    @property
+    def ColumnInfoSet(self):
+        return self._ColumnInfoSet
+
+    @ColumnInfoSet.setter
+    def ColumnInfoSet(self, ColumnInfoSet):
+        self._ColumnInfoSet = ColumnInfoSet
+
+
+    def _deserialize(self, params):
+        self._TableName = params.get("TableName")
+        self._ParentId = params.get("ParentId")
+        self._MetastoreType = params.get("MetastoreType")
+        self._ParentSet = params.get("ParentSet")
+        self._ChildSet = params.get("ChildSet")
+        if params.get("ColumnInfoSet") is not None:
+            self._ColumnInfoSet = []
+            for item in params.get("ColumnInfoSet"):
+                obj = SimpleColumnInfo()
+                obj._deserialize(item)
+                self._ColumnInfoSet.append(obj)
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
+class ColumnLineageInfo(AbstractModel):
+    """血缘字段信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: 血缘id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param _PrefixPath: 由中心节点出发的路径信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PrefixPath: str
+        :param _DatasourceId: 数据源ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DatasourceId: str
+        :param _TableId: 表ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TableId: str
+        :param _ColumnName: 字段名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ColumnName: str
+        :param _ColumnNameCn: 字段中文名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ColumnNameCn: str
+        :param _ColumnType: 字段类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ColumnType: str
+        :param _RelationParams: 关系参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RelationParams: str
+        :param _Params: 参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Params: str
+        :param _ParentId: 父id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParentId: str
+        :param _MetastoreType: 元数据类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MetastoreType: str
+        :param _MetastoreTypeName: 元数据类型名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MetastoreTypeName: str
+        :param _TableName: 表名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TableName: str
+        :param _QualifiedName: 字段全名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QualifiedName: str
+        :param _DownStreamCount: 下游节点数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DownStreamCount: int
+        :param _UpStreamCount: 上游节点数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpStreamCount: int
+        :param _Description: 描述信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param _CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param _ModifyTime: 更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModifyTime: str
+        :param _Tasks: 任务id列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tasks: list of str
+        :param _ParentSet: 父节点列表字符串
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParentSet: str
+        :param _ChildSet: 子节点列表字符串
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ChildSet: str
+        :param _ExtParams: 额外参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExtParams: list of LineageParamRecord
+        """
+        self._Id = None
+        self._PrefixPath = None
+        self._DatasourceId = None
+        self._TableId = None
+        self._ColumnName = None
+        self._ColumnNameCn = None
+        self._ColumnType = None
+        self._RelationParams = None
+        self._Params = None
+        self._ParentId = None
+        self._MetastoreType = None
+        self._MetastoreTypeName = None
+        self._TableName = None
+        self._QualifiedName = None
+        self._DownStreamCount = None
+        self._UpStreamCount = None
+        self._Description = None
+        self._CreateTime = None
+        self._ModifyTime = None
+        self._Tasks = None
+        self._ParentSet = None
+        self._ChildSet = None
+        self._ExtParams = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def PrefixPath(self):
+        return self._PrefixPath
+
+    @PrefixPath.setter
+    def PrefixPath(self, PrefixPath):
+        self._PrefixPath = PrefixPath
+
+    @property
+    def DatasourceId(self):
+        return self._DatasourceId
+
+    @DatasourceId.setter
+    def DatasourceId(self, DatasourceId):
+        self._DatasourceId = DatasourceId
+
+    @property
+    def TableId(self):
+        return self._TableId
+
+    @TableId.setter
+    def TableId(self, TableId):
+        self._TableId = TableId
+
+    @property
+    def ColumnName(self):
+        return self._ColumnName
+
+    @ColumnName.setter
+    def ColumnName(self, ColumnName):
+        self._ColumnName = ColumnName
+
+    @property
+    def ColumnNameCn(self):
+        return self._ColumnNameCn
+
+    @ColumnNameCn.setter
+    def ColumnNameCn(self, ColumnNameCn):
+        self._ColumnNameCn = ColumnNameCn
+
+    @property
+    def ColumnType(self):
+        return self._ColumnType
+
+    @ColumnType.setter
+    def ColumnType(self, ColumnType):
+        self._ColumnType = ColumnType
+
+    @property
+    def RelationParams(self):
+        return self._RelationParams
+
+    @RelationParams.setter
+    def RelationParams(self, RelationParams):
+        self._RelationParams = RelationParams
+
+    @property
+    def Params(self):
+        return self._Params
+
+    @Params.setter
+    def Params(self, Params):
+        self._Params = Params
+
+    @property
+    def ParentId(self):
+        return self._ParentId
+
+    @ParentId.setter
+    def ParentId(self, ParentId):
+        self._ParentId = ParentId
+
+    @property
+    def MetastoreType(self):
+        return self._MetastoreType
+
+    @MetastoreType.setter
+    def MetastoreType(self, MetastoreType):
+        self._MetastoreType = MetastoreType
+
+    @property
+    def MetastoreTypeName(self):
+        return self._MetastoreTypeName
+
+    @MetastoreTypeName.setter
+    def MetastoreTypeName(self, MetastoreTypeName):
+        self._MetastoreTypeName = MetastoreTypeName
+
+    @property
+    def TableName(self):
+        return self._TableName
+
+    @TableName.setter
+    def TableName(self, TableName):
+        self._TableName = TableName
+
+    @property
+    def QualifiedName(self):
+        return self._QualifiedName
+
+    @QualifiedName.setter
+    def QualifiedName(self, QualifiedName):
+        self._QualifiedName = QualifiedName
+
+    @property
+    def DownStreamCount(self):
+        return self._DownStreamCount
+
+    @DownStreamCount.setter
+    def DownStreamCount(self, DownStreamCount):
+        self._DownStreamCount = DownStreamCount
+
+    @property
+    def UpStreamCount(self):
+        return self._UpStreamCount
+
+    @UpStreamCount.setter
+    def UpStreamCount(self, UpStreamCount):
+        self._UpStreamCount = UpStreamCount
+
+    @property
+    def Description(self):
+        return self._Description
+
+    @Description.setter
+    def Description(self, Description):
+        self._Description = Description
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def ModifyTime(self):
+        return self._ModifyTime
+
+    @ModifyTime.setter
+    def ModifyTime(self, ModifyTime):
+        self._ModifyTime = ModifyTime
+
+    @property
+    def Tasks(self):
+        return self._Tasks
+
+    @Tasks.setter
+    def Tasks(self, Tasks):
+        self._Tasks = Tasks
+
+    @property
+    def ParentSet(self):
+        return self._ParentSet
+
+    @ParentSet.setter
+    def ParentSet(self, ParentSet):
+        self._ParentSet = ParentSet
+
+    @property
+    def ChildSet(self):
+        return self._ChildSet
+
+    @ChildSet.setter
+    def ChildSet(self, ChildSet):
+        self._ChildSet = ChildSet
+
+    @property
+    def ExtParams(self):
+        return self._ExtParams
+
+    @ExtParams.setter
+    def ExtParams(self, ExtParams):
+        self._ExtParams = ExtParams
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._PrefixPath = params.get("PrefixPath")
+        self._DatasourceId = params.get("DatasourceId")
+        self._TableId = params.get("TableId")
+        self._ColumnName = params.get("ColumnName")
+        self._ColumnNameCn = params.get("ColumnNameCn")
+        self._ColumnType = params.get("ColumnType")
+        self._RelationParams = params.get("RelationParams")
+        self._Params = params.get("Params")
+        self._ParentId = params.get("ParentId")
+        self._MetastoreType = params.get("MetastoreType")
+        self._MetastoreTypeName = params.get("MetastoreTypeName")
+        self._TableName = params.get("TableName")
+        self._QualifiedName = params.get("QualifiedName")
+        self._DownStreamCount = params.get("DownStreamCount")
+        self._UpStreamCount = params.get("UpStreamCount")
+        self._Description = params.get("Description")
+        self._CreateTime = params.get("CreateTime")
+        self._ModifyTime = params.get("ModifyTime")
+        self._Tasks = params.get("Tasks")
+        self._ParentSet = params.get("ParentSet")
+        self._ChildSet = params.get("ChildSet")
+        if params.get("ExtParams") is not None:
+            self._ExtParams = []
+            for item in params.get("ExtParams"):
+                obj = LineageParamRecord()
+                obj._deserialize(item)
+                self._ExtParams.append(obj)
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
 class CommitExportTaskRequest(AbstractModel):
     """CommitExportTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -9586,14 +10015,154 @@
             for item in params.get("Namespaces"):
                 obj = Namespace()
                 obj._deserialize(item)
                 self._Namespaces.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeColumnLineageRequest(AbstractModel):
+    """DescribeColumnLineage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Direction: 查询方向，INPUT,OUTPUT,BOTH枚举值
+        :type Direction: str
+        :param _Data: 字段信息
+        :type Data: :class:`tencentcloud.wedata.v20210820.models.ColumnLineageInfo`
+        :param _InputDepth: 单次查询入度
+        :type InputDepth: int
+        :param _OutputDepth: 单次查询出度
+        :type OutputDepth: int
+        :param _ExtParams: 额外参数（传递调用方信息）
+        :type ExtParams: list of RecordField
+        :param _IgnoreTemp: 是否过滤临时表 默认值为true
+        :type IgnoreTemp: bool
+        """
+        self._Direction = None
+        self._Data = None
+        self._InputDepth = None
+        self._OutputDepth = None
+        self._ExtParams = None
+        self._IgnoreTemp = None
+
+    @property
+    def Direction(self):
+        return self._Direction
+
+    @Direction.setter
+    def Direction(self, Direction):
+        self._Direction = Direction
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def InputDepth(self):
+        return self._InputDepth
+
+    @InputDepth.setter
+    def InputDepth(self, InputDepth):
+        self._InputDepth = InputDepth
+
+    @property
+    def OutputDepth(self):
+        return self._OutputDepth
+
+    @OutputDepth.setter
+    def OutputDepth(self, OutputDepth):
+        self._OutputDepth = OutputDepth
+
+    @property
+    def ExtParams(self):
+        return self._ExtParams
+
+    @ExtParams.setter
+    def ExtParams(self, ExtParams):
+        self._ExtParams = ExtParams
+
+    @property
+    def IgnoreTemp(self):
+        return self._IgnoreTemp
+
+    @IgnoreTemp.setter
+    def IgnoreTemp(self, IgnoreTemp):
+        self._IgnoreTemp = IgnoreTemp
+
+
+    def _deserialize(self, params):
+        self._Direction = params.get("Direction")
+        if params.get("Data") is not None:
+            self._Data = ColumnLineageInfo()
+            self._Data._deserialize(params.get("Data"))
+        self._InputDepth = params.get("InputDepth")
+        self._OutputDepth = params.get("OutputDepth")
+        if params.get("ExtParams") is not None:
+            self._ExtParams = []
+            for item in params.get("ExtParams"):
+                obj = RecordField()
+                obj._deserialize(item)
+                self._ExtParams.append(obj)
+        self._IgnoreTemp = params.get("IgnoreTemp")
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
+class DescribeColumnLineageResponse(AbstractModel):
+    """DescribeColumnLineage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ColumnAggregationLineage: 字段血缘信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ColumnAggregationLineage: :class:`tencentcloud.wedata.v20210820.models.ColumnAggregationLineage`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._ColumnAggregationLineage = None
+        self._RequestId = None
+
+    @property
+    def ColumnAggregationLineage(self):
+        return self._ColumnAggregationLineage
+
+    @ColumnAggregationLineage.setter
+    def ColumnAggregationLineage(self, ColumnAggregationLineage):
+        self._ColumnAggregationLineage = ColumnAggregationLineage
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
+        if params.get("ColumnAggregationLineage") is not None:
+            self._ColumnAggregationLineage = ColumnAggregationLineage()
+            self._ColumnAggregationLineage._deserialize(params.get("ColumnAggregationLineage"))
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeDataBasesRequest(AbstractModel):
     """DescribeDataBases请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -18654,14 +19223,154 @@
             for item in params.get("TableInfo"):
                 obj = TableInfo()
                 obj._deserialize(item)
                 self._TableInfo.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeTableLineageRequest(AbstractModel):
+    """DescribeTableLineage请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Direction: 查询方向，INPUT,OUTPUT,BOTH枚举值
+        :type Direction: str
+        :param _Data: 表信息
+        :type Data: :class:`tencentcloud.wedata.v20210820.models.TableLineageInfo`
+        :param _InputDepth: 单次查询入度,默认 1
+        :type InputDepth: int
+        :param _OutputDepth: 单次查询出度,默认 1
+        :type OutputDepth: int
+        :param _ExtParams: 额外参数（传递调用方信息）
+        :type ExtParams: list of LineageParamRecord
+        :param _IgnoreTemp: 是否过滤临时表,默认true
+        :type IgnoreTemp: bool
+        """
+        self._Direction = None
+        self._Data = None
+        self._InputDepth = None
+        self._OutputDepth = None
+        self._ExtParams = None
+        self._IgnoreTemp = None
+
+    @property
+    def Direction(self):
+        return self._Direction
+
+    @Direction.setter
+    def Direction(self, Direction):
+        self._Direction = Direction
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def InputDepth(self):
+        return self._InputDepth
+
+    @InputDepth.setter
+    def InputDepth(self, InputDepth):
+        self._InputDepth = InputDepth
+
+    @property
+    def OutputDepth(self):
+        return self._OutputDepth
+
+    @OutputDepth.setter
+    def OutputDepth(self, OutputDepth):
+        self._OutputDepth = OutputDepth
+
+    @property
+    def ExtParams(self):
+        return self._ExtParams
+
+    @ExtParams.setter
+    def ExtParams(self, ExtParams):
+        self._ExtParams = ExtParams
+
+    @property
+    def IgnoreTemp(self):
+        return self._IgnoreTemp
+
+    @IgnoreTemp.setter
+    def IgnoreTemp(self, IgnoreTemp):
+        self._IgnoreTemp = IgnoreTemp
+
+
+    def _deserialize(self, params):
+        self._Direction = params.get("Direction")
+        if params.get("Data") is not None:
+            self._Data = TableLineageInfo()
+            self._Data._deserialize(params.get("Data"))
+        self._InputDepth = params.get("InputDepth")
+        self._OutputDepth = params.get("OutputDepth")
+        if params.get("ExtParams") is not None:
+            self._ExtParams = []
+            for item in params.get("ExtParams"):
+                obj = LineageParamRecord()
+                obj._deserialize(item)
+                self._ExtParams.append(obj)
+        self._IgnoreTemp = params.get("IgnoreTemp")
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
+class DescribeTableLineageResponse(AbstractModel):
+    """DescribeTableLineage返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TableLineage: 表血缘信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TableLineage: :class:`tencentcloud.wedata.v20210820.models.TableLineageInfo`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TableLineage = None
+        self._RequestId = None
+
+    @property
+    def TableLineage(self):
+        return self._TableLineage
+
+    @TableLineage.setter
+    def TableLineage(self, TableLineage):
+        self._TableLineage = TableLineage
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
+        if params.get("TableLineage") is not None:
+            self._TableLineage = TableLineageInfo()
+            self._TableLineage._deserialize(params.get("TableLineage"))
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeTableQualityDetailsRequest(AbstractModel):
     """DescribeTableQualityDetails请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -26206,14 +26915,60 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class LineageParamRecord(AbstractModel):
+    """血缘参数记录
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Name: 字段名
+        :type Name: str
+        :param _Value: 字段值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Value: str
+        """
+        self._Name = None
+        self._Value = None
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def Value(self):
+        return self._Value
+
+    @Value.setter
+    def Value(self, Value):
+        self._Value = Value
+
+
+    def _deserialize(self, params):
+        self._Name = params.get("Name")
+        self._Value = params.get("Value")
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
 class LockIntegrationTaskRequest(AbstractModel):
     """LockIntegrationTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -37131,14 +37886,230 @@
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self._Data = BatchOperateResult()
             self._Data._deserialize(params.get("Data"))
         self._RequestId = params.get("RequestId")
 
 
+class SimpleColumnInfo(AbstractModel):
+    """血缘列描述
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: 列ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param _QualifiedName: 限定名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QualifiedName: str
+        :param _ColumnName: 列名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ColumnName: str
+        :param _ColumnNameCn: 列中文名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ColumnNameCn: str
+        :param _ColumnType: 列类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ColumnType: str
+        :param _Description: 列描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param _PrefixPath: 前缀路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PrefixPath: str
+        :param _CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param _ModifyTime: 修改时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModifyTime: str
+        :param _DatasourceId: 数据源ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DatasourceId: str
+        :param _DownStreamCount: 下游数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DownStreamCount: int
+        :param _UpStreamCount: 上游数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpStreamCount: int
+        :param _RelationParams: 关系参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RelationParams: str
+        :param _Params: 参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Params: str
+        :param _Tasks: 任务集合
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tasks: list of str
+        """
+        self._Id = None
+        self._QualifiedName = None
+        self._ColumnName = None
+        self._ColumnNameCn = None
+        self._ColumnType = None
+        self._Description = None
+        self._PrefixPath = None
+        self._CreateTime = None
+        self._ModifyTime = None
+        self._DatasourceId = None
+        self._DownStreamCount = None
+        self._UpStreamCount = None
+        self._RelationParams = None
+        self._Params = None
+        self._Tasks = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def QualifiedName(self):
+        return self._QualifiedName
+
+    @QualifiedName.setter
+    def QualifiedName(self, QualifiedName):
+        self._QualifiedName = QualifiedName
+
+    @property
+    def ColumnName(self):
+        return self._ColumnName
+
+    @ColumnName.setter
+    def ColumnName(self, ColumnName):
+        self._ColumnName = ColumnName
+
+    @property
+    def ColumnNameCn(self):
+        return self._ColumnNameCn
+
+    @ColumnNameCn.setter
+    def ColumnNameCn(self, ColumnNameCn):
+        self._ColumnNameCn = ColumnNameCn
+
+    @property
+    def ColumnType(self):
+        return self._ColumnType
+
+    @ColumnType.setter
+    def ColumnType(self, ColumnType):
+        self._ColumnType = ColumnType
+
+    @property
+    def Description(self):
+        return self._Description
+
+    @Description.setter
+    def Description(self, Description):
+        self._Description = Description
+
+    @property
+    def PrefixPath(self):
+        return self._PrefixPath
+
+    @PrefixPath.setter
+    def PrefixPath(self, PrefixPath):
+        self._PrefixPath = PrefixPath
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def ModifyTime(self):
+        return self._ModifyTime
+
+    @ModifyTime.setter
+    def ModifyTime(self, ModifyTime):
+        self._ModifyTime = ModifyTime
+
+    @property
+    def DatasourceId(self):
+        return self._DatasourceId
+
+    @DatasourceId.setter
+    def DatasourceId(self, DatasourceId):
+        self._DatasourceId = DatasourceId
+
+    @property
+    def DownStreamCount(self):
+        return self._DownStreamCount
+
+    @DownStreamCount.setter
+    def DownStreamCount(self, DownStreamCount):
+        self._DownStreamCount = DownStreamCount
+
+    @property
+    def UpStreamCount(self):
+        return self._UpStreamCount
+
+    @UpStreamCount.setter
+    def UpStreamCount(self, UpStreamCount):
+        self._UpStreamCount = UpStreamCount
+
+    @property
+    def RelationParams(self):
+        return self._RelationParams
+
+    @RelationParams.setter
+    def RelationParams(self, RelationParams):
+        self._RelationParams = RelationParams
+
+    @property
+    def Params(self):
+        return self._Params
+
+    @Params.setter
+    def Params(self, Params):
+        self._Params = Params
+
+    @property
+    def Tasks(self):
+        return self._Tasks
+
+    @Tasks.setter
+    def Tasks(self, Tasks):
+        self._Tasks = Tasks
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._QualifiedName = params.get("QualifiedName")
+        self._ColumnName = params.get("ColumnName")
+        self._ColumnNameCn = params.get("ColumnNameCn")
+        self._ColumnType = params.get("ColumnType")
+        self._Description = params.get("Description")
+        self._PrefixPath = params.get("PrefixPath")
+        self._CreateTime = params.get("CreateTime")
+        self._ModifyTime = params.get("ModifyTime")
+        self._DatasourceId = params.get("DatasourceId")
+        self._DownStreamCount = params.get("DownStreamCount")
+        self._UpStreamCount = params.get("UpStreamCount")
+        self._RelationParams = params.get("RelationParams")
+        self._Params = params.get("Params")
+        self._Tasks = params.get("Tasks")
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
 class SimpleTaskInfo(AbstractModel):
     """简单Task信息
 
     """
 
     def __init__(self):
         r"""
@@ -38489,14 +39460,292 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TableLineageInfo(AbstractModel):
+    """表血缘详细信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _MetastoreType: 元数据类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MetastoreType: str
+        :param _PrefixPath: 由中心节点到该节点的路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PrefixPath: str
+        :param _ProjectId: 空间id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProjectId: str
+        :param _DatasourceId: 数据源id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DatasourceId: str
+        :param _TableId: 表id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TableId: str
+        :param _Params: 表血缘参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Params: list of LineageParamRecord
+        :param _ParentSet: 父节点列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParentSet: str
+        :param _ChildSet: 子节点列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ChildSet: str
+        :param _ExtParams: 额外参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExtParams: list of RecordField
+        :param _Id: 血缘id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param _MetastoreTypeName: 元数据类型名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MetastoreTypeName: str
+        :param _TableName: 表名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TableName: str
+        :param _QualifiedName: 表全称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QualifiedName: str
+        :param _DownStreamCount: 血缘下游节点数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DownStreamCount: int
+        :param _UpStreamCount: 血缘上游节点数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpStreamCount: int
+        :param _Description: 血缘描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Description: str
+        :param _CreateTime: 血缘创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param _ModifyTime: 血缘更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModifyTime: str
+        :param _Tasks: 修改血缘的任务id列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Tasks: list of str
+        """
+        self._MetastoreType = None
+        self._PrefixPath = None
+        self._ProjectId = None
+        self._DatasourceId = None
+        self._TableId = None
+        self._Params = None
+        self._ParentSet = None
+        self._ChildSet = None
+        self._ExtParams = None
+        self._Id = None
+        self._MetastoreTypeName = None
+        self._TableName = None
+        self._QualifiedName = None
+        self._DownStreamCount = None
+        self._UpStreamCount = None
+        self._Description = None
+        self._CreateTime = None
+        self._ModifyTime = None
+        self._Tasks = None
+
+    @property
+    def MetastoreType(self):
+        return self._MetastoreType
+
+    @MetastoreType.setter
+    def MetastoreType(self, MetastoreType):
+        self._MetastoreType = MetastoreType
+
+    @property
+    def PrefixPath(self):
+        return self._PrefixPath
+
+    @PrefixPath.setter
+    def PrefixPath(self, PrefixPath):
+        self._PrefixPath = PrefixPath
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def DatasourceId(self):
+        return self._DatasourceId
+
+    @DatasourceId.setter
+    def DatasourceId(self, DatasourceId):
+        self._DatasourceId = DatasourceId
+
+    @property
+    def TableId(self):
+        return self._TableId
+
+    @TableId.setter
+    def TableId(self, TableId):
+        self._TableId = TableId
+
+    @property
+    def Params(self):
+        return self._Params
+
+    @Params.setter
+    def Params(self, Params):
+        self._Params = Params
+
+    @property
+    def ParentSet(self):
+        return self._ParentSet
+
+    @ParentSet.setter
+    def ParentSet(self, ParentSet):
+        self._ParentSet = ParentSet
+
+    @property
+    def ChildSet(self):
+        return self._ChildSet
+
+    @ChildSet.setter
+    def ChildSet(self, ChildSet):
+        self._ChildSet = ChildSet
+
+    @property
+    def ExtParams(self):
+        return self._ExtParams
+
+    @ExtParams.setter
+    def ExtParams(self, ExtParams):
+        self._ExtParams = ExtParams
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def MetastoreTypeName(self):
+        return self._MetastoreTypeName
+
+    @MetastoreTypeName.setter
+    def MetastoreTypeName(self, MetastoreTypeName):
+        self._MetastoreTypeName = MetastoreTypeName
+
+    @property
+    def TableName(self):
+        return self._TableName
+
+    @TableName.setter
+    def TableName(self, TableName):
+        self._TableName = TableName
+
+    @property
+    def QualifiedName(self):
+        return self._QualifiedName
+
+    @QualifiedName.setter
+    def QualifiedName(self, QualifiedName):
+        self._QualifiedName = QualifiedName
+
+    @property
+    def DownStreamCount(self):
+        return self._DownStreamCount
+
+    @DownStreamCount.setter
+    def DownStreamCount(self, DownStreamCount):
+        self._DownStreamCount = DownStreamCount
+
+    @property
+    def UpStreamCount(self):
+        return self._UpStreamCount
+
+    @UpStreamCount.setter
+    def UpStreamCount(self, UpStreamCount):
+        self._UpStreamCount = UpStreamCount
+
+    @property
+    def Description(self):
+        return self._Description
+
+    @Description.setter
+    def Description(self, Description):
+        self._Description = Description
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def ModifyTime(self):
+        return self._ModifyTime
+
+    @ModifyTime.setter
+    def ModifyTime(self, ModifyTime):
+        self._ModifyTime = ModifyTime
+
+    @property
+    def Tasks(self):
+        return self._Tasks
+
+    @Tasks.setter
+    def Tasks(self, Tasks):
+        self._Tasks = Tasks
+
+
+    def _deserialize(self, params):
+        self._MetastoreType = params.get("MetastoreType")
+        self._PrefixPath = params.get("PrefixPath")
+        self._ProjectId = params.get("ProjectId")
+        self._DatasourceId = params.get("DatasourceId")
+        self._TableId = params.get("TableId")
+        if params.get("Params") is not None:
+            self._Params = []
+            for item in params.get("Params"):
+                obj = LineageParamRecord()
+                obj._deserialize(item)
+                self._Params.append(obj)
+        self._ParentSet = params.get("ParentSet")
+        self._ChildSet = params.get("ChildSet")
+        if params.get("ExtParams") is not None:
+            self._ExtParams = []
+            for item in params.get("ExtParams"):
+                obj = RecordField()
+                obj._deserialize(item)
+                self._ExtParams.append(obj)
+        self._Id = params.get("Id")
+        self._MetastoreTypeName = params.get("MetastoreTypeName")
+        self._TableName = params.get("TableName")
+        self._QualifiedName = params.get("QualifiedName")
+        self._DownStreamCount = params.get("DownStreamCount")
+        self._UpStreamCount = params.get("UpStreamCount")
+        self._Description = params.get("Description")
+        self._CreateTime = params.get("CreateTime")
+        self._ModifyTime = params.get("ModifyTime")
+        self._Tasks = params.get("Tasks")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class TableQualityDetail(AbstractModel):
     """表质量详情
 
     """
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1320,14 +1320,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeColumnLineage(self, request):
+        """列出字段血缘信息
+
+        :param request: Request instance for DescribeColumnLineage.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeColumnLineageRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeColumnLineageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeColumnLineage", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeColumnLineageResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeDataBases(self, request):
         """查询数据来源列表
 
         :param request: Request instance for DescribeDataBases.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDataBasesRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeDataBasesResponse`
 
@@ -3076,14 +3099,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeTableLineage(self, request):
+        """列出表血缘信息
+
+        :param request: Request instance for DescribeTableLineage.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTableLineageRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeTableLineageResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeTableLineage", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeTableLineageResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeTableQualityDetails(self, request):
         """质量报告-查询表质量详情
 
         :param request: Request instance for DescribeTableQualityDetails.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeTableQualityDetailsRequest`
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.932/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wedata-3.0.933/tencentcloud/__init__.py`

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

