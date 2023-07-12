# Comparing `tmp/pyathena-3.0.4.tar.gz` & `tmp/pyathena-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyathena-3.0.4.tar", max compression
+gzip compressed data, was "pyathena-3.0.5.tar", max compression
```

## Comparing `pyathena-3.0.4.tar` & `pyathena-3.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1055 2023-06-29 14:51:30.473008 pyathena-3.0.4/LICENSE
--rw-r--r--   0        0        0    70055 2023-06-29 14:51:30.473008 pyathena-3.0.4/README.rst
--rw-r--r--   0        0        0     1959 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/__init__.py
--rw-r--r--   0        0        0       24 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     5193 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2590 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     7250 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9791 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2457 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/util.py
--rw-r--r--   0        0        0     5409 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/async_cursor.py
--rw-r--r--   0        0        0    21206 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/common.py
--rw-r--r--   0        0        0    10452 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/connection.py
--rw-r--r--   0        0        0     4245 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/converter.py
--rw-r--r--   0        0        0     5835 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/cursor.py
--rw-r--r--   0        0        0      660 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/error.py
--rw-r--r--   0        0        0       24 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/fastparquet/__init__.py
--rw-r--r--   0        0        0     2475 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/fastparquet/util.py
--rw-r--r--   0        0        0       24 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/filesystem/__init__.py
--rw-r--r--   0        0        0    20510 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/filesystem/s3.py
--rw-r--r--   0        0        0     1252 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/filesystem/s3_object.py
--rw-r--r--   0        0        0     6571 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/formatter.py
--rw-r--r--   0        0        0    17121 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/model.py
--rw-r--r--   0        0        0      220 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5865 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1866 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     8327 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    13625 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0     9858 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/util.py
--rw-r--r--   0        0        0        0 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/py.typed
--rw-r--r--   0        0        0    25140 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/result_set.py
--rw-r--r--   0        0        0       24 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      661 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/arrow.py
--rw-r--r--   0        0        0    37022 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/base.py
--rw-r--r--   0        0        0      884 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/pandas.py
--rw-r--r--   0        0        0     2638 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      173 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/rest.py
--rw-r--r--   0        0        0     1246 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/types.py
--rw-r--r--   0        0        0      142 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/util.py
--rw-r--r--   0        0        0     1984 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/util.py
--rw-r--r--   0        0        0     3482 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyproject.toml
--rw-r--r--   0        0        0    71294 1970-01-01 00:00:00.000000 pyathena-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-12 05:00:18.290483 pyathena-3.0.5/LICENSE
+-rw-r--r--   0        0        0    71913 2023-07-12 05:00:18.290483 pyathena-3.0.5/README.rst
+-rw-r--r--   0        0        0     1959 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     5193 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2590 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     7250 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9791 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2457 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/arrow/util.py
+-rw-r--r--   0        0        0     5409 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    21206 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/common.py
+-rw-r--r--   0        0        0    10452 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/connection.py
+-rw-r--r--   0        0        0     4245 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/converter.py
+-rw-r--r--   0        0        0     5835 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/cursor.py
+-rw-r--r--   0        0        0      660 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/error.py
+-rw-r--r--   0        0        0       24 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2475 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    20510 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0     1252 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0     6571 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/formatter.py
+-rw-r--r--   0        0        0    17910 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/model.py
+-rw-r--r--   0        0        0      220 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5865 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1866 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     8327 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13625 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0     9858 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/pandas/util.py
+-rw-r--r--   0        0        0        0 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/py.typed
+-rw-r--r--   0        0        0    25140 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/result_set.py
+-rw-r--r--   0        0        0       24 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    39146 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      884 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2638 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1246 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0     1984 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyathena/util.py
+-rw-r--r--   0        0        0     3482 2023-07-12 05:00:18.294483 pyathena-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0    73152 1970-01-01 00:00:00.000000 pyathena-3.0.5/PKG-INFO
```

### Comparing `pyathena-3.0.4/LICENSE` & `pyathena-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/README.rst` & `pyathena-3.0.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -314,27 +314,76 @@
         Specifies a key for partitioning data.
     Value:
         True / False
     Example:
         .. code:: python
 
             Column("some_column", types.String, ..., awsathena_partition=True)
