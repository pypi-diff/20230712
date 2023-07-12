# Comparing `tmp/huhk-1.6.3.tar.gz` & `tmp/huhk-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.6.3.tar", last modified: Wed Jul 12 06:13:56 2023, max compression
+gzip compressed data, was "huhk-1.6.4.tar", last modified: Wed Jul 12 07:15:40 2023, max compression
```

## Comparing `huhk-1.6.3.tar` & `huhk-1.6.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 06:13:56.400977 huhk-1.6.3/
--rw-rw-rw-   0        0        0      223 2023-07-12 06:13:56.400977 huhk-1.6.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 06:13:56.361694 huhk-1.6.3/huhk/
--rw-rw-rw-   0        0        0      931 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/__init__.py
--rw-rw-rw-   0        0        0      532 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:13:56.377145 huhk-1.6.3/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/case_project/base_project.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      720 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/case_project/main.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-12 06:13:56.000000 huhk-1.6.3/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    29291 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:13:56.378143 huhk-1.6.3/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:13:56.399016 huhk-1.6.3/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.3/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7303 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      517 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1544 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2144 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      564 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2615 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1692 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1612 2023-07-12 02:24:22.000000 huhk-1.6.3/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      549 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22779 2023-07-12 02:54:58.000000 huhk-1.6.3/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    24883 2023-07-12 06:13:25.000000 huhk-1.6.3/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9212 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.3/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:13:56.368677 huhk-1.6.3/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-12 06:13:56.000000 huhk-1.6.3/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1077 2023-07-12 06:13:56.000000 huhk-1.6.3/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 06:13:56.000000 huhk-1.6.3/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-12 06:13:56.000000 huhk-1.6.3/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-12 06:13:56.000000 huhk-1.6.3/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-12 06:13:56.000000 huhk-1.6.3/huhk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 06:13:56.400977 huhk-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.340015 huhk-1.6.4/
+-rw-rw-rw-   0        0        0      223 2023-07-12 07:15:40.339018 huhk-1.6.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.300121 huhk-1.6.4/huhk/
+-rw-rw-rw-   0        0        0      931 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.317110 huhk-1.6.4/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3072 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/case_project/base_project.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      762 2023-07-12 06:28:58.000000 huhk-1.6.4/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    29291 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/init_project.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.318087 huhk-1.6.4/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.337023 huhk-1.6.4/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.4/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7303 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      517 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1544 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2144 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      564 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2615 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1692 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1612 2023-07-12 02:24:22.000000 huhk-1.6.4/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      549 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22779 2023-07-12 02:54:58.000000 huhk-1.6.4/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    25666 2023-07-12 07:15:19.000000 huhk-1.6.4/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9212 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.4/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-12 07:15:40.308140 huhk-1.6.4/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1077 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 07:15:40.000000 huhk-1.6.4/huhk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 07:15:40.340015 huhk-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.4/setup.py
```

### Comparing `huhk-1.6.3/huhk/__init__.py` & `huhk-1.6.4/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/__main__.py` & `huhk-1.6.4/huhk/__main__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/case_project/base_project.py` & `huhk-1.6.4/huhk/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/case_project/json_coder.py` & `huhk-1.6.4/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/case_project/setup_set.py` & `huhk-1.6.4/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/init_project.py` & `huhk-1.6.4/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/beam_class.py` & `huhk-1.6.4/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/data.py` & `huhk-1.6.4/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/par_do.py` & `huhk-1.6.4/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.6.4/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/test_file.py` & `huhk-1.6.4/huhk/testcase/apache/test_file.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/test_fiter.py` & `huhk-1.6.4/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/test_flatmap.py` & `huhk-1.6.4/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/test_map.py` & `huhk-1.6.4/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/test_par_do.py` & `huhk-1.6.4/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/test_regex.py` & `huhk-1.6.4/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/test_time.py` & `huhk-1.6.4/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/testcase/apache/test_to_string.py` & `huhk-1.6.4/huhk/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/unit_apache_beam.py` & `huhk-1.6.4/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/unit_dict.py` & `huhk-1.6.4/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/unit_encryption.py` & `huhk-1.6.4/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/unit_fun.py` & `huhk-1.6.4/huhk/unit_fun.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 import random
 import time
 import requests
 import datetime
 # import pymysql
