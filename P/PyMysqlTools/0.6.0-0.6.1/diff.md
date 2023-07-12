# Comparing `tmp/PyMysqlTools-0.6.0.tar.gz` & `tmp/PyMysqlTools-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMysqlTools-0.6.0.tar", last modified: Fri Jul  7 10:15:20 2023, max compression
+gzip compressed data, was "PyMysqlTools-0.6.1.tar", last modified: Wed Jul 12 08:28:57 2023, max compression
```

## Comparing `PyMysqlTools-0.6.0.tar` & `PyMysqlTools-0.6.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 10:15:20.916002 PyMysqlTools-0.6.0/
--rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      143 2023-02-06 01:25:52.000000 PyMysqlTools-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2610 2023-07-07 10:15:20.914013 PyMysqlTools-0.6.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-07 10:15:20.905030 PyMysqlTools-0.6.0/PyMysqlTools/
--rw-rw-rw-   0        0        0      432 2023-07-07 10:14:57.000000 PyMysqlTools-0.6.0/PyMysqlTools/__init__.py
--rw-rw-rw-   0        0        0      698 2023-07-07 08:55:05.000000 PyMysqlTools-0.6.0/PyMysqlTools/actuator.py
--rw-rw-rw-   0        0        0     6014 2023-07-07 09:40:25.000000 PyMysqlTools-0.6.0/PyMysqlTools/generator.py
--rw-rw-rw-   0        0        0    26989 2023-07-07 10:14:57.000000 PyMysqlTools-0.6.0/PyMysqlTools/main.py
--rw-rw-rw-   0        0        0     3992 2023-07-07 10:15:18.000000 PyMysqlTools-0.6.0/PyMysqlTools/result_set.py
--rw-rw-rw-   0        0        0       98 2023-07-07 09:32:12.000000 PyMysqlTools-0.6.0/PyMysqlTools/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:15:20.913009 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/
--rw-rw-rw-   0        0        0     2610 2023-07-07 10:15:20.000000 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-07-07 10:15:20.000000 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 10:15:20.000000 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-07 10:15:20.000000 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-07 10:15:20.000000 PyMysqlTools-0.6.0/PyMysqlTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2007 2023-02-06 01:33:20.000000 PyMysqlTools-0.6.0/README.md
--rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 10:15:20.916002 PyMysqlTools-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:28:57.279802 PyMysqlTools-0.6.1/
+-rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-02-06 01:25:52.000000 PyMysqlTools-0.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2610 2023-07-12 08:28:57.278806 PyMysqlTools-0.6.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 08:28:57.258641 PyMysqlTools-0.6.1/PyMysqlTools/
+-rw-rw-rw-   0        0        0      424 2023-07-12 08:26:13.000000 PyMysqlTools-0.6.1/PyMysqlTools/__init__.py
+-rw-rw-rw-   0        0        0      698 2023-07-07 08:55:05.000000 PyMysqlTools-0.6.1/PyMysqlTools/actuator.py
+-rw-rw-rw-   0        0        0      431 2023-07-12 02:25:29.000000 PyMysqlTools-0.6.1/PyMysqlTools/exceptions.py
+-rw-rw-rw-   0        0        0     6039 2023-07-12 06:20:01.000000 PyMysqlTools-0.6.1/PyMysqlTools/generator.py
+-rw-rw-rw-   0        0        0    14182 2023-07-12 03:47:57.000000 PyMysqlTools-0.6.1/PyMysqlTools/main.py
+-rw-rw-rw-   0        0        0     4185 2023-07-11 02:31:54.000000 PyMysqlTools-0.6.1/PyMysqlTools/result_set.py
+-rw-rw-rw-   0        0        0      624 2023-07-12 02:58:20.000000 PyMysqlTools-0.6.1/PyMysqlTools/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-12 08:28:57.277807 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/
+-rw-rw-rw-   0        0        0     2610 2023-07-12 08:28:57.000000 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-07-12 08:28:57.000000 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 08:28:57.000000 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-12 08:28:57.000000 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 08:28:57.000000 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2007 2023-02-06 01:33:20.000000 PyMysqlTools-0.6.1/README.md
+-rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 08:28:57.279802 PyMysqlTools-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.1/setup.py
```

### Comparing `PyMysqlTools-0.6.0/LICENSE` & `PyMysqlTools-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.0/PKG-INFO` & `PyMysqlTools-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
```

### Comparing `PyMysqlTools-0.6.0/PyMysqlTools/actuator.py` & `PyMysqlTools-0.6.1/PyMysqlTools/actuator.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.0/PyMysqlTools/generator.py` & `PyMysqlTools-0.6.1/PyMysqlTools/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from PyMysqlTools.exceptions import TypeMismatchError
+
+
 class SqlGenerator:
 
     def __init__(self):
         self.sql = ""
         self._clause_generator = ClauseGenerator()
 
     def insert_one(self, tb_name, data: dict):
