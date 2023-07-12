# Comparing `tmp/wcfhttp-37.1.25.5.tar.gz` & `tmp/wcfhttp-39.0.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcfhttp-37.1.25.5.tar", last modified: Sat May 20 15:15:52 2023, max compression
+gzip compressed data, was "wcfhttp-39.0.0.0a0.tar", last modified: Wed Jul 12 04:11:01 2023, max compression
```

## Comparing `wcfhttp-37.1.25.5.tar` & `wcfhttp-39.0.0.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 15:15:52.475955 wcfhttp-37.1.25.5/
--rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1829 2023-05-20 15:15:52.474955 wcfhttp-37.1.25.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-20 15:15:52.476955 wcfhttp-37.1.25.5/setup.cfg
--rw-rw-rw-   0        0        0     1422 2023-05-20 15:12:55.000000 wcfhttp-37.1.25.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 15:15:52.456955 wcfhttp-37.1.25.5/wcfhttp/
--rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.5/wcfhttp/__init__.py
--rw-rw-rw-   0        0        0    14500 2023-05-20 15:15:47.000000 wcfhttp-37.1.25.5/wcfhttp/core.py
--rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-37.1.25.5/wcfhttp/main.py
-drwxrwxrwx   0        0        0        0 2023-05-20 15:15:52.472955 wcfhttp-37.1.25.5/wcfhttp.egg-info/
--rw-rw-rw-   0        0        0     1829 2023-05-20 15:15:52.000000 wcfhttp-37.1.25.5/wcfhttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-20 15:15:52.000000 wcfhttp-37.1.25.5/wcfhttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 15:15:52.000000 wcfhttp-37.1.25.5/wcfhttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-20 15:15:52.000000 wcfhttp-37.1.25.5/wcfhttp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-20 15:15:52.000000 wcfhttp-37.1.25.5/wcfhttp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-20 15:15:52.000000 wcfhttp-37.1.25.5/wcfhttp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 04:11:01.322278 wcfhttp-39.0.0.0a0/
+-rw-rw-rw-   0        0        0       46 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1830 2023-07-12 04:11:01.306656 wcfhttp-39.0.0.0a0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-12 04:11:01.322278 wcfhttp-39.0.0.0a0/setup.cfg
+-rw-rw-rw-   0        0        0     1423 2023-07-12 03:00:09.000000 wcfhttp-39.0.0.0a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:11:01.306656 wcfhttp-39.0.0.0a0/wcfhttp/
+-rw-rw-rw-   0        0        0       69 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a0/wcfhttp/__init__.py
+-rw-rw-rw-   0        0        0    14705 2023-07-12 04:06:57.000000 wcfhttp-39.0.0.0a0/wcfhttp/core.py
+-rw-rw-rw-   0        0        0     1780 2023-05-08 03:47:03.000000 wcfhttp-39.0.0.0a0/wcfhttp/main.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:11:01.306656 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/
+-rw-rw-rw-   0        0        0     1830 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 04:11:01.000000 wcfhttp-39.0.0.0a0/wcfhttp.egg-info/top_level.txt
```

### Comparing `wcfhttp-37.1.25.5/PKG-INFO` & `wcfhttp-39.0.0.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 37.1.25.5
+Version: 39.0.0.0a0
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

