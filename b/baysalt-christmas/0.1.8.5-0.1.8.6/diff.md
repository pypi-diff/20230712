# Comparing `tmp/baysalt_christmas-0.1.8.5.tar.gz` & `tmp/baysalt_christmas-0.1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.8.5.tar", last modified: Mon Jul 10 06:54:35 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.8.6.tar", last modified: Wed Jul 12 10:17:58 2023, max compression
```

## Comparing `baysalt_christmas-0.1.8.5.tar` & `baysalt_christmas-0.1.8.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.110879 baysalt_christmas-0.1.8.5/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.8.5/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.8.5/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-10 06:54:35.110723 baysalt_christmas-0.1.8.5/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.8.5/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.101476 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-10 06:54:35.000000 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-10 06:54:35.000000 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-10 06:54:35.000000 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-10 06:54:35.000000 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-10 06:54:35.000000 baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.104076 baysalt_christmas-0.1.8.5/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.8.5/christmas/Blogging.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.104682 baysalt_christmas-0.1.8.5/christmas/Pyshell/
--rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-0.1.8.5/christmas/Pyshell/RS_File.py
--rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.8.5/christmas/Pyshell/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.8.5/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-03 02:25:27.000000 baysalt_christmas-0.1.8.5/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.8.5/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.8.5/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.109516 baysalt_christmas-0.1.8.5/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-10 06:54:35.110371 baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.8.5/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     9260 2023-07-10 06:49:33.000000 baysalt_christmas-0.1.8.5/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.8.5/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.8.5/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.8.5/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-10 06:54:35.110934 baysalt_christmas-0.1.8.5/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-10 06:54:31.000000 baysalt_christmas-0.1.8.5/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.202878 baysalt_christmas-0.1.8.6/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-06-13 08:58:02.000000 baysalt_christmas-0.1.8.6/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.8.6/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-12 10:17:58.202727 baysalt_christmas-0.1.8.6/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.8.6/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.193847 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-07-12 10:17:58.000000 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      788 2023-07-12 10:17:58.000000 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-07-12 10:17:58.000000 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-07-12 10:17:58.000000 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-07-12 10:17:58.000000 baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.197383 baysalt_christmas-0.1.8.6/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    22036 2023-07-12 10:17:28.000000 baysalt_christmas-0.1.8.6/christmas/Blogging.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.197869 baysalt_christmas-0.1.8.6/christmas/Pyshell/
+-rw-r--r--   0 christmas   (501) staff       (20)     5957 2023-07-04 08:34:25.000000 baysalt_christmas-0.1.8.6/christmas/Pyshell/RS_File.py
+-rw-r--r--   0 christmas   (501) staff       (20)      249 2023-07-03 02:25:19.000000 baysalt_christmas-0.1.8.6/christmas/Pyshell/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.8.6/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      405 2023-07-03 02:25:27.000000 baysalt_christmas-0.1.8.6/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.8.6/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.8.6/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.201633 baysalt_christmas-0.1.8.6/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-07-12 10:17:58.202400 baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.8.6/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     9260 2023-07-10 06:49:33.000000 baysalt_christmas-0.1.8.6/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3679 2023-06-12 03:11:04.000000 baysalt_christmas-0.1.8.6/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.8.6/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.8.6/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-07-12 10:17:58.202929 baysalt_christmas-0.1.8.6/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-07-12 10:17:56.000000 baysalt_christmas-0.1.8.6/setup.py
```

### Comparing `baysalt_christmas-0.1.8.5/.DS_Store` & `baysalt_christmas-0.1.8.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/PKG-INFO` & `baysalt_christmas-0.1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.8.5
+Version: 0.1.8.6
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.8.5/README.md` & `baysalt_christmas-0.1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.8.5
+Version: 0.1.8.6
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.8.5/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.8.6/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/Blogging.py` & `baysalt_christmas-0.1.8.6/christmas/Blogging.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,120 +43,125 @@
             %(process)d 进程ID。可能没有
             %(message)s用户输出的消息
     """
     
     def __init__(self, _loger_name='Christmas',  # 日志记录器名称
                  _log_filename=None,  # 日志文件名
                  _switch_write_all_log=False,  # 是否写入日志
-                 _switch_write_error_plus_log=False,  # 是否写入日志
+                 _switch_write_bug_log=False,  # 是否写入日志
                  _switch_print_log=True,  # 是否打印日志
                  _switch_write_debug_log=False,  # 是否写入单独的debug日志
                  _switch_write_info_log=False,  # 是否写入单独的info日志
                  _switch_write_warning_log=False,  # 是否写入单独的warning日志
                  _switch_write_error_log=False,  # 是否写入单独的error日志
-                 _switch_write_critical_log=False):  # 是否写入单独的critical日志
+                 _switch_write_critical_log=False, # 是否写入单独的critical日志
+                 _manual_setBlog=False ): # 是否手动设置参数
         
-        self.CRITICAL = 50
+        self.CRITICAL = logging.CRITICAL
         self.FATAL = self.CRITICAL
-        self.ERROR = 40
-        self.WARNING = 30
+        self.ERROR = logging.ERROR
+        self.WARNING = logging.WARNING
         self.WARN = self.WARNING
-        self.INFO = 20
-        self.DEBUG = 10
-        self.NOTSET = 0
+        self.INFO = logging.INFO
+        self.DEBUG = logging.DEBUG
+        self.NOTSET = logging.NOTSET
 
         self.loger_name = _loger_name  # 日志记录器名称
         self.logfile_name = _log_filename  # 日志文件名
         self.switch_write_all_log = _switch_write_all_log  # 是否写入全部日志
-        self.switch_write_error_plus_log = _switch_write_error_plus_log  # 是否写入错误日志
+        self.switch_write_bugs_log = _switch_write_bug_log  # 是否写入错误日志
         self.switch_print_log = _switch_print_log  # 是否打印日志
         self.switch_write_debug_log = _switch_write_debug_log  # 是否写入单独的debug日志
         self.switch_write_info_log = _switch_write_info_log  # 是否写入单独的info日志
         self.switch_write_warning_log = _switch_write_warning_log  # 是否写入单独的warning日志
         self.switch_write_error_log = _switch_write_error_log  # 是否写入单独的error日志
         self.switch_write_critical_log = _switch_write_critical_log  # 是否写入单独的critical日志
         
         self.log_level = None  # 日志级别
         self.maxBytes = None  # 日志文件大小
         self.backupCount = None  # 日志文件数量
         self.write_mode = None  # 日志写入模式
         self.colors_config = None  # 控制台打印颜色配置信息
         self.log_ddt_fmt = None  # 日志文件名时间格式
-        self.__all_log_path = None  # 所有日志文件路径
-        self.__error_plus_log_path = None  # 错误日志文件路径
+        self.all_log_filename = None  # 所有日志文件路径
+        self.bug_log_filename = None  # 错误日志文件路径
         self.debug_log_filename = None  # debug日志文件路径
         self.info_log_filename = None  # info日志文件路径
         self.warning_log_filename = None  # warning日志文件路径
         self.error_log_filename = None  # error日志文件路径
         self.critical_log_filename = None  # critical日志文件路径
         self.Rotating = None  # 日志文件处理器 time or size
         self.when = None  # 日志文件处理器 time --> S M H D W
         self.interval = None  # 日志文件处理器 time --> 间隔
         self.logger = logging.getLogger(self.loger_name)  # 创建日志记录器
         
         self.PARA_DEFAULT = {
             'maxBytes': 1024 * 1024 * 10,  # 日志文件大小
             'backupCount': 5,  # 日志文件数量
             'colors_config': self.__set_console_color_default(),  # 日志输出颜色
-            'log_level': logging.DEBUG,  # 日志级别
+            'log_level': logging.INFO,  # 日志级别
             'log_ddt_fmt': '%Y-%m-%d',  # 日志文件名时间格式
             'logfile_name': 'log',  # 日志文件名
             'write_mode': 'a',  # 日志文件写入模式
-            '__all_log_path': 'ALL.log',  # 日志文件路径
-            '__error_plus_log_path': 'BUG.log',  # 日志文件路径
+            'all_log_filename': 'ALL.log',  # 日志文件路径
+            'bug_log_filename': 'BUG.log',  # 日志文件路径
             'debug_log_filename': 'debug.log',  # 日志文件路径
             'info_log_filename': 'info.log',  # 日志文件路径
             'warning_log_filename': 'warning.log',  # 日志文件路径
             'error_log_filename': 'error.log',  # 日志文件路径
             'critical_log_filename': 'critical.log',  # 日志文件路径
             'Rotating': 'size',  # 日志文件处理器 time or size
             'when': 'D',  # 日志文件处理器 time --> S M H D W
             'interval': 1,  # 日志文件处理器 time --> 间隔
         }
         if self.logfile_name is not None:
-            self.PARA_DEFAULT['__all_log_path'] = f'{self.logfile_name}_ALL.log'
-            self.PARA_DEFAULT['__error_plus_log_path'] = f'{self.logfile_name}_BUG.log'
+            self.PARA_DEFAULT['all_log_filename'] = f'{self.logfile_name}_ALL.log'
+            self.PARA_DEFAULT['bug_log_filename'] = f'{self.logfile_name}_BUG.log'
             self.PARA_DEFAULT['debug_log_filename'] = f'{self.logfile_name}_debug.log'
             self.PARA_DEFAULT['info_log_filename'] = f'{self.logfile_name}_info.log'
             self.PARA_DEFAULT['warning_log_filename'] = f'{self.logfile_name}_warning.log'
             self.PARA_DEFAULT['error_log_filename'] = f'{self.logfile_name}_error.log'
             self.PARA_DEFAULT['critical_log_filename'] = f'{self.logfile_name}_critical.log'
         
         self.PARA = self.PARA_DEFAULT
-        self.setup_Blog()
-        self.console()
+        if not _manual_setBlog:
+            self.setup_Blog()
+            self.console()
     
     def setup_Blog(self, **kwargs):
         
         self.PARA.update(kwargs)
         self.maxBytes = self.PARA['maxBytes']
         self.backupCount = self.PARA['backupCount']
         self.colors_config = self.PARA['colors_config']
         self.log_level = self.PARA['log_level']
         self.log_ddt_fmt = self.PARA['log_ddt_fmt']
         self.write_mode = self.PARA['write_mode']
-        self.__all_log_path = self.PARA['__all_log_path']
-        self.__error_plus_log_path = self.PARA['__error_plus_log_path']
+        self.all_log_filename = self.PARA['all_log_filename']
+        self.bug_log_filename = self.PARA['bug_log_filename']
         self.debug_log_filename = self.PARA['debug_log_filename']
         self.info_log_filename = self.PARA['info_log_filename']
         self.warning_log_filename = self.PARA['warning_log_filename']
         self.error_log_filename = self.PARA['error_log_filename']
         self.critical_log_filename = self.PARA['critical_log_filename']
         self.Rotating = self.PARA['Rotating']
         self.when = self.PARA['when']
         self.interval = self.PARA['interval']
         
         if self.write_mode == 'w':  # 删除已存在的日志文件
-            rmfiles(self.__all_log_path,
-                    self.__error_plus_log_path,
+            rmfiles(self.all_log_filename,
+                    self.bug_log_filename,
                     self.debug_log_filename,
                     self.info_log_filename,
                     self.warning_log_filename,
                     self.error_log_filename,
                     self.critical_log_filename)
+        self.__rm_random_FileHandler()  # 删除日志记录器handler
+        #       实例化之后，再次调用setup_Blog()，会重复添加handler，导致日志重复打印 --> 已解决
+        # TODO: 实例化之后，再次调用setup_Blog()，会重复添加handler，删除日志记录器handler时，文件已经存在，需要删除文件 --> 未解决
         self.console()
     
     def __init_logger_handler(self, logfile_path, Rotating='time', when='H', interval=1):
         # sourcery skip: inline-immediately-returned-variable
         """
         创建日志记录器handler，用于收集日志
         :param logfile_path: 日志文件路径