+
+partition_transform
+    Type:
+        str
+    Description:
+        Specifies a partition transform function for partitioning data.
+        Only has an effect for ICEBERG tables and when partition is set to true for the column.
+    Value:
+        * year
+        * month
+        * day
+        * hour
+        * bucket
+        * truncate
+    Example:
+        .. code:: python
+
+            Column("some_column", types.Date, ..., awsathena_partition=True, awsathena_partition_transform='year')
+
+partition_transform_bucket_count
+    Type:
+        int
+    Description:
+        Used for N in the bucket partition transform function, partitions by hashed value mod N buckets.
+        Only has an effect for ICEBERG tables and when partition is set to true and
+        when the partition transform is set to 'bucket' for the column.
+    Value:
+        Integer value greater than or equal to 0
+    Example:
+        .. code:: python
+
+            Column("some_column", types.String, ..., awsathena_partition=True, awsathena_partition_transform='bucket', awsathena_partition_transform_bucket_count=5)
+
+partition_transform_truncate_length
+    Type:
+        int
+    Description:
+        Used for L in the truncate partition transform function, partitions by value truncated to L.
+        Only has an effect for ICEBERG tables and when partition is set to true and
+        when the partition transform is set to 'truncate' for the column.
+    Value:
+        Integer value greater than or equal to 0
+    Example:
+        .. code:: python
+
+            Column("some_column", types.String, ..., awsathena_partition=True, awsathena_partition_transform='truncate', awsathena_partition_transform_truncate_length=5)
+
 cluster
     Type:
         bool
     Description:
         Divides the data in the specified column into data subsets called buckets, with or without partitioning.
     Value:
         True / False
     Example:
         .. code:: python
 
             Column("some_column", types.String, ..., awsathena_cluster=True)
 
 To configure column options from the connection string, specify the column name as a comma-separated string.
+The options partition_transform, partition_transform_bucket_count, partition_transform_truncate_length are not supported
+to be configured from the connection string.
 
 .. code:: text
 
     awsathena+rest://:@athena.us-west-2.amazonaws.com:443/default?partition=column1%2Ccolumn2&cluster=column1%2Ccolumn2&...
 
 If you want to limit the column options to specific table names only, specify the table and column names connected by dots as a comma-separated string.
```

### Comparing `pyathena-3.0.4/pyathena/__init__.py` & `pyathena-3.0.5/pyathena/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING, FrozenSet, Type
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection
 
-__version__: str = "3.0.4"
+__version__: str = "3.0.5"
 user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 2
 paramstyle: str = "pyformat"
```

### Comparing `pyathena-3.0.4/pyathena/arrow/async_cursor.py` & `pyathena-3.0.5/pyathena/arrow/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/arrow/converter.py` & `pyathena-3.0.5/pyathena/arrow/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/arrow/cursor.py` & `pyathena-3.0.5/pyathena/arrow/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/arrow/result_set.py` & `pyathena-3.0.5/pyathena/arrow/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/arrow/util.py` & `pyathena-3.0.5/pyathena/arrow/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/async_cursor.py` & `pyathena-3.0.5/pyathena/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/common.py` & `pyathena-3.0.5/pyathena/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/connection.py` & `pyathena-3.0.5/pyathena/connection.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/converter.py` & `pyathena-3.0.5/pyathena/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/cursor.py` & `pyathena-3.0.5/pyathena/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/error.py` & `pyathena-3.0.5/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/fastparquet/util.py` & `pyathena-3.0.5/pyathena/fastparquet/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/filesystem/s3.py` & `pyathena-3.0.5/pyathena/filesystem/s3.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/filesystem/s3_object.py` & `pyathena-3.0.5/pyathena/filesystem/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/formatter.py` & `pyathena-3.0.5/pyathena/formatter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/model.py` & `pyathena-3.0.5/pyathena/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -483,7 +483,27 @@
             AthenaCompression.COMPRESSION_GZIP,
             AthenaCompression.COMPRESSION_LZ4,
             AthenaCompression.COMPRESSION_LZO,
             AthenaCompression.COMPRESSION_SNAPPY,
             AthenaCompression.COMPRESSION_ZLIB,
             AthenaCompression.COMPRESSION_ZSTD,
         ]
