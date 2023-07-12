# Comparing `tmp/bbat-5.2.5.tar.gz` & `tmp/bbat-5.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbat-5.2.5.tar", last modified: Mon Jul 10 08:41:55 2023, max compression
+gzip compressed data, was "bbat-5.2.6.tar", last modified: Wed Jul 12 02:28:31 2023, max compression
```

## Comparing `bbat-5.2.5.tar` & `bbat-5.2.6.tar`

### file list

```diff
@@ -1,45 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.275664 bbat-5.2.5/
--rw-rw-rw-   0        0        0      289 2023-07-10 08:41:55.273663 bbat-5.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-10 01:19:32.000000 bbat-5.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.225149 bbat-5.2.5/bbat/
--rw-rw-rw-   0        0        0        0 2023-07-10 08:21:51.000000 bbat-5.2.5/bbat/__init__.py
--rw-rw-rw-   0        0        0     1654 2023-07-10 07:31:31.000000 bbat-5.2.5/bbat/config.py
--rw-rw-rw-   0        0        0     1228 2023-07-10 03:21:13.000000 bbat-5.2.5/bbat/date.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.247152 bbat-5.2.5/bbat/db/
--rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/db/__init__.py
--rw-rw-rw-   0        0        0     5371 2023-07-10 05:33:54.000000 bbat-5.2.5/bbat/db/aio_mysql.py
--rw-rw-rw-   0        0        0     2632 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/db/aio_sqlite.py
--rw-rw-rw-   0        0        0     2339 2023-07-10 05:34:01.000000 bbat-5.2.5/bbat/db/mysql.py
--rw-rw-rw-   0        0        0      287 2023-07-10 03:36:58.000000 bbat-5.2.5/bbat/hash.py
--rw-rw-rw-   0        0        0       30 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/hi.py
--rw-rw-rw-   0        0        0     1978 2023-07-10 03:27:55.000000 bbat-5.2.5/bbat/image.py
--rw-rw-rw-   0        0        0      920 2023-07-10 08:19:47.000000 bbat-5.2.5/bbat/log.py
--rw-rw-rw-   0        0        0      822 2023-07-10 08:19:52.000000 bbat-5.2.5/bbat/machine.py
--rw-rw-rw-   0        0        0     1670 2023-07-10 04:38:59.000000 bbat-5.2.5/bbat/notice.py
--rw-rw-rw-   0        0        0     2413 2023-07-10 06:14:27.000000 bbat-5.2.5/bbat/np.py
--rw-rw-rw-   0        0        0      981 2023-07-10 08:07:34.000000 bbat-5.2.5/bbat/path.py
--rw-rw-rw-   0        0        0     4198 2023-07-10 06:52:29.000000 bbat-5.2.5/bbat/text.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.255152 bbat-5.2.5/bbat/web/
--rw-rw-rw-   0        0        0     1756 2023-07-10 07:07:01.000000 bbat-5.2.5/bbat/web/__init__.py
--rw-rw-rw-   0        0        0      504 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/web/cors.py
--rw-rw-rw-   0        0        0     4503 2023-07-10 07:58:06.000000 bbat-5.2.5/bbat/web/db_server.py
--rw-rw-rw-   0        0        0      177 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/web/flask_app.py
--rw-rw-rw-   0        0        0     1571 2023-07-10 08:38:58.000000 bbat-5.2.5/bbat/web/sanic_app.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.268664 bbat-5.2.5/bbat/web/url_to_sql/
--rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/web/url_to_sql/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-07-10 07:04:39.000000 bbat-5.2.5/bbat/web/url_to_sql/field.py
--rw-rw-rw-   0        0        0     7552 2023-07-10 07:04:45.000000 bbat-5.2.5/bbat/web/url_to_sql/query.py
--rw-rw-rw-   0        0        0     2256 2023-07-10 07:04:49.000000 bbat-5.2.5/bbat/web/url_to_sql/relation.py
--rw-rw-rw-   0        0        0      722 2023-07-10 07:04:52.000000 bbat-5.2.5/bbat/web/url_to_sql/test.py
--rw-rw-rw-   0        0        0      964 2023-07-10 01:19:32.000000 bbat-5.2.5/bbat/web/url_to_sql/util.py
--rw-rw-rw-   0        0        0     1473 2023-07-10 07:04:56.000000 bbat-5.2.5/bbat/web/url_to_sql/where.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.240148 bbat-5.2.5/bbat.egg-info/
--rw-rw-rw-   0        0        0      289 2023-07-10 08:41:54.000000 bbat-5.2.5/bbat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-07-10 08:41:55.000000 bbat-5.2.5/bbat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 08:41:54.000000 bbat-5.2.5/bbat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-10 08:41:54.000000 bbat-5.2.5/bbat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 08:41:55.275664 bbat-5.2.5/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-07-10 08:41:43.000000 bbat-5.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:41:55.272662 bbat-5.2.5/test/
--rw-rw-rw-   0        0        0      209 2023-07-10 06:44:06.000000 bbat-5.2.5/test/test_config.py
--rw-rw-rw-   0        0        0      194 2023-07-10 06:44:18.000000 bbat-5.2.5/test/test_db_mysql.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.430219 bbat-5.2.6/
+-rw-rw-rw-   0        0        0      289 2023-07-12 02:28:31.428220 bbat-5.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-10 01:19:32.000000 bbat-5.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.382219 bbat-5.2.6/bbat/
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:21:51.000000 bbat-5.2.6/bbat/__init__.py
+-rw-rw-rw-   0        0        0     1720 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/config.py
+-rw-rw-rw-   0        0        0     3085 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/crypto.py
+-rw-rw-rw-   0        0        0     1230 2023-07-11 01:11:37.000000 bbat-5.2.6/bbat/date.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.402223 bbat-5.2.6/bbat/db/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/db/__init__.py
+-rw-rw-rw-   0        0        0     5371 2023-07-10 05:33:54.000000 bbat-5.2.6/bbat/db/aio_mysql.py
+-rw-rw-rw-   0        0        0     2632 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/db/aio_sqlite.py
+-rw-rw-rw-   0        0        0     2339 2023-07-10 05:34:01.000000 bbat-5.2.6/bbat/db/mysql.py
+-rw-rw-rw-   0        0        0       30 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/hi.py
+-rw-rw-rw-   0        0        0     1978 2023-07-11 01:47:46.000000 bbat-5.2.6/bbat/image.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.405219 bbat-5.2.6/bbat/llm/
+-rw-rw-rw-   0        0        0        0 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/llm/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/llm/chatgpt.py
+-rw-rw-rw-   0        0        0      920 2023-07-10 08:19:47.000000 bbat-5.2.6/bbat/log.py
+-rw-rw-rw-   0        0        0      822 2023-07-11 01:47:51.000000 bbat-5.2.6/bbat/machine.py
+-rw-rw-rw-   0        0        0     1868 2023-07-11 02:21:26.000000 bbat-5.2.6/bbat/notice.py
+-rw-rw-rw-   0        0        0     2413 2023-07-10 06:14:27.000000 bbat-5.2.6/bbat/np.py
+-rw-rw-rw-   0        0        0      981 2023-07-10 08:07:34.000000 bbat-5.2.6/bbat/path.py
+-rw-rw-rw-   0        0        0     4198 2023-07-10 06:52:29.000000 bbat-5.2.6/bbat/text.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.414222 bbat-5.2.6/bbat/web/
+-rw-rw-rw-   0        0        0        0 2023-07-11 01:54:28.000000 bbat-5.2.6/bbat/web/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-07-11 01:55:27.000000 bbat-5.2.6/bbat/web/client.py
+-rw-rw-rw-   0        0        0      504 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/web/cors.py
+-rw-rw-rw-   0        0        0     3929 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/web/db_server.py
+-rw-rw-rw-   0        0        0      177 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/web/flask_app.py
+-rw-rw-rw-   0        0        0     1566 2023-07-11 01:11:37.000000 bbat-5.2.6/bbat/web/sanic_app.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.424222 bbat-5.2.6/bbat/web/url_to_sql/
+-rw-rw-rw-   0        0        0        0 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/web/url_to_sql/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-07-10 07:04:39.000000 bbat-5.2.6/bbat/web/url_to_sql/field.py
+-rw-rw-rw-   0        0        0     7552 2023-07-10 07:04:45.000000 bbat-5.2.6/bbat/web/url_to_sql/query.py
+-rw-rw-rw-   0        0        0     2256 2023-07-10 07:04:49.000000 bbat-5.2.6/bbat/web/url_to_sql/relation.py
+-rw-rw-rw-   0        0        0      722 2023-07-10 07:04:52.000000 bbat-5.2.6/bbat/web/url_to_sql/test.py
+-rw-rw-rw-   0        0        0      964 2023-07-10 01:19:32.000000 bbat-5.2.6/bbat/web/url_to_sql/util.py
+-rw-rw-rw-   0        0        0     1473 2023-07-10 07:04:56.000000 bbat-5.2.6/bbat/web/url_to_sql/where.py
+-rw-rw-rw-   0        0        0     2156 2023-07-12 02:26:35.000000 bbat-5.2.6/bbat/zcli.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.395221 bbat-5.2.6/bbat.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-07-12 02:28:31.000000 bbat-5.2.6/bbat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2023-07-12 02:28:31.000000 bbat-5.2.6/bbat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 02:28:31.000000 bbat-5.2.6/bbat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-12 02:28:31.000000 bbat-5.2.6/bbat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 02:28:31.000000 bbat-5.2.6/bbat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 02:28:31.430219 bbat-5.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-07-12 02:28:27.000000 bbat-5.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 02:28:31.427221 bbat-5.2.6/test/
+-rw-rw-rw-   0        0        0      209 2023-07-10 06:44:06.000000 bbat-5.2.6/test/test_config.py
+-rw-rw-rw-   0        0        0      194 2023-07-10 06:44:18.000000 bbat-5.2.6/test/test_db_mysql.py
```

### Comparing `bbat-5.2.5/bbat/config.py` & `bbat-5.2.6/bbat/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 def get_env(key, default=""): 
     val = os.getenv(key)
     return val if val else default
 
 class Config:
     def __init__(self):
         self.config = {}
