# Comparing `tmp/yplib-2.4.6.tar.gz` & `tmp/yplib-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-2.4.6.tar", last modified: Tue Jul 11 06:31:23 2023, max compression
+gzip compressed data, was "dist\yplib-2.4.7.tar", last modified: Wed Jul 12 00:17:43 2023, max compression
```

## Comparing `yplib-2.4.6.tar` & `yplib-2.4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 06:31:23.328307 yplib-2.4.6/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.6/LICENSE
--rw-rw-rw-   0        0        0      352 2023-07-11 06:31:23.327700 yplib-2.4.6/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 06:31:23.328307 yplib-2.4.6/setup.cfg
--rw-rw-rw-   0        0        0      513 2023-07-11 06:31:03.000000 yplib-2.4.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 06:31:23.316658 yplib-2.4.6/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.6/yplib/__init__.py
--rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.6/yplib/chart.py
--rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.6/yplib/chart_html.py
--rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.6/yplib/db.py
--rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.6/yplib/file.py
--rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.4.6/yplib/http_util.py
--rw-rw-rw-   0        0        0    32950 2023-07-11 06:30:56.000000 yplib-2.4.6/yplib/index.py
--rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.6/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.6/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.6/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.6/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2023-07-11 06:31:23.326877 yplib-2.4.6/yplib.egg-info/
--rw-rw-rw-   0        0        0      352 2023-07-11 06:31:23.000000 yplib-2.4.6/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-11 06:31:23.000000 yplib-2.4.6/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 06:31:23.000000 yplib-2.4.6/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-11 06:31:23.000000 yplib-2.4.6/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 00:17:43.897287 yplib-2.4.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-2.4.7/LICENSE
+-rw-rw-rw-   0        0        0      352 2023-07-12 00:17:43.896821 yplib-2.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-06-14 02:50:41.000000 yplib-2.4.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 00:17:43.897788 yplib-2.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      513 2023-07-12 00:17:24.000000 yplib-2.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 00:17:43.893093 yplib-2.4.7/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 01:30:34.000000 yplib-2.4.7/yplib/__init__.py
+-rw-rw-rw-   0        0        0    10012 2023-07-10 07:39:00.000000 yplib-2.4.7/yplib/chart.py
+-rw-rw-rw-   0        0        0     8406 2023-07-03 06:54:51.000000 yplib-2.4.7/yplib/chart_html.py
+-rw-rw-rw-   0        0        0     1534 2023-07-10 07:30:11.000000 yplib-2.4.7/yplib/db.py
+-rw-rw-rw-   0        0        0     4002 2023-06-29 01:38:59.000000 yplib-2.4.7/yplib/file.py
+-rw-rw-rw-   0        0        0     6117 2023-07-11 01:16:49.000000 yplib-2.4.7/yplib/http_util.py
+-rw-rw-rw-   0        0        0    33102 2023-07-12 00:15:30.000000 yplib-2.4.7/yplib/index.py
+-rw-rw-rw-   0        0        0     6196 2023-06-30 06:17:57.000000 yplib-2.4.7/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 02:49:14.000000 yplib-2.4.7/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 01:47:01.000000 yplib-2.4.7/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 07:57:19.000000 yplib-2.4.7/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2023-07-12 00:17:43.896321 yplib-2.4.7/yplib.egg-info/
+-rw-rw-rw-   0        0        0      352 2023-07-12 00:17:43.000000 yplib-2.4.7/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-12 00:17:43.000000 yplib-2.4.7/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 00:17:43.000000 yplib-2.4.7/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-12 00:17:43.000000 yplib-2.4.7/yplib.egg-info/top_level.txt
```

### Comparing `yplib-2.4.6/LICENSE` & `yplib-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-2.4.6/setup.py` & `yplib-2.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="2.4.6",
+  version="2.4.7",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

### Comparing `yplib-2.4.6/yplib/__init__.py` & `yplib-2.4.7/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.6/yplib/chart.py` & `yplib-2.4.7/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.6/yplib/chart_html.py` & `yplib-2.4.7/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.6/yplib/db.py` & `yplib-2.4.7/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.6/yplib/file.py` & `yplib-2.4.7/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.6/yplib/http_util.py` & `yplib-2.4.7/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.6/yplib/index.py` & `yplib-2.4.7/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 
 
 # 是否是 linux 系统, 不是 windows , 就是 linux 系统
 def is_linux():
     return not is_win()
 
 
+# 获得整数类型的 timestamp
+def get_timestamp():
+    return int(time.time())
+
+
 # 记录日志, 如果是对象会转化为 json
 def to_log(a1='tag', a2='', a3='', a4='', a5='', a6='', a7='', a8='', a9='', a10='', a11='', a12='',
            a13='', a14='', a15='', a16='', a17='', a18='', a19='', a20='', time_prefix=True):
     l = [a1, a2, a3, a4, a5, a6, a7, a8, a9, a10, a11, a12, a13, a14, a15, a16, a17, a18, a19, a20]
     d = ' '.join(list(map(lambda x: json.dumps(x) if can_use_json(x) else str(x), l)))
     lo = datetime.today().strftime('%Y-%m-%d %H:%M:%S') + ' ' + d if time_prefix else d
     print(lo)
@@ -249,14 +254,15 @@
         return 0.0
     if precision is None:
         return float(s)
     s1 = s.split('.')
     return float(s1[0] + '.' + s1[1][0:len(s1[1]) if len(s1[1]) < int(precision) else int(precision)])
 
 
+# @see https://www.runoob.com/python3/python3-date-time.html
 # 将字符串 s 转化成 datetime
 def to_datetime(s=None, r_str=False):
     if s is None or s == '':
         return str(datetime.today()) if r_str else datetime.today()
     s = str(s)
     r = None
     m_s = {
```

### Comparing `yplib-2.4.6/yplib/mail.py` & `yplib-2.4.7/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.6/yplib/mail_html.py` & `yplib-2.4.7/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-2.4.6/yplib/markdown.py` & `yplib-2.4.7/yplib/markdown.py`

 * *Files identical despite different names*

