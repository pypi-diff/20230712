# Comparing `tmp/tg-botting-1.6.2.7.tar.gz` & `tmp/tg-botting-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-1.6.2.7.tar", last modified: Wed May 24 15:31:24 2023, max compression
+gzip compressed data, was "tg-botting-2.0.tar", last modified: Wed Jul 12 19:38:05 2023, max compression
```

## Comparing `tg-botting-1.6.2.7.tar` & `tg-botting-2.0.tar`

### file list

```diff
@@ -1,17 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 15:31:24.241020 tg-botting-1.6.2.7/
--rw-rw-rw-   0        0        0      920 2023-05-24 15:31:24.241020 tg-botting-1.6.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 15:31:24.242017 tg-botting-1.6.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1447 2023-05-24 15:31:06.000000 tg-botting-1.6.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:31:24.236033 tg-botting-1.6.2.7/tg_botting/
--rw-rw-rw-   0        0        0    31783 2023-05-22 17:49:59.000000 tg-botting-1.6.2.7/tg_botting/bot.py
--rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.2.7/tg_botting/cog.py
--rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.2.7/tg_botting/generals.py
--rw-rw-rw-   0        0        0    17322 2023-05-24 15:31:06.000000 tg-botting-1.6.2.7/tg_botting/objects.py
--rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.2.7/tg_botting/user_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:31:24.240023 tg-botting-1.6.2.7/tg_botting.egg-info/
--rw-rw-rw-   0        0        0      920 2023-05-24 15:31:24.000000 tg-botting-1.6.2.7/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-24 15:31:24.000000 tg-botting-1.6.2.7/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 15:31:24.000000 tg-botting-1.6.2.7/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-24 15:31:24.000000 tg-botting-1.6.2.7/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-24 15:31:24.000000 tg-botting-1.6.2.7/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 19:38:05.357666 tg-botting-2.0/
+-rw-rw-rw-   0        0        0     3405 2023-07-12 19:38:05.357076 tg-botting-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 19:38:05.357666 tg-botting-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:38:05.350094 tg-botting-2.0/tg_botting/
+-rw-rw-rw-   0        0        0      771 2023-07-12 19:35:29.000000 tg-botting-2.0/tg_botting/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.0/tg_botting/_types.py
+-rw-rw-rw-   0        0        0     1247 2023-07-12 16:09:02.000000 tg-botting-2.0/tg_botting/abstract.py
+-rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.0/tg_botting/bot.py
+-rw-rw-rw-   0        0        0    26953 2023-07-12 16:28:14.000000 tg-botting-2.0/tg_botting/client.py
+-rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.0/tg_botting/cog.py
+-rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.0/tg_botting/commands.py
+-rw-rw-rw-   0        0        0     7686 2023-07-12 16:20:46.000000 tg-botting-2.0/tg_botting/context.py
+-rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.0/tg_botting/context_managers.py
+-rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.0/tg_botting/conversions.py
+-rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.0/tg_botting/cooldowns.py
+-rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.0/tg_botting/exceptions.py
+-rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.0/tg_botting/general.py
+-rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.0/tg_botting/group.py
+-rw-rw-rw-   0        0        0    19102 2023-07-12 16:28:14.000000 tg-botting-2.0/tg_botting/message.py
+-rw-rw-rw-   0        0        0    29358 2023-07-12 16:28:14.000000 tg-botting-2.0/tg_botting/objects.py
+-rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.0/tg_botting/permissions.py
+-rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.0/tg_botting/user.py
+-rw-rw-rw-   0        0        0     1021 2023-07-12 15:20:00.000000 tg-botting-2.0/tg_botting/utils.py
+-rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.0/tg_botting/view.py
+drwxrwxrwx   0        0        0        0 2023-07-12 19:38:05.356078 tg-botting-2.0/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0     3405 2023-07-12 19:38:05.000000 tg-botting-2.0/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-07-12 19:38:05.000000 tg-botting-2.0/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 19:38:05.000000 tg-botting-2.0/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-12 19:38:05.000000 tg-botting-2.0/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-12 19:38:05.000000 tg-botting-2.0/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-1.6.2.7/tg_botting/generals.py` & `tg-botting-2.0/tg_botting/general.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 import aiohttp
 
-token = ''
-
-
-class RoleException(BaseException):
-    pass
-
 
 def convert_params(params):
     for param in list(params):
         if params[param] is None:
             params.pop(param)
         elif not isinstance(params[param], (str, int)):
             params[param] = str(params[param])
@@ -22,10 +16,9 @@
     params = convert_params(params)
     timeout = aiohttp.ClientTimeout(total=100, connect=10)
     async with aiohttp.ClientSession(timeout=timeout) as session:
         res = await session.post(url, data=params) if post else await session.get(url, params=params)
         return await res.json()
 
 
-async def tg_request(method, post=False, **kwargs):
-    return await general_request('https://api.telegram.org/bot{}/{}'.format(token, method), post=post,
-                                 **kwargs)
+async def tg_request(method, token, post=False, **kwargs):
+    return await general_request('https://api.telegram.org/bot{}/{}'.format(token,method), post=post, **kwargs)
```

