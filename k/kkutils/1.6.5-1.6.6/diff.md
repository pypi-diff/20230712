# Comparing `tmp/kkutils-1.6.5.tar.gz` & `tmp/kkutils-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkutils-1.6.5.tar", last modified: Sun Jun 11 23:10:38 2023, max compression
+gzip compressed data, was "kkutils-1.6.6.tar", last modified: Wed Jul 12 05:04:14 2023, max compression
```

## Comparing `kkutils-1.6.5.tar` & `kkutils-1.6.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:10:38.897494 kkutils-1.6.5/
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-11 23:10:38.897494 kkutils-1.6.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:10:38.893493 kkutils-1.6.5/kkutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-11 23:10:38.000000 kkutils-1.6.5/kkutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      619 2023-06-11 23:10:38.000000 kkutils-1.6.5/kkutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 23:10:38.000000 kkutils-1.6.5/kkutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-11 23:10:38.000000 kkutils-1.6.5/kkutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-11 23:10:38.000000 kkutils-1.6.5/kkutils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3985 2022-11-07 22:39:49.000000 kkutils-1.6.5/processor.py
--rw-r--r--   0 root         (0) root         (0)      245 2023-03-04 16:36:32.000000 kkutils-1.6.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 23:10:38.897494 kkutils-1.6.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1190 2023-06-11 23:10:36.000000 kkutils-1.6.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:10:38.893493 kkutils-1.6.5/tornado_utils/
--rw-r--r--   0 root         (0) root         (0)      408 2022-07-14 13:13:22.000000 kkutils-1.6.5/tornado_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6018 2022-11-15 06:06:44.000000 kkutils-1.6.5/tornado_utils/application.py
--rw-r--r--   0 root         (0) root         (0)     9723 2023-06-03 05:59:58.000000 kkutils-1.6.5/tornado_utils/basehandler.py
--rw-r--r--   0 root         (0) root         (0)    12696 2023-03-16 13:15:20.000000 kkutils-1.6.5/tornado_utils/userhandler.py
--rw-r--r--   0 root         (0) root         (0)     3803 2022-07-14 13:13:22.000000 kkutils-1.6.5/tornado_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:10:38.897494 kkutils-1.6.5/utils/
--rw-r--r--   0 root         (0) root         (0)     2005 2023-01-04 06:47:48.000000 kkutils-1.6.5/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10493 2023-06-10 09:51:09.000000 kkutils-1.6.5/utils/base_utils.py
--rw-r--r--   0 root         (0) root         (0)     4219 2022-07-14 13:13:22.000000 kkutils-1.6.5/utils/cached_property.py
--rw-r--r--   0 root         (0) root         (0)     5564 2022-07-14 13:13:22.000000 kkutils-1.6.5/utils/config_utils.py
--rw-r--r--   0 root         (0) root         (0)     2749 2023-05-01 12:38:54.000000 kkutils-1.6.5/utils/crypto.py
--rw-r--r--   0 root         (0) root         (0)    10699 2023-06-11 01:44:37.000000 kkutils-1.6.5/utils/curl_utils.py
--rw-r--r--   0 root         (0) root         (0)    16416 2023-04-18 08:50:58.000000 kkutils-1.6.5/utils/db_utils.py
--rw-r--r--   0 root         (0) root         (0)     2078 2022-07-14 13:13:22.000000 kkutils-1.6.5/utils/decorator.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-06-02 07:24:05.000000 kkutils-1.6.5/utils/email_utils.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-01-24 01:54:34.000000 kkutils-1.6.5/utils/fire.py
--rw-r--r--   0 root         (0) root         (0)    26557 2023-06-11 01:22:42.000000 kkutils-1.6.5/utils/http_utils.py
--rw-r--r--   0 root         (0) root         (0)     2688 2022-11-15 06:06:44.000000 kkutils-1.6.5/utils/log_utils.py
--rw-r--r--   0 root         (0) root         (0)     6563 2023-06-03 06:12:56.000000 kkutils-1.6.5/utils/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-01-19 13:35:24.000000 kkutils-1.6.5/utils/stopwatch.py
--rw-r--r--   0 root         (0) root         (0)     5796 2022-10-21 05:24:23.000000 kkutils-1.6.5/utils/xdb_searcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:04:14.295596 kkutils-1.6.6/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-12 05:04:14.295596 kkutils-1.6.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:04:14.291596 kkutils-1.6.6/kkutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-12 05:04:14.000000 kkutils-1.6.6/kkutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      619 2023-07-12 05:04:14.000000 kkutils-1.6.6/kkutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 05:04:14.000000 kkutils-1.6.6/kkutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      260 2023-07-12 05:04:14.000000 kkutils-1.6.6/kkutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-07-12 05:04:14.000000 kkutils-1.6.6/kkutils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3985 2022-11-07 22:39:49.000000 kkutils-1.6.6/processor.py
+-rw-r--r--   0 root         (0) root         (0)      245 2023-03-04 16:36:32.000000 kkutils-1.6.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 05:04:14.295596 kkutils-1.6.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-07-12 05:04:11.000000 kkutils-1.6.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:04:14.291596 kkutils-1.6.6/tornado_utils/
+-rw-r--r--   0 root         (0) root         (0)      408 2022-07-14 13:13:22.000000 kkutils-1.6.6/tornado_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6018 2022-11-15 06:06:44.000000 kkutils-1.6.6/tornado_utils/application.py
+-rw-r--r--   0 root         (0) root         (0)    10163 2023-06-25 07:50:09.000000 kkutils-1.6.6/tornado_utils/basehandler.py
+-rw-r--r--   0 root         (0) root         (0)    13207 2023-06-25 02:21:16.000000 kkutils-1.6.6/tornado_utils/userhandler.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2022-07-14 13:13:22.000000 kkutils-1.6.6/tornado_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 05:04:14.295596 kkutils-1.6.6/utils/
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-01-04 06:47:48.000000 kkutils-1.6.6/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10598 2023-07-02 08:38:20.000000 kkutils-1.6.6/utils/base_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2022-07-14 13:13:22.000000 kkutils-1.6.6/utils/cached_property.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2022-07-14 13:13:22.000000 kkutils-1.6.6/utils/config_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-05-01 12:38:54.000000 kkutils-1.6.6/utils/crypto.py
+-rw-r--r--   0 root         (0) root         (0)    10699 2023-06-11 01:44:37.000000 kkutils-1.6.6/utils/curl_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16416 2023-04-18 08:50:58.000000 kkutils-1.6.6/utils/db_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2022-07-14 13:13:22.000000 kkutils-1.6.6/utils/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2023-06-17 00:17:19.000000 kkutils-1.6.6/utils/email_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-01-24 01:54:34.000000 kkutils-1.6.6/utils/fire.py
+-rw-r--r--   0 root         (0) root         (0)    26557 2023-06-11 01:22:42.000000 kkutils-1.6.6/utils/http_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2688 2022-11-15 06:06:44.000000 kkutils-1.6.6/utils/log_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6563 2023-06-03 06:12:56.000000 kkutils-1.6.6/utils/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-01-19 13:35:24.000000 kkutils-1.6.6/utils/stopwatch.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2022-10-21 05:24:23.000000 kkutils-1.6.6/utils/xdb_searcher.py
```

### Comparing `kkutils-1.6.5/PKG-INFO` & `kkutils-1.6.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkutils
-Version: 1.6.5
+Version: 1.6.6
 Summary: python utils
 Home-page: https://www.ishield.cn
 Author: digua
 Author-email: zkdfbb@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kkutils-1.6.5/kkutils.egg-info/PKG-INFO` & `kkutils-1.6.6/kkutils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kkutils
