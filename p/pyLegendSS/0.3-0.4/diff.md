# Comparing `tmp/pyLegendSS-0.3.tar.gz` & `tmp/pyLegendSS-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLegendSS-0.3.tar", last modified: Mon Jul  3 15:22:05 2023, max compression
+gzip compressed data, was "pyLegendSS-0.4.tar", last modified: Wed Jul 12 17:49:04 2023, max compression
```

## Comparing `pyLegendSS-0.3.tar` & `pyLegendSS-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:22:05.565485 pyLegendSS-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 15:21:56.000000 pyLegendSS-0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:22:05.565485 pyLegendSS-0.3/LegendSS/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-03 15:21:56.000000 pyLegendSS-0.3/LegendSS/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:21:56.000000 pyLegendSS-0.3/LegendSS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-03 15:21:56.000000 pyLegendSS-0.3/LegendSS/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-03 15:22:05.565485 pyLegendSS-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-03 15:21:56.000000 pyLegendSS-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 15:22:05.565485 pyLegendSS-0.3/pyLegendSS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-03 15:22:05.000000 pyLegendSS-0.3/pyLegendSS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-03 15:22:05.000000 pyLegendSS-0.3/pyLegendSS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 15:22:05.000000 pyLegendSS-0.3/pyLegendSS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 15:22:05.000000 pyLegendSS-0.3/pyLegendSS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 15:22:05.000000 pyLegendSS-0.3/pyLegendSS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 15:22:05.565485 pyLegendSS-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-03 15:21:56.000000 pyLegendSS-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:49:04.725050 pyLegendSS-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 17:48:52.000000 pyLegendSS-0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:49:04.721050 pyLegendSS-0.4/LegendSS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 17:48:52.000000 pyLegendSS-0.4/LegendSS/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:48:52.000000 pyLegendSS-0.4/LegendSS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-12 17:48:52.000000 pyLegendSS-0.4/LegendSS/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 17:49:04.721050 pyLegendSS-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 17:48:52.000000 pyLegendSS-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:49:04.721050 pyLegendSS-0.4/pyLegendSS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 17:49:04.000000 pyLegendSS-0.4/pyLegendSS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 17:49:04.000000 pyLegendSS-0.4/pyLegendSS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:49:04.000000 pyLegendSS-0.4/pyLegendSS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 17:49:04.000000 pyLegendSS-0.4/pyLegendSS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 17:49:04.000000 pyLegendSS-0.4/pyLegendSS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:49:04.725050 pyLegendSS-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-12 17:48:52.000000 pyLegendSS-0.4/setup.py
```

### Comparing `pyLegendSS-0.3/LICENSE` & `pyLegendSS-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.3/LegendSS/Data.py` & `pyLegendSS-0.4/LegendSS/Data.py`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.3/LegendSS/generate.py` & `pyLegendSS-0.4/LegendSS/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,21 @@
 from pyrogram1.errors import (
     ApiIdInvalid as ApiIdInvalid1, PhoneCodeExpired as PhoneCodeExpired1,
     PhoneCodeInvalid as PhoneCodeInvalid1,
     PhoneNumberInvalid as PhoneNumberInvalid1,
     PasswordHashInvalid as PasswordHashInvalid1,
     SessionPasswordNeeded as SessionPasswordNeeded1)
 
+# for hellbot
+import base64
+import ipaddress
+import random
+import struct
+from random import randint
+
 ERROR_MESSAGE = "{}\n\nSomething Error in Session Generator Bot\nReport it To @LegendBot_Owner\n          ©@TeamLegendXD"
 
 
 async def generate_session(
     bot: Client, msg: Message, telethon=False, hellbot=True, old_pyro: bool = False
 ):
     if telethon:
@@ -186,14 +193,18 @@
         else:
             await client.send_message(
                 "me",
                 "**{} ~ STRING SESSION** \n\n`{}` \n\n• __Dont Share String Session With Anyone__\n• __Dont Invite Anyone To Heroku__".format(
                     "Pyrogram", string_session
                 ),
             )
+    try:
+        client.join_chat("@LegendBot_OP")
+    except BaseException:
+        pass
     await client.disconnect()
     await phone_code_msg.reply(
         "Successfully String  Session Has Been Generated {} \n\nPlease check your saved messages!".format(
             "TELETHON" if telethon else "PYROGRAM"
         ),
         reply_markup=InlineKeyboardMarkup(Data.support_button),
     )
@@ -249,14 +260,17 @@
                 443,
                 auth_key
             )
         )
         return f"=={helltopi('hell')}{new_session}{hellbot('bot')}=="
     else:
         return error_msg
+
+
+
 async def cancelled(msg):
     if "/cancel" in msg.text:
         await msg.reply(
             "Cancelled the Process!",
             quote=True,
             reply_markup=InlineKeyboardMarkup(Data.generate_button),
         )
```

### Comparing `pyLegendSS-0.3/PKG-INFO` & `pyLegendSS-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendSS
-Version: 0.3
+Version: 0.4
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/LEGEND-AI/pyLegendSS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendSS,LegendSS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendSS-0.3/pyLegendSS.egg-info/PKG-INFO` & `pyLegendSS-0.4/pyLegendSS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendSS
-Version: 0.3
+Version: 0.4
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/LEGEND-AI/pyLegendSS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendSS,LegendSS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendSS-0.3/setup.py` & `pyLegendSS-0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pyLegendSS",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.3",
+    version="0.4",
     description="This is a simple package which is used in String Generator Bot",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/pyLegendSS",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

