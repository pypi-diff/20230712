# Comparing `tmp/villa-0.6.2.tar.gz` & `tmp/villa-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.6.2.tar", max compression
+gzip compressed data, was "villa-0.6.3.tar", max compression
```

## Comparing `villa-0.6.2.tar` & `villa-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1062 2023-07-05 01:35:03.201101 villa-0.6.2/LICENSE
--rw-r--r--   0        0        0     3428 2023-07-05 01:35:03.201101 villa-0.6.2/README.md
--rw-r--r--   0        0        0     1034 2023-07-05 01:35:03.201101 villa-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      323 2023-07-05 01:35:03.201101 villa-0.6.2/villa/__init__.py
--rw-r--r--   0        0        0    36853 2023-07-05 01:35:03.201101 villa-0.6.2/villa/bot.py
--rw-r--r--   0        0        0    11947 2023-07-05 01:35:03.201101 villa-0.6.2/villa/event.py
--rw-r--r--   0        0        0      728 2023-07-05 01:35:03.201101 villa-0.6.2/villa/exception.py
--rw-r--r--   0        0        0     3177 2023-07-05 01:35:03.201101 villa-0.6.2/villa/handle.py
--rw-r--r--   0        0        0     1524 2023-07-05 01:35:03.201101 villa-0.6.2/villa/log.py
--rw-r--r--   0        0        0    21270 2023-07-05 01:35:03.201101 villa-0.6.2/villa/message.py
--rw-r--r--   0        0        0     9352 2023-07-05 01:35:03.205101 villa-0.6.2/villa/models.py
--rw-r--r--   0        0        0      935 2023-07-05 01:35:03.205101 villa-0.6.2/villa/store.py
--rw-r--r--   0        0        0      240 2023-07-05 01:35:03.205101 villa-0.6.2/villa/typing.py
--rw-r--r--   0        0        0      995 2023-07-05 01:35:03.205101 villa-0.6.2/villa/utils.py
--rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 villa-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-12 12:19:47.928516 villa-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3617 2023-07-12 12:19:47.928516 villa-0.6.3/README.md
+-rw-r--r--   0        0        0     2127 2023-07-12 12:19:47.928516 villa-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      277 2023-07-12 12:19:47.928516 villa-0.6.3/villa/__init__.py
+-rw-r--r--   0        0        0    37466 2023-07-12 12:19:47.928516 villa-0.6.3/villa/bot.py
+-rw-r--r--   0        0        0    12215 2023-07-12 12:19:47.928516 villa-0.6.3/villa/event.py
+-rw-r--r--   0        0        0      728 2023-07-12 12:19:47.928516 villa-0.6.3/villa/exception.py
+-rw-r--r--   0        0        0     3337 2023-07-12 12:19:47.928516 villa-0.6.3/villa/handle.py
+-rw-r--r--   0        0        0     1537 2023-07-12 12:19:47.928516 villa-0.6.3/villa/log.py
+-rw-r--r--   0        0        0    21359 2023-07-12 12:19:47.932516 villa-0.6.3/villa/message.py
+-rw-r--r--   0        0        0     9304 2023-07-12 12:19:47.932516 villa-0.6.3/villa/models.py
+-rw-r--r--   0        0        0      935 2023-07-12 12:19:47.932516 villa-0.6.3/villa/store.py
+-rw-r--r--   0        0        0      240 2023-07-12 12:19:47.932516 villa-0.6.3/villa/typing.py
+-rw-r--r--   0        0        0      968 2023-07-12 12:19:47.932516 villa-0.6.3/villa/utils.py
+-rw-r--r--   0        0        0     4569 1970-01-01 00:00:00.000000 villa-0.6.3/PKG-INFO
```

### Comparing `villa-0.6.2/LICENSE` & `villa-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.6.2/README.md` & `villa-0.6.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
 <a href="https://pypi.python.org/pypi/villa">
   <img src="https://img.shields.io/pypi/dm/villa" alt="pypi download">
 </a>
 <a href="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/d3b88a99-17c2-4c98-bbc2-c1949ce7c078">
   <img src="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/d3b88a99-17c2-4c98-bbc2-c1949ce7c078.svg" alt="wakatime">
 </a>
+<a href="https://github.com/astral-sh/ruff">
+  <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="ruff">
+</a>
 
 </div>
 
 ## 特性
 
 - 基于`FastAPI`和`Pydantic`，异步优先、快速、高性能！
 - 完整的类型注解支持，便于开发。
