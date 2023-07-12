# Comparing `tmp/tsc-es-0.6.tar.gz` & `tmp/tsc-es-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsc-es-0.6.tar", last modified: Tue Jul 11 16:18:30 2023, max compression
+gzip compressed data, was "tsc-es-0.7.tar", last modified: Wed Jul 12 04:59:30 2023, max compression
```

## Comparing `tsc-es-0.6.tar` & `tsc-es-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:18:30.857484 tsc-es-0.6/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-07-09 06:18:57.000000 tsc-es-0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 16:18:30.857484 tsc-es-0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 16:18:30.857484 tsc-es-0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      857 2023-07-11 16:06:27.000000 tsc-es-0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:18:30.841484 tsc-es-0.6/tsc_es/
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-09 06:30:27.000000 tsc-es-0.6/tsc_es/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17239 2023-07-11 16:06:46.000000 tsc-es-0.6/tsc_es/mongo_es.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 16:18:30.857484 tsc-es-0.6/tsc_es.egg-info/
--rw-r--r--   0 root         (0) root         (0)      441 2023-07-11 16:18:30.000000 tsc-es-0.6/tsc_es.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-11 16:18:30.000000 tsc-es-0.6/tsc_es.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 16:18:30.000000 tsc-es-0.6/tsc_es.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-11 16:18:30.000000 tsc-es-0.6/tsc_es.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-11 16:18:30.000000 tsc-es-0.6/tsc_es.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 04:59:30.792218 tsc-es-0.7/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-09 06:18:57.000000 tsc-es-0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-12 04:59:30.792218 tsc-es-0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 04:59:30.792218 tsc-es-0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      857 2023-07-12 04:47:22.000000 tsc-es-0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 04:59:30.792218 tsc-es-0.7/tsc_es/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-09 06:30:27.000000 tsc-es-0.7/tsc_es/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17814 2023-07-12 04:58:42.000000 tsc-es-0.7/tsc_es/mongo_es.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 04:59:30.792218 tsc-es-0.7/tsc_es.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-12 04:59:30.000000 tsc-es-0.7/tsc_es.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-12 04:59:30.000000 tsc-es-0.7/tsc_es.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 04:59:30.000000 tsc-es-0.7/tsc_es.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-12 04:59:30.000000 tsc-es-0.7/tsc_es.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-12 04:59:30.000000 tsc-es-0.7/tsc_es.egg-info/top_level.txt
```

### Comparing `tsc-es-0.6/LICENSE` & `tsc-es-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tsc-es-0.6/setup.py` & `tsc-es-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = ''
 
 setup(
     name='tsc-es',
-    version='0.6',
+    version='0.7',
     description="mongo to es",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='tsc',
     license='GPLv3',
     url='',
     keywords='tools',
```

### Comparing `tsc-es-0.6/tsc_es/mongo_es.py` & `tsc-es-0.7/tsc_es/mongo_es.py`

 * *Files 3% similar despite different names*

```diff
@@ -283,15 +283,16 @@
             batch = []
     if batch:
         yield batch
 
 
 def mongo_to_es(client: Elasticsearch, index_name: str, collection: Collection, map_fields: dict,
           time_field_es: str, time_field_mongo: str, mongo_is_date=False, timestamp_tz='Asia/Shanghai',
-          doc_skip_f=None, get_id=None, batch_size=500, is_stream=False, raise_on_error=True, op_type='index'):
+          doc_skip_f=None, get_id=None, batch_size=500, is_stream=False, raise_on_error=True, op_type='index',
+          mongo_filter: dict=None, es_filter: list=None):
     """
     从 mongo 导入到 es
     :param client: es 客户端
     :param index_name: 索引名称
     :param collection: mongo 的集合
     :param map_fields: 映射字段
     :param time_field_es: es 中的时间字段, 用于增量更新
@@ -300,21 +301,28 @@
     :param timestamp_tz: time_field_mongo 为时间戳时候的时区
     :param doc_skip_f: 参见 get_docs_from_cursor
     :param get_id: 参见 get_docs_from_cursor
     :param batch_size: 参见 get_docs_from_cursor
     :param is_stream: 是否是 date_stream 索引
     :param raise_on_error: 在插入一条出现错误的时候是否报错, False 表示不管这个错误继续插入下一条
     :param op_type: 索引类型, data stream 会自动修改为 create
+    :param mongo_filter: 一些针对 collection 进行的额外过滤, 以便于同步一部分. 要与 es_filter 配合
+        例子: {'source_db_summary.source_id': {'$exists': False}}
+    :param es_filter: 一些针对 index_name 进行的额外过滤, 以便于同步一部分. 要与 mongo_filter 配合
+        例子: [{'term': {'source_summary_id.keyword': ''}}]
     :return: 
     """
     op_type = 'create' if is_stream else op_type
     body = {
         "size": 1,
         "query": {
-            "match_all": {},
+            "bool": {
+                'must': [{"match_all": {}}],
+                "filter": es_filter if es_filter else [],
+            }
         },
         "sort": {
             time_field_es: {"order": "desc"},
         },
     }
     es_res = client.search(index=index_name, **body)
     start_time = None
@@ -328,15 +336,15 @@
                 start_time = start_time.timestamp() + 0.001
         else:
             start_time += 1e-6  # 要求是精确到微秒的秒级时间戳
             if mongo_is_date:
                 start_time = datetime.fromtimestamp(start_time, tz=pytz.timezone(timestamp_tz))
     logging.info(str(start_time))
         
-    mongo_filter = {}
+    mongo_filter = mongo_filter if mongo_filter else {}
     if start_time:
         mongo_filter[time_field_mongo] = {'$gte': start_time}
     info = collection.find(mongo_filter).sort(time_field_mongo, ASCENDING)
     info_count = collection.count_documents(mongo_filter)
     ret = {
         'time_field_es': time_field_es,
         'time_field_mongo': time_field_mongo,
```

