# Comparing `tmp/gustavselfbot-0.0.7.tar.gz` & `tmp/gustavselfbot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gustavselfbot-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gustavselfbot-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gustavselfbot-0.0.7.tar` & `gustavselfbot-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     3185 2023-07-10 21:22:00.617362 gustavselfbot-0.0.7/.gitignore
--rw-r--r--   0        0        0      380 2023-07-10 21:34:48.787151 gustavselfbot-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      336 2023-07-11 17:07:43.799643 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__init__.py
--rw-r--r--   0        0        0     2127 2023-07-11 17:17:09.656597 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__logs__.py
--rw-r--r--   0        0        0      578 2023-07-11 14:00:16.016242 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__ping__.py
--rw-r--r--   0        0        0     2379 2023-07-11 14:00:16.006242 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__quote__.py
--rw-r--r--   0        0        0     2524 2023-07-11 17:17:09.649930 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__search__.py
--rw-r--r--   0        0        0     2030 2023-07-11 14:00:15.989575 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/helpers/__embed__.py
--rw-r--r--   0        0        0      151 2023-07-11 12:19:26.583238 gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/helpers/__init__.py
--rw-r--r--   0        0        0     1824 2023-07-11 17:07:43.812977 gustavselfbot-0.0.7/GustavSelfBot/Commands/__commands__.py
--rw-r--r--   0        0        0      140 2023-07-11 17:07:43.826310 gustavselfbot-0.0.7/GustavSelfBot/Commands/__init__.py
--rw-r--r--   0        0        0      276 2023-07-10 20:59:21.691270 gustavselfbot-0.0.7/GustavSelfBot/Events/__init__.py
--rw-r--r--   0        0        0     2160 2023-07-11 18:27:30.654611 gustavselfbot-0.0.7/GustavSelfBot/Events/__on_message__.py
--rw-r--r--   0        0        0      195 2023-07-11 14:00:15.999575 gustavselfbot-0.0.7/GustavSelfBot/Events/__on_ready__.py
--rw-r--r--   0        0        0     4255 2023-07-11 14:00:16.009575 gustavselfbot-0.0.7/GustavSelfBot/Events/__on_voice_state_update__.py
--rw-r--r--   0        0        0      657 2023-07-11 16:32:51.605685 gustavselfbot-0.0.7/GustavSelfBot/__bot__.py
--rw-r--r--   0        0        0      265 2023-07-10 21:07:11.012427 gustavselfbot-0.0.7/GustavSelfBot/__config__.py
--rw-r--r--   0        0        0      633 2023-07-11 20:08:55.098294 gustavselfbot-0.0.7/GustavSelfBot/__init__.py
--rw-r--r--   0        0        0     1489 2023-07-10 21:07:11.009094 gustavselfbot-0.0.7/GustavSelfBot/__logging__.py
--rw-r--r--   0        0        0        0 2023-07-10 21:15:47.984536 gustavselfbot-0.0.7/LICENSE
--rw-r--r--   0        0        0      707 2023-07-10 21:55:07.903400 gustavselfbot-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.7/_chatlogs/PLACEHOLDER
--rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.7/_recordings/PLACEHOLDER
--rw-r--r--   0        0        0       87 2023-07-10 12:32:13.422010 gustavselfbot-0.0.7/config.json
--rw-r--r--   0        0        0      246 2023-07-10 21:49:04.177889 gustavselfbot-0.0.7/main.py
--rw-r--r--   0        0        0      613 2023-07-10 21:32:16.773381 gustavselfbot-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       48 2023-07-10 21:31:18.695261 gustavselfbot-0.0.7/requirements.txt
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 gustavselfbot-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     3185 2023-07-10 21:22:00.617362 gustavselfbot-0.0.8/.gitignore
+-rw-r--r--   0        0        0      380 2023-07-10 21:34:48.787151 gustavselfbot-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      336 2023-07-11 17:07:43.799643 gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/__init__.py
+-rw-r--r--   0        0        0     2127 2023-07-11 17:17:09.656597 gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/__logs__.py
+-rw-r--r--   0        0        0      578 2023-07-11 14:00:16.016242 gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/__ping__.py
+-rw-r--r--   0        0        0     2379 2023-07-11 14:00:16.006242 gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/__quote__.py
+-rw-r--r--   0        0        0     2524 2023-07-11 17:17:09.649930 gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/__search__.py
+-rw-r--r--   0        0        0     2030 2023-07-11 14:00:15.989575 gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/helpers/__embed__.py
+-rw-r--r--   0        0        0      151 2023-07-11 12:19:26.583238 gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/helpers/__init__.py
+-rw-r--r--   0        0        0     2029 2023-07-12 21:31:41.413506 gustavselfbot-0.0.8/GustavSelfBot/Commands/__commands__.py
+-rw-r--r--   0        0        0      140 2023-07-11 17:07:43.826310 gustavselfbot-0.0.8/GustavSelfBot/Commands/__init__.py
+-rw-r--r--   0        0        0      276 2023-07-10 20:59:21.691270 gustavselfbot-0.0.8/GustavSelfBot/Events/__init__.py
+-rw-r--r--   0        0        0     2160 2023-07-11 18:27:30.654611 gustavselfbot-0.0.8/GustavSelfBot/Events/__on_message__.py
+-rw-r--r--   0        0        0      195 2023-07-11 14:00:15.999575 gustavselfbot-0.0.8/GustavSelfBot/Events/__on_ready__.py
+-rw-r--r--   0        0        0     4255 2023-07-11 14:00:16.009575 gustavselfbot-0.0.8/GustavSelfBot/Events/__on_voice_state_update__.py
+-rw-r--r--   0        0        0      657 2023-07-11 16:32:51.605685 gustavselfbot-0.0.8/GustavSelfBot/__bot__.py
+-rw-r--r--   0        0        0      351 2023-07-12 10:23:27.823180 gustavselfbot-0.0.8/GustavSelfBot/__config__.py
+-rw-r--r--   0        0        0      663 2023-07-12 21:32:09.071350 gustavselfbot-0.0.8/GustavSelfBot/__init__.py
+-rw-r--r--   0        0        0     1489 2023-07-10 21:07:11.009094 gustavselfbot-0.0.8/GustavSelfBot/__logging__.py
+-rw-r--r--   0        0        0        0 2023-07-10 21:15:47.984536 gustavselfbot-0.0.8/LICENSE
+-rw-r--r--   0        0        0      707 2023-07-10 21:55:07.903400 gustavselfbot-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.8/_chatlogs/PLACEHOLDER
+-rw-r--r--   0        0        0        0 2023-07-10 19:20:59.498601 gustavselfbot-0.0.8/_recordings/PLACEHOLDER
+-rw-r--r--   0        0        0       87 2023-07-10 12:32:13.422010 gustavselfbot-0.0.8/config.json
+-rw-r--r--   0        0        0      246 2023-07-10 21:49:04.177889 gustavselfbot-0.0.8/main.py
+-rw-r--r--   0        0        0      613 2023-07-10 21:32:16.773381 gustavselfbot-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-07-10 21:31:18.695261 gustavselfbot-0.0.8/requirements.txt
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 gustavselfbot-0.0.8/PKG-INFO
```

### Comparing `gustavselfbot-0.0.7/.gitignore` & `gustavselfbot-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__logs__.py` & `gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/__logs__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__ping__.py` & `gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/__ping__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__quote__.py` & `gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/__quote__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/__search__.py` & `gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/__search__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/Commands/Functions/helpers/__embed__.py` & `gustavselfbot-0.0.8/GustavSelfBot/Commands/Functions/helpers/__embed__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/Commands/__commands__.py` & `gustavselfbot-0.0.8/GustavSelfBot/Commands/__commands__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import aiohttp.client_exceptions
 import discord
 from discord.ext import commands
 
 from GustavSelfBot import log
 
 from GustavSelfBot.Commands.Functions import func_ping, func_quote, func_logs, func_search
 
