# Comparing `tmp/PyEasySQL-2.0.2.tar.gz` & `tmp/PyEasySQL-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEasySQL-2.0.2.tar", last modified: Sat Jun 25 11:47:27 2022, max compression
+gzip compressed data, was "PyEasySQL-3.0.2.tar", last modified: Wed Jul 12 13:10:09 2023, max compression
```

## Comparing `PyEasySQL-2.0.2.tar` & `PyEasySQL-3.0.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-06-25 11:47:27.081693 PyEasySQL-2.0.2/
-drwxrwxrwx   0        0        0        0 2022-06-25 11:47:27.012500 PyEasySQL-2.0.2/EasySQL/
--rw-rw-rw-   0        0        0     3222 2022-05-29 10:39:30.000000 PyEasySQL-2.0.2/EasySQL/ABC.py
--rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 PyEasySQL-2.0.2/EasySQL/Characters.py
--rw-rw-rw-   0        0        0    10130 2022-06-25 11:35:33.000000 PyEasySQL-2.0.2/EasySQL/Classes.py
--rw-rw-rw-   0        0        0     5655 2022-06-25 11:35:34.000000 PyEasySQL-2.0.2/EasySQL/Commands.py
--rw-rw-rw-   0        0        0      496 2022-05-29 10:50:25.000000 PyEasySQL-2.0.2/EasySQL/Exceptions.py
--rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 PyEasySQL-2.0.2/EasySQL/Logging.py
--rw-rw-rw-   0        0        0     2512 2022-05-07 16:36:16.000000 PyEasySQL-2.0.2/EasySQL/Types.py
--rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 PyEasySQL-2.0.2/EasySQL/Where.py
--rw-rw-rw-   0        0        0      192 2021-06-24 12:24:03.000000 PyEasySQL-2.0.2/EasySQL/__init__.py
--rw-rw-rw-   0        0        0     6112 2022-06-25 11:47:27.078155 PyEasySQL-2.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-06-25 11:47:27.068941 PyEasySQL-2.0.2/PyEasySQL.egg-info/
--rw-rw-rw-   0        0        0     6112 2022-06-25 11:47:25.000000 PyEasySQL-2.0.2/PyEasySQL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2022-06-25 11:47:26.000000 PyEasySQL-2.0.2/PyEasySQL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-25 11:47:25.000000 PyEasySQL-2.0.2/PyEasySQL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-06-25 11:47:25.000000 PyEasySQL-2.0.2/PyEasySQL.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-06-25 11:47:25.000000 PyEasySQL-2.0.2/PyEasySQL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4756 2022-06-25 11:46:52.000000 PyEasySQL-2.0.2/README.md
--rw-rw-rw-   0        0        0       42 2022-06-25 11:47:27.082689 PyEasySQL-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      859 2022-06-25 11:35:34.000000 PyEasySQL-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 13:10:09.478943 PyEasySQL-3.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-12 13:10:09.450027 PyEasySQL-3.0.2/EasySQL/
+-rw-rw-rw-   0        0        0     3452 2023-07-09 09:35:55.000000 PyEasySQL-3.0.2/EasySQL/ABC.py
+-rw-rw-rw-   0        0        0     2887 2021-06-27 12:24:21.000000 PyEasySQL-3.0.2/EasySQL/Characters.py
+-rw-rw-rw-   0        0        0    14208 2023-07-11 13:02:37.000000 PyEasySQL-3.0.2/EasySQL/Classes.py
+-rw-rw-rw-   0        0        0     5655 2022-06-25 11:35:34.000000 PyEasySQL-3.0.2/EasySQL/Commands.py
+-rw-rw-rw-   0        0        0      305 2023-07-11 12:44:34.000000 PyEasySQL-3.0.2/EasySQL/Decorators.py
+-rw-rw-rw-   0        0        0     2097 2023-07-09 09:35:55.000000 PyEasySQL-3.0.2/EasySQL/EasyInstances.py
+-rw-rw-rw-   0        0        0      757 2023-06-08 19:41:42.000000 PyEasySQL-3.0.2/EasySQL/Exceptions.py
+-rw-rw-rw-   0        0        0      457 2021-04-04 16:17:30.000000 PyEasySQL-3.0.2/EasySQL/Logging.py
+-rw-rw-rw-   0        0        0      134 2023-07-09 09:35:55.000000 PyEasySQL-3.0.2/EasySQL/Tags.py
+-rw-rw-rw-   0        0        0     2602 2023-07-11 12:55:43.000000 PyEasySQL-3.0.2/EasySQL/Types.py
+-rw-rw-rw-   0        0        0     2496 2022-04-15 06:15:51.000000 PyEasySQL-3.0.2/EasySQL/Where.py
+-rw-rw-rw-   0        0        0      290 2023-07-09 11:50:43.000000 PyEasySQL-3.0.2/EasySQL/__init__.py
+-rw-rw-rw-   0        0        0     6499 2023-07-12 13:10:09.477280 PyEasySQL-3.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 13:10:09.469844 PyEasySQL-3.0.2/PyEasySQL.egg-info/
+-rw-rw-rw-   0        0        0     6499 2023-07-12 13:10:08.000000 PyEasySQL-3.0.2/PyEasySQL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-07-12 13:10:08.000000 PyEasySQL-3.0.2/PyEasySQL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 13:10:08.000000 PyEasySQL-3.0.2/PyEasySQL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-12 13:10:08.000000 PyEasySQL-3.0.2/PyEasySQL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 13:10:08.000000 PyEasySQL-3.0.2/PyEasySQL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5119 2023-07-09 10:37:27.000000 PyEasySQL-3.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 13:10:09.479462 PyEasySQL-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      859 2023-07-11 12:35:42.000000 PyEasySQL-3.0.2/setup.py
```

### Comparing `PyEasySQL-2.0.2/EasySQL/ABC.py` & `PyEasySQL-3.0.2/EasySQL/ABC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from abc import ABC
 from typing import Callable, Any
 
 