@@ -69,14 +72,14 @@
 
 ## 交流、建议和反馈
 
 > 注意：本SDK并非官方SDK
 
 大别野 Bot 和本 SDK 均为开发测试中，如遇问题请提出 [issue](https://github.com/CMHopeSunshine/villa-py/issues) ，感谢支持！
 
-也欢迎来我的大别野[「尘世闲游」]((https://dby.miyoushe.com/chat/1047/21652))(ID: `wgiJNaU`)进行交流~ 
+也欢迎来我的大别野[「尘世闲游」]((https://dby.miyoushe.com/chat/1047/21652))(ID: `wgiJNaU`)进行交流~
 
 ## 相关项目
 
 - [NoneBot2](https://github.com/nonebot/nonebot2) 非常好用的 Python 跨平台机器人框架！
 - [nonebot-adapter-villa](https://github.com/CMHopeSunshine/nonebot-adapter-villa) NoneBot2 的大别野 Bot 适配器。
 - [Herta-villa-SDK](https://github.com/MingxuanGame/Herta-villa-SDK) 另一个大别野 Python SDK。
```

### Comparing `villa-0.6.2/villa/bot.py` & `villa-0.6.3/villa/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-import re
 import asyncio
+from collections import defaultdict
 from itertools import product
+import re
+from typing import Any, DefaultDict, Dict, List, Literal, Optional, Set, Type, Union
 from urllib.parse import urlparse
-from collections import defaultdict
-from typing import Any, Set, Dict, List, Type, Union, Literal, Optional, DefaultDict
-
-import httpx
-import uvicorn
-from pydantic import parse_obj_as
-from httpx._types import TimeoutTypes
-from fastapi.responses import JSONResponse
-from fastapi import FastAPI, BackgroundTasks
 
-from .models import *
-from .message import Message
-from .utils import escape_tag
+from .event import Event, event_classes, pre_handle_event, SendMessageEvent
+from .exception import ActionFailed, StopPropagation
 from .handle import EventHandler
-from .message import MessageSegment
-from .log import logger, _log_patcher
-from .typing import T_Func, T_Handler
-from .message import Link as LinkSegment
-from .message import Text as TextSegment
-from .message import Image as ImageSegment
+from .log import _log_patcher, logger
+from .message import (
+    Image as ImageSegment,
+    Link as LinkSegment,
+    MentionAll as MentionAllSegment,
+    MentionRobot as MentionRobotSegment,
+    MentionUser as MentionUserSegment,
+    Message,
+    MessageSegment,
+    RoomLink as RoomLinkSegment,
+    Text as TextSegment,
+)
+from .models import *
 from .store import get_app, get_bot, store_bot
-from .message import RoomLink as RoomLinkSegment
-from .exception import ActionFailed, StopPropagation
-from .message import MentionAll as MentionAllSegment
-from .message import MentionUser as MentionUserSegment
-from .message import MentionRobot as MentionRobotSegment
-from .event import Event, SendMessageEvent, event_classes, pre_handle_event
+from .typing import T_Func, T_Handler
+from .utils import escape_tag
+
+from fastapi import BackgroundTasks, FastAPI
+from fastapi.responses import JSONResponse
+import httpx
+from httpx._types import TimeoutTypes
+from pydantic import parse_obj_as
+import uvicorn
 
 
 class Bot:
     """Villa Bot"""
 
     _event_handlers: DefaultDict[int, List[EventHandler]] = defaultdict(list)
     """事件处理函数"""
@@ -106,31 +108,37 @@
     def current_villa_id(self) -> int:
         """Bot 最后收到的事件的大别野 ID"""
         if self._bot_info is None:
             raise ValueError(f"Bot {self.bot_id} not connected")
         return self._bot_info.villa_id
 
     def on_event(
-        self, *event_type: Type[Event], block: bool = False, priority: int = 1
+        self,
+        *event_type: Type[Event],
+        block: bool = False,
+        priority: int = 1,
     ):
         """注册一个事件处理函数
 
         当事件属于 event_type 中的任意一个时，执行处理函数。
 
         参数:
             *event_type: 事件类型列表.
             block: 是否阻止更低优先级的处理函数执行. 默认为 False.
             priority: 优先级. 默认为 1.
         """
 
         def _decorator(func: T_Handler) -> T_Handler:
             self._event_handlers[priority].append(
                 EventHandler(
-                    event_type=event_type, func=func, block=block, priority=priority
-                )
+                    event_type=event_type,
+                    func=func,
+                    block=block,
+                    priority=priority,
+                ),
             )
             return func
 
         return _decorator
 
     def on_message(self, block: bool = False, priority: int = 1):
         """注册一个消息事件处理函数
@@ -145,59 +153,61 @@
         def _decorator(func: T_Handler) -> T_Handler:
             self._event_handlers[priority].append(
                 EventHandler(
                     event_type=(SendMessageEvent,),
                     func=func,
                     block=block,
                     priority=priority,
-                )
+                ),
             )
             return func
 
         return _decorator
 
     def on_startswith(
         self,
         *startswith: str,
-        prefix: Union[str, Set[str]] = set(""),
+        prefix: Union[str, Set[str], None] = None,
         block: bool = False,
         priority: int = 1,
     ):
         """注册一个消息事件处理函数
 
-        当事件属于 SendMessageEvent 消息事件且纯文本部分以指定字符串开头时，执行处理函数。
+        当事件属于 SendMessageEvent 消息事件且纯文本部分以指定字符串开头时，执行处理函数
 
         参数:
             *startswith: 字符串列表.
             prefix: 字符串前缀. 可以是字符串或字符串集合. 默认为 "".
             block: 是否阻止更低优先级的处理函数执行. 默认为 False.
             priority: 优先级. 默认为 1.
         """
+        if prefix is None:
+            prefix = {""}
         if isinstance(prefix, str):
             prefix = {prefix}
-        startswith = tuple(set(p + s for p, s in list(product(prefix, startswith))))
+        startswith = tuple({p + s for p, s in list(product(prefix, startswith))})
 
         def _decorator(func: T_Handler) -> T_Handler:
             self._event_handlers[priority].append(
                 EventHandler(
                     event_type=(SendMessageEvent,),
                     func=func,
                     block=block,
                     priority=priority,
                     startswith=startswith or None,
-                )
+                ),
             )
             return func
 
         return _decorator
 
     def on_endswith(self, *endswith: str, block: bool = False, priority: int = 1):
         """注册一个消息事件处理函数
 
-        当事件属于 SendMessageEvent 消息事件且纯文本部分以指定字符串结尾时，执行处理函数。
+        当事件属于 SendMessageEvent 消息事件且纯文本部分以指定字符串结尾时，执行处理函数
 
         参数:
             *endswith: 字符串列表.
             block: 是否阻止更低优先级的处理函数执行. 默认为 False.
             priority: 优先级. 默认为 1.
         """
 
@@ -205,15 +215,15 @@
             self._event_handlers[priority].append(
                 EventHandler(
                     event_type=(SendMessageEvent,),
                     func=func,
                     block=block,
                     priority=priority,
                     endswith=endswith or None,
-                )
+                ),
             )
             return func
 
         return _decorator
 
     def on_keyword(self, *keywords: str, block: bool = False, priority: int = 1):
         """注册一个消息事件处理函数
@@ -230,26 +240,29 @@
             self._event_handlers[priority].append(
                 EventHandler(
                     event_type=(SendMessageEvent,),
                     func=func,
                     block=block,
                     priority=priority,
                     keywords=keywords or None,
-                )
+                ),
             )
             return func
 
         return _decorator
 
     def on_regex(
-        self, pattern: Union[str, re.Pattern], block: bool = False, priority: int = 1
+        self,
+        pattern: Union[str, re.Pattern],
+        block: bool = False,
+        priority: int = 1,
     ):
         """注册一个消息事件处理函数
 
-        当事件属于 SendMessageEvent 消息事件且纯文本部分与正则表达式匹配时，执行处理函数。
+        当事件属于 SendMessageEvent 消息事件且纯文本部分与正则表达式匹配时，执行处理函数
 
         参数:
             pattern: 正则表达式.
             block: 是否阻止更低优先级的处理函数执行. 默认为 False.
             priority: 优先级. 默认为 1.
         """
         if isinstance(pattern, str):
@@ -259,22 +272,25 @@
             self._event_handlers[priority].append(
                 EventHandler(
                     event_type=(SendMessageEvent,),
                     func=func,
                     block=block,
                     priority=priority,
                     regex=pattern,
-                )
+                ),
             )
             return func
 
         return _decorator
 
     async def send(
-        self, villa_id: int, room_id: int, message: Union[str, Message, MessageSegment]
+        self,
+        villa_id: int,
+        room_id: int,
+        message: Union[str, Message, MessageSegment],
     ) -> str:
         """发送消息
 
         参数:
             villa_id: 大别野 ID
             room_id: 房间 ID
             message: 消息内容
@@ -297,15 +313,17 @@
             villa_id=villa_id,
             room_id=room_id,
             object_name=object_name,
             msg_content=content_info.json(by_alias=True, exclude_none=True),
         )
 
     async def check_member_bot_access_token(
-        self, token: str, villa_id: Optional[int] = None
+        self,
+        token: str,
+        villa_id: Optional[int] = None,
     ) -> CheckMemberBotAccessTokenReturn:
         """校验用户机器人访问凭证，并返回用户信息
 
         参数:
             token: 用户机器人访问凭证
             villa_id: 大别野 ID. 默认为 None.
 
@@ -314,28 +332,28 @@
         """
         return CheckMemberBotAccessTokenReturn.parse_obj(
             await self._request(
                 "GET",
                 "checkMemberBotAccessToken",
                 villa_id,
                 json={"token": token},
-            )
+            ),
         )
 
     async def get_villa(self, villa_id: int) -> Villa:
         """获取大别野信息
 
         参数:
             villa_id: 大别野 ID
 
         返回:
             Villa: 大别野信息
         """
         return Villa.parse_obj(
-            (await self._request("GET", "getVilla", villa_id, json={}))["villa"]
+            (await self._request("GET", "getVilla", villa_id, json={}))["villa"],
         )
 
     async def get_member(self, villa_id: int, uid: int) -> Member:
         """获取用户信息
 
         参数:
             villa_id: 大别野
@@ -348,19 +366,22 @@
             (
                 await self._request(
                     "GET",
                     "getMember",
                     villa_id,
                     json={"uid": uid},
                 )
-            )["member"]
+            )["member"],
         )
 
     async def get_villa_members(
-        self, villa_id: int, offset: int, size: int
+        self,
+        villa_id: int,
+        offset: int,
+        size: int,
     ) -> MemberListReturn:
         """获取大别野成员列表
 
         参数:
             villa_id: 大别野 ID
             offset: 偏移量
             size: 分页大小
@@ -370,15 +391,15 @@
         """
         return MemberListReturn.parse_obj(
             await self._request(
                 "GET",
                 "getVillaMembers",
                 villa_id,
                 json={"offset": offset, "size": size},
-            )
+            ),
         )
 
     async def delete_villa_member(self, villa_id: int, uid: int) -> None:
         """踢出大别野用户
 
         参数:
             villa_id: 大别野 ID
@@ -388,15 +409,20 @@
             "POST",
             "deleteVillaMember",
             villa_id,
             json={"uid": uid},
         )
 
     async def pin_message(
-        self, villa_id: int, msg_uid: str, is_cancel: bool, room_id: int, send_at: int
+        self,
+        villa_id: int,
+        msg_uid: str,
+        is_cancel: bool,
+        room_id: int,
+        send_at: int,
     ) -> None:
         """置顶消息
 
         参数:
             villa_id: 大别野 ID
             msg_uid: 消息 ID
             is_cancel: 是否取消置顶
@@ -412,15 +438,19 @@
                 "is_cancel": is_cancel,
                 "room_id": room_id,
                 "send_at": send_at,
             },
         )
 
     async def recall_message(
-        self, villa_id: int, msg_uid: str, room_id: int, msg_time: int
+        self,
+        villa_id: int,
+        msg_uid: str,
+        room_id: int,
+        msg_time: int,
     ) -> None:
         """撤回消息
 
         参数:
             villa_id: 大别野 ID
             msg_uid: 消息 ID
             room_id: 房间 ID
@@ -589,35 +619,36 @@
             (
                 await self._request(
                     "GET",
                     "getRoom",
                     villa_id,
                     json={"room_id": room_id},
                 )
-            )["room"]
+            )["room"],
         )
 
-    async def get_villa_group_room_list(self, villa_id: int) -> GroupRoom:
+    async def get_villa_group_room_list(self, villa_id: int) -> List[GroupRoom]:
         """获取房间列表信息
 
         参数:
             villa_id: 大别野 ID
 
         返回:
             GroupRoom: 房间列表
         """
-        return GroupRoom.parse_obj(
+        return parse_obj_as(
+            List[GroupRoom],
             (
                 await self._request(
                     "GET",
                     "getVillaGroupRoomList",
                     villa_id,
                     json={},
                 )
-            )["list"]
+            )["list"],
         )
 
     async def sort_room_list(self, villa_id: int, room_list: List[RoomSort]) -> None:
         """房间列表排序
 
         参数:
             villa_id: 大别野 ID