+
+    def __call__(self, key):
+        return self.get_env(key)
     
     def load_yaml(self, file):
         import yaml
         with open(file, 'r') as conf_file:
             self.config = yaml.safe_load(conf_file)
 
     def load_json(self, file):
```

### Comparing `bbat-5.2.5/bbat/date.py` & `bbat-5.2.6/bbat/date.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import time
 import datetime
 
-def time_to_str(timestamp=None, f="%Y-%m-%d %H:%M:%S"):
+def time_to_str(timestamp=None, format="%Y-%m-%d %H:%M:%S"):
     '''
     Args 
         f - %Y-%m-%d %H:%M:%S 格式化时间
     '''
     if timestamp:
         ts = datetime.datetime.fromtimestamp(timestamp)
     else:
         ts = datetime.datetime.now()
-    formatted = ts.strftime(f)
+    formatted = ts.strftime(format)
     return formatted
 
-def str_to_time(date, f="%Y-%m-%d %H:%M:%S"):
+def str_to_time(date, format="%Y-%m-%d %H:%M:%S"):
     '''
     Args:
         str_date - 字符时间
         f - 默认 %Y-%m-%d %H:%M:%S '''
-    return datetime.datetime.strptime(date, "%Y-%m-%d %H:%M:%S")
+    return datetime.datetime.strptime(date, format)
 
 
 def timestamp():
     return time.time()
 
 def date_diff(fmt='%Y-%m-%d %H:%M:%S', start_date=None, **kwargs):
     """
```

### Comparing `bbat-5.2.5/bbat/db/aio_mysql.py` & `bbat-5.2.6/bbat/db/aio_mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/db/aio_sqlite.py` & `bbat-5.2.6/bbat/db/aio_sqlite.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/db/mysql.py` & `bbat-5.2.6/bbat/db/mysql.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/image.py` & `bbat-5.2.6/bbat/image.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/log.py` & `bbat-5.2.6/bbat/log.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/machine.py` & `bbat-5.2.6/bbat/machine.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/notice.py` & `bbat-5.2.6/bbat/notice.py`

 * *Files 17% similar despite different names*

```diff
@@ -83,23 +83,35 @@
 00000520: e58f 91e9 8081 e688 90e5 8a9f 2229 0d0a  ............")..
 00000530: 2020 2020 6578 6365 7074 2073 6d74 706c      except smtpl
 00000540: 6962 2e53 4d54 5045 7863 6570 7469 6f6e  ib.SMTPException
 00000550: 2061 7320 653a 0d0a 2020 2020 2020 2020   as e:..        
 00000560: 7072 696e 7428 6622 7b65 7d3a 20e6 97a0  print(f"{e}: ...
 00000570: e6b3 95e5 8f91 e980 81e9 82ae e4bb b622  ..............."
 00000580: 290d 0a0d 0a0d 0a0d 0a64 6566 2073 656e  )........def sen
-00000590: 645f 6665 6973 6875 2874 6974 6c65 3d27  d_feishu(title='
-000005a0: 5445 5354 272c 2074 6578 743d 2727 2c20  TEST', text='', 
-000005b0: 686f 6f6b 5f75 726c 3d27 6c6f 6767 6572  hook_url='logger
-000005c0: 2729 3a0d 0a20 2020 2072 6571 7565 7374  '):..    request
-000005d0: 732e 706f 7374 2868 6f6f 6b5f 7572 6c2c  s.post(hook_url,
-000005e0: 206a 736f 6e3d 7b22 7469 746c 6522 3a20   json={"title": 
-000005f0: 7374 7228 7469 746c 6529 2c20 2274 6578  str(title), "tex
-00000600: 7422 3a20 6627 7b74 6578 747d 2027 7d29  t": f'{text} '})
-00000610: 0d0a 0d0a 0d0a 6966 205f 5f6e 616d 655f  ......if __name_
-00000620: 5f20 3d3d 2027 5f5f 6d61 696e 5f5f 273a  _ == '__main__':
-00000630: 0d0a 2020 2020 7365 6e64 5f66 6569 7368  ..    send_feish
-00000640: 7528 686f 6f6b 5f75 726c 3d27 2729 0d0a  u(hook_url='')..
-00000650: 0d0a 2020 2020 7365 6e64 5f65 6d61 696c  ..    send_email
-00000660: 2822 e6b5 8be8 af95 e982 aee4 bbb6 222c  ("............",
-00000670: 206d 7367 3d27 e982 aee4 bbb6 e586 85e5   msg='..........
-00000680: aeb9 2729 0d0a                           ..')..
+00000590: 645f 6665 6973 6875 2875 726c 2c20 7465  d_feishu(url, te
+000005a0: 7874 293a 0d0a 2020 2020 6865 6164 6572  xt):..    header
+000005b0: 7320 3d20 7b27 436f 6e74 656e 742d 7479  s = {'Content-ty
+000005c0: 7065 273a 2027 6170 706c 6963 6174 696f  pe': 'applicatio
+000005d0: 6e2f 6a73 6f6e 277d 0d0a 2020 2020 6d73  n/json'}..    ms
+000005e0: 6720 3d20 7b0d 0a20 2020 2020 2020 2022  g = {..        "
+000005f0: 6d73 675f 7479 7065 223a 2022 7465 7874  msg_type": "text
+00000600: 222c 0d0a 2020 2020 2020 2020 2263 6f6e  ",..        "con
+00000610: 7465 6e74 223a 207b 0d0a 2020 2020 2020  tent": {..      
+00000620: 2020 2020 2020 2274 6578 7422 3a20 7465        "text": te
+00000630: 7874 0d0a 2020 2020 2020 2020 7d0d 0a20  xt..        }.. 
+00000640: 2020 207d 0d0a 2020 2020 7265 7175 6573     }..    reques
+00000650: 7473 2e70 6f73 7428 7572 6c2c 2068 6561  ts.post(url, hea
+00000660: 6465 7273 3d68 6561 6465 7273 2c20 6a73  ders=headers, js
+00000670: 6f6e 3d6d 7367 290d 0a0d 0a0d 0a69 6620  on=msg)......if 
+00000680: 5f5f 6e61 6d65 5f5f 203d 3d20 275f 5f6d  __name__ == '__m
+00000690: 6169 6e5f 5f27 3a0d 0a20 2020 2075 726c  ain__':..    url
+000006a0: 203d 2022 6874 7470 733a 2f2f 6f70 656e   = "https://open
+000006b0: 2e66 6569 7368 752e 636e 2f6f 7065 6e2d  .feishu.cn/open-
+000006c0: 6170 6973 2f62 6f74 2f76 322f 686f 6f6b  apis/bot/v2/hook
+000006d0: 2f64 6236 3234 3237 312d 3931 3530 2d34  /db624271-9150-4
+000006e0: 6365 362d 6265 3331 2d39 3064 3561 3562  ce6-be31-90d5a5b
+000006f0: 3563 3565 3222 0d0a 2020 2020 7365 6e64  5c5e2"..    send
+00000700: 5f66 6569 7368 7528 686f 6f6b 5f75 726c  _feishu(hook_url
+00000710: 3d27 2729 0d0a 0d0a 2020 2020 7365 6e64  ='')....    send
+00000720: 5f65 6d61 696c 2822 e6b5 8be8 af95 e982  _email("........
+00000730: aee4 bbb6 222c 206d 7367 3d27 e982 aee4  ....", msg='....
+00000740: bbb6 e586 85e5 aeb9 2729 0d0a            ........')..
```

### Comparing `bbat-5.2.5/bbat/np.py` & `bbat-5.2.6/bbat/np.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/path.py` & `bbat-5.2.6/bbat/path.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/text.py` & `bbat-5.2.6/bbat/text.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/web/__init__.py` & `bbat-5.2.6/bbat/web/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,55 @@
-
-from ctypes import Union
 import requests
 
 
-def req(url, method='GET', json=False, timeout=3, encoding=None, **kwargs):
-    '''Args
+def http(url, method="GET", json=False, timeout=3, encoding=None, **kwargs):
+    """Args
     url - 地址
     method - http method