### Comparing `wcfhttp-37.1.25.5/setup.py` & `wcfhttp-39.0.0.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             'wcfhttp=wcfhttp.main:main'
         ]
     },
     install_requires=[
         "setuptools",
         "fastapi",
         "uvicorn[standard]",
-        "wcferry==37.1.25.5",
+        "wcferry==39.0.0.0a2",
     ],
     classifiers=[
         "Environment :: Win32 (MS Windows)",
         "Intended Audience :: Developers",
         "Intended Audience :: Customer Service",
         "Topic :: Communications :: Chat",
         "Operating System :: Microsoft :: Windows",
```

### Comparing `wcfhttp-37.1.25.5/wcfhttp/core.py` & `wcfhttp-39.0.0.0a0/wcfhttp/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any
 
 import requests
 from fastapi import Body, FastAPI
 from pydantic import BaseModel
 from wcferry import Wcf, WxMsg
 
-__version__ = "37.1.25.5"
+__version__ = "39.0.0.0a0"
 
 
 class Msg(BaseModel):
     id: str
     type: int
     xml: str
     sender: str
@@ -46,16 +46,16 @@
         self.add_api_route("/friends", self.get_friends, methods=["GET"], summary="获取好友列表")
         self.add_api_route("/dbs", self.get_dbs, methods=["GET"], summary="获取所有数据库")
         self.add_api_route("/{db}/tables", self.get_tables, methods=["GET"], summary="获取 db 中所有表")
 
         self.add_api_route("/text", self.send_text, methods=["POST"], summary="发送文本消息")
         self.add_api_route("/image", self.send_image, methods=["POST"], summary="发送图片消息")
         self.add_api_route("/file", self.send_file, methods=["POST"], summary="发送文件消息")
-        self.add_api_route("/xml", self.send_xml, methods=["POST"], summary="发送 XML 消息")
-        self.add_api_route("/emotion", self.send_emotion, methods=["POST"], summary="发送表情消息")
+        # self.add_api_route("/xml", self.send_xml, methods=["POST"], summary="发送 XML 消息")
+        # self.add_api_route("/emotion", self.send_emotion, methods=["POST"], summary="发送表情消息")
         self.add_api_route("/sql", self.query_sql, methods=["POST"], summary="执行 SQL，如果数据量大注意分页，以免 OOM")
         self.add_api_route("/new-friend", self.accept_new_friend, methods=["POST"], summary="通过好友申请")
         self.add_api_route("/chatroom-member", self.add_chatroom_members, methods=["POST"], summary="添加群成员")
         self.add_api_route("/transfer", self.receive_transfer, methods=["POST"], summary="接收转账")
         self.add_api_route("/dec-image", self.decrypt_image, methods=["POST"], summary="解密图片")
 
     def _set_cb(self, cb):
@@ -289,25 +289,27 @@
             int: 1 为成功，其他失败
         """
         ret = self.wcf.add_chatroom_members(roomid, wxids)
         return {"status": ret, "message": "成功"if ret == 1 else "失败"}
 
     def receive_transfer(self,
                          wxid: str = Body("wxid_xxxxxxxxxxxxx", description="转账消息里的发送人 wxid"),
-                         transferid: str = Body("transferid", description="转账消息里的 transferid")) -> dict:
+                         transferid: str = Body("transferid", description="转账消息里的 transferid"),
+                         transactionid: str = Body("transactionid", description="转账消息里的 transactionid")) -> dict:
         """接收转账
 
         Args:
             wxid (str): 转账消息里的发送人 wxid
             transferid (str): 转账消息里的 transferid
+            transactionid (str): 转账消息里的 transactionid
 
         Returns:
             int: 1 为成功，其他失败
         """
-        ret = self.wcf.receive_transfer(wxid, transferid)
+        ret = self.wcf.receive_transfer(wxid, transferid, transactionid)
         return {"status": ret, "message": "成功"if ret == 1 else "失败"}
 
     def decrypt_image(self,
                       src: str = Body("C:\\...", description="加密的图片路径，从图片消息中获取"),
                       dst: str = Body("C:\\...", description="解密的图片路径")) -> dict:
         """解密图片:
```

### Comparing `wcfhttp-37.1.25.5/wcfhttp/main.py` & `wcfhttp-39.0.0.0a0/wcfhttp/main.py`

 * *Files identical despite different names*

### Comparing `wcfhttp-37.1.25.5/wcfhttp.egg-info/PKG-INFO` & `wcfhttp-39.0.0.0a0/wcfhttp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcfhttp
-Version: 37.1.25.5
+Version: 39.0.0.0a0
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
```

