# Comparing `tmp/nonebot_adapter_villa-0.5.4.tar.gz` & `tmp/nonebot_adapter_villa-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.5.4.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.5.5.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.5.4.tar` & `nonebot_adapter_villa-0.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1062 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/LICENSE
--rw-r--r--   0        0        0     6796 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/README.md
--rw-r--r--   0        0        0      235 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0    10977 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     2905 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     3714 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    12434 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9536 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    13338 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      649 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0    11651 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0    10115 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0     1435 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/permission.py
--rw-r--r--   0        0        0       76 2023-07-06 07:29:51.681559 nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-07-06 07:29:51.685559 nonebot_adapter_villa-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/LICENSE
+-rw-r--r--   0        0        0     6796 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/README.md
+-rw-r--r--   0        0        0      235 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0    10977 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0     2911 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/client.pyi
+-rw-r--r--   0        0        0    12460 2023-07-12 12:10:54.690336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0     9459 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    13338 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      649 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0    11651 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0    10115 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0     1435 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/permission.py
+-rw-r--r--   0        0        0       76 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-07-12 12:10:54.694336 nonebot_adapter_villa-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.5.5/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.5.4/LICENSE` & `nonebot_adapter_villa-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.4/README.md` & `nonebot_adapter_villa-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     async def get_group_list(self, *, villa_id: int) -> List[Group]: ...
     async def sort_group_list(self, *, villa_id: int, group_ids: List[int]) -> None: ...
     async def edit_room(
         self, *, villa_id: int, room_id: int, room_name: str
     ) -> None: ...
     async def delete_room(self, *, villa_id: int, room_id: int) -> None: ...
     async def get_room(self, *, villa_id: int, room_id: int) -> Room: ...
-    async def get_villa_group_room_list(self, *, villa_id: int) -> GroupRoom: ...
+    async def get_villa_group_room_list(self, *, villa_id: int) -> List[GroupRoom]: ...
     async def sort_room_list(
         self, *, villa_id: int, room_list: List[RoomSort]
     ) -> None: ...
     async def operate_member_to_role(
         self, *, villa_id: int, role_id: int, uid: int, is_add: bool
     ) -> None: ...
     async def create_member_role(
```

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,21 +224,23 @@
         json={"room_id": room_id},
     )
     return parse_obj_as(Room, (await _request(adapter, bot, request))["room"])
 
 
 async def _get_villa_group_room_list(
     adapter: "Adapter", bot: "Bot", villa_id: int
-) -> GroupRoom:
+) -> List[GroupRoom]:
     request = Request(
         method="GET",
         url=adapter.base_url / "vila/api/bot/platform/getVillaGroupRoomList",
         headers=bot.get_authorization_header(villa_id),
     )
-    return parse_obj_as(GroupRoom, (await _request(adapter, bot, request))["list"])
+    return parse_obj_as(
+        List[GroupRoom], (await _request(adapter, bot, request))["list"]
+    )
 
 
 async def _sort_room_list(
     adapter: "Adapter", bot: "Bot", villa_id: int, room_list: List[RoomSort]
 ) -> None:
     request = Request(
         method="POST",
```

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,16 +240,16 @@
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
@@ -271,15 +271,15 @@
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
 
@@ -300,21 +300,14 @@
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
```

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/config.py` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.4/nonebot/adapters/villa/permission.py` & `nonebot_adapter_villa-0.5.5/nonebot/adapters/villa/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.5.4/pyproject.toml` & `nonebot_adapter_villa-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.5.4"
+version = "0.5.5"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.5.4/PKG-INFO` & `nonebot_adapter_villa-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.5.4
+Version: 0.5.5
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.5.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.5.5 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

