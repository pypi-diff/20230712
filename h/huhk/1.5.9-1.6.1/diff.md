# Comparing `tmp/huhk-1.5.9.tar.gz` & `tmp/huhk-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\huhk-1.5.9.tar", last modified: Tue Jul 11 23:52:15 2023, max compression
+gzip compressed data, was "huhk-1.6.1.tar", last modified: Wed Jul 12 02:39:19 2023, max compression
```

## Comparing `huhk-1.5.9.tar` & `huhk-1.6.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 23:52:15.000000 huhk-1.5.9/
--rw-rw-rw-   0        0        0      153 2023-07-11 23:52:15.000000 huhk-1.5.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 23:52:15.000000 huhk-1.5.9/huhk/
--rw-rw-rw-   0        0        0      931 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/__init__.py
--rw-rw-rw-   0        0        0      532 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:52:15.000000 huhk-1.5.9/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/case_project/base_project.py
--rw-rw-rw-   0        0        0      639 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      720 2023-07-11 14:36:42.000000 huhk-1.5.9/huhk/case_project/main.py
--rw-rw-rw-   0        0        0      908 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-11 23:52:14.000000 huhk-1.5.9/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    29291 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:52:15.000000 huhk-1.5.9/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:52:15.000000 huhk-1.5.9/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-11 14:08:30.000000 huhk-1.5.9/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7303 2023-07-11 14:11:21.000000 huhk-1.5.9/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      517 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1544 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2144 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      564 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2615 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1692 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0      515 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      549 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    21927 2023-07-11 14:22:19.000000 huhk-1.5.9/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    24874 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9212 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-11 13:40:55.000000 huhk-1.5.9/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-11 23:52:15.000000 huhk-1.5.9/huhk.egg-info/
--rw-rw-rw-   0        0        0      153 2023-07-11 23:52:14.000000 huhk-1.5.9/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-07-11 23:52:15.000000 huhk-1.5.9/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 23:52:14.000000 huhk-1.5.9/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-11 23:52:14.000000 huhk-1.5.9/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-11 23:52:14.000000 huhk-1.5.9/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-11 23:52:14.000000 huhk-1.5.9/huhk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 23:52:15.000000 huhk-1.5.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.844793 huhk-1.6.1/
+-rw-rw-rw-   0        0        0      223 2023-07-12 02:39:19.844793 huhk-1.6.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.810883 huhk-1.6.1/huhk/
+-rw-rw-rw-   0        0        0      931 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.825843 huhk-1.6.1/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3072 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/case_project/base_project.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      720 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0      908 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    29291 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/init_project.py
+-rw-rw-rw-   0        0        0      274 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.826840 huhk-1.6.1/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.843796 huhk-1.6.1/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.6.1/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7303 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      517 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1544 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2144 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      564 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2615 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1692 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1612 2023-07-12 02:24:22.000000 huhk-1.6.1/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      549 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22698 2023-07-12 02:38:06.000000 huhk-1.6.1/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    24874 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9212 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.6.1/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:39:19.817865 huhk-1.6.1/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1077 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 02:39:19.000000 huhk-1.6.1/huhk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 02:39:19.845791 huhk-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0        2 2023-07-03 11:51:22.000000 huhk-1.6.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `huhk-1.5.9/huhk/__init__.py` & `huhk-1.6.1/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/__main__.py` & `huhk-1.6.1/huhk/__main__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/case_project/base_project.py` & `huhk-1.6.1/huhk/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/case_project/json_coder.py` & `huhk-1.6.1/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/case_project/main.py` & `huhk-1.6.1/huhk/case_project/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/case_project/setup_set.py` & `huhk-1.6.1/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/init_project.py` & `huhk-1.6.1/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/testcase/apache/beam_class.py` & `huhk-1.6.1/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/testcase/apache/data.py` & `huhk-1.6.1/huhk/testcase/apache/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import apache_beam as beam
-data_type = 1
+data_type = 2
 data_list = ['annual', 'biennial', 'perennial']
 data_list2 = ['🥕', '🍅', '🍅', '🥕', '🍆', '🍅', '🍅', '🍅', '🥕', '🍅']
 data_list3 = [3, 4, 1, 2]
 data_list_dict = [
         {'icon': '🍓', 'name': 'Strawberry', 'duration': 'perennial'},
         {'icon': '🥕', 'name': 'Carrot', 'duration': 'biennial'},
         {'icon': '🍆', 'name': 'Eggplant', 'duration': 'perennial'},
```