+
+
+class AthenaPartitionTransform:
+    PARTITION_TRANSFORM_YEAR: str = "year"
+    PARTITION_TRANSFORM_MONTH: str = "month"
+    PARTITION_TRANSFORM_DAY: str = "day"
+    PARTITION_TRANSFORM_HOUR: str = "hour"
+    PARTITION_TRANSFORM_BUCKET: str = "bucket"
+    PARTITION_TRANSFORM_TRUNCATE: str = "truncate"
+
+    @staticmethod
+    def is_valid(value: str) -> bool:
+        return value.lower() in [
+            AthenaPartitionTransform.PARTITION_TRANSFORM_YEAR,
+            AthenaPartitionTransform.PARTITION_TRANSFORM_MONTH,
+            AthenaPartitionTransform.PARTITION_TRANSFORM_DAY,
+            AthenaPartitionTransform.PARTITION_TRANSFORM_HOUR,
+            AthenaPartitionTransform.PARTITION_TRANSFORM_BUCKET,
+            AthenaPartitionTransform.PARTITION_TRANSFORM_TRUNCATE,
+        ]
```

### Comparing `pyathena-3.0.4/pyathena/pandas/async_cursor.py` & `pyathena-3.0.5/pyathena/pandas/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/pandas/converter.py` & `pyathena-3.0.5/pyathena/pandas/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/pandas/cursor.py` & `pyathena-3.0.5/pyathena/pandas/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/pandas/result_set.py` & `pyathena-3.0.5/pyathena/pandas/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/pandas/util.py` & `pyathena-3.0.5/pyathena/pandas/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/result_set.py` & `pyathena-3.0.5/pyathena/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/sqlalchemy/arrow.py` & `pyathena-3.0.5/pyathena/sqlalchemy/arrow.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/sqlalchemy/base.py` & `pyathena-3.0.5/pyathena/sqlalchemy/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,19 @@
     DDLCompiler,
     GenericTypeCompiler,
     IdentifierPreparer,
     SQLCompiler,
 )
 
 import pyathena
