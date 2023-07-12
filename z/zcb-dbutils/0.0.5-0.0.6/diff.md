# Comparing `tmp/zcb_dbutils-0.0.5.tar.gz` & `tmp/zcb_dbutils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcb_dbutils-0.0.5.tar", last modified: Thu Jun 29 12:59:57 2023, max compression
+gzip compressed data, was "zcb_dbutils-0.0.6.tar", last modified: Wed Jul 12 10:42:18 2023, max compression
```

## Comparing `zcb_dbutils-0.0.5.tar` & `zcb_dbutils-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-30 02:02:44.033681 zcb_dbutils-0.0.5/
--rwxrwxrwx   0 root         (0) root         (0)     1083 2023-06-28 11:16:31.000000 zcb_dbutils-0.0.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1204 2023-06-30 02:02:44.031681 zcb_dbutils-0.0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      797 2023-06-30 02:02:09.000000 zcb_dbutils-0.0.5/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-30 02:02:44.034681 zcb_dbutils-0.0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      755 2023-06-30 02:01:49.000000 zcb_dbutils-0.0.5/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-30 02:02:43.926654 zcb_dbutils-0.0.5/test/
--rwxrwxrwx   0 root         (0) root         (0)      757 2023-06-30 02:00:18.000000 zcb_dbutils-0.0.5/test/test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-30 02:02:43.951915 zcb_dbutils-0.0.5/zcb_dbutils/
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-06-28 10:37:05.000000 zcb_dbutils-0.0.5/zcb_dbutils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5738 2023-06-30 02:01:23.000000 zcb_dbutils-0.0.5/zcb_dbutils/dbutils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-30 02:02:44.012647 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1204 2023-06-30 02:02:43.000000 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      260 2023-06-30 02:02:43.000000 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-30 02:02:43.000000 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2023-06-30 02:02:43.000000 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-06-30 02:02:43.000000 zcb_dbutils-0.0.5/zcb_dbutils.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-12 10:42:18.808517 zcb_dbutils-0.0.6/
+-rwxrwxrwx   0 root         (0) root         (0)     1083 2023-06-28 11:16:31.000000 zcb_dbutils-0.0.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-12 10:42:18.807002 zcb_dbutils-0.0.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      956 2023-07-12 10:39:53.000000 zcb_dbutils-0.0.6/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-12 10:42:18.809525 zcb_dbutils-0.0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      755 2023-07-12 10:36:39.000000 zcb_dbutils-0.0.6/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-12 10:42:18.705244 zcb_dbutils-0.0.6/test/
+-rwxrwxrwx   0 root         (0) root         (0)      935 2023-07-12 10:39:00.000000 zcb_dbutils-0.0.6/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-12 10:42:18.728337 zcb_dbutils-0.0.6/zcb_dbutils/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-06-28 10:37:05.000000 zcb_dbutils-0.0.6/zcb_dbutils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6123 2023-07-12 10:36:39.000000 zcb_dbutils-0.0.6/zcb_dbutils/dbutils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-12 10:42:18.792945 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-07-12 10:42:18.000000 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      260 2023-07-12 10:42:18.000000 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-12 10:42:18.000000 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2023-07-12 10:42:18.000000 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       12 2023-07-12 10:42:18.000000 zcb_dbutils-0.0.6/zcb_dbutils.egg-info/top_level.txt
```

### Comparing `zcb_dbutils-0.0.5/LICENSE` & `zcb_dbutils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zcb_dbutils-0.0.5/PKG-INFO` & `zcb_dbutils-0.0.6/zcb_dbutils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zcb_dbutils
-Version: 0.0.5
+Name: zcb-dbutils
+Version: 0.0.6
 Summary: db utils with pymysql by chzcb
 Home-page: https://github.com/chzcb/dbutils
 Author: chzcb
 Author-email: chzcb.04@163.com
 License: MIT
 Keywords: python,pymysql,zcb_dbutils
 Classifier: Development Status :: 3 - Alpha
@@ -36,8 +36,12 @@
 print(pd.DataFrame.from_dict(ret))
 
 ret = dbconn.show_table_index('basic', 'tb_user')
 print(pd.DataFrame.from_dict(ret))
 
 rows = dbconn.fetch_list('select user_id,id from tb_user')
 print(rows)
+
+id = dbconn.insert('insert into tb_role (role_name,role_type,remark_info,created,updated) value (%s,1,%s,0,0)',('xxx', 'xxxx'))
+dbconn.commit()
+print(id)
 ```
```

### Comparing `zcb_dbutils-0.0.5/setup.py` & `zcb_dbutils-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'db utils with pymysql by chzcb'
 
 setup(
     name="zcb_dbutils",
     version=VERSION,
     author="chzcb",
     author_email="chzcb.04@163.com",
```

### Comparing `zcb_dbutils-0.0.5/test/test.py` & `zcb_dbutils-0.0.6/test/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,8 +15,12 @@
 ret = dbconn.showtable('basic', 'tb_user')
 print(pd.DataFrame.from_dict(ret))
 
 ret = dbconn.show_table_index('basic', 'tb_user')
 print(pd.DataFrame.from_dict(ret))
 
 rows = dbconn.fetch_list('select user_id,id from tb_user')
-print(rows)
+print(rows)
+
+id = dbconn.insert('insert into tb_role (org_id,role_no,role_name,role_type,remark_info,created,updated) value (1,1,%s,1,%s,0,0)',('xxx', 'xxxx'))
+dbconn.commit()
+print(id)
```

### Comparing `zcb_dbutils-0.0.5/zcb_dbutils/dbutils.py` & `zcb_dbutils-0.0.6/zcb_dbutils/dbutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,28 @@
                 self.cursor.execute(command)
                 self.conn.commit()
             except Exception as e:
                 logging.info(e, exc_info=True, stack_info=True)
                 return False
         return True
 
+    def insert(self, sql, args=None):
+        """
+        插入一条，返回自增ID
+        :param sql:
+        :param args:
+        :return:
+        """
+        try:
+            self.cursor.execute(sql, args)
+            return self.cursor.lastrowid
+        except Exception as e:
+            logging.info(e, exc_info=True, stack_info=True)
+            return None
+
     def exec_sql(self, command):
         try:
             self.cursor.execute(command)
             return True
         except Exception as e:
             logging.info(e, exc_info=True, stack_info=True)
             return False
```

### Comparing `zcb_dbutils-0.0.5/zcb_dbutils.egg-info/PKG-INFO` & `zcb_dbutils-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zcb-dbutils
-Version: 0.0.5
+Name: zcb_dbutils
+Version: 0.0.6
 Summary: db utils with pymysql by chzcb
 Home-page: https://github.com/chzcb/dbutils
 Author: chzcb
 Author-email: chzcb.04@163.com
 License: MIT
 Keywords: python,pymysql,zcb_dbutils
 Classifier: Development Status :: 3 - Alpha
@@ -36,8 +36,12 @@
 print(pd.DataFrame.from_dict(ret))
 
 ret = dbconn.show_table_index('basic', 'tb_user')
 print(pd.DataFrame.from_dict(ret))
 
 rows = dbconn.fetch_list('select user_id,id from tb_user')
 print(rows)
+
+id = dbconn.insert('insert into tb_role (role_name,role_type,remark_info,created,updated) value (%s,1,%s,0,0)',('xxx', 'xxxx'))
+dbconn.commit()
+print(id)
 ```
```