@@ -630,15 +661,19 @@
             json={
                 "villa_id": villa_id,
                 "room_list": [room.dict() for room in room_list],
             },
         )
 
     async def operate_member_to_role(
-        self, villa_id: int, role_id: int, uid: int, is_add: bool
+        self,
+        villa_id: int,
+        role_id: int,
+        uid: int,
+        is_add: bool,
     ) -> None:
         """向身份组操作用户
 
         参数:
             villa_id: 大别野 ID
             role_id: 身份组 ID
             uid: 用户 ID
@@ -648,15 +683,19 @@
             "POST",
             "operateMemberToRole",
             villa_id,
             json={"role_id": role_id, "uid": uid, "is_add": is_add},
         )
 
     async def create_member_role(
-        self, villa_id: int, name: str, color: Color, permissions: List[Permission]
+        self,
+        villa_id: int,
+        name: str,
+        color: Color,
+        permissions: List[Permission],
     ) -> int:
         """创建身份组
 
         参数:
             villa_id: 大别野 ID
             name: 身份组名称
             color: 身份组颜色
@@ -714,15 +753,17 @@
             "POST",
             "deleteMemberRole",
             villa_id,
             json={"id": role_id},
         )
 
     async def get_member_role_info(
-        self, villa_id: int, role_id: int
+        self,
+        villa_id: int,
+        role_id: int,
     ) -> MemberRoleDetail:
         """获取身份组
 
         参数:
             villa_id: 大别野 ID
             role_id: 身份组 ID
 
@@ -733,15 +774,15 @@
             (
                 await self._request(
                     "GET",
                     "getMemberRoleInfo",
                     villa_id,
                     json={"role_id": role_id},
                 )
-            )["role"]
+            )["role"],
         )
 
     async def get_villa_member_roles(self, villa_id: int) -> List[MemberRoleDetail]:
         """获取大别野下所有身份组
 
         参数:
             villa_id: 大别野 ID
@@ -853,29 +894,28 @@
             ActionFailed: 动作失败
             e: 其他请求异常
 
         返回:
             Any: 返回结果
         """
         logger.opt(colors=True).debug(
-            f"<b><m>{self.bot_id}</m></b> | Calling API <y>{api}</y>"
+            f"<b><m>{self.bot_id}</m></b> | Calling API <y>{api}</y>",
         )
         try:
             resp = await self._client.request(
                 method=method,
                 url=api,
                 headers=self._get_headers(villa_id),
                 json=json,
                 **kwargs,
             )
             resp = ApiResponse.parse_raw(resp.content)
             if resp.retcode == 0:
                 return resp.data
-            else:
-                raise ActionFailed(resp.retcode, resp)
+            raise ActionFailed(resp.retcode, resp)
         except Exception as e:
             raise e
 
     async def _close_client(self) -> None:
         """关闭 HTTP Client"""
         await self._client.aclose()
 
@@ -885,25 +925,28 @@
         参数:
             event: 事件
         """
         is_handled = False
         for priority in sorted(self._event_handlers.keys()):
             try:
                 await asyncio.gather(
-                    *[handler._run(event) for handler in self._event_handlers[priority]]
+                    *[
+                        handler._run(event)
+                        for handler in self._event_handlers[priority]
+                    ],
                 )
                 is_handled = True
             except StopPropagation as e:
                 logger.opt(colors=True).debug(
-                    f"<b><y>[{event.__class__.__name__}]</y></b> stop handled by <y>{e.handler}</y>"
+                    f"{event.get_event_name()} stop handled by <y>{e.handler}</y>",
                 )
                 break
         if is_handled:
             logger.opt(colors=True).success(
-                f"{event.get_event_name()} handle completed"
+                f"{event.get_event_name()} handle completed",
             )
 
     async def _parse_message_content(self, message: Message) -> MessageContentInfo:
         """解析消息内容"""
         if quote := message["quote", 0]:
             quote = QuoteInfo(**quote.dict())
 
@@ -925,15 +968,18 @@
                     else None,
                     file_size=seg.file_size,
                 )
                 for seg in images_msg
             ]
         else:
             images = None
-        cal_len = lambda x: len(x.encode("utf-16")) // 2 - 1
+
+        def cal_len(x):
+            return len(x.encode("utf-16")) // 2 - 1
+
         message_text = ""
         message_offset = 0
         entities: List[TextEntity] = []
         mentioned = MentionedInfo(type=MentionType.PART)
         for seg in message:  # type: ignore
             try:
                 if seg.type in ("quote", "image", "post", "preview_link", "badge"):
