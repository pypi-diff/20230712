# Comparing `tmp/mypylib-0.1.79.tar.gz` & `tmp/mypylib-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.1.79.tar", last modified: Thu Jul  6 14:52:50 2023, max compression
+gzip compressed data, was "mypylib-0.1.80.tar", last modified: Wed Jul 12 15:07:40 2023, max compression
```

## Comparing `mypylib-0.1.79.tar` & `mypylib-0.1.80.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-06 14:52:50.957095 mypylib-0.1.79/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-07-06 14:52:50.956894 mypylib-0.1.79/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.79/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-06 14:52:50.954477 mypylib-0.1.79/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.79/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    47196 2023-07-06 14:52:14.000000 mypylib-0.1.79/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.79/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.79/mypylib/binance_copy_bot_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.79/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2412 2023-07-06 14:22:34.000000 mypylib-0.1.79/mypylib/crawler.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.79/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.79/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.79/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-06-01 04:56:52.000000 mypylib-0.1.79/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.79/mypylib/mytest.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.79/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.79/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.79/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.79/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.79/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.79/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-06-01 04:56:52.000000 mypylib-0.1.79/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-06 14:52:50.956288 mypylib-0.1.79/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.79/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.79/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.79/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8466 2023-06-19 13:26:50.000000 mypylib-0.1.79/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8217 2023-07-03 23:14:11.000000 mypylib-0.1.79/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-06 14:52:50.955884 mypylib-0.1.79/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-07-06 14:52:50.000000 mypylib-0.1.79/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      673 2023-07-06 14:52:50.000000 mypylib-0.1.79/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-07-06 14:52:50.000000 mypylib-0.1.79/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-07-06 14:52:50.000000 mypylib-0.1.79/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-07-06 14:52:50.957171 mypylib-0.1.79/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.79/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-12 15:07:40.232627 mypylib-0.1.80/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-07-12 15:07:40.232361 mypylib-0.1.80/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.80/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-12 15:07:40.229312 mypylib-0.1.80/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.80/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    47236 2023-07-12 15:07:00.000000 mypylib-0.1.80/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.80/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.80/mypylib/binance_copy_bot_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.80/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5333 2023-07-12 15:06:31.000000 mypylib-0.1.80/mypylib/crawler.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.80/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.80/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.80/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-06-01 04:56:52.000000 mypylib-0.1.80/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.80/mypylib/mytest.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.80/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.80/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.80/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.80/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.80/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.80/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-06-01 04:56:52.000000 mypylib-0.1.80/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-12 15:07:40.231707 mypylib-0.1.80/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.80/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.80/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.80/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8466 2023-06-19 13:26:50.000000 mypylib-0.1.80/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8217 2023-07-03 23:14:11.000000 mypylib-0.1.80/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-12 15:07:40.231139 mypylib-0.1.80/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-07-12 15:07:39.000000 mypylib-0.1.80/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      673 2023-07-12 15:07:40.000000 mypylib-0.1.80/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-07-12 15:07:39.000000 mypylib-0.1.80/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-07-12 15:07:40.000000 mypylib-0.1.80/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-07-12 15:07:40.232718 mypylib-0.1.80/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.80/setup.py
```

### Comparing `mypylib-0.1.79/README.md` & `mypylib-0.1.80/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/MP_shioaji_ticks.py` & `mypylib-0.1.80/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/__init__.py` & `mypylib-0.1.80/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,19 +67,20 @@
     '2023/05/10: 0.1.72 改用shioaji API',
     '2023/05/17: 0.1.73 shioaji 1.0 改 Mmvp.py & ti.py',
     '2023/05/22: 0.1.74 mvp() 不繼承 base class。因為shioaji升級的關係。先可以跑再說',
     '2023/06/01: 0.1.75 Apply Carey change',
     '2023/06/15: 0.1.76 Add crawler',
     '2023/06/19: 0.1.77 Not using stupid Redis connection pool',
     '2023/07/05: 0.1.78 cynes api v1 support',
-    '2023/07/06: 0.1.79 news crawler little modification'
+    '2023/07/06: 0.1.79 news crawler little modification',
+    '2023/07/12: 0.1.80 修改crawler'
 
 }
 
-__version__ = '0.1.79'
+__version__ = '0.1.80'
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
```

### Comparing `mypylib-0.1.79/mypylib/binance_copy_bot.py` & `mypylib-0.1.80/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/binance_copy_bot_test.py` & `mypylib-0.1.80/mypylib/binance_copy_bot_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/chdbif.py` & `mypylib-0.1.80/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/crypto.py` & `mypylib-0.1.80/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/finmind.py` & `mypylib-0.1.80/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/libexcel.py` & `mypylib-0.1.80/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/mvp.py` & `mypylib-0.1.80/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/mytest.py` & `mypylib-0.1.80/mypylib/mytest.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/option_test.py` & `mypylib-0.1.80/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/shioaji_history_ticks.py` & `mypylib-0.1.80/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/shioaji_kline.py` & `mypylib-0.1.80/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/shioaji_ticks.py` & `mypylib-0.1.80/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/sjtools.py` & `mypylib-0.1.80/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/tLineNotify.py` & `mypylib-0.1.80/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/ti.py` & `mypylib-0.1.80/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.1.80/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/tplaysound.py` & `mypylib-0.1.80/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/tredis.py` & `mypylib-0.1.80/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib/warrant.py` & `mypylib-0.1.80/mypylib/warrant.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/mypylib.egg-info/SOURCES.txt` & `mypylib-0.1.80/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.79/setup.py` & `mypylib-0.1.80/setup.py`

 * *Files identical despite different names*