-Version: 1.6.5
+Version: 1.6.6
 Summary: python utils
 Home-page: https://www.ishield.cn
 Author: digua
 Author-email: zkdfbb@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kkutils-1.6.5/kkutils.egg-info/SOURCES.txt` & `kkutils-1.6.6/kkutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/processor.py` & `kkutils-1.6.6/processor.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/setup.py` & `kkutils-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Last modified: 2019-04-07 00:07:43
 '''
 
 from setuptools import setup
 
 setup(
     name="kkutils",
-    version="1.6.5",
+    version="1.6.6",
     description="python utils",
     author="digua",
     author_email="zkdfbb@qq.com",
     url="https://www.ishield.cn",
     license="MIT",
     python_requires='>=3.6',
     data_files=[('', ['requirements.txt'])],
```

### Comparing `kkutils-1.6.5/tornado_utils/application.py` & `kkutils-1.6.6/tornado_utils/application.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/tornado_utils/basehandler.py` & `kkutils-1.6.6/tornado_utils/basehandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 Author: zhangkai
 Email: kai.zhang1@nio.com
 Last modified: 2018-04-14 14:21:15
 '''
+
 import copy
 import datetime
 import hashlib
 import json
 import math
 import re
 import time
 import traceback
 import urllib.parse
+import uuid
 
 import tornado.web
 from bson import ObjectId
 from utils import (Dict, JSONEncoder, Logger, Mongo, Motor, awaitable,
                    cached_property)
 
 