@@ -945,84 +991,87 @@
                     seg_text = f"@{seg.show_text} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
                             entity=MentionedAll(show_text=seg.show_text),
-                        )
+                        ),
                     )
                     mentioned.type = MentionType.ALL
                 elif isinstance(seg, MentionRobotSegment):
                     seg_text = f"@{seg.bot_name} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
                             entity=MentionedRobot(
-                                bot_id=seg.bot_id, bot_name=seg.bot_name
+                                bot_id=seg.bot_id,
+                                bot_name=seg.bot_name,
                             ),
-                        )
+                        ),
                     )
                     mentioned.user_id_list.append(seg.bot_id)
                 elif isinstance(seg, MentionUserSegment):
                     # 需要调用API获取被@的用户的昵称
                     if not seg.user_name and seg.villa_id:
                         user = await self.get_member(
-                            villa_id=seg.villa_id, uid=seg.user_id
+                            villa_id=seg.villa_id,
+                            uid=seg.user_id,
                         )
                         seg_text = f"@{user.basic.nickname} "
                         seg.user_name = user.basic.nickname
                     else:
                         seg_text = f"@{seg.user_name} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
                             entity=MentionedUser(
                                 user_id=str(seg.user_id),
                                 user_name=seg.user_name,  # type: ignore
                             ),
-                        )
+                        ),
                     )
                     mentioned.user_id_list.append(str(seg.user_id))
                 elif isinstance(seg, RoomLinkSegment):
                     # 需要调用API获取房间的名称
                     room = await self.get_room(
-                        villa_id=seg.villa_id, room_id=seg.room_id
+                        villa_id=seg.villa_id,
+                        room_id=seg.room_id,
                     )
                     seg_text = f"#{room.room_name} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
                             entity=VillaRoomLink(
                                 villa_id=str(seg.villa_id),
                                 room_id=str(seg.room_id),
                                 room_name=room.room_name,
                             ),
-                        )
+                        ),
                     )
                 else:
                     seg: LinkSegment
                     seg_text = seg.show_text
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
                             entity=Link(
                                 url=seg.url,
                                 show_text=seg.show_text,
                                 requires_bot_access_token=seg.requires_bot_access_token,
                             ),
-                        )
+                        ),
                     )
                 message_offset += length
                 message_text += seg_text
             except Exception as e:
                 logger.opt(exception=e).warning("error when parse message content")
 
         if not (mentioned.type == MentionType.ALL and mentioned.user_id_list):
@@ -1037,15 +1086,17 @@
                         preview_link=preview_link,
                         badge=badge,
                     )
                 else:
                     content = ImageMessageContent(**images[0].dict())
             elif preview_link:
                 content = TextMessageContent(
-                    text="\u200B", preview_link=preview_link, badge=badge
+                    text="\u200B",
+                    preview_link=preview_link,
+                    badge=badge,
                 )
             elif post:
                 content = PostMessageContent(post_id=post.post_id)
             else:
                 raise ValueError("message content is empty")
         else:
             content = TextMessageContent(
@@ -1058,21 +1109,22 @@
 
         return MessageContentInfo(content=content, mentionedInfo=mentioned, quote=quote)
 
     def init_app(self, app: FastAPI):
         if self.callback_endpoint is not None:
             logger.opt(colors=True).info(f"Initializing Bot <m>{self.bot_id}</m>...")
             logger.opt(colors=True).debug(
-                f"With Secret: <m>{self.bot_secret}</m> and Callback Endpoint: <m>{self.callback_endpoint}</m>"
+                f"With Secret: <m>{self.bot_secret}</m> "
+                f"and Callback Endpoint: <m>{self.callback_endpoint}</m>",
             )
             app.post(self.callback_endpoint, status_code=200)(handle_event)
             app.on_event("shutdown")(self._close_client)
         else:
             logger.opt(colors=True).warning(
-                f"Bot <m>{self.bot_id}</m> missing callback url endpoint."
+                f"Bot <m>{self.bot_id}</m> missing callback url endpoint.",
             )
 
     def run(
         self,
         host: str = "127.0.0.1",
         port: int = 13350,
         log_level: str = "INFO",
@@ -1137,36 +1189,43 @@
             },
         },
         **uvicorn_kwargs,
     )
 
 
 async def handle_event(
-    data: Dict[str, Any], backgroud_tasks: BackgroundTasks
+    data: Dict[str, Any],
+    backgroud_tasks: BackgroundTasks,
 ) -> JSONResponse:
     """处理事件"""
     if not (payload_data := data.get("event", None)):
         logger.warning(f"Received invalid data: {escape_tag(str(data))}")
         return JSONResponse(
-            status_code=400, content={"retcode": -1, "msg": "Invalid data"}
+            status_code=400,
+            content={"retcode": -1, "msg": "Invalid data"},
         )
     try:
         event = parse_obj_as(event_classes, pre_handle_event(payload_data))
         if (bot := get_bot(event.bot_id)) is None:
             raise ValueError(f"Bot {event.bot_id} not found")
         bot._bot_info = event.robot
         logger.opt(colors=True).success(
-            f"<b><m>{bot.bot_id}</m></b> | <b><y>[{event.__class__.__name__}]</y></b>: {event.get_event_description()}"
+            (
+                f"<b><m>{bot.bot_id}</m></b>"
+                f" | <b><y>[{event.__class__.__name__}]</y></b>: "
+                f"{event.get_event_description()}",
+            ),
         )
     except Exception as e:
         logger.opt(exception=e).warning(
-            f"Failed to parse payload {escape_tag(str(payload_data))}"
+            f"Failed to parse payload {escape_tag(str(payload_data))}",
         )
         return JSONResponse(
-            status_code=400, content={"retcode": -1, "msg": "Invalid data"}
+            status_code=400,
+            content={"retcode": -1, "msg": "Invalid data"},
         )
     else:
         if bot.wait_util_complete:
             await bot._handle_event(event=event)
         else:
             backgroud_tasks.add_task(bot._handle_event, event=event)
     return JSONResponse(status_code=200, content={"retcode": 0, "message": "success"})
```

### Comparing `villa-0.6.2/villa/event.py` & `villa-0.6.3/villa/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import json
 from enum import IntEnum
-from typing import Any, Dict, Union, Literal, Optional
-
-from pydantic import BaseModel, root_validator
+import json
+from typing import Any, Dict, Literal, Optional, Union
 
+from .message import Message, MessageSegment
+from .models import MessageContentInfoGet, Robot
 from .store import get_bot
 from .utils import escape_tag
-from .message import Message, MessageSegment
-from .models import Robot, MessageContentInfoGet
+
+from pydantic import BaseModel, root_validator
 
 
 class EventType(IntEnum):
     """事件类型"""
 
     JoinVilla = 1
     SendMessage = 2
@@ -74,15 +74,16 @@
     @property
     def villa_id(self) -> int:
         """大别野ID"""
         return self.robot.villa_id
 
     def get_event_description(self) -> str:
         return escape_tag(
-            f"User(nickname={self.join_user_nickname},id={self.join_uid}) join Villa(id={self.villa_id})"
+            f"User(nickname={self.join_user_nickname},"
+            f"id={self.join_uid}) join Villa(id={self.villa_id})",
         )
 
 
 class SendMessageEvent(Event):
     """用户@机器人发送消息事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html###SendMessage"""