@@ -121,15 +124,15 @@
         if isinstance(data, dict):
             for key, value in data.items():
                 schema.append(f""" `{key}` {value}""")
 
             self.clause = ',\n'.join(schema)
             return self.clause
 
-        raise ValueError('[数据类型错误]', "'schema' 只能是 list/dict 类型")
+        raise TypeMismatchError("'schema' 只能是 list/dict 类型")
 
     def build_where_clause(self, condition):
         condition_str = ''
 
         if not condition:
             return condition_str
 
@@ -139,15 +142,15 @@
                 temp.append(f"""`{k}`='{v}'""")
             condition_str = ' AND '.join(temp)
         elif isinstance(condition, list):
             condition_str = ' AND '.join(condition)
         elif isinstance(condition, str):
             condition_str = condition
         else:
-            raise ValueError("[参数类型错误]", "'condition' 参数必须是 dict/list/str 类型")
+            raise TypeMismatchError("'condition' 参数必须是 dict/list/str 类型")
 
         self.clause = f"""WHERE {condition_str}"""
         return self.clause
 
     def build_set_clause(self, data: dict):
         temp = []
         for k, v in data.items():
```

### Comparing `PyMysqlTools-0.6.0/PyMysqlTools/main.py` & `PyMysqlTools-0.6.1/PyMysqlTools/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pymysql
 
 __all__ = ['Connect', 'ConnectPool', 'ConnectType']
 
 from . import settings
+from .exceptions import TypeMismatchError, ParameterError
 from .generator import ClauseGenerator
 from .actuator import SqlActuator
 from .generator import SqlGenerator
 from .result_set import ResultSet
 
 from enum import Enum
 from dbutils.persistent_db import PersistentDB
@@ -14,57 +15,57 @@
 
 
 class ConnectType(Enum):
     persistent_db = 1
     pooled_db = 2
 
 
-class Connect:
+class BaseConnect:
 
     def __init__(
             self,
-            database,
-            username=None,
-            password=None,
-            host='localhost',
-            port=3306,
-            charset='utf8mb4',
+            connect_args: dict,
+            connect_type: ConnectType = None,
+            **pool_args
     ):
-        self.host = host
-        self.port = port
-        self.username = username
-        self.password = password
-        self.database = database
-        self.charset = charset
-
-        self._connect = pymysql.connect(
-            host=host,
-            port=port,
-            user=username,
-            password=password,
-            database=database,
-            charset=charset
-        )
+        self.connect_args = connect_args
+        self.connect_type = connect_type
+        self._creator = pymysql
+
+        if self.connect_type is None:
+            self._connect = pymysql.connect(**self.connect_args)
+        elif self.connect_type == ConnectType.persistent_db:
+            self._pool_args = {**settings.DEFAULT_PERSISTENT_DB_POOL_ARGS.copy(), **pool_args}
+            self._pool = PersistentDB(creator=self._creator, **self._pool_args, **self.connect_args)
+            self._connect = self._pool.connection()
+        elif self.connect_type == ConnectType.pooled_db:
+            self._pool_args = {**settings.DEFAULT_POOLED_DB_POOL_ARGS.copy(), **pool_args}
+            self._pool = PooledDB(creator=self._creator, **self._pool_args, **self.connect_args)
+            self._connect = self._pool.connection()
+        else:
+            valid_types = [attr for attr in ConnectType.__dict__.keys() if not attr.startswith('_')]
+            raise ParameterError(f"'connect_type' 参数的类型必须是 {', '.join(valid_types)} 中的一种")
+
         self._cursor = self._connect.cursor()
         self._clause_generator = ClauseGenerator()
         self._sql_generator = SqlGenerator()
         self._sql_actuator = SqlActuator(self._connect)
 
