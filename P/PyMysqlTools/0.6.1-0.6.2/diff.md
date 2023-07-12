# Comparing `tmp/PyMysqlTools-0.6.1.tar.gz` & `tmp/PyMysqlTools-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMysqlTools-0.6.1.tar", last modified: Wed Jul 12 08:28:57 2023, max compression
+gzip compressed data, was "PyMysqlTools-0.6.2.tar", last modified: Wed Jul 12 09:26:50 2023, max compression
```

## Comparing `PyMysqlTools-0.6.1.tar` & `PyMysqlTools-0.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 08:28:57.279802 PyMysqlTools-0.6.1/
--rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.1/LICENSE
--rw-rw-rw-   0        0        0      143 2023-02-06 01:25:52.000000 PyMysqlTools-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2610 2023-07-12 08:28:57.278806 PyMysqlTools-0.6.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 08:28:57.258641 PyMysqlTools-0.6.1/PyMysqlTools/
--rw-rw-rw-   0        0        0      424 2023-07-12 08:26:13.000000 PyMysqlTools-0.6.1/PyMysqlTools/__init__.py
--rw-rw-rw-   0        0        0      698 2023-07-07 08:55:05.000000 PyMysqlTools-0.6.1/PyMysqlTools/actuator.py
--rw-rw-rw-   0        0        0      431 2023-07-12 02:25:29.000000 PyMysqlTools-0.6.1/PyMysqlTools/exceptions.py
--rw-rw-rw-   0        0        0     6039 2023-07-12 06:20:01.000000 PyMysqlTools-0.6.1/PyMysqlTools/generator.py
--rw-rw-rw-   0        0        0    14182 2023-07-12 03:47:57.000000 PyMysqlTools-0.6.1/PyMysqlTools/main.py
--rw-rw-rw-   0        0        0     4185 2023-07-11 02:31:54.000000 PyMysqlTools-0.6.1/PyMysqlTools/result_set.py
--rw-rw-rw-   0        0        0      624 2023-07-12 02:58:20.000000 PyMysqlTools-0.6.1/PyMysqlTools/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:28:57.277807 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/
--rw-rw-rw-   0        0        0     2610 2023-07-12 08:28:57.000000 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-07-12 08:28:57.000000 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 08:28:57.000000 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-12 08:28:57.000000 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 08:28:57.000000 PyMysqlTools-0.6.1/PyMysqlTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2007 2023-02-06 01:33:20.000000 PyMysqlTools-0.6.1/README.md
--rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 08:28:57.279802 PyMysqlTools-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:26:50.142478 PyMysqlTools-0.6.2/
+-rw-rw-rw-   0        0        0     1083 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0      143 2023-02-06 01:25:52.000000 PyMysqlTools-0.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2601 2023-07-12 09:26:50.141197 PyMysqlTools-0.6.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 09:26:50.132426 PyMysqlTools-0.6.2/PyMysqlTools/
+-rw-rw-rw-   0        0        0      424 2023-07-12 09:21:06.000000 PyMysqlTools-0.6.2/PyMysqlTools/__init__.py
+-rw-rw-rw-   0        0        0      698 2023-07-07 08:55:05.000000 PyMysqlTools-0.6.2/PyMysqlTools/actuator.py
+-rw-rw-rw-   0        0        0      431 2023-07-12 02:25:29.000000 PyMysqlTools-0.6.2/PyMysqlTools/exceptions.py
+-rw-rw-rw-   0        0        0     6039 2023-07-12 06:20:01.000000 PyMysqlTools-0.6.2/PyMysqlTools/generator.py
+-rw-rw-rw-   0        0        0    14473 2023-07-12 09:18:09.000000 PyMysqlTools-0.6.2/PyMysqlTools/main.py
+-rw-rw-rw-   0        0        0     4185 2023-07-11 02:31:54.000000 PyMysqlTools-0.6.2/PyMysqlTools/result_set.py
+-rw-rw-rw-   0        0        0      624 2023-07-12 02:58:20.000000 PyMysqlTools-0.6.2/PyMysqlTools/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:26:50.139379 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/
+-rw-rw-rw-   0        0        0     2601 2023-07-12 09:26:50.000000 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-07-12 09:26:50.000000 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 09:26:50.000000 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-12 09:26:50.000000 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-12 09:26:50.000000 PyMysqlTools-0.6.2/PyMysqlTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1998 2023-07-12 09:26:16.000000 PyMysqlTools-0.6.2/README.md
+-rw-rw-rw-   0        0        0       50 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 09:26:50.142478 PyMysqlTools-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2022-11-09 07:31:21.000000 PyMysqlTools-0.6.2/setup.py
```

### Comparing `PyMysqlTools-0.6.1/LICENSE` & `PyMysqlTools-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.1/PKG-INFO` & `PyMysqlTools-0.6.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
@@ -16,19 +16,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PyMysqlTools
 
 
-PyMysqlTools 是一个通过避免编写SQL语句的方式来操作mysql的工具库
+PyMysqlTools 是一个使用封装好的函数替代SQL语句来操作mysql的工具库
 
 
 
