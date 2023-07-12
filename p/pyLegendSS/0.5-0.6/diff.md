# Comparing `tmp/pyLegendSS-0.5.tar.gz` & `tmp/pyLegendSS-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLegendSS-0.5.tar", last modified: Wed Jul 12 17:58:54 2023, max compression
+gzip compressed data, was "pyLegendSS-0.6.tar", last modified: Wed Jul 12 18:23:08 2023, max compression
```

## Comparing `pyLegendSS-0.5.tar` & `pyLegendSS-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:58:54.459367 pyLegendSS-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 17:58:38.000000 pyLegendSS-0.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:58:54.459367 pyLegendSS-0.5/LegendSS/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 17:58:38.000000 pyLegendSS-0.5/LegendSS/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:58:38.000000 pyLegendSS-0.5/LegendSS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-07-12 17:58:38.000000 pyLegendSS-0.5/LegendSS/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 17:58:54.459367 pyLegendSS-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 17:58:38.000000 pyLegendSS-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:58:54.459367 pyLegendSS-0.5/pyLegendSS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 17:58:54.000000 pyLegendSS-0.5/pyLegendSS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 17:58:54.000000 pyLegendSS-0.5/pyLegendSS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:58:54.000000 pyLegendSS-0.5/pyLegendSS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 17:58:54.000000 pyLegendSS-0.5/pyLegendSS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 17:58:54.000000 pyLegendSS-0.5/pyLegendSS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:58:54.459367 pyLegendSS-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-12 17:58:38.000000 pyLegendSS-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:23:08.657229 pyLegendSS-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 18:22:51.000000 pyLegendSS-0.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:23:08.657229 pyLegendSS-0.6/LegendSS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 18:22:51.000000 pyLegendSS-0.6/LegendSS/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:22:51.000000 pyLegendSS-0.6/LegendSS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-12 18:22:51.000000 pyLegendSS-0.6/LegendSS/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 18:23:08.657229 pyLegendSS-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 18:22:51.000000 pyLegendSS-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:23:08.657229 pyLegendSS-0.6/pyLegendSS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 18:23:08.000000 pyLegendSS-0.6/pyLegendSS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 18:23:08.000000 pyLegendSS-0.6/pyLegendSS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:23:08.000000 pyLegendSS-0.6/pyLegendSS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 18:23:08.000000 pyLegendSS-0.6/pyLegendSS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 18:23:08.000000 pyLegendSS-0.6/pyLegendSS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:23:08.657229 pyLegendSS-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-12 18:22:51.000000 pyLegendSS-0.6/setup.py
```

### Comparing `pyLegendSS-0.5/LICENSE` & `pyLegendSS-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.5/LegendSS/Data.py` & `pyLegendSS-0.6/LegendSS/Data.py`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.5/LegendSS/generate.py` & `pyLegendSS-0.6/LegendSS/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from .Data import Data
+
+import base64
+import ipaddress
+import random
+import struct
+from random import randint
+from telethon.sessions.string import (_STRUCT_PREFORMAT, CURRENT_VERSION,
+                                          StringSession)
 from pyrogram import Client, filters
 from pyrogram1 import Client as Client1
 from telethon.sync import TelegramClient
 from asyncio.exceptions import TimeoutError
-from telethon.sessions import StringSession
 from pyrogram.types import Message, InlineKeyboardButton, InlineKeyboardMarkup
 from telethon.tl.functions.channels import (
     JoinChannelRequest, LeaveChannelRequest)
 from pyrogram.errors import (
     ApiIdInvalid, PhoneCodeExpired, PhoneCodeInvalid, PhoneNumberInvalid,
     PasswordHashInvalid, SessionPasswordNeeded)
 from telethon.errors import (
@@ -17,24 +24,14 @@
 from pyrogram1.errors import (
     ApiIdInvalid as ApiIdInvalid1, PhoneCodeExpired as PhoneCodeExpired1,
     PhoneCodeInvalid as PhoneCodeInvalid1,
     PhoneNumberInvalid as PhoneNumberInvalid1,
     PasswordHashInvalid as PasswordHashInvalid1,
     SessionPasswordNeeded as SessionPasswordNeeded1)
 
-# for hellbot
-import base64
-import ipaddress
-import random
-import struct
-from random import randint
-from telethon.sessions.string import (_STRUCT_PREFORMAT, CURRENT_VERSION,
-                                          StringSession)
-
-
 ERROR_MESSAGE = "{}\n\nSomething Error in Session Generator Bot\nReport it To @LegendBot_Owner\n          ©@TeamLegendXD"
 
 
 async def generate_session(
     bot: Client, msg: Message, telethon=False, hellbot=True, old_pyro: bool = False
 ):
     if telethon:
@@ -235,15 +232,15 @@
         1: "149.154.175.53",
         2: "149.154.167.51",
         3: "149.154.175.100",
         4: "149.154.167.91",
         5: "91.108.56.130",
     }
 
-    error_msg = "Error in generating session! Report it in Hell Chats"
+    error_msg = "Error in generating session! Report it in Comments of @TeamLegendBots"
 
     # converting pyrogram session
     if len(session) in pyro_format.keys():
         if len(session) in [351, 356]:
             dc_id, _, auth_key, _, _ = struct.unpack(
                 pyro_format[len(session)],
                 base64.urlsafe_b64decode(session + "=" * (-len(session) % 4)),
@@ -260,15 +257,15 @@
                 _STRUCT_PREFORMAT.format(4),
                 dc_id,
                 ipaddress.ip_address(ipv4_dc[dc_id]).packed,
                 443,
                 auth_key
             )
         )
-        return f"=={helltopi('hell')}{new_session}{hellbot('bot')}=="
+        return f"=={helltopi('hell')}{new_session}{helltopi('bot')}=="
     else:
         return error_msg
 
 
 
 async def cancelled(msg):
     if "/cancel" in msg.text:
```

### Comparing `pyLegendSS-0.5/PKG-INFO` & `pyLegendSS-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendSS
-Version: 0.5
+Version: 0.6
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/LEGEND-AI/pyLegendSS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendSS,LegendSS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendSS-0.5/pyLegendSS.egg-info/PKG-INFO` & `pyLegendSS-0.6/pyLegendSS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendSS
-Version: 0.5
+Version: 0.6
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/LEGEND-AI/pyLegendSS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendSS,LegendSS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendSS-0.5/setup.py` & `pyLegendSS-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pyLegendSS",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.5",
+    version="0.6",
     description="This is a simple package which is used in String Generator Bot",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/pyLegendSS",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

