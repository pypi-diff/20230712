# Comparing `tmp/huhk-1.6.1.tar.gz` & `tmp/huhk-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.6.1.tar", last modified: Wed Jul 12 02:39:19 2023, max compression
+gzip compressed data, was "huhk-1.6.2.tar", last modified: Wed Jul 12 02:56:01 2023, max compression
```

## Comparing `huhk-1.6.1.tar` & `huhk-1.6.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.844793 huhk-1.6.1/
--rw-rw-rw-   0        0        0      223 2023-07-12 02:39:19.844793 huhk-1.6.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.810883 huhk-1.6.1/huhk/
--rw-rw-rw-   0        0        0      931 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/__init__.py
--rw-rw-rw-   0        0        0      532 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.825843 huhk-1.6.1/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/case_project/base_project.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      720 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/case_project/main.py
--rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    29291 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.826840 huhk-1.6.1/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.843796 huhk-1.6.1/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.1/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7303 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      517 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1544 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2144 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      564 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2615 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1692 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1612 2023-07-12 02:24:22.000000 huhk-1.6.1/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      549 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22698 2023-07-12 02:38:06.000000 huhk-1.6.1/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    24874 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9212 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.817865 huhk-1.6.1/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1077 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 02:39:19.845791 huhk-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:56:01.844497 huhk-1.6.2/
+-rw-rw-rw-   0        0        0      223 2023-07-12 02:56:01.844497 huhk-1.6.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 02:56:01.807592 huhk-1.6.2/huhk/
+-rw-rw-rw-   0        0        0      931 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:56:01.822553 huhk-1.6.2/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3072 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/case_project/base_project.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      720 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-12 02:56:01.000000 huhk-1.6.2/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    29291 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/init_project.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:56:01.824547 huhk-1.6.2/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:56:01.841502 huhk-1.6.2/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.2/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7303 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      517 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1544 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2144 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      564 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2615 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1692 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1612 2023-07-12 02:24:22.000000 huhk-1.6.2/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      549 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22779 2023-07-12 02:54:58.000000 huhk-1.6.2/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    24874 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9212 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.2/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:56:01.815570 huhk-1.6.2/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-12 02:56:01.000000 huhk-1.6.2/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1077 2023-07-12 02:56:01.000000 huhk-1.6.2/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 02:56:01.000000 huhk-1.6.2/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-12 02:56:01.000000 huhk-1.6.2/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-12 02:56:01.000000 huhk-1.6.2/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 02:56:01.000000 huhk-1.6.2/huhk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 02:56:01.845493 huhk-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.2/setup.py
```

### Comparing `huhk-1.6.1/huhk/__init__.py` & `huhk-1.6.2/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/__main__.py` & `huhk-1.6.2/huhk/__main__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/case_project/base_project.py` & `huhk-1.6.2/huhk/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/case_project/json_coder.py` & `huhk-1.6.2/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/case_project/main.py` & `huhk-1.6.2/huhk/case_project/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/case_project/setup_set.py` & `huhk-1.6.2/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/init_project.py` & `huhk-1.6.2/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/beam_class.py` & `huhk-1.6.2/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/data.py` & `huhk-1.6.2/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/par_do.py` & `huhk-1.6.2/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.6.2/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/test_file.py` & `huhk-1.6.2/huhk/testcase/apache/test_file.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/test_fiter.py` & `huhk-1.6.2/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/test_flatmap.py` & `huhk-1.6.2/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/test_map.py` & `huhk-1.6.2/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/test_par_do.py` & `huhk-1.6.2/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/test_regex.py` & `huhk-1.6.2/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/test_time.py` & `huhk-1.6.2/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/testcase/apache/test_to_string.py` & `huhk-1.6.2/huhk/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/unit_apache_beam.py` & `huhk-1.6.2/huhk/unit_apache_beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,18 @@
 
     def window_info(self, fn, *args, **kwargs):
         self.value = self.out = self.get_out() | self._name() >> beam.WindowInto(fn, *args, **kwargs)
         return self
 
     def get_out(self):
         """判断是否已经是管道"""
-        return self.out if isinstance(self.out, PCollection) else self.create().value
+        if self.data_type == 1:
+            return self.out if isinstance(self.out, PCollection) else self.create().value
+        else:
+            return self.out
 
     def map(self, fn, *args, **kwargs):
         """对集合中的每个元素应用简单的 1 对 1 映射函数。"""
         self.value = self.out = self.get_out() | self._name() >> beam.Map(fn, *args, **kwargs)
         return self
 
     def map_tuple(self, fn, *args, **kwargs):
```

### Comparing `huhk-1.6.1/huhk/unit_dict.py` & `huhk-1.6.2/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/unit_encryption.py` & `huhk-1.6.2/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/unit_fun.py` & `huhk-1.6.2/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/unit_logger.py` & `huhk-1.6.2/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/unit_request.py` & `huhk-1.6.2/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/unit_tasks.py` & `huhk-1.6.2/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk/常用命令.py` & `huhk-1.6.2/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.6.1/huhk.egg-info/SOURCES.txt` & `huhk-1.6.2/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