-    json - return json type'''
+    json - return json type"""
     params = {}
-    params['timeout'] = timeout
-    params['headers'] = {
-        'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) '
-                      'Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE '
-    }
+    params["timeout"] = timeout
+    params["headers"] = {"User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) " "Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE "}
     kwargs.update(params)
     resp = requests.request(method, url, **kwargs)
     resp.encoding = encoding if encoding else resp.apparent_encoding
     return resp.json() if json else resp
 
 
-
 def download(url, output="./"):
-    '''Args
-        url - URL to download
-        output - Output file'''
+    """Args
+    url - URL to download
+    output - Output file"""
     response = requests.get(url, stream=True)
     response.raise_for_status()
     filename = url.split("/")[-1]
-    with open(f"{output}/{filename}", 'wb') as file:
+    with open(f"{output}/{filename}", "wb") as file:
         for chunk in response.iter_content(chunk_size=8192):
             if chunk:
                 file.write(chunk)
     return output
 
 
-
-def xpath(url, path="//text()", encoding='utf-8', **kwargs):
-    '''
+def xpath(url, path="//text()", encoding="utf-8", **kwargs):
+    """
     Args:
         url - string URL to
         path - xpath ql
         encoding - default utf-8
-    '''
+    """
     from lxml.etree import HTML
+
     if not isinstance(path, list):
         path = [path]
     result = []