### Comparing `huhk-1.5.9/huhk/testcase/apache/par_do.py` & `huhk-1.6.1/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.6.1/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/testcase/apache/test_file.py` & `huhk-1.6.1/huhk/testcase/apache/test_file.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/testcase/apache/test_fiter.py` & `huhk-1.6.1/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/testcase/apache/test_flatmap.py` & `huhk-1.6.1/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/testcase/apache/test_map.py` & `huhk-1.6.1/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/testcase/apache/test_par_do.py` & `huhk-1.6.1/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/testcase/apache/test_regex.py` & `huhk-1.6.1/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/testcase/apache/test_time.py` & `huhk-1.6.1/huhk/testcase/apache/test_time.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,7 +8,31 @@
         ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season").print()
 
     def test_times_002(self):
         ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season2").print()
 
     def test_times_003(self):
         ApacheFun(data_list_dict3, data_type=data_type).timestamped_value().print()
+
+    def test_times_004(self):
+        ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season", type="utc").print()
+
+    def test_times_005(self):
+        ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season", type="bj").print()
+
+    def test_times_006(self):
+        ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season", type="rfc").print()
+
+    def test_times_007(self):
+        ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season", type="proto").print()
+
+    def test_times_008(self):
+        ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season", type="s").print()
+
+    def test_times_009(self):
+        ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season", type="m").print()
+
+    def test_times_010(self):
+        ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season", type="h").print()
+
+    def test_times_011(self):
+        ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season", type="t").print()
```

### Comparing `huhk-1.5.9/huhk/testcase/apache/test_to_string.py` & `huhk-1.6.1/huhk/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/unit_apache_beam.py` & `huhk-1.6.1/huhk/unit_apache_beam.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,14 +228,22 @@
                     _time = timestamp.to_utc_datetime()
                 elif type == "bj":
                     _time = datetime.datetime.fromtimestamp(timestamp.micros / 1e6).strftime("%Y-%m-%d %H:%M:%S")
                 elif type == "rfc":
                     _time = timestamp.to_rfc3339()
                 elif type == "proto":
                     _time = timestamp.to_proto()
+                elif type == "s":
+                    _time = timestamp.to_proto().seconds
+                elif type == "m":
+                    _time = timestamp.to_proto().seconds // 60
+                elif type == "h":
+                    _time = timestamp.to_proto().seconds // 3600
+                elif type in ("t", "d"):
+                    _time = timestamp.to_proto().seconds // 3600 // 24
                 plant[key] = _time
                 yield plant
 
         def get_key(plant):
             if key and (isinstance(plant, dict) and plant.get(key)):
                 _time = plant[key]
             elif key and (isinstance(plant, (list, tuple)) and len(plant) == 2 and
@@ -260,15 +268,24 @@
             else:
                 self.value = self.out = self.get_out() | self._name() >> beam.Map(get_plant2) | self._name() >> beam.ParDo(
                     GetTimestamp(key=key))
         else:
             def get_plant(plant):
                 micros = get_key(plant)
                 micros = int(int(float(micros)) / (10 ** (len(str(int(float(micros))))-10)))
-                plant[key] = datetime.datetime.fromtimestamp(micros).strftime("%Y-%m-%d %H:%M:%S")
+                if type == "s":
+                    plant[key] = micros
+                elif type == "m":
+                    plant[key] = micros // 60
+                elif type == "h":
+                    plant[key] = micros // 3600
+                elif type in ("t", "d"):
+                    plant[key] = micros // 3600 // 24
+                else:
+                    plant[key] = datetime.datetime.fromtimestamp(micros).strftime("%Y-%m-%d %H:%M:%S")
                 return plant
             self.value = self.out = self.get_out() | beam.Map(get_plant)
         return self
 
     def kvswap(self, data=None):
         """获取一个键值对集合并返回一个键值对集合，其中每个键值对都进行了交换。"""
         self.value = self.create(data).value | self._name() >> beam.KvSwap()
```

### Comparing `huhk-1.5.9/huhk/unit_dict.py` & `huhk-1.6.1/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/unit_encryption.py` & `huhk-1.6.1/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/unit_fun.py` & `huhk-1.6.1/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/unit_logger.py` & `huhk-1.6.1/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/unit_request.py` & `huhk-1.6.1/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/unit_tasks.py` & `huhk-1.6.1/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk/常用命令.py` & `huhk-1.6.1/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.9/huhk.egg-info/SOURCES.txt` & `huhk-1.6.1/huhk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+setup.py
 huhk/__init__.py
 huhk/__main__.py
 huhk/init_project.py
 huhk/setup_run.py
 huhk/unit_apache_beam.py
 huhk/unit_dict.py
 huhk/unit_encryption.py
```