-    def insert_one(self, tb_name, data: dict):
+    def insert_one(self, tb_name, data: dict) -> int:
         """
         插入单条记录
         :param tb_name: 表名
         :param data: 待插入的数据
         :return: 受影响的行数
         """
         sql = self._sql_generator.insert_one(tb_name, data)
         args = list(data.values())
         return self._sql_actuator.actuator_dml(sql, args)
 
-    def batch_insert(self, tb_name: str, data):
+    def batch_insert(self, tb_name: str, data) -> int:
         """
         批量插入记录
         :param tb_name: 表名
         :param data: 待插入的数据
         :return: 受影响的行数
         """
         row_num = -1
@@ -88,15 +89,15 @@
                 data_list.append(dict(zip(self.show_table_fields(tb_name), row)))
 
         for i in data_list:
             self.insert_one(tb_name, i)
             row_num += 1
 
         if row_num == -1:
-            raise ValueError('[参数类型错误]', "'data' 只能是 dict{str: list}/list[dict]/ResultSet 的类型格式")
+            raise TypeMismatchError("'data' 只能是 dict{str: list}/list[dict]/ResultSet 的类型格式")
         return row_num + 1
 
     def update_insert(self, tb_name: str, data: dict):
         """
         插入单条记录, 如果存在则更新, 不存在则插入
         :param tb_name: 表名
         :param data: 待插入/更新的数据
@@ -164,15 +165,15 @@
         if type_ is None:
             type_ = settings.DEFAULT_RESULT_SET_TYPE
 
         sql = self._sql_generator.find_by(tb_name, fields, condition)
         return ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=type_,
-            fields_=fields or self.show_table_fields(tb_name).all()
+            fields=fields or self.show_table_fields(tb_name).all()
         )
 
     def find_by_id(self, tb_name: str, id_: int, fields: list = None, type_=None) -> ResultSet:
         """
         根据id查询记录
         :param tb_name: 表名
         :param id_: id
@@ -197,15 +198,15 @@
             type_ = settings.DEFAULT_RESULT_SET_TYPE
 
         sql = self._sql_generator.find_by(tb_name, fields, condition)
         sql += self._clause_generator.build_limit_clause(1)
         return ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=type_,
-            fields_=fields or self.show_table_fields(tb_name).all()
+            fields=fields or self.show_table_fields(tb_name).all()
         )
 
     def find_all(self, tb_name: str, type_=None) -> ResultSet:
         """
         查询全表记录
         :param tb_name: 表名
         :param type_: 返回集结构类型 [dict/list]
@@ -217,15 +218,15 @@
 
     def show_table_fields(self, tb_name: str) -> ResultSet:
         """
         查看表字段
         :param tb_name:表名
         :return: 结果集
         """
-        sql = self._sql_generator.show_table_fields(self.database, tb_name)
+        sql = self._sql_generator.show_table_fields(self.connect_args['database'], tb_name)
         return ResultSet(
             self._sql_actuator.actuator_dql(sql),
             type_=list
         )
 
     def show_table_desc(self, tb_name: str) -> ResultSet:
         """
@@ -275,15 +276,15 @@
 
     def show_table_primary_field(self, tb_name: str) -> ResultSet:
         """
         查询主键字段名称
         :param tb_name: 表名
         :return: 结果集
         """