+__all__ = ['SQLType', 'SQLTag', 'SQLCommand', 'SQLCommandExecutable', 'SQLExecutable',
+           'CHARSET', 'make_collection', 'is_collection']
+
+
 class SQLType:
     def __init__(self, name, *args, caster: Callable[[Any], Any] = None, get_caster: Callable[["SQLType"], Callable[[Any], Any]] = None, default: Any = None, parser: Callable[[Any], str] = None, modifiable: bool = False):
         self._name = name
         self._args = args
 
         self._modify_args = dict(caster=caster, get_caster=get_caster, default=default, parser=parser)
 
@@ -64,14 +68,19 @@
         return self._args
 
     @property
     def modifiable(self):
         return self._modifiable
 
 
+class SQLTag:
+    def __init__(self, value):
+        self.value = value
+
+
 class CHARSET:
     def __init__(self, name, collation, maxlen=1, description=None):
         self._name = name
         self.__doc__ = description
         self._collation = collation
         self._maxlen = maxlen
```

### Comparing `PyEasySQL-2.0.2/EasySQL/Characters.py` & `PyEasySQL-3.0.2/EasySQL/Characters.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-2.0.2/EasySQL/Commands.py` & `PyEasySQL-3.0.2/EasySQL/Commands.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-2.0.2/EasySQL/Types.py` & `PyEasySQL-3.0.2/EasySQL/Types.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,17 +63,18 @@
     DEC: ['decimal', 'dec'],
     STRING: ['varchar'],
     CHAR: ['char']
 }
 
 
 def string_to_type(string: str):
-    args = string[string.find('(') + 1:string.rfind(')')]
-    string = string[:string.find('(')].lower()
+    args = string[string.find('(') + 1:string.rfind(')')] if string.find('(') >= 0 else None
+    string = string[:string.find('(')].lower() if string.find('(') >= 0 else string
+
     for key, value in type_dict.items():
         if string in value:
             if key == BIT and string != 'bit':
                 return BOOL
-            if not key.modifiable:
+            if not key.modifiable or args is None:
                 return key
             return key(*[int(arg) for arg in args.split(',')])
     return None
```

### Comparing `PyEasySQL-2.0.2/EasySQL/Where.py` & `PyEasySQL-3.0.2/EasySQL/Where.py`

 * *Files identical despite different names*

### Comparing `PyEasySQL-2.0.2/PKG-INFO` & `PyEasySQL-3.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,116 @@
 Metadata-Version: 2.1
 Name: PyEasySQL