@@ -12,44 +13,44 @@
 
 
 @log.catch
 async def ping(bot: commands.Bot, ctx: commands.Context, message: discord.Message):
     log.info(f"Command {message.content.replace('>', '')} called by {ctx.author.display_name} (ID: {ctx.author.id})")
     try:
         await func_ping(bot, ctx, message)
-    except discord.errors.ClientException as e:
+    except (discord.errors.ClientException, aiohttp.client_exceptions.ClientOSError) as e:
         log.error(e)
         await ctx.send("Error")
         raise Exception(e)
 
 
 @log.catch
 async def quote(bot: commands.Bot, ctx: commands.Context, message: discord.Message):
     log.info(f"Command {message.content.replace('>', '')} called by {ctx.author.display_name} (ID: {ctx.author.id})")
     try:
         await func_quote(bot, ctx, message)
-    except discord.errors.ClientException as e:
+    except (discord.errors.ClientException, aiohttp.client_exceptions.ClientOSError) as e:
         log.error(e)
         await ctx.send("Error")
         raise Exception(e)
 
 
 @log.catch
 async def logs(bot: commands.Bot, ctx: commands.Context, message: discord.Message):
     log.info(f"Command {message.content.replace('>', '')} called by {ctx.author.display_name} (ID: {ctx.author.id})")
     try:
         await func_logs(bot, ctx, message)