@@ -111,30 +112,33 @@
     @property
     def villa_id(self) -> int:
         """大别野ID"""
         return self.robot.villa_id
 
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Message(id={self.msg_uid}) was sent from User(nickname={self.nickname},id={self.from_user_id}) in Room(id={self.room_id}) of Villa(id={self.villa_id}), content={repr(self.message)}"
+            f"Message(id={self.msg_uid}) was sent from User(nickname={self.nickname},"
+            f"id={self.from_user_id}) in Room(id={self.room_id}) of "
+            f"Villa(id={self.villa_id}), content={repr(self.message)}",
         )
 
     @root_validator(pre=True)
+    @classmethod
     def _(cls, data: Dict[str, Any]):
         if not data.get("content"):
             return data
         msg = Message()
         data["content"] = json.loads(data["content"])
         msg_content_info = data["content"]
         if quote := msg_content_info.get("quote"):
             msg.append(
                 MessageSegment.quote(
                     message_id=quote["quoted_message_id"],
                     message_send_time=quote["quoted_message_send_time"],
-                )
+                ),
             )
 
         content = msg_content_info["content"]
         text = content["text"]
         entities = content["entities"]
         if not entities:
             return Message(MessageSegment.plain_text(text))
@@ -146,45 +150,47 @@
             offset: int = entity["offset"]
             length: int = entity["length"]
             entity_detail = entity["entity"]
             if offset != end_offset:
                 msg.append(
                     MessageSegment.plain_text(
                         text[((end_offset + 1) * 2) : ((offset + 1) * 2)].decode(
-                            "utf-16"
-                        )
-                    )
+                            "utf-16",
+                        ),
+                    ),
                 )
             entity_text = text[(offset + 1) * 2 : (offset + length + 1) * 2].decode(
-                "utf-16"
+                "utf-16",
             )
             if entity_detail["type"] == "mentioned_robot":
                 entity_detail["bot_name"] = entity_text.lstrip("@")[:-1]
                 msg.append(
                     MessageSegment.mention_robot(
-                        entity_detail["bot_id"], entity_detail["bot_name"]
-                    )
+                        entity_detail["bot_id"],
+                        entity_detail["bot_name"],
+                    ),
                 )
             elif entity_detail["type"] == "mentioned_user":
                 entity_detail["user_name"] = entity_text.lstrip("@")[:-1]
                 msg.append(
                     MessageSegment.mention_user(
-                        int(entity_detail["user_id"]), data["villa_id"]
-                    )
+                        int(entity_detail["user_id"]),
+                        data["villa_id"],
+                    ),
                 )
             elif entity_detail["type"] == "mention_all":
                 entity_detail["show_text"] = entity_text.lstrip("@")[:-1]
                 msg.append(MessageSegment.mention_all(entity_detail["show_text"]))
             elif entity_detail["type"] == "villa_room_link":
                 entity_detail["room_name"] = entity_text.lstrip("#")[:-1]
                 msg.append(
                     MessageSegment.room_link(
                         int(entity_detail["villa_id"]),
                         int(entity_detail["room_id"]),
-                    )
+                    ),
                 )
             else:
                 entity_detail["show_text"] = entity_text
                 msg.append(MessageSegment.link(entity_detail["url"], entity_text))
             last_offset = offset
             last_length = length
         end_offset = last_offset + last_length
@@ -216,15 +222,17 @@
             raise ValueError(f"Bot {self.bot_id} not found. Cannot send message.")
         if isinstance(message, (str, MessageSegment)):
             message = Message(message)
         if mention_sender:
             message.insert(
                 0,
                 MessageSegment.mention_user(
-                    self.from_user_id, self.content.user.name, self.villa_id
+                    self.from_user_id,
+                    self.content.user.name,
+                    self.villa_id,
                 ),
             )
         if quote_message:
             message.append(MessageSegment.quote(self.msg_uid, self.send_at))
         return await bot.send(self.villa_id, self.room_id, message)
 
 
@@ -235,30 +243,30 @@
 
     type: Literal[EventType.CreateRobot] = EventType.CreateRobot
     villa_id: int
     """大别野ID"""
 
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Bot(id={self.bot_id}) was added to Villa(id={self.villa_id})"
+            f"Bot(id={self.bot_id}) was added to Villa(id={self.villa_id})",
         )
 
 
 class DeleteRobotEvent(Event):
     """大别野删除机器人实例事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html###DeleteRobot"""
 
     type: Literal[EventType.DeleteRobot] = EventType.DeleteRobot
     villa_id: int
     """大别野ID"""
 
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Bot(id={self.bot_id}) was removed from Villa(id={self.villa_id})"
+            f"Bot(id={self.bot_id}) was removed from Villa(id={self.villa_id})",
         )
 
 
 class AddQuickEmoticonEvent(Event):
     """用户使用表情回复消息表态事件
 
     see https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AddQuickEmoticon"""