-from pyathena.model import AthenaFileFormat, AthenaRowFormatSerde
+from pyathena.model import (
+    AthenaFileFormat,
+    AthenaPartitionTransform,
+    AthenaRowFormatSerde,
+)
 from pyathena.sqlalchemy.types import AthenaDate, AthenaTimestamp
 from pyathena.sqlalchemy.util import _HashableDict
 
 if TYPE_CHECKING:
     from types import ModuleType
 
     from sqlalchemy import (
@@ -768,16 +772,46 @@
         if connect_opts:
             bucket = cast(str, connect_opts.get("cluster"))
             buckets = bucket.split(",") if bucket else []
         else:
             buckets = []
         return buckets
 
+    def _prepared_partitions(self, column):
+        # https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-creating-tables.html#querying-iceberg-partitioning
+        column_dialect_opts = column.dialect_options["awsathena"]
+        partition_transform = column_dialect_opts["partition_transform"]
+
+        column_name = self.preparer.format_column(column)
+        transform_column = None
+
+        partitions = []
+
+        if partition_transform:
+            if AthenaPartitionTransform.is_valid(partition_transform):
+                if partition_transform == AthenaPartitionTransform.PARTITION_TRANSFORM_BUCKET:
+                    bucket_count = column_dialect_opts["partition_transform_bucket_count"]
+                    if bucket_count:
+                        transform_column = f"{bucket_count}, {column_name}"
+                elif partition_transform == AthenaPartitionTransform.PARTITION_TRANSFORM_TRUNCATE:
+                    truncate_length = column_dialect_opts["partition_transform_truncate_length"]
+                    if truncate_length:
+                        transform_column = f"{truncate_length}, {column_name}"
+                else:
+                    transform_column = column_name
+
+                if transform_column:
+                    partitions.append(f"\t{partition_transform}({transform_column})")
+        else:
+            partitions.append(f"\t{column_name}")
+
+        return partitions
+
     def _prepared_columns(
-        self, table, create_columns: List["CreateColumn"], connect_opts: Dict[str, Any]
+        self, table, is_iceberg, create_columns: List["CreateColumn"], connect_opts: Dict[str, Any]
     ) -> Tuple[List[str], List[str], List[str]]:
         columns, partitions, buckets = [], [], []
         conn_partitions = self._get_connect_option_partitions(connect_opts)
         conn_buckets = self._get_connect_option_buckets(connect_opts)
         for create_column in create_columns:
             column = create_column.element
             column_dialect_opts = column.dialect_options["awsathena"]
@@ -785,15 +819,20 @@
                 processed = self.process(create_column)
                 if processed is not None:
                     if (
                         column_dialect_opts["partition"]
                         or column.name in conn_partitions
                         or f"{table.name}.{column.name}" in conn_partitions
                     ):
-                        partitions.append(f"\t{processed}")
+                        # https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-creating-tables.html#querying-iceberg-partitioning
+                        if is_iceberg:
+                            partitions.extend(self._prepared_partitions(column=column))
+                            columns.append(f"\t{processed}")
+                        else:
+                            partitions.append(f"\t{processed}")
                     else:
                         columns.append(f"\t{processed}")
                     if (
                         column_dialect_opts["cluster"]
                         or column.name in conn_buckets
                         or f"{table.name}.{column.name}" in conn_buckets
                     ):
@@ -809,27 +848,33 @@
         dialect_opts = table.dialect_options["awsathena"]
         dialect = cast(AthenaDialect, self.dialect)
         connect_opts = dialect._connect_options
 
         table_properties = self._get_table_properties_specification(
             dialect_opts, connect_opts
         ).lower()
+        is_iceberg = False
         if ("table_type" in table_properties) and ("iceberg" in table_properties):
+            is_iceberg = True
+
+        if is_iceberg:
             # https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg-creating-tables.html
             text = ["\nCREATE TABLE"]
         else:
             text = ["\nCREATE EXTERNAL TABLE"]
 
         if create.if_not_exists:
             text.append("IF NOT EXISTS")
         text.append(self.preparer.format_table(table))
         text.append("(")
         text = [" ".join(text)]
 
-        columns, partitions, buckets = self._prepared_columns(table, create.columns, connect_opts)
+        columns, partitions, buckets = self._prepared_columns(
+            table, is_iceberg, create.columns, connect_opts
+        )
         text.append(",\n".join(columns))
         text.append(")")
 
         if table.comment:
             text.append(self._get_comment_specification(table.comment))
 
         if partitions:
@@ -896,14 +941,17 @@
                 "bucket_count": None,
             },
         ),
         (
             schema.Column,
             {
                 "partition": False,
+                "partition_transform": None,
+                "partition_transform_bucket_count": None,
+                "partition_transform_truncate_length": None,
                 "cluster": False,
             },
         ),
     ]
 
     colspecs = {
         types.DATE: AthenaDate,
```

### Comparing `pyathena-3.0.4/pyathena/sqlalchemy/pandas.py` & `pyathena-3.0.5/pyathena/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/sqlalchemy/requirements.py` & `pyathena-3.0.5/pyathena/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/sqlalchemy/types.py` & `pyathena-3.0.5/pyathena/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyathena/util.py` & `pyathena-3.0.5/pyathena/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.4/pyproject.toml` & `pyathena-3.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyAthena"
-version = "3.0.4"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
+version = "3.0.5"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
 description = "Python DB API 2.0 (PEP 249) client for Amazon Athena"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyathena-3.0.4/PKG-INFO` & `pyathena-3.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyathena
-Version: 3.0.4
+Version: 3.0.5
 Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
 Home-page: https://github.com/laughingman7743/PyAthena/
 License: MIT
 Author: laughingman7743
 Author-email: laughingman7743@gmail.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
@@ -347,27 +347,76 @@
         Specifies a key for partitioning data.
     Value:
         True / False
     Example:
         .. code:: python
 
             Column("some_column", types.String, ..., awsathena_partition=True)
+
+partition_transform
+    Type:
+        str
+    Description:
+        Specifies a partition transform function for partitioning data.
+        Only has an effect for ICEBERG tables and when partition is set to true for the column.
+    Value:
+        * year
+        * month
+        * day
+        * hour
+        * bucket
+        * truncate
+    Example:
+        .. code:: python
+
+            Column("some_column", types.Date, ..., awsathena_partition=True, awsathena_partition_transform='year')
+
+partition_transform_bucket_count
+    Type:
+        int
+    Description:
+        Used for N in the bucket partition transform function, partitions by hashed value mod N buckets.
+        Only has an effect for ICEBERG tables and when partition is set to true and
+        when the partition transform is set to 'bucket' for the column.
+    Value:
+        Integer value greater than or equal to 0
+    Example:
+        .. code:: python
+
+            Column("some_column", types.String, ..., awsathena_partition=True, awsathena_partition_transform='bucket', awsathena_partition_transform_bucket_count=5)
+
+partition_transform_truncate_length
+    Type:
+        int
+    Description:
+        Used for L in the truncate partition transform function, partitions by value truncated to L.
+        Only has an effect for ICEBERG tables and when partition is set to true and
+        when the partition transform is set to 'truncate' for the column.
+    Value:
+        Integer value greater than or equal to 0
+    Example:
+        .. code:: python
+
+            Column("some_column", types.String, ..., awsathena_partition=True, awsathena_partition_transform='truncate', awsathena_partition_transform_truncate_length=5)
+
 cluster
     Type:
         bool
     Description:
         Divides the data in the specified column into data subsets called buckets, with or without partitioning.
     Value:
         True / False
     Example:
         .. code:: python
 
             Column("some_column", types.String, ..., awsathena_cluster=True)
 
 To configure column options from the connection string, specify the column name as a comma-separated string.
+The options partition_transform, partition_transform_bucket_count, partition_transform_truncate_length are not supported
+to be configured from the connection string.
 
 .. code:: text
 
     awsathena+rest://:@athena.us-west-2.amazonaws.com:443/default?partition=column1%2Ccolumn2&cluster=column1%2Ccolumn2&...
 
 If you want to limit the column options to specific table names only, specify the table and column names connected by dots as a comma-separated string.
```