-    except discord.errors.ClientException as e:
+    except (discord.errors.ClientException, aiohttp.client_exceptions.ClientOSError) as e:
         log.error(e)
         await ctx.send("Error")
         raise Exception(e)
 
 
 @log.catch
 async def search(bot: commands.Bot, ctx: commands.Context, message: discord.Message):
     log.info(f"Command {message.content.replace('>', '')} called by {ctx.author.display_name} (ID: {ctx.author.id})")
     try:
         await func_search(bot, ctx, message)
-    except discord.errors.ClientException as e:
+    except (discord.errors.ClientException, aiohttp.client_exceptions.ClientOSError) as e:
         log.error(e)
         await ctx.send("Error")
         raise Exception(e)
```

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/Events/__on_message__.py` & `gustavselfbot-0.0.8/GustavSelfBot/Events/__on_message__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/Events/__on_voice_state_update__.py` & `gustavselfbot-0.0.8/GustavSelfBot/Events/__on_voice_state_update__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/__bot__.py` & `gustavselfbot-0.0.8/GustavSelfBot/__bot__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/__init__.py` & `gustavselfbot-0.0.8/GustavSelfBot/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 My self bot!
 Current implementation of GustavSelfBot includes chat logs and commands.
 TODO: make custom command and hooks possible
 """
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 import os
 
 from GustavSelfBot.__logging__ import *
 from GustavSelfBot.__config__ import Config
 from GustavSelfBot.__bot__ import bot
 
@@ -16,10 +16,10 @@
 
 if Config["token"] == "":
     log.error("No token provided!")
     raise Exception("No token provided!")
 
 try:
     os.makedirs("_chatlogs", exist_ok=True)
-except PermissionError as e:
+except (FileNotFoundError, IOError, PermissionError) as e:
     log.error(f"Could not create _chatlogs folder: {e}")
     raise Exception(f"Could not create _chatlogs folder: {e}")
```

### Comparing `gustavselfbot-0.0.7/GustavSelfBot/__logging__.py` & `gustavselfbot-0.0.8/GustavSelfBot/__logging__.py`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/README.md` & `gustavselfbot-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/pyproject.toml` & `gustavselfbot-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gustavselfbot-0.0.7/PKG-INFO` & `gustavselfbot-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GustavSelfBot
-Version: 0.0.7
+Version: 0.0.8
 Summary: My self bot!
 Author-email: Gustavo Schip <gustavoschip@proton.me>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: discord.py-self[voice]
 Requires-Dist: aiohttp
```

