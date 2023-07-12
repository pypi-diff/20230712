# Comparing `tmp/quickstart_rhy-0.7.3.tar.gz` & `tmp/quickstart_rhy-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart_rhy-0.7.3.tar", max compression
+gzip compressed data, was "quickstart_rhy-0.7.4.tar", max compression
```

## Comparing `quickstart_rhy-0.7.3.tar` & `quickstart_rhy-0.7.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1067 2019-09-20 01:32:29.136250 quickstart_rhy-0.7.3/LICENSE
--rw-r--r--   0        0        0     5952 2023-02-05 05:20:04.108908 quickstart_rhy-0.7.3/QuickStart_Rhy/API/AliCloud.py
--rw-r--r--   0        0        0     3525 2023-03-27 00:35:40.568103 quickstart_rhy-0.7.3/QuickStart_Rhy/API/BaiduCloud.py
--rw-r--r--   0        0        0     4041 2023-05-18 09:09:18.744642 quickstart_rhy-0.7.3/QuickStart_Rhy/API/ChatGPT.py
--rw-r--r--   0        0        0      462 2023-02-24 04:34:17.917996 quickstart_rhy-0.7.3/QuickStart_Rhy/API/DeepL.py
--rw-r--r--   0        0        0     1221 2023-05-18 04:35:41.557810 quickstart_rhy-0.7.3/QuickStart_Rhy/API/DeepLX.py
--rw-r--r--   0        0        0     1191 2023-04-30 06:41:55.816233 quickstart_rhy-0.7.3/QuickStart_Rhy/API/Lolicon.py
--rw-r--r--   0        0        0     6264 2023-01-22 11:43:21.457920 quickstart_rhy-0.7.3/QuickStart_Rhy/API/QiniuOSS.py
--rw-r--r--   0        0        0     9434 2023-01-22 17:11:40.937202 quickstart_rhy-0.7.3/QuickStart_Rhy/API/SimpleAPI.py
--rw-r--r--   0        0        0     7276 2023-02-22 02:46:13.021767 quickstart_rhy-0.7.3/QuickStart_Rhy/API/TencentCloud.py
--rw-r--r--   0        0        0     1701 2023-03-04 05:55:10.455205 quickstart_rhy-0.7.3/QuickStart_Rhy/API/__init__.py
--rw-r--r--   0        0        0    16615 2023-02-22 02:45:56.238555 quickstart_rhy-0.7.3/QuickStart_Rhy/API/alapi.py
--rw-r--r--   0        0        0     2420 2023-01-16 11:59:57.162445 quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ColorTools.py
--rw-r--r--   0        0        0    13292 2023-04-18 12:58:33.288943 quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ImagePreview.py
--rw-r--r--   0        0        0     3805 2023-04-18 12:54:35.211459 quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ImageTools.py
--rw-r--r--   0        0        0     4035 2023-01-16 12:04:31.734545 quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/VideoTools.py
--rw-r--r--   0        0        0       75 2021-01-14 15:40:19.416041 quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/__init__.py
--rw-r--r--   0        0        0     1768 2022-11-18 20:23:12.379800 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/HttpServer.py
--rw-r--r--   0        0        0     5133 2023-01-22 12:27:25.009662 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/M3u8DL.py
--rw-r--r--   0        0        0     8878 2023-06-30 12:58:44.682083 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/MultiSingleDL.py
--rw-r--r--   0        0        0    14748 2023-04-04 03:26:04.977775 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/NormalDL.py
--rw-r--r--   0        0        0     3818 2022-11-18 20:23:25.282202 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/WiFi.py
--rw-r--r--   0        0        0     3227 2022-11-18 20:23:28.660759 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/WiFiDarwin.py
--rw-r--r--   0        0        0     6001 2023-02-16 12:56:59.801774 quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/__init__.py
--rw-r--r--   0        0        0     1075 2023-05-04 07:12:24.212283 quickstart_rhy-0.7.3/QuickStart_Rhy/NumbaTools/__init__.py
--rw-r--r--   0        0        0     8935 2023-01-16 13:31:49.562044 quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/Compress.py
--rw-r--r--   0        0        0     5145 2023-01-16 13:34:40.162030 quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/Diff.py
--rw-r--r--   0        0        0     1377 2022-11-18 19:05:09.495382 quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/DiskMac.py
--rw-r--r--   0        0        0     1130 2022-11-18 20:23:45.475865 quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/FileHash.py
--rw-r--r--   0        0        0      795 2023-01-29 05:36:58.386300 quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/__init__.py
--rw-r--r--   0        0        0     3255 2023-01-17 09:56:11.282076 quickstart_rhy-0.7.3/QuickStart_Rhy/ThreadTools/__init__.py
--rw-r--r--   0        0        0     1603 2023-04-22 06:36:51.515102 quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Bar.py
--rw-r--r--   0        0        0     1268 2022-11-18 20:24:15.189225 quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Line.py
--rw-r--r--   0        0        0     1753 2023-01-16 10:23:26.070865 quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Table.py
--rw-r--r--   0        0        0       18 2022-05-03 07:21:41.109725 quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/__init__.py
--rw-r--r--   0        0        0     3782 2023-01-22 07:37:58.889811 quickstart_rhy-0.7.3/QuickStart_Rhy/Wrapper/__init__.py
--rw-r--r--   0        0        0      772 2022-11-18 20:24:38.518900 quickstart_rhy-0.7.3/QuickStart_Rhy/__cache__.py
--rw-r--r--   0        0        0     8625 2023-05-04 11:46:15.495588 quickstart_rhy-0.7.3/QuickStart_Rhy/__config__.py
--rw-r--r--   0        0        0    14948 2023-05-04 11:44:40.865270 quickstart_rhy-0.7.3/QuickStart_Rhy/__init__.py
--rw-r--r--   0        0        0    38978 2023-05-15 09:52:32.288702 quickstart_rhy-0.7.3/QuickStart_Rhy/apiTools.py
--rw-r--r--   0        0        0     6720 2023-05-04 11:42:01.250240 quickstart_rhy-0.7.3/QuickStart_Rhy/funcList.py
--rw-r--r--   0        0        0     5844 2023-04-18 12:49:20.558808 quickstart_rhy-0.7.3/QuickStart_Rhy/imageDeal.py
--rw-r--r--   0        0        0    35036 2023-05-18 15:01:45.230103 quickstart_rhy-0.7.3/QuickStart_Rhy/lang.json
--rw-r--r--   0        0        0     1729 2023-05-18 14:59:51.881230 quickstart_rhy-0.7.3/QuickStart_Rhy/main.py
--rw-r--r--   0        0        0    11808 2023-05-04 08:04:12.459408 quickstart_rhy-0.7.3/QuickStart_Rhy/netTools.py
--rw-r--r--   0        0        0     1957 2023-01-22 12:33:43.387980 quickstart_rhy-0.7.3/QuickStart_Rhy/qsLesson.py
--rw-r--r--   0        0        0     6096 2023-03-16 03:09:08.732591 quickstart_rhy-0.7.3/QuickStart_Rhy/system.py
--rw-r--r--   0        0        0      701 2023-01-16 10:30:39.811901 quickstart_rhy-0.7.3/README.md
--rw-r--r--   0        0        0      548 2023-06-30 12:59:06.312351 quickstart_rhy-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.3/setup.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2019-09-20 01:32:29.136250 quickstart_rhy-0.7.4/LICENSE
+-rw-r--r--   0        0        0     5952 2023-02-05 05:20:04.108908 quickstart_rhy-0.7.4/QuickStart_Rhy/API/AliCloud.py
+-rw-r--r--   0        0        0     3525 2023-03-27 00:35:40.568103 quickstart_rhy-0.7.4/QuickStart_Rhy/API/BaiduCloud.py
+-rw-r--r--   0        0        0     4041 2023-05-18 09:09:18.744642 quickstart_rhy-0.7.4/QuickStart_Rhy/API/ChatGPT.py
+-rw-r--r--   0        0        0      462 2023-02-24 04:34:17.917996 quickstart_rhy-0.7.4/QuickStart_Rhy/API/DeepL.py
+-rw-r--r--   0        0        0     1221 2023-05-18 04:35:41.557810 quickstart_rhy-0.7.4/QuickStart_Rhy/API/DeepLX.py
+-rw-r--r--   0        0        0     1191 2023-04-30 06:41:55.816233 quickstart_rhy-0.7.4/QuickStart_Rhy/API/Lolicon.py
+-rw-r--r--   0        0        0     6264 2023-01-22 11:43:21.457920 quickstart_rhy-0.7.4/QuickStart_Rhy/API/QiniuOSS.py
+-rw-r--r--   0        0        0     9434 2023-01-22 17:11:40.937202 quickstart_rhy-0.7.4/QuickStart_Rhy/API/SimpleAPI.py
+-rw-r--r--   0        0        0     7276 2023-02-22 02:46:13.021767 quickstart_rhy-0.7.4/QuickStart_Rhy/API/TencentCloud.py
+-rw-r--r--   0        0        0     1701 2023-03-04 05:55:10.455205 quickstart_rhy-0.7.4/QuickStart_Rhy/API/__init__.py
+-rw-r--r--   0        0        0    15327 2023-07-12 06:46:26.939473 quickstart_rhy-0.7.4/QuickStart_Rhy/API/alapi.py
+-rw-r--r--   0        0        0     2420 2023-01-16 11:59:57.162445 quickstart_rhy-0.7.4/QuickStart_Rhy/ImageTools/ColorTools.py
+-rw-r--r--   0        0        0    13292 2023-04-18 12:58:33.288943 quickstart_rhy-0.7.4/QuickStart_Rhy/ImageTools/ImagePreview.py
+-rw-r--r--   0        0        0     3805 2023-04-18 12:54:35.211459 quickstart_rhy-0.7.4/QuickStart_Rhy/ImageTools/ImageTools.py
+-rw-r--r--   0        0        0     4035 2023-01-16 12:04:31.734545 quickstart_rhy-0.7.4/QuickStart_Rhy/ImageTools/VideoTools.py
+-rw-r--r--   0        0        0       75 2021-01-14 15:40:19.416041 quickstart_rhy-0.7.4/QuickStart_Rhy/ImageTools/__init__.py
+-rw-r--r--   0        0        0     1768 2022-11-18 20:23:12.379800 quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/HttpServer.py
+-rw-r--r--   0        0        0     5133 2023-01-22 12:27:25.009662 quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/M3u8DL.py
+-rw-r--r--   0        0        0     8885 2023-07-02 12:33:01.241267 quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/MultiSingleDL.py
+-rw-r--r--   0        0        0    14748 2023-04-04 03:26:04.977775 quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/NormalDL.py
+-rw-r--r--   0        0        0     3818 2022-11-18 20:23:25.282202 quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/WiFi.py
+-rw-r--r--   0        0        0     3227 2022-11-18 20:23:28.660759 quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/WiFiDarwin.py
+-rw-r--r--   0        0        0     6001 2023-02-16 12:56:59.801774 quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/__init__.py
+-rw-r--r--   0        0        0     1075 2023-05-04 07:12:24.212283 quickstart_rhy-0.7.4/QuickStart_Rhy/NumbaTools/__init__.py
+-rw-r--r--   0        0        0     8935 2023-01-16 13:31:49.562044 quickstart_rhy-0.7.4/QuickStart_Rhy/SystemTools/Compress.py
+-rw-r--r--   0        0        0     5145 2023-01-16 13:34:40.162030 quickstart_rhy-0.7.4/QuickStart_Rhy/SystemTools/Diff.py
+-rw-r--r--   0        0        0     1377 2022-11-18 19:05:09.495382 quickstart_rhy-0.7.4/QuickStart_Rhy/SystemTools/DiskMac.py
+-rw-r--r--   0        0        0     1130 2022-11-18 20:23:45.475865 quickstart_rhy-0.7.4/QuickStart_Rhy/SystemTools/FileHash.py
+-rw-r--r--   0        0        0      795 2023-01-29 05:36:58.386300 quickstart_rhy-0.7.4/QuickStart_Rhy/SystemTools/__init__.py
+-rw-r--r--   0        0        0     3255 2023-01-17 09:56:11.282076 quickstart_rhy-0.7.4/QuickStart_Rhy/ThreadTools/__init__.py
+-rw-r--r--   0        0        0     1603 2023-04-22 06:36:51.515102 quickstart_rhy-0.7.4/QuickStart_Rhy/TuiTools/Bar.py
+-rw-r--r--   0        0        0     1268 2022-11-18 20:24:15.189225 quickstart_rhy-0.7.4/QuickStart_Rhy/TuiTools/Line.py
+-rw-r--r--   0        0        0     1753 2023-01-16 10:23:26.070865 quickstart_rhy-0.7.4/QuickStart_Rhy/TuiTools/Table.py
+-rw-r--r--   0        0        0       18 2022-05-03 07:21:41.109725 quickstart_rhy-0.7.4/QuickStart_Rhy/TuiTools/__init__.py
+-rw-r--r--   0        0        0     3782 2023-01-22 07:37:58.889811 quickstart_rhy-0.7.4/QuickStart_Rhy/Wrapper/__init__.py
+-rw-r--r--   0        0        0      772 2022-11-18 20:24:38.518900 quickstart_rhy-0.7.4/QuickStart_Rhy/__cache__.py
+-rw-r--r--   0        0        0     8625 2023-05-04 11:46:15.495588 quickstart_rhy-0.7.4/QuickStart_Rhy/__config__.py
+-rw-r--r--   0        0        0    14948 2023-05-04 11:44:40.865270 quickstart_rhy-0.7.4/QuickStart_Rhy/__init__.py
+-rw-r--r--   0        0        0    38978 2023-05-15 09:52:32.288702 quickstart_rhy-0.7.4/QuickStart_Rhy/apiTools.py
+-rw-r--r--   0        0        0     6720 2023-05-04 11:42:01.250240 quickstart_rhy-0.7.4/QuickStart_Rhy/funcList.py
+-rw-r--r--   0        0        0     5844 2023-04-18 12:49:20.558808 quickstart_rhy-0.7.4/QuickStart_Rhy/imageDeal.py
+-rw-r--r--   0        0        0    35036 2023-05-18 15:01:45.230103 quickstart_rhy-0.7.4/QuickStart_Rhy/lang.json
+-rw-r--r--   0        0        0     1729 2023-05-18 14:59:51.881230 quickstart_rhy-0.7.4/QuickStart_Rhy/main.py
+-rw-r--r--   0        0        0    11808 2023-05-04 08:04:12.459408 quickstart_rhy-0.7.4/QuickStart_Rhy/netTools.py
+-rw-r--r--   0        0        0     1957 2023-01-22 12:33:43.387980 quickstart_rhy-0.7.4/QuickStart_Rhy/qsLesson.py
+-rw-r--r--   0        0        0     6096 2023-03-16 03:09:08.732591 quickstart_rhy-0.7.4/QuickStart_Rhy/system.py
+-rw-r--r--   0        0        0      701 2023-01-16 10:30:39.811901 quickstart_rhy-0.7.4/README.md
+-rw-r--r--   0        0        0      548 2023-07-12 06:46:56.068830 quickstart_rhy-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.4/setup.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 quickstart_rhy-0.7.4/PKG-INFO
```

### Comparing `quickstart_rhy-0.7.3/LICENSE` & `quickstart_rhy-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/API/AliCloud.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/API/AliCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/API/BaiduCloud.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/API/BaiduCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/API/ChatGPT.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/API/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/API/DeepLX.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/API/DeepLX.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/API/Lolicon.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/API/Lolicon.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/API/QiniuOSS.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/API/QiniuOSS.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/API/SimpleAPI.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/API/SimpleAPI.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/API/TencentCloud.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/API/TencentCloud.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/API/__init__.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/API/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/API/alapi.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/API/alapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
 from . import *
 from .. import user_currency
 import json
 from urllib.parse import quote
 import requests
 