-
+from pandas import DataFrame, ExcelWriter
 from typing import List
 from faker import Faker
 from huhk.unit_logger import logger
 
 
 class FunBase:
     def __init__(self):
@@ -19,14 +19,15 @@
         # self.locale_list = {"zh_CN": "简体中文", "de_DE": "德语-德国", "sv_SE": "Swedish", "ja_JP": "日语-日本", "ko_KR": "朝鲜语-韩国"}
         # faker方法： http://www.manongjc.com/detail/28-mhkegnrmyzaafky.html
         self._faker = Faker(locale='zh_CN')
         self._db = {}
         self._route = ""
         self._token = ""
         self._host = ""
+        self._files = {}
 
     # mock 方法，默认中国，详情搜python Faker模块
     def faker(self, locale='zh_CN'):
         return Faker(locale=locale)
 
     def seelp(self, v=1, *args, **kwargs):
         if isinstance(v, int):
@@ -461,100 +462,128 @@
                     elif isinstance(value, dict):
                         for key2, value2 in value.items():
                             if isinstance(value2, list):
                                 return [i.get(name) for i in value2 if i.get(name)]
             return []
 
     @staticmethod
+    def _to_excel(f, data, sheet_name="sheet", set_column=[], header_format=None, column_header=[],
+                  column_default=[], isdigitl=True):
+        if data and isinstance(data[0], (list, tuple)):
+            h = data[0]
+            data1 = []
+            for i in data[1:]:
+                data1.append({x[0]: str(x[1]) for x in zip(h, i)})
+            data = data1
+        elif data and isinstance(data[0], dict):
+            data = [{k: str(v) for k, v in i.items()} for i in data]
+
+        if column_header:
+            column_header = column_header if isinstance(column_header, list) else column_header.split(",")
+            _header = {k: None for k in column_header}
+            if column_default:
+                _default = column_default if isinstance(column_default, list) else column_default.split(",")
+                for i, v in enumerate(_default):
+                    try:
+                        _header[column_header[i]] = v
+                    except:
+                        pass
+            for i, v in enumerate(data):
+                _data = _header.copy()
+                _data.update(v)
+                data[i] = _data
+        if isdigitl:
+            for i, d in enumerate(data):
+                for k, v in d.items():
+                    try:
+                        if v.isdigit():
+                            data[i][k] = int(v)
+                    except:
+                        pass
+        result = DataFrame(data)
+        result.to_excel(f, sheet_name=sheet_name, index=False, engine="openpyxl")
+
+        try:
+            worksheet = f.sheets.get(sheet_name) or f.sheets.get("sheet1")
+            for idx, v in enumerate(set_column):
+                try:
+                    if idx < len(result.columns.values):
+                        worksheet.set_column(idx, idx, float(v.strip()))
+                except Exception as e:
+                    logger.info(str(e))
+        except Exception as e:
+            logger.info(str(e))
+
+        try:
+            if header_format:
+                if isinstance(header_format, str):
+                    header_format = eval(header_format)
+                elif isinstance(header_format, dict):
+                    header_format = [header_format]
+
+                if isinstance(header_format, list):
+                    header_format = header_format
+                    workbook = f.book
+                    worksheet = f.sheets.get(sheet_name) or f.sheets.get("sheet1")
+                    for format in header_format:
+                        if "left_column" in format.keys():
+                            left_colume = format['left_column']
+                            del format['left_column']
+                        else:
+                            left_colume = 0
+                        if "right_column" in format.keys():
+                            right_column = format['right_column']
+                            del format['right_column']
+                        else:
+                            right_column = 999
+                        format = workbook.add_format(format)
+                        for col_num, value in enumerate(result.columns.values):
+                            if col_num >= left_colume and col_num <= right_column:
+                                try:
+                                    worksheet.write(0, col_num, value, format)
+                                except Exception as e:
+                                    logger.info(str(e))
+        except Exception as e:
+            logger.info(str(e))
+
+    @staticmethod
     def excelWriter(filename, data, sheet_name="sheet", set_column=[], header_format=None, column_header=[],
                     column_default=[], isdigitl=True):
-        from pandas import DataFrame, ExcelWriter
+
         filename = filename[:4] + filename[4:].replace(":", "").replace(' ', '_')
         try:
             with ExcelWriter(filename) as writer:
                 # 写入到第一个sheet