-        sql = self._sql_generator.show_table_primary_field(self.database, tb_name)
+        sql = self._sql_generator.show_table_primary_field(self.connect_args['database'], tb_name)
         return ResultSet(self._sql_actuator.actuator_dql(sql), type_=list)
 
     def is_exist_database(self, db_name: str) -> bool:
         """
         判断数据库是否存在
         :param db_name:
         :return: True: 存在<br>False: 不存在
@@ -388,403 +389,32 @@
         """
         这个方法是方便作者debugger用的, 未来可能会移除
         :return:
         """
         return self._sql_generator
 
 
-class ConnectPool:
-    def __init__(self, connect_type: ConnectType, connect_args: dict, **pool_args):
-        self.creator = pymysql
-        self.connect_type = connect_type
-        self.connect_args = connect_args
-        if self.connect_type == ConnectType.persistent_db:
-            self._max_usage = pool_args.get('max_usage', None)
-            self._set_session = pool_args.get('set_session', None)
-            self._failures = pool_args.get('failures', None)
-            self._ping = pool_args.get('ping', 1)
-            self._closeable = pool_args.get('closeable', False)
-            self._thread_local = pool_args.get('thread_local', None)
-            self._pool = PersistentDB(
-                creator=self.creator,
-                maxusage=self._max_usage,
-                setsession=self._set_session,
-                failures=self._failures,
-                ping=self._ping,
-                closeable=self._closeable,
-                threadlocal=self._thread_local,
-                **connect_args
-            )
-        elif self.connect_type == ConnectType.pooled_db:
-            self._min_cached = pool_args.get('min_cached', 0)
-            self._max_cached = pool_args.get('max_cached', 0)
-            self._max_shared = pool_args.get('max_shared', 0)
-            self._max_connections = pool_args.get('max_connections', 0)
-            self._blocking = pool_args.get('blocking', False)
-            self._max_usage = pool_args.get('max_usage', None)
-            self._set_session = pool_args.get('set_session', None)
-            self._reset = pool_args.get('reset', True)
-            self._failures = pool_args.get('failures', None)
-            self._ping = pool_args.get('ping', 1)
-            self._pool = PooledDB(
-                creator=self.creator,
-                mincached=self._min_cached,
-                maxcached=self._max_cached,
-                maxshared=self._max_shared,
-                maxconnections=self._max_connections,
-                blocking=self._blocking,
-                maxusage=self._max_usage,
-                setsession=self._set_session,
-                reset=self._reset,
-                failures=self._failures,
-                ping=self._ping,
-                **connect_args
-            )
-        else:
-            raise Exception('ConnectTypeError')
-        self._connect = self._pool.connection()
-        self._cursor = self._connect.cursor()
-        self._clause_generator = ClauseGenerator()
-        self._sql_generator = SqlGenerator()
-        self._sql_actuator = SqlActuator(self._connect)
-
-    def insert_one(self, tb_name, data: dict) -> int:
-        """
-        插入单条记录
-        :param tb_name: 表名
-        :param data: 待插入的数据
-        :return: 受影响的行数
-        """
-        sql = self._sql_generator.insert_one(tb_name, data)
-        args = list(data.values())
-        result = self._sql_actuator.actuator_dml(sql, args)
-        self._connect.close()
-        return result
-
-    def batch_insert(self, tb_name: str, data) -> int:
-        """
-        批量插入记录
-        :param tb_name: 表名
-        :param data: 待插入的数据
-        :return: 受影响的行数
-        """
-        row_num = -1
-        data_list = []
-
-        if isinstance(data, dict):
-            if isinstance(list(data.values())[0], list):
-                # [类型转换, dict{str: list} -> list[dict]]
-                for index in range(len(list(data.values())[0])):
-                    temp = {}
-                    for key in data.keys():
-                        temp[key] = data.get(key)[index]
-                    data_list.append(temp)
-
-        if isinstance(data, list):
-            if isinstance(data[0], dict):
-                data_list = data
-
-        if isinstance(data, ResultSet):
-            for row in data:
-                data_list.append(dict(zip(self.show_table_fields(tb_name), row)))
-
-        for i in data_list:
-            self.insert_one(tb_name, i)
-            row_num += 1
-
-        if row_num == -1:
-            raise ValueError('[参数类型错误]', "'data' 只能是 dict{str: list}/list[dict]/ResultSet 的类型格式")
-
-        self._connect.close()
-        return row_num + 1
-
-    def update_insert(self, tb_name: str, data: dict):
-        """
-        插入单条记录, 如果存在则更新, 不存在则插入
-        :param tb_name: 表名
-        :param data: 待插入/更新的数据
-        :return: None
-        """
-        try:
-            self.insert_one(tb_name, data)
-        except pymysql.err.IntegrityError as err:
-            self.update_by(
-                tb_name,
-                data,
-                {self.show_table_primary_field(tb_name).all()[0]: err.args[1].split("'")[1]}
-            )
-
-    def delete_by(self, tb_name: str, condition=None) -> int:
-        """
-        根据条件删除记录
-        :param tb_name: 表名
-        :param condition: 删除条件
-        :return: 受影响的行数
-        """
-        sql = self._sql_generator.delete_by(tb_name, condition)
-        result = self._sql_actuator.actuator_dml(sql)
-        self._connect.close()
-        return result
-
-    def delete_by_id(self, tb_name: str, id_: int) -> int:
-        """
-        根据id删除记录
-        :param tb_name: 表名
-        :param id_: id
-        :return: 受影响的行数
-        """
-        return self.delete_by(tb_name, {'id': id_})
-
-    def update_by(self, tb_name: str, data: dict, condition=None) -> int:
-        """
-        根据条件更新记录
-        :param tb_name: 表名
-        :param data: 待更新的数据
-        :param condition: 更新条件
-        :return: 受影响的行数
-        """
-        sql = self._sql_generator.update_by(tb_name, data, condition)
-        args = list(data.values())
-        result = self._sql_actuator.actuator_dml(sql, args)
-        self._connect.close()
-        return result
-
-    def update_by_id(self, tb_name: str, data: dict, id_: int) -> int:
-        """
-        根据id更新记录
-        :param tb_name: 表名
-        :param data: 待更新的数据
-        :param id_: id
-        :return: 受影响的行数
-        """
-        return self.update_by(tb_name, data, {'id': id_})
-
-    def find_by(self, tb_name: str, fields: list = None, condition=None, type_=None) -> ResultSet:
-        """
-        根据条件查询记录
-        :param tb_name: 表名
-        :param fields: 需要查询的字段
-        :param condition: 查询条件
-        :param type_: 返回集结构类型 [dict/list]
-        :return: 结果集
-        """
-        if type_ is None:
-            type_ = settings.DEFAULT_RESULT_SET_TYPE
-
-        sql = self._sql_generator.find_by(tb_name, fields, condition)
-        result = ResultSet(
-            self._sql_actuator.actuator_dql(sql),
-            type_=type_,
-            fields_=fields or self.show_table_fields(tb_name).all()
-        )
-        self._connect.close()
-        return result
-
-    def find_by_id(self, tb_name: str, id_: int, fields: list = None, type_=None) -> ResultSet:
-        """
-        根据id查询记录
-        :param tb_name: 表名
-        :param id_: id
-        :param fields: 需要查询的字段
-        :param type_: 返回集结构类型 [dict/list]
-        :return: 结果集
-        """
-        if type_ is None:
-            type_ = settings.DEFAULT_RESULT_SET_TYPE
-        return self.find_by(tb_name, fields, {'id': id_}, type_=type_)
-
-    def find_one(self, tb_name: str, fields: list = None, condition=None, type_=None) -> ResultSet:
-        """
-        根据条件查询单条记录
-        :param tb_name: 表名
-        :param fields: 需要查询的字段
-        :param condition: 查询条件
-        :param type_: 返回集结构类型 [dict/list]
-        :return: 结果集
-        """
-        if type_ is None:
-            type_ = settings.DEFAULT_RESULT_SET_TYPE
-
-        sql = self._sql_generator.find_by(tb_name, fields, condition)
-        sql += self._clause_generator.build_limit_clause(1)
-        return ResultSet(
-            self._sql_actuator.actuator_dql(sql),
-            type_=type_,
-            fields_=fields or self.show_table_fields(tb_name).all()
-        )
-
-    def find_all(self, tb_name: str, type_=None) -> ResultSet:
-        """
-        查询全表记录
-        :param tb_name: 表名
-        :param type_: 返回集结构类型 [dict/list]
-        :return: 结果集
-        """
-        if type_ is None:
-            type_ = settings.DEFAULT_RESULT_SET_TYPE
-        return self.find_by(tb_name, type_=type_)
-
-    def show_table_fields(self, tb_name: str) -> ResultSet:
-        """
-        查看表字段
-        :param tb_name:表名
-        :return: 结果集
-        """
-        sql = self._sql_generator.show_table_fields(self.connect_args.get('database', None), tb_name)
-        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list)
-        self._connect.close()
-        return result
-
-    def show_table_desc(self, tb_name: str) -> ResultSet:
-        """
-        查看表结构
-        :param tb_name: 表名
-        :return: 表结构
-        """
-        sql = self._sql_generator.desc_table(tb_name)
-        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list)
-        self._connect.close()
-        return result
-
-    def show_table_size(self, tb_name: str) -> int:
-        """
-        查询表有多少条记录
-        :param tb_name: 表名
-        :return: 记录数
-        """
-        sql = self._sql_generator.show_table_size(tb_name)
-        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get()
-        self._connect.close()
-        return result
-
-    def show_table_vague_size(self, tb_name: str) -> int:
-        """
-        估算表有多少条记录, 准确度低, 但速度快
-        :param tb_name:
-        :return: 记录数
-        """
-        sql = self._sql_generator.show_table_vague_size(tb_name)
-        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list).get()
-        self._connect.close()
-        return result
-
-    def show_databases(self) -> ResultSet:
-        """
-        查看所有数据库
-        :return: 所有数据库
-        """
-        sql = self._clause_generator.build_show_clause('DATABASES')
-        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list)
-        self._connect.close()
-        return result
-
-    def show_tables(self) -> ResultSet:
-        """
-        查看所有数据表
-        :return: 所有数据表
-        """
-        sql = self._clause_generator.build_show_clause('TABLES')
-        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list)
-        self._connect.close()
-        return result
-
-    def show_table_primary_field(self, tb_name: str) -> ResultSet:
-        """
-        查询主键字段名称
-        :param tb_name: 表名
-        :return: 结果集
-        """
-        sql = self._sql_generator.show_table_primary_field(self.connect_args.get('database', None), tb_name)
-        result = ResultSet(self._sql_actuator.actuator_dql(sql), type_=list)
-        self._connect.close()
-        return result
-
-    def is_exist_database(self, db_name: str) -> bool:
-        """
-        判断数据库是否存在
-        :param db_name:
-        :return: True: 存在<br>False: 不存在
-        """
-        return db_name in self.show_databases()
-
-    def is_exist_table(self, tb_name: str) -> bool:
-        """
-        判断数据表是否存在
-        :param tb_name: 表名
-        :return: True: 存在<br>False: 不存在
-        """
-        return tb_name in self.show_tables()
+class Connect(BaseConnect):
 
-    def truncate_table(self, tb_name: str) -> bool:
-        """
-        清空表数据
-        :param tb_name: 表名
-        :return: 执行结果
-        """
-        sql = self._sql_generator.truncate_table(tb_name)
-        result = self._sql_actuator.actuator_dml(sql) > 0
-        self._connect.close()
-        return result
-
-    def delete_table(self, tb_name: str) -> bool:
-        """
-        删除表所有记录
-        :param tb_name: 表名
-        :return: 执行结果
-        """
-        sql = self._sql_generator.delete_table(tb_name)
-        result = self._sql_actuator.actuator_dml(sql) > 0
-        self._connect.close()
-        return result
-
-    def create_table(self, tb_name: str, schema) -> int:
-        """
-        创建数据表
-        :param tb_name: 表名
-        :param schema: 表结构
-        :return: 0表示创建成功
-        """
-        sql = self._sql_generator.create_table(tb_name, schema)
-        result = self._sql_actuator.actuator_dml(sql)
-        self._connect.close()
-        return result
-
-    def create_table_not_exists(self, tb_name: str, schema) -> int:
-        """
-        如果表不存在就创建数据表
-        :param tb_name: 表名
-        :param schema: 表结构
-        :return: 0表示创建成功
-        """
-        sql = self._sql_generator.create_table(tb_name, schema)
-        result = self._sql_actuator.actuator_dml(sql)
-        self._connect.close()
-        return result
-
-    def migration_table(self, for_tb_name: str, to_tb_name: str) -> int:
-        """
-        将一张表的数据迁移到另一张表中
-        :param for_tb_name: 数据源表的表名
-        :param to_tb_name: 目标表的表名
-        :return: 已迁移的数据行数
-        """
-        row_num = 0
-        for row in self.find_all(for_tb_name):
-            self.insert_one(to_tb_name, dict(zip(self.show_table_fields(to_tb_name), row)))
-            row_num += 1
-        result = row_num
-        self._connect.close()
-        return result
+    def __init__(
+            self,
+            database: str,
+            username: str = None,
+            password: str = None,
+            host: str = 'localhost',
+            port: int = 3306,
+            charset: str = 'utf8mb4',
+    ):
+        connect_args = {
+            'database': database,
+            'username': username,
+            'password': password,
+            'host': host,
+            'port': port,
+            'charset': charset,
+        }
+        super().__init__(connect_args)
 
-    def close(self):
-        """
-        关闭数据库连接
-        :return:
-        """
-        self._connect.close()
 
-    def reconnect(self):
-        """
-        重新与MySQL服务建立连接
-        :return:
-        """
-        self._connect.ping(reconnect=True)
+class ConnectPool(BaseConnect):
+    def __init__(self, connect_args: dict, connect_type: ConnectType, **pool_args):
+        super().__init__(connect_args, connect_type, **pool_args)
```

### Comparing `PyMysqlTools-0.6.0/PyMysqlTools/result_set.py` & `PyMysqlTools-0.6.1/PyMysqlTools/result_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from . import settings
+from .exceptions import TypeMismatchError, ParameterError
 
 
 class ResultSet:
 
     def __init__(
             self,
             result=None,
             type_=settings.DEFAULT_RESULT_SET_TYPE,
-            fields_=None
+            fields=None
     ):
         """
         ResultSet 结果集