@@ -67,24 +69,37 @@
 
         if raise_error:
             self.logger.warning(f'authorized referers: {referers}, referer: {self.referer}')
             raise tornado.web.HTTPError(403)
         else:
             return False
 
-    async def check_sign(self, prefix='digua', method='md5'):
+    def sign(self, url, prefix='digua', n=None):
+        t = hex(int(time.time()))[2:]
+        n = n or uuid.uuid4().hex[:8]
+        s = hashlib.md5(f'digua_{t}_{n}'.encode()).hexdigest()[:8]
+        ret = urllib.parse.urlparse(url)
+        query = urllib.parse.parse_qs(ret.query)
+        query['t'] = t
+        query['n'] = n
+        query['s'] = s
+        url = urllib.parse.urlunparse((ret.scheme, ret.netloc, ret.path, ret.params,
+                                       urllib.parse.urlencode(query, doseq=True), ret.fragment))
+        return url
+
+    def check_sign(self, prefix='digua'):
         self.args.t = self.args.t[0] if isinstance(self.args.t, list) else self.args.t
         if not (self.args.t and self.args.n and self.args.s):
             raise tornado.web.HTTPError(403)
 
         if time.time() - int(self.args.t, 16) >= 3600:
             raise tornado.web.HTTPError(403)
 
         key = f'{prefix}_{self.args.t}_{self.args.n}'.encode()
-        if self.args.s[:8] != getattr(hashlib, method)(key).hexdigest()[:8]:
+        if self.args.s[:8] != hashlib.md5(key).hexdigest()[:8]:
             raise tornado.web.HTTPError(403)
 
     async def get_current_user(self):
         token = self.get_cookie('token', self.args.token)
         if token and hasattr(self.app, 'db') and isinstance(self.app.db, (Mongo, Motor)):
             user = await awaitable(self.app.db.users.find_one({'token': token}))
             if user:
@@ -221,16 +236,14 @@
 
     def query(self, collection, query=None, projection=None, include=[], exclude=[], schema=None):
         schema = copy.deepcopy(schema or {})
         schema.setdefault('_id', ObjectId)
         query = copy.deepcopy(query or self.args)
         query = self.filter(query, include=include, exclude=exclude)
         query = self.format(query, schema)
-        if isinstance(projection, list):
-            projection = {k: 1 for k in projection}
         cursor = self.db[collection].find(query, projection)
 
         self.args.setdefault('order', -1)
         self.args.setdefault('page', 1)
         self.args.setdefault('size', 20)
         if self.args.sort:
             cursor = cursor.sort(self.args.sort, self.args.order)