@@ -279,15 +287,18 @@
     bot_msg_id: Optional[str]
     """如果被回复的消息从属于机器人，则该字段不为空字符串"""
     is_cancel: bool = False
     """是否是取消表情"""
 
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Emoticon(name={self.emoticon}, id={self.emoticon_id}) was {'removed from' if self.is_cancel else 'added to'} Message(id={self.msg_uid}) by User(id={self.uid}) in Room(id=Villa(id={self.room_id}) of Villa(id={self.villa_id})"
+            f"Emoticon(name={self.emoticon}, id={self.emoticon_id}) "
+            f"was {'removed from' if self.is_cancel else 'added to'} "
+            f"Message(id={self.msg_uid}) by User(id={self.uid}) in "
+            f"Room(id=Villa(id={self.room_id}) of Villa(id={self.villa_id})",
         )
 
     async def send(
         self,
         message: Union[str, MessageSegment, Message],
         mention_sender: bool = False,
         quote_message: bool = False,
@@ -307,15 +318,16 @@
         """
         if (bot := get_bot(self.bot_id)) is None:
             raise ValueError(f"Bot {self.bot_id} not found. Cannot send message.")
         if isinstance(message, (str, MessageSegment)):
             message = Message(message)
         if mention_sender:
             message.insert(
-                0, MessageSegment.mention_user(self.uid, None, self.villa_id)
+                0,
+                MessageSegment.mention_user(self.uid, None, self.villa_id),
             )
         if quote_message:
             message.append(MessageSegment.quote(self.msg_uid, self.send_at))
         return await bot.send(self.villa_id, self.room_id, message)
 
 
 class AuditCallbackEvent(Event):
@@ -337,15 +349,17 @@
     pass_through: str
     """透传数据（和审核接口调用方传入的值一致）"""
     audit_result: AuditResult
     """审核结果"""
 
     def get_event_description(self) -> str:
         return escape_tag(
-            f"Audit(id={self.audit_id},result={self.audit_result}) of User(id={self.user_id}) in Room(id={self.room_id}) of Villa(id={self.villa_id})"
+            f"Audit(id={self.audit_id},result={self.audit_result}) of "
+            f"User(id={self.user_id}) in Room(id={self.room_id}) of "
+            f"Villa(id={self.villa_id})",
         )
 
 
 event_classes = Union[
     JoinVillaEvent,
     SendMessageEvent,
     CreateRobotEvent,
@@ -354,15 +368,15 @@
     AuditCallbackEvent,
 ]
 
 
 def pre_handle_event(payload: Dict[str, Any]):
     if (event_type := EventType._value2member_map_.get(payload["type"])) is None:
         raise ValueError(
-            f"Unknown event type: {payload['type']} data={escape_tag(str(payload))}"
+            f"Unknown event type: {payload['type']} data={escape_tag(str(payload))}",
         )
     event_name = event_type.name
     if event_name not in payload["extend_data"]["EventData"]:
         raise ValueError("Cannot find event data for event type: {event_name}")
     payload |= payload["extend_data"]["EventData"][event_name]
     payload.pop("extend_data")
     return payload
```

### Comparing `villa-0.6.2/villa/exception.py` & `villa-0.6.3/villa/exception.py`

 * *Files identical despite different names*

### Comparing `villa-0.6.2/villa/handle.py` & `villa-0.6.3/villa/handle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,90 @@
-import re
 import asyncio
-from typing import Type, Tuple, Optional
-
-from pydantic import BaseModel
+import re
+from typing import Optional, Tuple, Type
 
+from .event import Event, SendMessageEvent
+from .exception import StopPropagation
 from .log import logger
-from .utils import run_sync
 from .typing import T_Handler
-from .exception import StopPropagation
-from .event import Event, SendMessageEvent
+from .utils import run_sync
+
+from pydantic import BaseModel
 
 
 class EventHandler(BaseModel):
     event_type: Tuple[Type[Event], ...]
     func: T_Handler
     priority: int = 1
     block: bool = False
 
     startswith: Optional[Tuple[str, ...]] = None
     endswith: Optional[Tuple[str, ...]] = None
     keywords: Optional[Tuple[str, ...]] = None
     regex: Optional[re.Pattern] = None
 
     def __str__(self) -> str:
-        return f"Handler(func={self.func.__name__}, priority={self.priority}, block={self.block})"
+        return (
+            f"Handler(func={self.func.__name__}, priority={self.priority}, "
+            f"block={self.block})"
+        )
 
     def __repr__(self) -> str:
         return super().__str__()
 
     def _check(self, event: Event) -> bool:
         """检查事件是否满足处理函数运行条件"""
         if isinstance(event, self.event_type):
             if isinstance(event, SendMessageEvent):
                 if self.startswith is not None and not event.message.startswith(
-                    self.startswith
+                    self.startswith,
                 ):
                     logger.opt(colors=True).trace(
-                        f"{event.get_event_name()} not startswith \"{'|'.join(self.startswith)}\" of <y>{self}</y>, pass"
+                        f"{event.get_event_name()} not startswith "
+                        f"\"{'|'.join(self.startswith)}\" of <y>{self}</y>, pass",
                     )
                     return False
                 if self.endswith is not None and not event.message.endswith(
-                    self.endswith
+                    self.endswith,
                 ):
                     logger.opt(colors=True).trace(
-                        f"{event.get_event_name()} not endswith \"{'|'.join(self.endswith)}\" of <y>{self}</y>, pass"
+                        f"{event.get_event_name()} not endswith "
+                        f"\"{'|'.join(self.endswith)}\" of <y>{self}</y>, pass",
                     )
                     return False
                 if self.keywords is not None and not any(
                     keyword in event.message for keyword in self.keywords
                 ):
                     logger.opt(colors=True).trace(
-                        f"{event.get_event_name()} not contains \"{'|'.join(self.keywords)}\" of <y>{self}</y>, pass"
+                        f"{event.get_event_name()} not contains "
+                        f"\"{'|'.join(self.keywords)}\" of <y>{self}</y>, pass",
                     )
                     return False
                 if self.regex is not None and not event.message.match(self.regex):
                     logger.opt(colors=True).trace(
-                        f'{event.get_event_name()} not match "{self.regex}" of <y>{self}</y>, <y>pass</y>'
+                        f"{event.get_event_name()} not match "
+                        f'"{self.regex}" of <y>{self}</y>, <y>pass</y>',
                     )
                     return False
             return True
         return False
 
     async def _run(self, event: Event):
         """运行事件处理器"""
         if not self._check(event):
             return
         try:
             logger.opt(colors=True).info(
-                f"{event.get_event_name()} will be handled by <y>{self}</y>"
+                f"{event.get_event_name()} will be handled by <y>{self}</y>",
             )
             if asyncio.iscoroutinefunction(self.func):
                 await self.func(event)
             else:
                 await run_sync(self.func)(event)
             if self.block:
                 raise StopPropagation(handler=self)
         except StopPropagation as e:
             raise e
         except Exception as e:
             logger.opt(colors=True, exception=e).error(
-                f"Error when running <y>{self}</y> for {event.get_event_name()}"
+                f"Error when running <y>{self}</y> for {event.get_event_name()}",
             )
```

### Comparing `villa-0.6.2/villa/log.py` & `villa-0.6.3/villa/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import sys
 import logging
+import sys
 from typing import TYPE_CHECKING
 
 import loguru
 
 if TYPE_CHECKING:
     from loguru import Logger, Record
 
@@ -21,15 +21,16 @@
 
         frame, depth = logging.currentframe(), 2
         while frame and frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
 
         logger.opt(depth=depth, exception=record.exc_info).log(
-            level, record.getMessage()
+            level,
+            record.getMessage(),
         )
 
 
 def default_filter(record: "Record"):
     """默认的日志过滤器，根据 `config.log_level` 配置改变日志等级。"""
     log_level = record["extra"].get("villa_log_level", "INFO")
     levelno = logger.level(log_level).no if isinstance(log_level, str) else log_level
```

### Comparing `villa-0.6.2/villa/message.py` & `villa-0.6.3/villa/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import re
 from abc import ABC
+import re
+from typing import Iterable, Iterator, List, Literal, Optional, overload, Tuple, Union
 from typing_extensions import Self
-from typing import List, Tuple, Union, Literal, Iterable, Iterator, Optional, overload
 
+from pydantic import BaseModel, Field, root_validator
 from pydantic.utils import get_args  # type: ignore
-from pydantic import Field, BaseModel, root_validator
 
 MessageType = Literal[
     "text",
     "mention_user",
     "mention_all",
     "mention_robot",
     "room_link",
@@ -31,15 +31,17 @@
 
     @staticmethod
     def mention_robot(bot_id: str, bot_name: str) -> "MentionRobot":
         return MentionRobot(bot_id=bot_id, bot_name=bot_name)
 
     @staticmethod
     def mention_user(
-        user_id: int, user_name: Optional[str] = None, villa_id: Optional[int] = None
+        user_id: int,
+        user_name: Optional[str] = None,
+        villa_id: Optional[int] = None,
     ) -> "MentionUser":
         return MentionUser(user_id=user_id, user_name=user_name, villa_id=villa_id)
 
     @staticmethod
     def mention_all(show_text: str = "全体成员") -> "MentionAll":
         return MentionAll(show_text=show_text)
 
@@ -104,20 +106,19 @@
     @staticmethod
     def badge(icon_url: str, text: str, url: str) -> "Badge":
         return Badge(icon_url=icon_url, text=text, url=url)
 
     def __add__(self, other: Union[str, "MessageSegment", "Message"]) -> "Message":
         if isinstance(other, str):
             return Message([self, MessageSegment.plain_text(other)])
-        elif isinstance(other, MessageSegment):
+        if isinstance(other, MessageSegment):
             return Message([self, other])
-        elif isinstance(other, Message):
+        if isinstance(other, Message):
             return Message([self, *other.__root__])
-        else:
-            raise TypeError(f"unsupported type: {type(other)}")
+        raise TypeError(f"unsupported type: {type(other)}")
 
     def __radd__(self, other: Union[str, "MessageSegment", "Message"]) -> "Message":
         return self.__add__(other)
 
     def __iadd__(self, other: Union[str, "MessageSegment", "Message"]) -> "Message":
         return self.__add__(other)
 
@@ -142,14 +143,15 @@
 
     type: Literal["mention_user"] = Field(default="mention_user", repr=False)
     user_id: int
     user_name: Optional[str] = None
     villa_id: Optional[int] = None
 
     @root_validator
+    @classmethod
     def _(cls, values):
         if values.get("user_name") is None and values.get("villa_id") is None:
             raise ValueError("user_name和villa_id必须至少有一个不为None")
         return values
 
 
 class MentionAll(MessageSegment):
@@ -229,15 +231,19 @@
 
 class Message(BaseModel):
     __root__: List[MessageSegment] = Field(default_factory=list)
 
     def __init__(
         self,
         message: Union[
-            str, MessageSegment, Iterable[MessageSegment], "Message", None
+            str,
+            MessageSegment,
+            Iterable[MessageSegment],
+            "Message",
+            None,
         ] = None,
     ):
         """消息类
 
         参数:
             message: 消息内容. 默认为 None.
 
@@ -285,15 +291,15 @@
             villa_id: 要提及的用户所在的大别野ID
             user_id: 要提及的用户ID
 
         返回:
             Self: 消息对象
         """
         self.__root__.append(
-            MentionUser(user_id=user_id, user_name=user_name, villa_id=villa_id)
+            MentionUser(user_id=user_id, user_name=user_name, villa_id=villa_id),
         )
         return self
 
     def mention_all(self) -> Self:
         """提及(@at)全体成员消息
 
         返回:
@@ -337,25 +343,25 @@
         """说明
 
         详细说明
 
         参数:
             url: 链接地址
             show_text: 链接显示的文本. 为 None 时与地址保持一致.
-            requires_bot_access_token: 访问时是否需要带上含有用户信息的token. 默认为 False.
+            requires_bot_access_token: 访问时是否需要带上含有用户信息的token.
 
         返回:
             Self: 返回说明
         """
         self.__root__.append(
             Link(
                 url=url,
                 show_text=show_text or url,
                 requires_bot_access_token=requires_bot_access_token,
-            )
+            ),
         )
         return self
 
     def image(
         self,
         url: str,
         width: Optional[int] = None,
@@ -370,15 +376,15 @@
             height: 图片高度. 默认为 None.
             file_size: 图片大小. 默认为 None.
 
         返回:
             Self: 消息对象
         """
         self.__root__.append(
-            Image(url=url, width=width, height=height, file_size=file_size)
+            Image(url=url, width=width, height=height, file_size=file_size),
         )
         return self
 
     def quote(self, message_id: str, message_send_time: int) -> Self:
         """引用消息
 
         参数:
@@ -390,15 +396,15 @@
         """
         self.__root__.append(
             Quote(
                 quoted_message_id=message_id,
                 quoted_message_send_time=message_send_time,
                 original_message_id=message_id,
                 original_message_send_time=message_send_time,
-            )
+            ),
         )
         return self
 
     def post(self, post_id: str) -> Self:
         """帖子转发消息
 
         参数:
@@ -439,15 +445,15 @@
                 icon_url=icon_url,
                 image_url=image_url,
                 is_internal_link=is_internal_link,
                 title=title,
                 content=content,
                 url=url,
                 source_name=source_name,
-            )
+            ),
         )
         return self
 
     def badge(self, icon_url: str, text: str, url: str) -> Self:
         self.__root__.append(Badge(icon_url=icon_url, text=text, url=url))
         return self
 