-                if data and isinstance(data[0], (list, tuple)):
-                    h = data[0]
-                    data1 = []
-                    for i in data[1:]:
-                        data1.append({x[0]: str(x[1]) for x in zip(h, i)})
-                    data = data1
-                elif data and isinstance(data[0], dict):
-                    data = [{k: str(v) for k, v in i.items()} for i in data]
-
-                if column_header:
-                    column_header = column_header if isinstance(column_header, list) else column_header.split(",")
-                    _header = {k: None for k in column_header}
-                    if column_default:
-                        _default = column_default if isinstance(column_default, list) else column_default.split(",")
-                        for i, v in enumerate(_default):
-                            try:
-                                _header[column_header[i]] = v
-                            except:
-                                pass
-                    for i, v in enumerate(data):
-                        _data = _header.copy()
-                        _data.update(v)
-                        data[i] = _data
-                if isdigitl:
-                    for i, d in enumerate(data):
-                        for k, v in d.items():
-                            try:
-                                if v.isdigit():
-                                    data[i][k] = int(v)
-                            except:
-                                pass
-                result = DataFrame(data)
-                result.to_excel(writer, sheet_name=sheet_name, index=False, engine="openpyxl")
-
-                try:
-                    worksheet = writer.sheets.get(sheet_name) or writer.sheets.get("sheet1")
-                    for idx, v in enumerate(set_column):
-                        try:
-                            if idx < len(result.columns.values):
-                                worksheet.set_column(idx, idx, float(v.strip()))
-                        except Exception as e:
-                            logger.info(str(e))
-                except Exception as e:
-                    logger.info(str(e))
-
-                try:
-                    if header_format:
-                        if isinstance(header_format, str):
-                            header_format = eval(header_format)
-                        elif isinstance(header_format, dict):
-                            header_format = [header_format]
-
-                        if isinstance(header_format, list):
-                            header_format = header_format
-                            workbook = writer.book
-                            worksheet = writer.sheets.get(sheet_name) or writer.sheets.get("sheet1")
-                            for format in header_format:
-                                if "left_column" in format.keys():
-                                    left_colume = format['left_column']
-                                    del format['left_column']
-                                else:
-                                    left_colume = 0
-                                if "right_column" in format.keys():
-                                    right_column = format['right_column']
-                                    del format['right_column']
-                                else:
-                                    right_column = 999
-                                format = workbook.add_format(format)
-                                for col_num, value in enumerate(result.columns.values):
-                                    if col_num >= left_colume and col_num <= right_column:
-                                        try:
-                                            worksheet.write(0, col_num, value, format)
-                                        except Exception as e:
-                                            logger.info(str(e))
-                except Exception as e:
-                    logger.info(str(e))
+                FunBase._to_excel(writer, data, sheet_name=sheet_name, set_column=set_column,
+                                  header_format=header_format, column_header=column_header,
+                                  column_default=column_default, isdigitl=isdigitl)
         except Exception as e:
             logger.info(str(e))
 
+    def excel_writer_sheet(self, filename, data, sheet_name="sheet", set_column=[], header_format=None,
+                           column_header=[], column_default=[], isdigitl=True):
+        filename = filename[:4] + filename[4:].replace(":", "").replace(' ', '_')
+        if self._files.get(filename):
+            f = self._files.get(filename)
+        else:
+            f = ExcelWriter(filename)
+            self._files[filename] = f
+        FunBase._to_excel(f, data, sheet_name=sheet_name, set_column=set_column,
+                          header_format=header_format, column_header=column_header,
+                          column_default=column_default, isdigitl=isdigitl)
+
+    def save(self, filename=None):
+        if filename:
+            if self._files.get(filename):
+                f = self._files.get(filename)
+                f.save()
+        else:
+            for f in self._files.values():
+                f.save()
+
     @staticmethod
     def get_version():
         from huhk.case_project.version import version
         version_l = [int(i) for i in version.split('.')]
         version_l[2] += 1
         if version_l[2] > 9:
             version_l[1] += 1
```

### Comparing `huhk-1.6.3/huhk/unit_logger.py` & `huhk-1.6.4/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/unit_request.py` & `huhk-1.6.4/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/unit_tasks.py` & `huhk-1.6.4/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk/常用命令.py` & `huhk-1.6.4/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.3/huhk.egg-info/SOURCES.txt` & `huhk-1.6.4/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