```

### Comparing `kkutils-1.6.5/tornado_utils/userhandler.py` & `kkutils-1.6.6/tornado_utils/userhandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 Author: zhangkai
 Email: kai.zhang1@nio.com
 Last modified: 2018-06-03 00:38:17
 '''
+
 import datetime
 import hashlib
+import os
 import random
 import re
 import uuid
 
 import pymongo
 import tornado.web
 from bson import ObjectId
@@ -73,14 +75,16 @@
 
     async def check_email(self):
         email = self.get_argument('email', None)
         if not email:
             return Dict({'err': 1, 'msg': '请输入邮箱'})
         if len(email) > 64:
             return Dict({'err': 1, 'msg': '邮箱地址太长'})
+        if email.find(' ') >= 0:
+            return Dict({'err': 1, 'msg': '邮箱地址不能包含空格'})
         if not re.match(r'.*@(.*)\.(\w+)$', email):
             return Dict({'err': 1, 'msg': '请填写正确的邮箱格式'})
         if not re.search(r'@(qq.com|gmail.com|163.com|126.com|yeah.net|outlook.com|live.com|foxmail.com|hotmail.com|sina.com|vip.qq.com|139.com|icloud.com|aliyun.com|88.com|sina.cn|tom.com|live.cn|yahoo.com|189.cn|msn.com|sohu.com|yandex.com|.edu.cn|vip.163.com|msn.cn)$', email.lower()):
             return Dict({'err': 1, 'msg': '请使用常用邮箱注册'})
         if await awaitable(self.db.users.find_one({'email': email})):
             return Dict({'err': 1, 'msg': '邮箱地址重复'})
         return Dict({'err': 0})
@@ -91,38 +95,34 @@
             return Dict({'err': 1, 'msg': f'scene is not defined: {scene}'})
 
         resp = await self.http.get(scene)
         if not resp.code == 200:
             return Dict({'err': 1, 'msg': f'get scene failed: {scene}'})
 
         ret = resp.json()
-        if not ret.err:
-            user = await awaitable(self.db.users.find_one({'openId': ret.openId}))
-            if user:
-                ret = user
-                # if self.current_user and self.current_user._id != user._id:
-                #    return {'err': 2, 'msg': f'该微信号已绑定用户{user.id}'}
-            else:
-                if self.current_user:
-                    ret.active = True
-                    ret.token = self.current_user.token
-                    keys = ['active', 'openId', 'avatarUrl', 'city', 'country', 'gender', 'language', 'nickName', 'province']
-                    update = {k: v for k, v in ret.items() if k in keys if v}
-                    await awaitable(self.db.users.update_one({'_id': self.current_user._id}, {'$set': update}))
-                else:
-                    ret.id = await awaitable(self.db.users.seq_id)
-                    ret.token = uuid.uuid4().hex
-                    ret.active = True
-                    ret.created_at = datetime.datetime.now().replace(microsecond=0)
-                    await awaitable(self.db.users.update_one({'openId': ret.openId}, {'$set': ret}, upsert=True))
-
-            self.set_cookie('token', ret.token, expires_days=365)
-            ret.err = 0
+        if ret.err:
+            return ret
 
-        return ret
+        user = await awaitable(self.db.users.find_one({'openId': ret.openId}))
+        if not user:
+            if self.current_user:
+                ret.active = True
+                keys = ['active', 'openId', 'avatarUrl', 'city', 'country', 'gender', 'language', 'nickName', 'province']
+                update = {k: v for k, v in ret.items() if k in keys if v}
+                user = await awaitable(self.db.users.find_one_and_update({'_id': self.current_user._id}, {'$set': update}, return_document=True))
+            else:
+                ret.active = True
+                ret.token = uuid.uuid4().hex
+                ret.id = await awaitable(self.db.users.seq_id)
+                ret.created_at = datetime.datetime.now().replace(microsecond=0)
+                user = await awaitable(self.db.users.find_one_and_update({'openId': ret.openId}, {'$set': ret}, upsert=True, return_document=True))
+
+        user.err = 0
+        self.set_cookie('token', user.token, expires_days=365)
+        return user
 
 
 @bp.route("/check")
 class CheckHandler(BaseHandler):
 
     async def get(self):
         for key, value in self.args.items():
@@ -176,26 +176,39 @@
         })
         try:
             user = await awaitable(self.db.users.find_one_and_update({'username': doc['username']},
                                                                      {'$set': doc},
                                                                      upsert=True,
                                                                      return_document=True))
         except pymongo.errors.DuplicateKeyError:
+            count = await awaitable(self.db.users.count_documents({'id': {'$exists': 0}}))
+            if count == 0:
+                return self.finish({'err': 1, 'msg': '用户名重复'})
+
             seq_id = await awaitable(self.db.users.seq_id)
             await awaitable(self.db.users.find_one_and_update({'id': {'$exists': 0}}, {'$set': {'id': seq_id}}))
             user = await awaitable(self.db.users.find_one_and_update({'username': doc['username']},
                                                                      {'$set': doc},
                                                                      upsert=True,
                                                                      return_document=True))
 
         update = {}
         if not user.id:
-            update['id'] = await awaitable(self.db.users.seq_id)
-            if update['id'] == 1:
-                update['admin'] = True
+            if os.environ.get('MISSING_IDS'):
+                ids = [int(x) for x in os.environ.get('MISSING_IDS', '').split(',')]
+                exist_ids = await awaitable(self.db.users.distinct('id', {'id': {'$in': ids}}))
+                missing_ids = sorted(set(ids) - set(exist_ids))
+                if missing_ids:
+                    update['id'] = missing_ids[0]
+
+            if 'id' not in update:
+                update['id'] = await awaitable(self.db.users.seq_id)
+                if update['id'] == 1:
+                    update['admin'] = True
+
         if update:
             await awaitable(self.db.users.update_one({'_id': user._id}, {'$set': update}))
             user.update(update)
 
         self.set_cookie('token', token, expires_days=365)
         self.finish({'err': 0, 'user': user})
```

### Comparing `kkutils-1.6.5/tornado_utils/utils.py` & `kkutils-1.6.6/tornado_utils/utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/__init__.py` & `kkutils-1.6.6/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/base_utils.py` & `kkutils-1.6.6/utils/base_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,19 +242,22 @@
 
 async def awaitable(ret):
     return await ret if inspect.isawaitable(ret) else ret
 
 
 def multi_apply(func, *args, **kwargs):
     workers = kwargs.pop('workers', os.cpu_count())
-    batch = kwargs.pop('batch', workers)
     backend = kwargs.pop('backend', 'thread')
+    batch = kwargs.pop('batch', None)
     size = len(args[0])
-    step = math.ceil(size / batch)
-    iterables = [[x[i::step] for i in range(step)] for x in args]
+    if batch:
+        step = math.ceil(size / batch)
+        iterables = [[x[i::step] for i in range(step)] for x in args]
+    else:
+        iterables = [[x[i::workers] for i in range(workers)] for x in args]
     func = partial(func, **kwargs) if kwargs else func
     Executor = ThreadPoolExecutor if backend == 'thread' else ProcessPoolExecutor
     with Executor(workers) as executor:
         results = executor.map(func, *iterables)
     results = list(results)
     if all([isinstance(x, (list, tuple)) for x in results]):
         results = list(chain(*zip_longest(*results)))[:size]
```

### Comparing `kkutils-1.6.5/utils/cached_property.py` & `kkutils-1.6.6/utils/cached_property.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/config_utils.py` & `kkutils-1.6.6/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/crypto.py` & `kkutils-1.6.6/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/curl_utils.py` & `kkutils-1.6.6/utils/curl_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/db_utils.py` & `kkutils-1.6.6/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/decorator.py` & `kkutils-1.6.6/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/email_utils.py` & `kkutils-1.6.6/utils/email_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 class EmailBase:
 
     def __init__(self, sender=None, smtp=None, user=None, pwd=None, use_tls=False):
         self.sender = sender or os.environ.get('EMAIL_SENDER')
         self.smtp = smtp or os.environ.get('EMAIL_SMTP')
         self.user = user or os.environ.get('EMAIL_USER')
         self.pwd = pwd or os.environ.get('EMAIL_PWD')
-        self.use_tls = use_tls or os.environ.get('EMAIL_TLS')
-        if isinstance(self.use_tls, str):
-            self.use_tls = self.use_tls.lower() == 'true'
+        self.use_tls = use_tls or os.environ.get('EMAIL_TLS') == 'true'
 
     @staticmethod
     def _format_addr(s):
         # format: username<email address>
         name, addr = parseaddr(s)
         return formataddr((Header(name, 'utf-8').encode(), addr)) if name else addr
```

### Comparing `kkutils-1.6.5/utils/fire.py` & `kkutils-1.6.6/utils/fire.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/http_utils.py` & `kkutils-1.6.6/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/log_utils.py` & `kkutils-1.6.6/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/rabbitmq.py` & `kkutils-1.6.6/utils/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/stopwatch.py` & `kkutils-1.6.6/utils/stopwatch.py`

 * *Files identical despite different names*

### Comparing `kkutils-1.6.5/utils/xdb_searcher.py` & `kkutils-1.6.6/utils/xdb_searcher.py`

 * *Files identical despite different names*