-        :param result: 暂时的结果集存储在这里
-        :param type_: 返回的结果集类型
-        :param fields_: 当type_为dict时, 需要字段名
+        :param result: 结果集
+        :param type_: 期望返回的结果集结构
+        :param fields: 当type_为dict时, 需要字段名
         """
         if result is None:
             result = []
 
         self._result = []
         self._type = type_
 
@@ -26,25 +27,25 @@
                 if len(row) > 1:
                     self._result.append(list(row))
                 elif len(row) == 1:
                     self._result.append(row[0])
                 else:
                     self._result.append([None])
         elif self._type == dict:
-            if fields_ is None:
-                raise ValueError('[参数错误]', "'type_'为dict时 'fields_' 需要传入参数")
+            if fields is None:
+                raise ParameterError("'type_'为dict时 'fields' 需要传入参数")
             else:
-                if isinstance(fields_[0], list):
-                    self._fields = fields_[0]
+                if isinstance(fields[0], list):
+                    self._fields = fields[0]
                 else:
-                    self._fields = fields_
+                    self._fields = fields
                 for row in result:
                     self._result.append(_extract_as_dict(self._fields, row))
         else:
-            raise ValueError('[参数数据类型错误]', "'type_' 只能是 list/dict 类型")
+            raise TypeMismatchError("'type_' 只能是 list/dict 类型")
 
         self._index = 0
 
     def __iter__(self):
         return self
 
     def __next__(self):
@@ -61,65 +62,71 @@
         return self._result.__str__()
 
     def __len__(self):
         return len(self._result)
 
     def all(self):
         """