@@ -477,15 +483,15 @@
         if isinstance(segment, str):
             segment = Text(content=segment)
         self.__root__.append(segment)
 
     def get_plain_text(self) -> str:
         """获取纯文本消息内容"""
         return "".join(
-            [segment.content for segment in self.__root__ if isinstance(segment, Text)]
+            [segment.content for segment in self.__root__ if isinstance(segment, Text)],
         )
 
     def __contains__(self, item: str) -> bool:
         """检查消息的纯文本内容是否包含指定字符串"""
         return item in self.get_plain_text()
 
     def __len__(self) -> int:
@@ -631,54 +637,58 @@
         返回:
             Text: 消息段类型为text的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(
-        self, __args: Tuple[Literal["mention_user"], int]
+        self,
+        __args: Tuple[Literal["mention_user"], int],
     ) -> Optional[MentionUser]:
         """
         参数:
             __args: mention_user消息段
 
         返回:
             MentionUser: 消息段类型为mention_user的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(
-        self, __args: Tuple[Literal["mention_all"], int]
+        self,
+        __args: Tuple[Literal["mention_all"], int],
     ) -> Optional[MentionAll]:
         """
         参数:
             __args: mention_all消息段
 
         返回:
             MentionAll: 消息段类型为mention_all的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(
-        self, __args: Tuple[Literal["mention_robot"], int]
+        self,
+        __args: Tuple[Literal["mention_robot"], int],
     ) -> Optional[MentionRobot]:
         """
         参数:
             __args: mention_robot消息段
 
         返回:
             MentionRobot: 消息段类型为mention_robot的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(
-        self, __args: Tuple[Literal["room_link"], int]
+        self,
+        __args: Tuple[Literal["room_link"], int],
     ) -> Optional[RoomLink]:
         """
         参数:
             __args: room_link消息段
 
         返回:
             RoomLink: 消息段类型为room_link的第 `__args[1]` 个消息段
@@ -727,15 +737,16 @@
         返回:
             Post: 消息段类型为post的第 `__args[1]` 个消息段
         """
         ...
 
     @overload
     def __getitem__(
-        self, __args: Tuple[Literal["preview_link"], int]
+        self,
+        __args: Tuple[Literal["preview_link"], int],
     ) -> Optional[PreviewLink]:
         """
         参数:
             __args: preview_link消息段
 
         返回:
             PreviewLink: 消息段类型为preview_link的第 `__args[1]` 个消息段
@@ -756,20 +767,20 @@
     def __getitem__(
         self,
         args: Union[int, slice, MessageType, Tuple[MessageType, Union[int, slice]]],
     ) -> Union[MessageSegment, "Message", None]:
         arg1, arg2 = args if isinstance(args, tuple) else (args, None)
         if isinstance(arg1, int) and arg2 is None:
             return self.__root__.__getitem__(arg1)
-        elif isinstance(arg1, slice) and arg2 is None:
+        if isinstance(arg1, slice) and arg2 is None:
             return Message(self.__root__.__getitem__(arg1))
-        elif isinstance(arg1, str) and arg1 in get_args(MessageType):  # type: ignore
+        if isinstance(arg1, str) and arg1 in get_args(MessageType):  # type: ignore
             if arg2 is None:
                 return Message([seg for seg in self.__root__ if seg.type == arg1])
-            elif isinstance(arg2, int):
+            if isinstance(arg2, int):
                 try:
                     return [seg for seg in self.__root__ if seg.type == arg1][arg2]
                 except IndexError:
                     return None
             elif isinstance(arg2, slice):
                 return Message([seg for seg in self.__root__ if seg.type == arg1][arg2])
             else:
```

### Comparing `villa-0.6.2/villa/models.py` & `villa-0.6.3/villa/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import sys
-import json
-import inspect
 from enum import Enum, IntEnum
