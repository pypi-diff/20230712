# Comparing `tmp/yplib-2.5.1.tar.gz` & `tmp/yplib-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.5.1.tar", last modified: Wed Jul 12 03:07:34 2023, max compression
+gzip compressed data, was "dist\yplib-2.5.2.tar", last modified: Wed Jul 12 03:12:26 2023, max compression
```

## Comparing `yplib-2.5.1.tar` & `yplib-2.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 03:07:34.587878 yplib-2.5.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.5.1/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-12 03:07:34.587878 yplib-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-12 03:07:34.587878 yplib-2.5.1/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-12 03:07:17.000000 yplib-2.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 03:07:34.577674 yplib-2.5.1/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.5.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.5.1/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.5.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.5.1/yplib/db.py
--rw-rw-rw-   0        0        0     4045 2023-07-12 01:25:12.000000 yplib-2.5.1/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.5.1/yplib/http_util.py
--rw-rw-rw-   0        0        0    33578 2023-07-12 03:06:12.000000 yplib-2.5.1/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.5.1/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.5.1/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.5.1/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.5.1/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-12 03:07:34.587015 yplib-2.5.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-12 03:07:34.000000 yplib-2.5.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-12 03:07:34.000000 yplib-2.5.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 03:07:34.000000 yplib-2.5.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-12 03:07:34.000000 yplib-2.5.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 03:12:26.844484 yplib-2.5.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.5.2/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-12 03:12:26.844268 yplib-2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 03:12:26.845007 yplib-2.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-12 03:12:05.000000 yplib-2.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 03:12:26.840808 yplib-2.5.2/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.5.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.5.2/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.5.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.5.2/yplib/db.py
+-rw-rw-rw-   0        0        0     4045 2023-07-12 01:25:12.000000 yplib-2.5.2/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.5.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    33615 2023-07-12 03:11:01.000000 yplib-2.5.2/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.5.2/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.5.2/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.5.2/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.5.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-12 03:12:26.843588 yplib-2.5.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-12 03:12:26.000000 yplib-2.5.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-12 03:12:26.000000 yplib-2.5.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 03:12:26.000000 yplib-2.5.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-12 03:12:26.000000 yplib-2.5.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.5.1/LICENSE` & `yplib-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.5.1/setup.py` & `yplib-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.5.1",
+  version="2.5.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.5.1/yplib/__init__.py` & `yplib-2.5.2/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.1/yplib/chart.py` & `yplib-2.5.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.1/yplib/chart_html.py` & `yplib-2.5.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.1/yplib/db.py` & `yplib-2.5.2/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.1/yplib/file.py` & `yplib-2.5.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.1/yplib/http_util.py` & `yplib-2.5.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.1/yplib/index.py` & `yplib-2.5.2/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,18 +311,19 @@
     return str(to_datetime_add(s=s, days=days, seconds=seconds, microseconds=microseconds,
                                milliseconds=milliseconds, minutes=minutes, hours=hours, weeks=weeks))[0:10]
 
 
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # data_list   : 数组数据, 也可以不是数组
 # file_name   : 文件名 , 默认 txt
-#               当文件名是 C:\Users\yangpu\Desktop\study\abc\d\e\f\a.txt 这种类型的时候, 可以直接创建文件夹,
-#                   会赋值 file_path=C:\Users\yangpu\Desktop\study\abc\d\e\f,
-#                         file_name=a.txt,
-#                         fixed_name=True
+#               当文件名是 C:\Users\yangpu\Desktop\study\abc\d\e\f\a.sql 这种类型的时候, 可以直接创建文件夹,
+#                   会赋值 file_name=a,
+#                         file_path=C:\Users\yangpu\Desktop\study\abc\d\e\f,
+#                         fixed_name=True,
+#                         suffix=.sql
 #               当文件名是 abc 的时候, 按照正常值,计算
 # file_path   : 文件路径
 # fixed_name  : 是否固定文件名
 # suffix      : 文件后缀, 默认 .txt
 # sep_list    : 当 data_list 是 list(list) 类型的时候 使用 sep_list 作为分割内部的分隔符,
 #               默认使用 \t 作为分隔符, 如果为 None , 则按照 json 去处理这个 list
 def to_txt(data_list,
@@ -335,15 +336,15 @@
     for sep in ['\\', '/']:
         f_n = file_name.split(sep)
         if len(f_n) > 1:
             file_name = f_n[-1]
             file_path = sep.join(f_n[0:-1])
             if '.' in file_name:
                 suffix = '.' + file_name.split('.')[-1]
-                file_name = file_name[0:file_name.find('.')]
+                file_name = file_name[0:file_name.rfind('.')]
                 fixed_name = True
 
     # 检查路径 file_path
     while file_path.endswith('/'):
         file_path = file_path[0:-1]
     check_file(file_path)
     # 生成 file_name
```

### Comparing `yplib-2.5.1/yplib/mail.py` & `yplib-2.5.2/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.1/yplib/mail_html.py` & `yplib-2.5.2/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.5.1/yplib/markdown.py` & `yplib-2.5.2/yplib/markdown.py`

 * *Files identical despite different names*