-__common_token__ = "hUxPTdnybk1XLUEFtzkj"
+
 alapi_token = pre_check("alapi_token", ext=False)
 if not alapi_token:
     from .. import qs_default_console, qs_error_string, qs_warning_string, _ask
 
     qs_default_console.print(
         qs_error_string, "This function require alapi token!\n这个功能需要alapi token\n"
     )
@@ -34,47 +34,17 @@
             alapi_token = _ask(
                 {
                     "type": "input",
                     "message": "Input alapi token | 输入alapi token:",
                 }
             )
             qs_config.apiUpdate("alapi_token", alapi_token)
-    elif _ask(
-        {
-            "type": "confirm",
-            "message": "Use common but limited token?\n是否愿意使用公共但是受限的token?",
-            "default": True,
-        }
-    ):
-        alapi_token = __common_token__
-        qs_config.apiUpdate("alapi_token", alapi_token)
-        qs_default_console.print(
-            qs_warning_string,
-            "Tokens with restricted applications may not be able to use the functions provided by alapi normally, "
-            "and you can try again multiple times."
-            if user_lang != "zh"
-            else "应用受限的token可能无法正常使用alapi提供的功能，可多次重新尝试。",
-        )
     else:
         exit()
 
-if not pre_check("__ban_warning", ext=False) and alapi_token == __common_token__:
-    from .. import qs_default_console, qs_warning_string
-
-    qs_default_console.print(
-        qs_warning_string,
-        "Using common but limited token." if user_lang != "zh" else "正在使用公共但受限的token",
-    )
-    qs_default_console.print(
-        qs_warning_string,
-        "If you do not want this, try to apply one:"
-        if user_lang != "zh"
-        else "如果您不想这样, 可以来申请一个自己的:",
-        "https://www.alapi.cn/",
-    )
 
 v2_url = "https://v2.alapi.cn/api/"
 
 
 def translate(text: str, from_lang: str = "auto", target_lang: str = user_lang):
     """
     获取翻译结果
```

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ColorTools.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/ImageTools/ColorTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ImagePreview.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/ImageTools/ImagePreview.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/ImageTools.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/ImageTools/ImageTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/ImageTools/VideoTools.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/ImageTools/VideoTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/HttpServer.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/HttpServer.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/M3u8DL.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/M3u8DL.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/MultiSingleDL.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/MultiSingleDL.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self.headers = headers
         if referer:
             self.headers["Referer"] = referer
         self.rt_dir = rt_dir
         self.save_to_mem = save_to_mem
         self.status_dict = {}
         self.infos = {}
-        self.urls = urls
+        self.urls = urls.copy()
         self.task_num = len(self.urls)
         if self.save_to_mem:
             self.content_ls = [b""] * self.task_num
         self.cur_task_num = 0
         self.task_num_lock = Lock()
         self.max_retry = 3
         self.job_queue = queue.Queue()
```

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/NormalDL.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/NormalDL.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/WiFi.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/WiFi.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/WiFiDarwin.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/WiFiDarwin.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/NetTools/__init__.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/NetTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/NumbaTools/__init__.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/NumbaTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/Compress.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/SystemTools/Compress.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/Diff.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/SystemTools/Diff.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/DiskMac.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/SystemTools/DiskMac.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/FileHash.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/SystemTools/FileHash.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/SystemTools/__init__.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/SystemTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/ThreadTools/__init__.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/ThreadTools/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Bar.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/TuiTools/Bar.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Line.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/TuiTools/Line.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/TuiTools/Table.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/TuiTools/Table.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/Wrapper/__init__.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/Wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/__cache__.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/__cache__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/__config__.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/__config__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/__init__.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/apiTools.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/apiTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/funcList.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/funcList.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/imageDeal.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/imageDeal.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/lang.json` & `quickstart_rhy-0.7.4/QuickStart_Rhy/lang.json`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/main.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/main.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/netTools.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/netTools.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/qsLesson.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/qsLesson.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/QuickStart_Rhy/system.py` & `quickstart_rhy-0.7.4/QuickStart_Rhy/system.py`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/README.md` & `quickstart_rhy-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `quickstart_rhy-0.7.3/pyproject.toml` & `quickstart_rhy-0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QuickStart-Rhy"
-version = "0.7.3"
+version = "0.7.4"
 description = "A Command Line Toolbox"
 authors = ["Rhythmicc <rhythmlian.cn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "QuickStart_Rhy"}, {include = "QuickStart_Rhy/lang.json"}]
 
 [tool.poetry.dependencies]
```

### Comparing `quickstart_rhy-0.7.3/setup.py` & `quickstart_rhy-0.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'urllib3>=1.26.15,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['qs = QuickStart_Rhy.main:main']}
 
 setup_kwargs = {
     'name': 'quickstart-rhy',
-    'version': '0.7.3',
+    'version': '0.7.4',
     'description': 'A Command Line Toolbox',
     'long_description': '# QuickStart_Rhy\n\n```shell\npip3 install quickstart-rhy                                         # stable version\npip3 install git+https://github.com/Rhythmicc/quickstart-rhy.git -U # beta version but more features\n```\n\n| Key  | Value                                              |\n| :--: | -------------------------------------------------- |\n| ENV  | **^Python 3.7**                                    |\n| FONT | **Cascadia Code / Meslo**                          |\n| DOCS | <https://rhythmlian.cn/2020/02/14/QuickStart-Rhy/> |\n\n## Tab Complete\n\n1. fig\n\n   ```shell\n   npx @fig/publish-spec -p complete/fig/qs-<your language>.ts --name qs\n   ```\n\n2. zsh\n\n   ```shell\n   mv _qs /path/in/$FPATH/\n   ```\n',
     'author': 'Rhythmicc',
     'author_email': 'rhythmlian.cn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `quickstart_rhy-0.7.3/PKG-INFO` & `quickstart_rhy-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-rhy
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Command Line Toolbox
 License: MIT
 Author: Rhythmicc
 Author-email: rhythmlian.cn@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