-        将结果集转换为一个方便迭代的结构(List)
+        获取结果集, 并将结果集转换为一个方便迭代的结构(List)
         :return: List结果集
         """
         if not self._result:
             return []
         if self._type == list and not isinstance(self._result, list):
             return [self._result]
         if isinstance(self._result, dict):
             return [self._result]
         return self._result
 
     def limit(self, num: int = 1):
         """
-        截取结果集的前n个结果, 仅List结构可用
+        截取结果集的前n个结果
         :param num: 需要截取的结果的数量
-        :return:
+        :return: 截取后的结果集
         """
         if not isinstance(self._result, list):
             raise ValueError('结果集结构类型不为 `list`, 不支持使用limit')
         if num > 0:
             return self._result[: num]
         else:
             raise ValueError("'num' 参数的值必须大于 0 ！")
 
     def next(self):
         """
-        获取结果集中的下一个结果, 仅List结构可用
-        :return:
+        获取结果集中的下一个结果
+        :return: 下一行数据
         """
         if not isinstance(self._result, list):
             return self._result
         if self._index < len(self._result):
             next_ = self._result[self._index]
             self._index += 1
             return next_
 
     def get(self, index: int = 0):
         """
-        获取特定索引位置的结果, 仅List结构可用
-        :param index:
-        :return:
+        获取特定索引位置的结果
+        :param index: 索引
+        :return: 索引行数据
         """
         if not self._result:
             return None
         if isinstance(self._result, list):
             return self._result[index]
         if self._type == dict or len(self._result) == 1:
             return self._result
 
 
 def _extract_as_dict(fields: list, value: list):
+    """
+    提取字段名和字段值组合后转换为dict结构
+    :param fields: 字段名
+    :param value: 字段值
+    :return: dict结构的单行数据
+    """
     fields_len = len(fields)
     value_len = len(value)
 
     if fields_len == value_len:
         return dict(zip(fields, value))
 
     row_data = {}
```

### Comparing `PyMysqlTools-0.6.0/PyMysqlTools.egg-info/PKG-INFO` & `PyMysqlTools-0.6.1/PyMysqlTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
```

### Comparing `PyMysqlTools-0.6.0/README.md` & `PyMysqlTools-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.0/setup.py` & `PyMysqlTools-0.6.1/setup.py`

 * *Files identical despite different names*