-**注意**
+**环境配置**
 
 PyMysqlTools 目前支持 Python3.6+ 且 MySQL5.6+ 版本
 
 
 
 ### 快速开始
 
@@ -53,15 +53,15 @@
    
    # 可以使用下面的示例代码直接获得一个mysql数据库的连接
    mysql = PyMysqlTools.connect(
        database='db_test',
        username='root',
        password='123456'
    )
-   print(mysql)
+   print(mysql) # <PyMysqlTools.main.Connect object>
    ```
 
 2. 简单使用
 
    - 添加数据
 
      ```python
@@ -105,28 +105,24 @@
 
      ```python
      # 查询全表数据并遍历输出
      for row in mysql.find_all('tb_test'):
          print(row)
      ```
 
-     
-
-   - 其他更多方法详见 api 文档
-   
-     - PS: api文档目前还没有。
 
 
 
-### 关于社区
+### 关于
 
 如果您在使用时遇到了意料之外的结果，请[提交Issue](https://gitee.com/uraurara/PyMysqlTools/issues/new?issue%5Bassignee_id%5D=0&issue%5Bmilestone_id%5D=0)帮助我们改进此项目。
 
 
 
 ### Thanks
 
+本项目在开发中使用了以下Python库
 - [PyMySQL](https://gitee.com/src-openeuler/python-PyMySQL)
 - [DBUtils](https://github.com/WebwareForPython/DBUtils)
```

### Comparing `PyMysqlTools-0.6.1/PyMysqlTools/actuator.py` & `PyMysqlTools-0.6.2/PyMysqlTools/actuator.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.1/PyMysqlTools/generator.py` & `PyMysqlTools-0.6.2/PyMysqlTools/generator.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.1/PyMysqlTools/main.py` & `PyMysqlTools-0.6.2/PyMysqlTools/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,19 +30,21 @@
         self.connect_args = connect_args
         self.connect_type = connect_type
         self._creator = pymysql
 
         if self.connect_type is None:
             self._connect = pymysql.connect(**self.connect_args)
         elif self.connect_type == ConnectType.persistent_db:
-            self._pool_args = {**settings.DEFAULT_PERSISTENT_DB_POOL_ARGS.copy(), **pool_args}
+            _pool_args = {**settings.DEFAULT_PERSISTENT_DB_POOL_ARGS.copy(), **pool_args}
+            self._pool_args = {key.replace('_', ''): value for key, value in _pool_args.items()}
             self._pool = PersistentDB(creator=self._creator, **self._pool_args, **self.connect_args)
             self._connect = self._pool.connection()
         elif self.connect_type == ConnectType.pooled_db:
-            self._pool_args = {**settings.DEFAULT_POOLED_DB_POOL_ARGS.copy(), **pool_args}
+            _pool_args = {**settings.DEFAULT_POOLED_DB_POOL_ARGS.copy(), **pool_args}
+            self._pool_args = {key.replace('_', ''): value for key, value in _pool_args.items()}
             self._pool = PooledDB(creator=self._creator, **self._pool_args, **self.connect_args)
             self._connect = self._pool.connection()
         else:
             valid_types = [attr for attr in ConnectType.__dict__.keys() if not attr.startswith('_')]
             raise ParameterError(f"'connect_type' 参数的类型必须是 {', '.join(valid_types)} 中的一种")
 
         self._cursor = self._connect.cursor()
@@ -402,19 +404,20 @@
             password: str = None,
             host: str = 'localhost',
             port: int = 3306,
             charset: str = 'utf8mb4',
     ):
         connect_args = {
             'database': database,
-            'username': username,
+            'user': username,
             'password': password,
             'host': host,
             'port': port,
             'charset': charset,
         }
         super().__init__(connect_args)
 
 
 class ConnectPool(BaseConnect):
     def __init__(self, connect_args: dict, connect_type: ConnectType, **pool_args):
+        connect_args = {'user' if key == 'username' else key: value for key, value in connect_args.items()}
         super().__init__(connect_args, connect_type, **pool_args)
```

### Comparing `PyMysqlTools-0.6.1/PyMysqlTools/result_set.py` & `PyMysqlTools-0.6.2/PyMysqlTools/result_set.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.1/PyMysqlTools/settings.py` & `PyMysqlTools-0.6.2/PyMysqlTools/settings.py`

 * *Files identical despite different names*

### Comparing `PyMysqlTools-0.6.1/PyMysqlTools.egg-info/PKG-INFO` & `PyMysqlTools-0.6.2/PyMysqlTools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMysqlTools
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library that makes MySQL operation more convenient.
 Home-page: https://gitee.com/uraurara/PyMysqlTools
 Author: ulala
 Author-email: 2713389652@qq.com
 License: MIT
 Keywords: mysql,client,mysqluitls,PyMysqlTools
 Platform: UNKNOWN
@@ -16,19 +16,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PyMysqlTools
 
 
-PyMysqlTools 是一个通过避免编写SQL语句的方式来操作mysql的工具库
+PyMysqlTools 是一个使用封装好的函数替代SQL语句来操作mysql的工具库
 
 
 
-**注意**
+**环境配置**
 
 PyMysqlTools 目前支持 Python3.6+ 且 MySQL5.6+ 版本
 
 
 
 ### 快速开始
 
@@ -53,15 +53,15 @@
    
    # 可以使用下面的示例代码直接获得一个mysql数据库的连接
    mysql = PyMysqlTools.connect(
        database='db_test',
        username='root',
        password='123456'
    )
-   print(mysql)
+   print(mysql) # <PyMysqlTools.main.Connect object>
    ```
 
 2. 简单使用
 
    - 添加数据
 
      ```python
@@ -105,28 +105,24 @@
 
      ```python
      # 查询全表数据并遍历输出
      for row in mysql.find_all('tb_test'):
          print(row)
      ```
 
-     
-
-   - 其他更多方法详见 api 文档
-   
-     - PS: api文档目前还没有。
 
 
 
-### 关于社区
+### 关于
 
 如果您在使用时遇到了意料之外的结果，请[提交Issue](https://gitee.com/uraurara/PyMysqlTools/issues/new?issue%5Bassignee_id%5D=0&issue%5Bmilestone_id%5D=0)帮助我们改进此项目。
 
 
 
 ### Thanks
 
+本项目在开发中使用了以下Python库
 - [PyMySQL](https://gitee.com/src-openeuler/python-PyMySQL)
 - [DBUtils](https://github.com/WebwareForPython/DBUtils)
```

### Comparing `PyMysqlTools-0.6.1/README.md` & `PyMysqlTools-0.6.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 # PyMysqlTools
 
 
-PyMysqlTools 是一个通过避免编写SQL语句的方式来操作mysql的工具库
+PyMysqlTools 是一个使用封装好的函数替代SQL语句来操作mysql的工具库
 
 
 
-**注意**
+**环境配置**
 
 PyMysqlTools 目前支持 Python3.6+ 且 MySQL5.6+ 版本
 
 
 
 ### 快速开始
 
@@ -35,15 +35,15 @@
    
    # 可以使用下面的示例代码直接获得一个mysql数据库的连接
    mysql = PyMysqlTools.connect(
        database='db_test',
        username='root',
        password='123456'
    )
-   print(mysql)
+   print(mysql) # <PyMysqlTools.main.Connect object>
    ```
 
 2. 简单使用
 
    - 添加数据
 
      ```python
@@ -87,26 +87,22 @@
 
      ```python
      # 查询全表数据并遍历输出
      for row in mysql.find_all('tb_test'):
          print(row)
      ```
 
-     
-
-   - 其他更多方法详见 api 文档
-   
-     - PS: api文档目前还没有。
 
 
 
-### 关于社区
+### 关于
 
 如果您在使用时遇到了意料之外的结果，请[提交Issue](https://gitee.com/uraurara/PyMysqlTools/issues/new?issue%5Bassignee_id%5D=0&issue%5Bmilestone_id%5D=0)帮助我们改进此项目。
 
 
 
 ### Thanks
 
+本项目在开发中使用了以下Python库
 - [PyMySQL](https://gitee.com/src-openeuler/python-PyMySQL)
 - [DBUtils](https://github.com/WebwareForPython/DBUtils)
```

### Comparing `PyMysqlTools-0.6.1/setup.py` & `PyMysqlTools-0.6.2/setup.py`

 * *Files identical despite different names*