-from typing import Any, Dict, List, Union, Literal, Optional
+import inspect
+import json
+import sys
+from typing import Any, Dict, List, Literal, Optional, Union
 
-from pydantic import Field, BaseModel, validator
+from pydantic import BaseModel, Field, validator
 
 
 class ApiResponse(BaseModel):
     retcode: int
     message: str
     data: Any
 
@@ -79,15 +79,15 @@
     basic: MemberBasic
     role_id_list: List[int]
     joined_at: int
     role_list: List["MemberRole"]
 
 
 class MemberListReturn(BaseModel):
-    list: List[Member]
+    list: List[Member]  # noqa: A003
     next_offset: int
 
 
 # 消息部分
 # see https://webstatic.mihoyo.com/vila/bot/doc/message_api/
 class MentionType(IntEnum):
     ALL = 1
@@ -166,14 +166,15 @@
     url: str
 
 
 class PostMessageContent(BaseModel):
     post_id: str
 
     @validator("post_id")
+    @classmethod
     def __deal_post_id(cls, v: str):
         s = v.split("/")[-1]
         if s.isdigit():
             return s
         raise ValueError(f"Invalid post_id: {v}, post_id must be a number.")
 
 
@@ -206,14 +207,15 @@
     extra: Dict[str, Any]
     name: str
     alias: str
     id: str
     portrait: str
 
     @validator("extra", pre=True)
+    @classmethod
     def extra_str_to_dict(cls, v: Any):
         if isinstance(v, str):
             return json.loads(v)
         return v
 
 
 class Trace(BaseModel):
@@ -240,16 +242,16 @@
 # 房间部分
 # see https://webstatic.mihoyo.com/vila/bot/doc/room_api/
 class Room(BaseModel):
     room_id: int
     room_name: str
     room_type: "RoomType"
     group_id: int
-    room_default_notify_type: "RoomDefaultNotifyType"
-    send_msg_auth_range: "SendMsgAuthRange"
+    room_default_notify_type: Optional["RoomDefaultNotifyType"] = None
+    send_msg_auth_range: Optional["SendMsgAuthRange"] = None
 
 
 class RoomType(str, Enum):
     CHAT = "BOT_PLATFORM_ROOM_TYPE_CHAT_ROOM"
     POST = "BOT_PLATFORM_ROOM_TYPE_POST_ROOM"
     SCENE = "BOT_PLATFORM_ROOM_TYPE_SCENE_ROOM"
     INVALID = "BOT_PLATFORM_ROOM_TYPE_INVALID"
@@ -271,15 +273,15 @@
     is_all_send_msg: bool
     roles: List[int]
 
 
 class GroupRoom(BaseModel):
     group_id: int
     group_name: str
-    room_list: "ListRoom"
+    room_list: List[Room]
 
 
 class ListRoomType(IntEnum):
     CHAT = 1
     POST = 2
     SCENE = 3
 
@@ -300,21 +302,14 @@
     NOTIFY = 1
     IGNORE = 2
 
     def __repr__(self) -> str:
         return self.name
 
 
-class ListRoom(BaseModel):
-    room_id: int
-    room_name: str
-    room_type: ListRoomType
-    group_id: int
-
-
 class Group(BaseModel):
     group_id: int
     group_name: str
 
 
 class RoomSort(BaseModel):
     room_id: int
@@ -394,15 +389,15 @@
 # see https://webstatic.mihoyo.com/vila/bot/doc/emoticon_api/
 class Emoticon(BaseModel):
     emoticon_id: int
     describe_text: str
     icon: str
 
 
-for name, obj in inspect.getmembers(sys.modules[__name__]):
+for _, obj in inspect.getmembers(sys.modules[__name__]):
     if inspect.isclass(obj) and issubclass(obj, BaseModel):
         obj.update_forward_refs()
 
 
 __all__ = [
     "ApiResponse",
     "BotAuth",
@@ -438,15 +433,14 @@
     "RoomType",
     "RoomDefaultNotifyType",
     "SendMsgAuthRange",
     "GroupRoom",
     "ListRoomType",
     "CreateRoomType",
     "CreateRoomDefaultNotifyType",
-    "ListRoom",
     "Group",
     "RoomSort",
     "MemberRole",
     "PermissionDetail",
     "MemberRoleDetail",
     "RoleType",
     "Permission",
```

### Comparing `villa-0.6.2/villa/store.py` & `villa-0.6.3/villa/store.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Dict, Optional
+from typing import Dict, Optional, TYPE_CHECKING
 
 from fastapi import FastAPI
 
 if TYPE_CHECKING:
     from .bot import Bot
 
 _bots: Dict[str, "Bot"] = {}
```

### Comparing `villa-0.6.2/villa/utils.py` & `villa-0.6.3/villa/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import re
 import asyncio
 from functools import partial, wraps
-from typing import Callable, TypeVar, Coroutine
+import re
+from typing import Callable, Coroutine, TypeVar
 from typing_extensions import ParamSpec
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
+
 def escape_tag(s: str) -> str:
     """用于记录带颜色日志时转义 `<tag>` 类型特殊标签
 
     参考: [loguru color 标签](https://loguru.readthedocs.io/en/stable/api/logger.html#color)
 
     参数:
         s: 需要转义的字符串
@@ -25,12 +26,10 @@
         call: 被装饰的同步函数
     """
 
     @wraps(call)
     async def _wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
         loop = asyncio.get_running_loop()
         pfunc = partial(call, *args, **kwargs)
-        result = await loop.run_in_executor(None, pfunc)
-        return result
+        return await loop.run_in_executor(None, pfunc)
 
     return _wrapper
-
```

### Comparing `villa-0.6.2/PKG-INFO` & `villa-0.6.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.6.2
+Version: 0.6.3
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
@@ -35,14 +35,17 @@
 <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
 <a href="https://pypi.python.org/pypi/villa">
   <img src="https://img.shields.io/pypi/dm/villa" alt="pypi download">
 </a>
 <a href="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/d3b88a99-17c2-4c98-bbc2-c1949ce7c078">
   <img src="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/d3b88a99-17c2-4c98-bbc2-c1949ce7c078.svg" alt="wakatime">
 </a>
+<a href="https://github.com/astral-sh/ruff">
+  <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="ruff">
+</a>
 
 </div>
 
 ## 特性
 
 - 基于`FastAPI`和`Pydantic`，异步优先、快速、高性能！
 - 完整的类型注解支持，便于开发。
@@ -93,15 +96,15 @@
 
 ## 交流、建议和反馈
 
 > 注意：本SDK并非官方SDK
 
 大别野 Bot 和本 SDK 均为开发测试中，如遇问题请提出 [issue](https://github.com/CMHopeSunshine/villa-py/issues) ，感谢支持！
 
-也欢迎来我的大别野[「尘世闲游」]((https://dby.miyoushe.com/chat/1047/21652))(ID: `wgiJNaU`)进行交流~ 
+也欢迎来我的大别野[「尘世闲游」]((https://dby.miyoushe.com/chat/1047/21652))(ID: `wgiJNaU`)进行交流~
 
 ## 相关项目
 
 - [NoneBot2](https://github.com/nonebot/nonebot2) 非常好用的 Python 跨平台机器人框架！
 - [nonebot-adapter-villa](https://github.com/CMHopeSunshine/nonebot-adapter-villa) NoneBot2 的大别野 Bot 适配器。
 - [Herta-villa-SDK](https://github.com/MingxuanGame/Herta-villa-SDK) 另一个大别野 Python SDK。
```

