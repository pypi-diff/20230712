# Comparing `tmp/anarchy_bot-23.0.1.tar.gz` & `tmp/anarchy_bot-23.0.2.tar.gz`

## Comparing `anarchy_bot-23.0.1.tar` & `anarchy_bot-23.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/build.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/changlog.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/pyrightcongig.json
--rwxr-xr-x   0        0        0     2024 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/setup.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/__main__.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/cb.py
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/chats.py
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/common.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/config.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/inline.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/lang.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/lists.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/main.py
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/msg.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/anarchy_bot/lang/en.yml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/.gitignore
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/pyproject.toml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/readme.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 anarchy_bot-23.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/build.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/changlog.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/pyrightconfig.json
+-rwxr-xr-x   0        0        0     2024 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/setup.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/__main__.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/cb.py
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/chats.py
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/common.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/config.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/inline.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/lang.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/lists.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/main.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/msg.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/anarchy_bot/lang/en.yml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/.gitignore
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/pyproject.toml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/readme.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 anarchy_bot-23.0.2/PKG-INFO
```

### Comparing `anarchy_bot-23.0.1/build.py` & `anarchy_bot-23.0.2/build.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/setup.py` & `anarchy_bot-23.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/anarchy_bot/cb.py` & `anarchy_bot-23.0.2/anarchy_bot/cb.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/anarchy_bot/chats.py` & `anarchy_bot-23.0.2/anarchy_bot/chats.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/anarchy_bot/common.py` & `anarchy_bot-23.0.2/anarchy_bot/common.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/anarchy_bot/config.py` & `anarchy_bot-23.0.2/anarchy_bot/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     import tgcrypto # type: ignore
     using_tgcrypto = True
 except Exception:
     using_tgcrypto = False
 
 
 app_name = 'anarchy_bot'
-app_version = '23.0.1'
+app_version = '23.0.2'
 c = rich.console.Console()
 c.log(f'imported [deep_sky_blue1]{__file__}')
 app_path = Path(
     __file__
 ).parent.parent.resolve()
 src_path = app_path / app_name
 data_path = app_path / f'{app_name}_data'
```

### Comparing `anarchy_bot-23.0.1/anarchy_bot/inline.py` & `anarchy_bot-23.0.2/anarchy_bot/inline.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/anarchy_bot/lang.py` & `anarchy_bot-23.0.2/anarchy_bot/lang.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/anarchy_bot/lists.py` & `anarchy_bot-23.0.2/anarchy_bot/lists.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/anarchy_bot/main.py` & `anarchy_bot-23.0.2/anarchy_bot/main.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/anarchy_bot/msg.py` & `anarchy_bot-23.0.2/anarchy_bot/msg.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,16 @@
     admins = {
         '/setlogs': setlogs_msg,
     }
     if msg.service:
         if msg.service == pg.enums.MessageServiceType.LEFT_CHAT_MEMBERS:
             await notify_removed(msg)
         return
+    if not msg.text:
+        return
     if not config.owner:
         await set_owner(
             msg,
         )
     if msg.chat.type == pg.enums.ChatType.PRIVATE:
         await chats.remember_user(msg.from_user.id)
         action = chats.users_dict[msg.from_user.id]
@@ -144,14 +146,18 @@
                     can_manage_chat = True,
                     can_change_info = True,
                 ),
             )
             text += f'\n\nsuccesfully promoted {mention(msg.from_user)} to admin'
             await responce.edit_text(text)
             break
+        except pyrogram.errors.ChatAdminRequired:
+            text += '\n\ni have no rights to make you an admin'
+            await responce.edit_text(text)
+            return
         except pyrogram.errors.UserCreator:
             text += '\n\nbro you are chat owner'
             await responce.edit_text(text)
             return
         except pyrogram.errors.AdminsTooMuch:
             admins: list[ChatMember] = await chats.list_chat_admins(
                 client = client,
```

### Comparing `anarchy_bot-23.0.1/anarchy_bot/lang/en.yml` & `anarchy_bot-23.0.2/anarchy_bot/lang/en.yml`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/pyproject.toml` & `anarchy_bot-23.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [ "gmanka_yml==23.0.*", "pyrogram==2.0.*", "tgcrypto==1.2.*", "uvloop==0.17.*", "rich==13.4.*",]
 name = "anarchy_bot"
-version = "23.0.1"
+version = "23.0.2"
 description = "telegram bot that can add users to minecraft whitelist"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "gmanka"
 email = "gmankab@gmail.com"
```

### Comparing `anarchy_bot-23.0.1/readme.md` & `anarchy_bot-23.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.1/PKG-INFO` & `anarchy_bot-23.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anarchy_bot
-Version: 23.0.1
+Version: 23.0.2
 Summary: telegram bot that can add users to minecraft whitelist
 Project-URL: Documentation, https://t.me/gmanka
 Project-URL: Bug Tracker, https://t.me/gmanka
 Project-URL: Homepage, https://t.me/gmanka
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