-    resp = req(url, encoding=encoding)
+    resp = http(url, encoding=encoding)
     html = HTML(resp.text)
     for pth in path:
         xpath_parsed = html.xpath(pth, **kwargs)
         result.append(xpath_parsed)
     return result
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     url = "https://top.baidu.com/board?tab=realtime"
     res = xpath(url, "//div[@class='c-single-text-ellipsis']/text()")
-    print(res, len(res))
+    print(res, len(res))
```

### Comparing `bbat-5.2.5/bbat/web/sanic_app.py` & `bbat-5.2.6/bbat/web/sanic_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from bbat.path import mkdir
 from bbat.web import cors
 
 
 app = Sanic('sanic_app')
 
 
-# Route: ping
-@app.route("/ping")
+# index
+@app.route("/")
 def ping(request):
-    return response.text('pong')
+    return response.text('Forbidden')
 
 # Public static dir
 mkdir('./static')
 app.static('/static', './static/')
 
 # middleware
 @app.middleware("request")
```

### Comparing `bbat-5.2.5/bbat/web/url_to_sql/field.py` & `bbat-5.2.6/bbat/web/url_to_sql/field.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/web/url_to_sql/query.py` & `bbat-5.2.6/bbat/web/url_to_sql/query.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/web/url_to_sql/relation.py` & `bbat-5.2.6/bbat/web/url_to_sql/relation.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/web/url_to_sql/test.py` & `bbat-5.2.6/bbat/web/url_to_sql/test.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/web/url_to_sql/util.py` & `bbat-5.2.6/bbat/web/url_to_sql/util.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat/web/url_to_sql/where.py` & `bbat-5.2.6/bbat/web/url_to_sql/where.py`

 * *Files identical despite different names*

### Comparing `bbat-5.2.5/bbat.egg-info/SOURCES.txt` & `bbat-5.2.6/bbat.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 README.md
 setup.py
 bbat/__init__.py
 bbat/config.py
+bbat/crypto.py
 bbat/date.py
-bbat/hash.py
 bbat/hi.py
 bbat/image.py
 bbat/log.py
 bbat/machine.py
 bbat/notice.py
 bbat/np.py
 bbat/path.py
 bbat/text.py
+bbat/zcli.py
 bbat.egg-info/PKG-INFO
 bbat.egg-info/SOURCES.txt
 bbat.egg-info/dependency_links.txt
+bbat.egg-info/entry_points.txt
 bbat.egg-info/top_level.txt
 bbat/db/__init__.py
 bbat/db/aio_mysql.py
 bbat/db/aio_sqlite.py
 bbat/db/mysql.py
+bbat/llm/__init__.py
+bbat/llm/chatgpt.py
 bbat/web/__init__.py
+bbat/web/client.py
 bbat/web/cors.py
 bbat/web/db_server.py
 bbat/web/flask_app.py
 bbat/web/sanic_app.py
 bbat/web/url_to_sql/__init__.py
 bbat/web/url_to_sql/field.py
 bbat/web/url_to_sql/query.py
```