-Version: 2.0.2
+Version: 3.0.2
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/ashenguard/easysql
 Author: Ashenguard
 Author-email: Ashenguard@agmdev.xyz
 License: MIT License
 Description: # EasySQL
         ![Downloads](https://pepy.tech/badge/pyeasysql)
         ![Downloads](https://pepy.tech/badge/pyeasysql/week)
         ![Downloads](https://pepy.tech/badge/pyeasysql/month)  
         This library allow you to run SQL Databases without knowing even SQL.  
         This library will create SQL queries and execute them as you request and is very simple to use.
         
-        ### Support
-        You can find support on our discord server here:
-        > https://discord.gg/6exsySK  
-        > Pay us a visit there ✌
+        ### Having an issue?
+        You can always find someone on our discord server here:
+        > https://discord.gg/6exsySK
         
         ### Wiki
         The official wiki of this library is now available at GitHub
-        > https://github.com/Ashengaurd/EasySQL/wiki
-        
+        > https://github.com/Ashenguard/EasySQL/wiki
         
         ## How to install
         ![](https://img.shields.io/github/v/release/Ashengaurd/EasySQL?label=Release&logo=github&style=plastic)
         ![](https://img.shields.io/github/last-commit/Ashengaurd/EasySQL/master?label=Date&logo=git&logoColor=blue&style=plastic)  
         ![](https://img.shields.io/github/v/release/Ashengaurd/EasySQL?include_prereleases&label=Development&logo=github&style=plastic)
         ![](https://img.shields.io/github/last-commit/Ashengaurd/EasySQL?label=Date&logo=git&logoColor=red&style=plastic)  
         To install just use following command
         ```shell
         pip install PyEasySQL
         ```
         This library will have dev/beta builds on the GitHub, to install them you can use
         
         ```shell
-        pip install --upgrade git+https://github.com/Ashengaurd/EasySQL.git
+        pip install --upgrade git+https://github.com/Ashenguard/EasySQL.git
         ```
         ***
         By installing this library following libraries and their dependencies will be installed too.
-        > mysql-connector: Which is the basic library for connecting to database
-        
+        ```yaml
+        mysql-connector: Which is the basic library for connecting to database
+        ```
         # Example
         
         ```python
         import EasySQL
         
-        # Define database which will be needed by any table you create.
-        database = EasySQL.EasyDatabase(host='127.0.0.1', port=3306,
-                                        database='DatabaseName',
-                                        user='username', password='PASSWORD')
-        
-        # Define tables and columns
-        ID = EasySQL.EasyColumn('ID', EasySQL.INT, primary=True, auto_increment=True)
-        Name = EasySQL.EasyColumn('Name', EasySQL.STRING(255), not_null=True, default='Missing')
-        Balance = EasySQL.EasyColumn('Balance', EasySQL.INT, not_null=True)
-        Premium = EasySQL.EasyColumn('Premium', EasySQL.BOOL, not_null=True, default=False)
-        
-        table = EasySQL.EasyTable(database, 'Users', [ID, Name, Balance, Premium])
+        # Simply provide connection info to your database
+        @EasySQL.auto_init
+        class MyDatabase(EasySQL.EasyDatabase):
+            _database = 'MyDatabase'
+            _password = '**********'
+            _host = '127.0.0.1'
+            _port = 3306
+            _user = 'root'
+        
+        # Simply create a MyTable with its columns!
+        @EasySQL.auto_init
+        class MyTable(EasySQL.EasyTable, database=MyDatabase, name='MyTable'):
+            ID = EasySQL.EasyColumn('ID', EasySQL.Types.BIGINT, EasySQL.Tags.PRIMARY, EasySQL.Tags.AUTO_INCREMENT)
+            Name = EasySQL.EasyColumn('Name', EasySQL.Types.STRING(255), EasySQL.Tags.NOT_NULL, default='Missing')
+            Balance = EasySQL.EasyColumn('Balance', EasySQL.Types.INT, EasySQL.Tags.NOT_NULL)
+            Premium = EasySQL.EasyColumn('Premium', EasySQL.Types.BOOL, EasySQL.Tags.NOT_NULL, default=False)
         
         # Insert values with a simple command
-        table.insert([Name, Premium, Balance], ['Ashenguard', True, 10])
-        table.insert([Name, Premium], ['Sam', False])
+        MyTable.insert([MyTable.Name, MyTable.Premium, MyTable.Balance], ['Ashenguard', True, 10])
+        MyTable.insert([MyTable.Name, MyTable.Premium], ['Sam', False])
         
-        # Some random data
+        # Let's add some random data 
         from random import randint
         for i in range(5):
-            table.insert([Name, Balance], [f'User-{i}', randint(0, 20)])
+            MyTable.insert(['Name', 'Balance'], [f'User-{i}', randint(0, 20)])
         
         # Selecting data with another simple command
-        ### Get all the data
-        all = table.select()
+        ### Let's get all the data
+        all = MyTable.select()
         ### Something that does not exist
-        empty = table.select(ID, where=EasySQL.WhereIsEqual(Name, "NO-ONE"))
+        empty = MyTable.select(MyTable.ID, where=EasySQL.WhereIsEqual(MyTable.Name, "NO-ONE"))
         ### To select multiple data give a list of columns as 1st argument
-        premiums = table.select([ID, Name], EasySQL.WhereIsEqual(Premium, True))
+        premiums = MyTable.select([MyTable.ID, MyTable.Name], EasySQL.WhereIsEqual(MyTable.Premium, True))
         ### You can have more complicated condition with AND (&), OR (|) and NOT (~)
-        specific = table.select(Name, where=EasySQL.WhereIsLike(Name, "Ash%").AND(EasySQL.WhereIsLesserEqual(ID, 5)))
-        ### Giving no column will select all the columns, Also you can use limit, offset and order sorting data
-        second = table.select(order=Balance, descending=True, limit=1, offset=1)
-        top5 = table.select(order=Balance, descending=True, limit=5)
-        ### If you want only one result not a sequence of them! It will return a SelectData id A data is found or return None if none is found.
-        one = table.select(where=EasySQL.WhereIsEqual(Name, "Ashenguard"), force_one=True)
+        specific = MyTable.select(MyTable.Name, where=EasySQL.WhereIsLike(MyTable.Name, "Ash%").AND(EasySQL.WhereIsLesserEqual(MyTable.ID, 5)))
+        ### Giving no column will select all the columns, Also you can use limit, offset and order to sort data
+        second = MyTable.select(order=MyTable.Balance, descending=True, limit=1, offset=1)
+        top5 = MyTable.select(order=MyTable.Balance, descending=True, limit=5)
+        ### If you want only one result not a sequence of them! It will return a SelectData if a data is found or return None if none is found.
+        one = MyTable.select(where=EasySQL.WhereIsEqual(MyTable.Name, "Ashenguard"), force_one=True)
         
         # The result will be an EmptySelectData if nothing was found, A SelectData if only one was found, Or a tuple of SelectData
         # All 3 of them are iterable, so it is safe to use a `for` loop for any result
         # To get data from the result you can use `get`, but it only contains columns requested in select method.
         for data in top5:
-            print(f'{data.get(ID)}: {data.get(Name)}\tBalance: {data.get(Balance)}')
+            print(f'{data.get(MyTable.ID)}: {data.get(MyTable.Name)}\tBalance: {data.get(MyTable.Balance)}')
         
         # To delete data just use the delete method
-        table.delete(EasySQL.WhereIsGreater(ID, 5))
+        MyTable.delete(EasySQL.WhereIsGreater(MyTable.ID, 5))
         
         # Update data with following command
-        table.update(Premium, True, EasySQL.WhereIsEqual(ID, 3).OR(EasySQL.WhereIsEqual(Name, 'Sam')))
+        MyTable.update(MyTable.Premium, True, EasySQL.WhereIsEqual(MyTable.ID, 3).OR(EasySQL.WhereIsEqual(MyTable.Name, 'Sam')))
         
         # Not sure if you should update or insert? Use set and it will be handled
-        table.set([ID, Name, Balance, Premium], [5, 'Nathaniel', 50, False], where=EasySQL.WhereIsEqual(ID, 5))
+        MyTable.set([MyTable.ID, MyTable.Name, MyTable.Balance, MyTable.Premium], [5, 'Nathaniel', 50, False], where=EasySQL.WhereIsEqual(MyTable.ID, 5))
         
         # Safety error on delete/update/set without a where statement
-        # table.delete() -> raise EasySQL.DatabaseSafetyException
+        # MyTable.delete() -> raise EasySQL.DatabaseSafetyException
         # Turn the safety off with following command.
-        database.remove_safety(confirm=True)
+        MyDatabase.remove_safety(confirm=True)
         # Now there will be no error, it will clean the all data that's why we had safety lock
-        table.delete()
+        MyTable.delete()
         ```
         
         [![AdFoc.us Banner](https://adfoc.us/images/banners/728x90-2.gif)](https://adfoc.us/?refid=497244)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyEasySQL-2.0.2/PyEasySQL.egg-info/PKG-INFO` & `PyEasySQL-3.0.2/PyEasySQL.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,116 @@
 Metadata-Version: 2.1
 Name: PyEasySQL
-Version: 2.0.2
+Version: 3.0.2
 Summary: SQL Database management without even a SQL line
 Home-page: https://github.com/ashenguard/easysql
 Author: Ashenguard
 Author-email: Ashenguard@agmdev.xyz
 License: MIT License
 Description: # EasySQL
         ![Downloads](https://pepy.tech/badge/pyeasysql)
         ![Downloads](https://pepy.tech/badge/pyeasysql/week)
         ![Downloads](https://pepy.tech/badge/pyeasysql/month)  
         This library allow you to run SQL Databases without knowing even SQL.  
         This library will create SQL queries and execute them as you request and is very simple to use.
         
-        ### Support
-        You can find support on our discord server here:
-        > https://discord.gg/6exsySK  
-        > Pay us a visit there ✌
+        ### Having an issue?
+        You can always find someone on our discord server here:
+        > https://discord.gg/6exsySK
         
         ### Wiki
         The official wiki of this library is now available at GitHub
-        > https://github.com/Ashengaurd/EasySQL/wiki
-        
+        > https://github.com/Ashenguard/EasySQL/wiki
         
         ## How to install
         ![](https://img.shields.io/github/v/release/Ashengaurd/EasySQL?label=Release&logo=github&style=plastic)
         ![](https://img.shields.io/github/last-commit/Ashengaurd/EasySQL/master?label=Date&logo=git&logoColor=blue&style=plastic)  
         ![](https://img.shields.io/github/v/release/Ashengaurd/EasySQL?include_prereleases&label=Development&logo=github&style=plastic)
         ![](https://img.shields.io/github/last-commit/Ashengaurd/EasySQL?label=Date&logo=git&logoColor=red&style=plastic)  
         To install just use following command
         ```shell
         pip install PyEasySQL
         ```
         This library will have dev/beta builds on the GitHub, to install them you can use
         
         ```shell
-        pip install --upgrade git+https://github.com/Ashengaurd/EasySQL.git
+        pip install --upgrade git+https://github.com/Ashenguard/EasySQL.git
         ```
         ***
         By installing this library following libraries and their dependencies will be installed too.
-        > mysql-connector: Which is the basic library for connecting to database
-        
+        ```yaml
+        mysql-connector: Which is the basic library for connecting to database
+        ```
         # Example
         
         ```python
         import EasySQL
         
-        # Define database which will be needed by any table you create.
-        database = EasySQL.EasyDatabase(host='127.0.0.1', port=3306,
-                                        database='DatabaseName',
-                                        user='username', password='PASSWORD')
-        
-        # Define tables and columns
-        ID = EasySQL.EasyColumn('ID', EasySQL.INT, primary=True, auto_increment=True)
-        Name = EasySQL.EasyColumn('Name', EasySQL.STRING(255), not_null=True, default='Missing')
-        Balance = EasySQL.EasyColumn('Balance', EasySQL.INT, not_null=True)
-        Premium = EasySQL.EasyColumn('Premium', EasySQL.BOOL, not_null=True, default=False)
-        
-        table = EasySQL.EasyTable(database, 'Users', [ID, Name, Balance, Premium])
+        # Simply provide connection info to your database
+        @EasySQL.auto_init
+        class MyDatabase(EasySQL.EasyDatabase):
+            _database = 'MyDatabase'
+            _password = '**********'
+            _host = '127.0.0.1'
+            _port = 3306
+            _user = 'root'
+        
+        # Simply create a MyTable with its columns!
+        @EasySQL.auto_init
+        class MyTable(EasySQL.EasyTable, database=MyDatabase, name='MyTable'):
+            ID = EasySQL.EasyColumn('ID', EasySQL.Types.BIGINT, EasySQL.Tags.PRIMARY, EasySQL.Tags.AUTO_INCREMENT)
+            Name = EasySQL.EasyColumn('Name', EasySQL.Types.STRING(255), EasySQL.Tags.NOT_NULL, default='Missing')
+            Balance = EasySQL.EasyColumn('Balance', EasySQL.Types.INT, EasySQL.Tags.NOT_NULL)
+            Premium = EasySQL.EasyColumn('Premium', EasySQL.Types.BOOL, EasySQL.Tags.NOT_NULL, default=False)
         
         # Insert values with a simple command
-        table.insert([Name, Premium, Balance], ['Ashenguard', True, 10])
-        table.insert([Name, Premium], ['Sam', False])
+        MyTable.insert([MyTable.Name, MyTable.Premium, MyTable.Balance], ['Ashenguard', True, 10])
+        MyTable.insert([MyTable.Name, MyTable.Premium], ['Sam', False])
         
-        # Some random data
+        # Let's add some random data 
         from random import randint
         for i in range(5):
-            table.insert([Name, Balance], [f'User-{i}', randint(0, 20)])
+            MyTable.insert(['Name', 'Balance'], [f'User-{i}', randint(0, 20)])
         
         # Selecting data with another simple command
-        ### Get all the data
-        all = table.select()
+        ### Let's get all the data
+        all = MyTable.select()
         ### Something that does not exist
-        empty = table.select(ID, where=EasySQL.WhereIsEqual(Name, "NO-ONE"))
+        empty = MyTable.select(MyTable.ID, where=EasySQL.WhereIsEqual(MyTable.Name, "NO-ONE"))
         ### To select multiple data give a list of columns as 1st argument
-        premiums = table.select([ID, Name], EasySQL.WhereIsEqual(Premium, True))
+        premiums = MyTable.select([MyTable.ID, MyTable.Name], EasySQL.WhereIsEqual(MyTable.Premium, True))
         ### You can have more complicated condition with AND (&), OR (|) and NOT (~)
-        specific = table.select(Name, where=EasySQL.WhereIsLike(Name, "Ash%").AND(EasySQL.WhereIsLesserEqual(ID, 5)))
-        ### Giving no column will select all the columns, Also you can use limit, offset and order sorting data
-        second = table.select(order=Balance, descending=True, limit=1, offset=1)
-        top5 = table.select(order=Balance, descending=True, limit=5)
-        ### If you want only one result not a sequence of them! It will return a SelectData id A data is found or return None if none is found.
-        one = table.select(where=EasySQL.WhereIsEqual(Name, "Ashenguard"), force_one=True)
+        specific = MyTable.select(MyTable.Name, where=EasySQL.WhereIsLike(MyTable.Name, "Ash%").AND(EasySQL.WhereIsLesserEqual(MyTable.ID, 5)))
+        ### Giving no column will select all the columns, Also you can use limit, offset and order to sort data
+        second = MyTable.select(order=MyTable.Balance, descending=True, limit=1, offset=1)
+        top5 = MyTable.select(order=MyTable.Balance, descending=True, limit=5)
+        ### If you want only one result not a sequence of them! It will return a SelectData if a data is found or return None if none is found.
+        one = MyTable.select(where=EasySQL.WhereIsEqual(MyTable.Name, "Ashenguard"), force_one=True)
         
         # The result will be an EmptySelectData if nothing was found, A SelectData if only one was found, Or a tuple of SelectData
         # All 3 of them are iterable, so it is safe to use a `for` loop for any result
         # To get data from the result you can use `get`, but it only contains columns requested in select method.
         for data in top5:
-            print(f'{data.get(ID)}: {data.get(Name)}\tBalance: {data.get(Balance)}')
+            print(f'{data.get(MyTable.ID)}: {data.get(MyTable.Name)}\tBalance: {data.get(MyTable.Balance)}')
         
         # To delete data just use the delete method
-        table.delete(EasySQL.WhereIsGreater(ID, 5))
+        MyTable.delete(EasySQL.WhereIsGreater(MyTable.ID, 5))
         
         # Update data with following command
-        table.update(Premium, True, EasySQL.WhereIsEqual(ID, 3).OR(EasySQL.WhereIsEqual(Name, 'Sam')))
+        MyTable.update(MyTable.Premium, True, EasySQL.WhereIsEqual(MyTable.ID, 3).OR(EasySQL.WhereIsEqual(MyTable.Name, 'Sam')))
         
         # Not sure if you should update or insert? Use set and it will be handled
-        table.set([ID, Name, Balance, Premium], [5, 'Nathaniel', 50, False], where=EasySQL.WhereIsEqual(ID, 5))
+        MyTable.set([MyTable.ID, MyTable.Name, MyTable.Balance, MyTable.Premium], [5, 'Nathaniel', 50, False], where=EasySQL.WhereIsEqual(MyTable.ID, 5))
         
         # Safety error on delete/update/set without a where statement
-        # table.delete() -> raise EasySQL.DatabaseSafetyException
+        # MyTable.delete() -> raise EasySQL.DatabaseSafetyException
         # Turn the safety off with following command.
-        database.remove_safety(confirm=True)
+        MyDatabase.remove_safety(confirm=True)
         # Now there will be no error, it will clean the all data that's why we had safety lock
-        table.delete()
+        MyTable.delete()
         ```
         
         [![AdFoc.us Banner](https://adfoc.us/images/banners/728x90-2.gif)](https://adfoc.us/?refid=497244)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyEasySQL-2.0.2/README.md` & `PyEasySQL-3.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,104 @@
 # EasySQL
 ![Downloads](https://pepy.tech/badge/pyeasysql)
 ![Downloads](https://pepy.tech/badge/pyeasysql/week)
 ![Downloads](https://pepy.tech/badge/pyeasysql/month)  
 This library allow you to run SQL Databases without knowing even SQL.  
 This library will create SQL queries and execute them as you request and is very simple to use.
 
-### Support
-You can find support on our discord server here:
-> https://discord.gg/6exsySK  
-> Pay us a visit there ✌
+### Having an issue?
+You can always find someone on our discord server here:
+> https://discord.gg/6exsySK
 
 ### Wiki
 The official wiki of this library is now available at GitHub
-> https://github.com/Ashengaurd/EasySQL/wiki
-
+> https://github.com/Ashenguard/EasySQL/wiki
 
 ## How to install
 ![](https://img.shields.io/github/v/release/Ashengaurd/EasySQL?label=Release&logo=github&style=plastic)
 ![](https://img.shields.io/github/last-commit/Ashengaurd/EasySQL/master?label=Date&logo=git&logoColor=blue&style=plastic)  
 ![](https://img.shields.io/github/v/release/Ashengaurd/EasySQL?include_prereleases&label=Development&logo=github&style=plastic)
 ![](https://img.shields.io/github/last-commit/Ashengaurd/EasySQL?label=Date&logo=git&logoColor=red&style=plastic)  
 To install just use following command
 ```shell
 pip install PyEasySQL
 ```
 This library will have dev/beta builds on the GitHub, to install them you can use
 
 ```shell
-pip install --upgrade git+https://github.com/Ashengaurd/EasySQL.git
+pip install --upgrade git+https://github.com/Ashenguard/EasySQL.git
 ```
 ***
 By installing this library following libraries and their dependencies will be installed too.
-> mysql-connector: Which is the basic library for connecting to database
-
+```yaml
+mysql-connector: Which is the basic library for connecting to database
+```
 # Example
 
 ```python
 import EasySQL
 
-# Define database which will be needed by any table you create.
-database = EasySQL.EasyDatabase(host='127.0.0.1', port=3306,
-                                database='DatabaseName',
-                                user='username', password='PASSWORD')
-
-# Define tables and columns
-ID = EasySQL.EasyColumn('ID', EasySQL.INT, primary=True, auto_increment=True)
-Name = EasySQL.EasyColumn('Name', EasySQL.STRING(255), not_null=True, default='Missing')
-Balance = EasySQL.EasyColumn('Balance', EasySQL.INT, not_null=True)
-Premium = EasySQL.EasyColumn('Premium', EasySQL.BOOL, not_null=True, default=False)
-
-table = EasySQL.EasyTable(database, 'Users', [ID, Name, Balance, Premium])
+# Simply provide connection info to your database
+@EasySQL.auto_init
+class MyDatabase(EasySQL.EasyDatabase):
+    _database = 'MyDatabase'
+    _password = '**********'
+    _host = '127.0.0.1'
+    _port = 3306
+    _user = 'root'
+
+# Simply create a MyTable with its columns!
+@EasySQL.auto_init
+class MyTable(EasySQL.EasyTable, database=MyDatabase, name='MyTable'):
+    ID = EasySQL.EasyColumn('ID', EasySQL.Types.BIGINT, EasySQL.Tags.PRIMARY, EasySQL.Tags.AUTO_INCREMENT)
+    Name = EasySQL.EasyColumn('Name', EasySQL.Types.STRING(255), EasySQL.Tags.NOT_NULL, default='Missing')
+    Balance = EasySQL.EasyColumn('Balance', EasySQL.Types.INT, EasySQL.Tags.NOT_NULL)
+    Premium = EasySQL.EasyColumn('Premium', EasySQL.Types.BOOL, EasySQL.Tags.NOT_NULL, default=False)
 
 # Insert values with a simple command
-table.insert([Name, Premium, Balance], ['Ashenguard', True, 10])
-table.insert([Name, Premium], ['Sam', False])
+MyTable.insert([MyTable.Name, MyTable.Premium, MyTable.Balance], ['Ashenguard', True, 10])
+MyTable.insert([MyTable.Name, MyTable.Premium], ['Sam', False])
 
-# Some random data
+# Let's add some random data 
 from random import randint
 for i in range(5):
-    table.insert([Name, Balance], [f'User-{i}', randint(0, 20)])
+    MyTable.insert(['Name', 'Balance'], [f'User-{i}', randint(0, 20)])
 
 # Selecting data with another simple command
-### Get all the data
-all = table.select()
+### Let's get all the data
+all = MyTable.select()
 ### Something that does not exist
-empty = table.select(ID, where=EasySQL.WhereIsEqual(Name, "NO-ONE"))
+empty = MyTable.select(MyTable.ID, where=EasySQL.WhereIsEqual(MyTable.Name, "NO-ONE"))
 ### To select multiple data give a list of columns as 1st argument
-premiums = table.select([ID, Name], EasySQL.WhereIsEqual(Premium, True))
+premiums = MyTable.select([MyTable.ID, MyTable.Name], EasySQL.WhereIsEqual(MyTable.Premium, True))
 ### You can have more complicated condition with AND (&), OR (|) and NOT (~)
-specific = table.select(Name, where=EasySQL.WhereIsLike(Name, "Ash%").AND(EasySQL.WhereIsLesserEqual(ID, 5)))
-### Giving no column will select all the columns, Also you can use limit, offset and order sorting data
-second = table.select(order=Balance, descending=True, limit=1, offset=1)
-top5 = table.select(order=Balance, descending=True, limit=5)
-### If you want only one result not a sequence of them! It will return a SelectData id A data is found or return None if none is found.
-one = table.select(where=EasySQL.WhereIsEqual(Name, "Ashenguard"), force_one=True)
+specific = MyTable.select(MyTable.Name, where=EasySQL.WhereIsLike(MyTable.Name, "Ash%").AND(EasySQL.WhereIsLesserEqual(MyTable.ID, 5)))
+### Giving no column will select all the columns, Also you can use limit, offset and order to sort data
+second = MyTable.select(order=MyTable.Balance, descending=True, limit=1, offset=1)
+top5 = MyTable.select(order=MyTable.Balance, descending=True, limit=5)
+### If you want only one result not a sequence of them! It will return a SelectData if a data is found or return None if none is found.
+one = MyTable.select(where=EasySQL.WhereIsEqual(MyTable.Name, "Ashenguard"), force_one=True)
 
 # The result will be an EmptySelectData if nothing was found, A SelectData if only one was found, Or a tuple of SelectData
 # All 3 of them are iterable, so it is safe to use a `for` loop for any result
 # To get data from the result you can use `get`, but it only contains columns requested in select method.
 for data in top5:
-    print(f'{data.get(ID)}: {data.get(Name)}\tBalance: {data.get(Balance)}')
+    print(f'{data.get(MyTable.ID)}: {data.get(MyTable.Name)}\tBalance: {data.get(MyTable.Balance)}')
 
 # To delete data just use the delete method
-table.delete(EasySQL.WhereIsGreater(ID, 5))
+MyTable.delete(EasySQL.WhereIsGreater(MyTable.ID, 5))
 
 # Update data with following command
-table.update(Premium, True, EasySQL.WhereIsEqual(ID, 3).OR(EasySQL.WhereIsEqual(Name, 'Sam')))
+MyTable.update(MyTable.Premium, True, EasySQL.WhereIsEqual(MyTable.ID, 3).OR(EasySQL.WhereIsEqual(MyTable.Name, 'Sam')))
 
 # Not sure if you should update or insert? Use set and it will be handled
-table.set([ID, Name, Balance, Premium], [5, 'Nathaniel', 50, False], where=EasySQL.WhereIsEqual(ID, 5))
+MyTable.set([MyTable.ID, MyTable.Name, MyTable.Balance, MyTable.Premium], [5, 'Nathaniel', 50, False], where=EasySQL.WhereIsEqual(MyTable.ID, 5))
 
 # Safety error on delete/update/set without a where statement
-# table.delete() -> raise EasySQL.DatabaseSafetyException
+# MyTable.delete() -> raise EasySQL.DatabaseSafetyException
 # Turn the safety off with following command.
-database.remove_safety(confirm=True)
+MyDatabase.remove_safety(confirm=True)
 # Now there will be no error, it will clean the all data that's why we had safety lock
-table.delete()
+MyTable.delete()
 ```
 
 [![AdFoc.us Banner](https://adfoc.us/images/banners/728x90-2.gif)](https://adfoc.us/?refid=497244)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyEasySQL-2.0.2/setup.py` & `PyEasySQL-3.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyEasySQL",
-    version="2.0.2",
+    version="3.0.2",
     license='MIT License',
     author="Ashenguard",
     author_email="Ashenguard@agmdev.xyz",
     description="SQL Database management without even a SQL line",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ashenguard/easysql",
```