@@ -262,50 +267,49 @@
         关闭日志记录器
         :param logger_handler: 日志记录器
         """
         logger_handler.close()
     
     def console(self):
         """构造日志收集器"""
-        # self.setup_Blog()  # 初始化
         self.logger.setLevel(self.log_level)  # 设置日志收集器级别
 
         if self.logger.hasHandlers():  # 如果已经有日志记录器，先关闭
             self.logger.handlers.clear()
         if self.logger.filters:  # 如果已经有日志过滤器，先关闭
             self.logger.filters.clear()
         if self.switch_write_all_log:  # 是否写入全部日志
             self.__write_all_log()
-        if self.switch_write_error_plus_log:  # 是否写入错误日志
+        if self.switch_write_bugs_log:  # 是否写入错误日志
             self.__write_error_plus_log()
         if self.switch_print_log:  # 是否打印日志
             self.__print_log()
-        if self.switch_write_debug_log:
+        if self.switch_write_debug_log: # 是否写入debug日志
             self.__write_random_log(level=logging.DEBUG, _level_log_name=self.debug_log_filename)
-        if self.switch_write_info_log:
+        if self.switch_write_info_log: # 是否写入info日志
             self.__write_random_log(level=logging.INFO, _level_log_name=self.info_log_filename)
-        if self.switch_write_warning_log:
+        if self.switch_write_warning_log: # 是否写入warning日志
             self.__write_random_log(level=logging.WARNING, _level_log_name=self.warning_log_filename)
-        if self.switch_write_error_log:
+        if self.switch_write_error_log: # 是否写入error日志
             self.__write_random_log(level=logging.ERROR, _level_log_name=self.error_log_filename)
-        if self.switch_write_critical_log:
+        if self.switch_write_critical_log: # 是否写入critical日志
             self.__write_random_log(level=logging.CRITICAL, _level_log_name=self.critical_log_filename)
             
         # 如果console被执行了一次，那么删除之前的执行结果，重新执行
         return self.logger
     
     def __write_all_log(self):
-        all_logger_handler = self.__init_logger_handler(self.__all_log_path, Rotating=self.Rotating, when=self.when,
+        all_logger_handler = self.__init_logger_handler(self.all_log_filename, Rotating=self.Rotating, when=self.when,
                                                         interval=self.interval)  # 收集所有日志文件
         self.__set_log_formatter(all_logger_handler)  # 设置日志输出格式-all日志文件
         self.__set_log_handler(all_logger_handler, level=logging.DEBUG)  # 设置handler级别并添加到logger收集器
         self.__close_log_handler(all_logger_handler)  # 关闭handler
     
     def __write_error_plus_log(self):
-        error_logger_handler = self.__init_logger_handler(self.__error_plus_log_path, Rotating=self.Rotating,
+        error_logger_handler = self.__init_logger_handler(self.bug_log_filename, Rotating=self.Rotating,
                                                           when=self.when, interval=self.interval)  # 收集错误日志信息文件
         self.__set_log_formatter(error_logger_handler)  # 设置日志输出格式-error日志文件
         self.__set_log_handler(error_logger_handler, level=logging.ERROR)  # 设置handler级别并添加到logger收集器
         self.__close_log_handler(error_logger_handler)  # 关闭handler
     
     def __print_log(self):
         console_handle = colorlog.StreamHandler()  # 创建终端日志记录器handler，用于输出到控制台
@@ -315,15 +319,22 @@
     
     def __write_random_log(self, level=logging.ERROR, _level_log_name='all.log'):  # 日志单独输出
         random_logger_handler = self.__init_logger_handler(_level_log_name, Rotating=self.Rotating, when=self.when,
                                                            interval=self.interval)  # 收集随机日志信息文件
         self.__set_log_formatter(random_logger_handler)  # 设置日志输出格式-random日志文件
         self.__set_log_Filter(random_logger_handler, level)  # 设置过滤器
         self.__close_log_handler(random_logger_handler)  # 关闭handler
-    
+
+    def __rm_random_FileHandler(self):  # 删除日志文件并关闭日志记录器
+        handlers = self.logger.handlers
+        for handler in handlers.copy():
+            if isinstance(handler, logging.FileHandler):  # 找到文件处理器，进行删除操作
+                self.logger.removeHandler(handler)
+                handler.close()  # 关闭文件处理器，释放资源
+
     @staticmethod
     def addLevelName(level, levelName):
         logging.addLevelName(level, levelName)
     
     @staticmethod
     def getLevelName(level):
         return logging.getLevelName(level)
@@ -392,15 +403,15 @@
         Blog().logger.log(level, msg, *args, **kwargs)
 
 
 def example_Blog():
     log2 = Blog(_loger_name='Christmas',  # 日志收集器名称
                 _log_filename='ChristmasWRITING',  # 日志文件名前缀
                 _switch_write_all_log=True,  # 是否写入全部日志 ALL.log
-                _switch_write_error_plus_log=True,  # 是否写入错误日志 BUG.log
+                _switch_write_bug_log=True,  # 是否写入错误日志 BUG.log
                 _switch_print_log=True,  # 是否打印日志到控制台
                 _switch_write_debug_log=True,  # 是否写入debug日志
                 _switch_write_info_log=True,  # 是否写入info日志
                 _switch_write_warning_log=True,  # 是否写入warning日志
                 _switch_write_error_log=True,  # 是否写入error日志
                 _switch_write_critical_log=True,  # 是否写入critical日志
                 )
```

### Comparing `baysalt_christmas-0.1.8.5/christmas/Pyshell/RS_File.py` & `baysalt_christmas-0.1.8.6/christmas/Pyshell/RS_File.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/S_DateTime.py` & `baysalt_christmas-0.1.8.6/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/commonCode.py` & `baysalt_christmas-0.1.8.6/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/cprintf.py` & `baysalt_christmas-0.1.8.6/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.8.6/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.8.6/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.8.6/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/mncPy/common.py` & `baysalt_christmas-0.1.8.6/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.8.6/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/processBar.py` & `baysalt_christmas-0.1.8.6/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/read_conf.py` & `baysalt_christmas-0.1.8.6/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/christmas/server_info.py` & `baysalt_christmas-0.1.8.6/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.8.5/setup.py` & `baysalt_christmas-0.1.8.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.8.5",
+    version="0.1.8.6",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

