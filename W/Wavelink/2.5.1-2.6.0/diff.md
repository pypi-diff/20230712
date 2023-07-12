# Comparing `tmp/Wavelink-2.5.1.tar.gz` & `tmp/Wavelink-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Wavelink-2.5.1.tar", last modified: Fri Jun 16 12:59:26 2023, max compression
+gzip compressed data, was "Wavelink-2.6.0.tar", last modified: Wed Jul 12 04:05:29 2023, max compression
```

## Comparing `Wavelink-2.5.1.tar` & `Wavelink-2.6.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.328668 Wavelink-2.5.1/
--rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.5.1/LICENSE
--rw-rw-rw-   0        0        0     5772 2023-06-16 12:59:26.328157 Wavelink-2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.313156 Wavelink-2.5.1/Wavelink.egg-info/
--rw-rw-rw-   0        0        0     5772 2023-06-16 12:59:26.000000 Wavelink-2.5.1/Wavelink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-16 12:59:26.000000 Wavelink-2.5.1/Wavelink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 12:59:26.000000 Wavelink-2.5.1/Wavelink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-16 12:59:26.000000 Wavelink-2.5.1/Wavelink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 12:59:26.000000 Wavelink-2.5.1/Wavelink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1006 2023-06-16 12:55:24.000000 Wavelink-2.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.5.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 12:59:26.328668 Wavelink-2.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.323151 Wavelink-2.5.1/wavelink/
--rw-rw-rw-   0        0        0     1495 2023-06-16 12:55:24.000000 Wavelink-2.5.1/wavelink/__init__.py
--rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/backoff.py
--rw-rw-rw-   0        0        0     3689 2023-06-05 10:25:32.000000 Wavelink-2.5.1/wavelink/enums.py
--rw-rw-rw-   0        0        0     3028 2023-06-05 09:44:43.000000 Wavelink-2.5.1/wavelink/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.295797 Wavelink-2.5.1/wavelink/ext/
-drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.323651 Wavelink-2.5.1/wavelink/ext/spotify/
--rw-rw-rw-   0        0        0    17836 2023-06-16 12:50:04.000000 Wavelink-2.5.1/wavelink/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/filters.py
--rw-rw-rw-   0        0        0    17836 2023-06-05 08:54:30.000000 Wavelink-2.5.1/wavelink/node.py
--rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.5.1/wavelink/payloads.py
--rw-rw-rw-   0        0        0    22017 2023-06-12 11:33:29.000000 Wavelink-2.5.1/wavelink/player.py
--rw-rw-rw-   0        0        0    12545 2023-06-15 00:04:14.000000 Wavelink-2.5.1/wavelink/queue.py
--rw-rw-rw-   0        0        0     9954 2023-06-15 00:00:10.000000 Wavelink-2.5.1/wavelink/tracks.py
-drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.327154 Wavelink-2.5.1/wavelink/types/
--rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/types/events.py
--rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/types/request.py
--rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/types/state.py
--rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/types/track.py
--rw-rw-rw-   0        0        0     9570 2023-05-20 08:53:53.000000 Wavelink-2.5.1/wavelink/websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.692616 Wavelink-2.6.0/
+-rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0     5812 2023-07-12 04:05:29.692616 Wavelink-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5011 2023-06-23 14:10:49.000000 Wavelink-2.6.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.676058 Wavelink-2.6.0/Wavelink.egg-info/
+-rw-rw-rw-   0        0        0     5812 2023-07-12 04:05:29.000000 Wavelink-2.6.0/Wavelink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-07-12 04:05:29.000000 Wavelink-2.6.0/Wavelink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 04:05:29.000000 Wavelink-2.6.0/Wavelink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-12 04:05:29.000000 Wavelink-2.6.0/Wavelink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 04:05:29.000000 Wavelink-2.6.0/Wavelink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1006 2023-07-12 04:05:10.000000 Wavelink-2.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 04:05:29.693117 Wavelink-2.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.686597 Wavelink-2.6.0/wavelink/
+-rw-rw-rw-   0        0        0     1495 2023-07-12 04:05:10.000000 Wavelink-2.6.0/wavelink/__init__.py
+-rw-rw-rw-   0        0        0      992 2023-06-24 08:28:29.000000 Wavelink-2.6.0/wavelink/__main__.py
+-rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.6.0/wavelink/backoff.py
+-rw-rw-rw-   0        0        0     3689 2023-06-05 10:25:32.000000 Wavelink-2.6.0/wavelink/enums.py
+-rw-rw-rw-   0        0        0     3028 2023-06-05 09:44:43.000000 Wavelink-2.6.0/wavelink/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.667128 Wavelink-2.6.0/wavelink/ext/
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.688102 Wavelink-2.6.0/wavelink/ext/spotify/
+-rw-rw-rw-   0        0        0    16863 2023-07-12 03:52:50.000000 Wavelink-2.6.0/wavelink/ext/spotify/__init__.py
+-rw-rw-rw-   0        0        0     5115 2023-06-27 13:30:40.000000 Wavelink-2.6.0/wavelink/ext/spotify/utils.py
+-rw-rw-rw-   0        0        0    20509 2023-06-21 14:04:01.000000 Wavelink-2.6.0/wavelink/filters.py
+-rw-rw-rw-   0        0        0    19314 2023-07-02 08:09:07.000000 Wavelink-2.6.0/wavelink/node.py
+-rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.6.0/wavelink/payloads.py
+-rw-rw-rw-   0        0        0    30563 2023-06-29 12:10:11.000000 Wavelink-2.6.0/wavelink/player.py
+-rw-rw-rw-   0        0        0    20409 2023-07-02 08:09:07.000000 Wavelink-2.6.0/wavelink/queue.py
+-rw-rw-rw-   0        0        0    11769 2023-07-02 08:09:07.000000 Wavelink-2.6.0/wavelink/tracks.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:05:29.691615 Wavelink-2.6.0/wavelink/types/
+-rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.6.0/wavelink/types/events.py
+-rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.6.0/wavelink/types/request.py
+-rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.6.0/wavelink/types/state.py
+-rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.6.0/wavelink/types/track.py
+-rw-rw-rw-   0        0        0    11011 2023-07-12 04:02:26.000000 Wavelink-2.6.0/wavelink/websocket.py
```

### Comparing `Wavelink-2.5.1/LICENSE` & `Wavelink-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.1/PKG-INFO` & `Wavelink-2.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.5.1
+Version: 2.6.0
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -55,15 +55,15 @@
 - Spotify Support
 - Node Balancing and Fail-over
 - Supports Lavalink 3.7+
 
 
 Documentation
 ---------------------------
-`Official Documentation <https://wavelink.readthedocs.io/en/latest/index.html>`_
+`Official Documentation <https://wavelink.dev/>`_
 
 Support
 ---------------------------
 For support using WaveLink, please join the official `support server
 <https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
 
 .. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
@@ -126,15 +126,20 @@
         """Simple play command."""
 
         if not ctx.voice_client:
             vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
         else:
             vc: wavelink.Player = ctx.voice_client
 
-        track = await wavelink.YouTubeTrack.search(search, return_first=True)
+        tracks = await wavelink.YouTubeTrack.search(search)
+        if not tracks:
+            await ctx.send(f'No tracks found with query: `{search}`')
+            return
+
+        track = tracks[0]
         await vc.play(track)
 
 
     @bot.command()
     async def disconnect(ctx: commands.Context) -> None:
         """Simple disconnect command.
 
@@ -143,20 +148,20 @@
         vc: wavelink.Player = ctx.voice_client
         await vc.disconnect()
 
 
 Lavalink Installation
 ---------------------
 
-Head to the official `Lavalink repo <https://github.com/freyacodes/Lavalink>`_ and give it a star!
+Head to the official `Lavalink repo <https://github.com/lavalink-devs/Lavalink>`_ and give it a star!
 
 - Create a folder for storing Lavalink.jar and related files/folders.
 - Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
 - Change your password in the ``application.yml`` and store it in a config for your bot.
 - Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
 - Save and exit.
 - Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
-- Download `Lavalink.jar <https://ci.fredboat.com/viewLog.html?buildId=lastSuccessful&buildTypeId=Lavalink_Build&tab=artifacts&guest=1>`_ and place it in the folder created earlier.
+- Download `Lavalink.jar <https://github.com/lavalink-devs/Lavalink/releases>`_ and place it in the folder created earlier.
 - Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
 - Run: ``java -jar Lavalink.jar``
 
 If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
```

### Comparing `Wavelink-2.5.1/README.rst` & `Wavelink-2.6.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 - Spotify Support
 - Node Balancing and Fail-over
 - Supports Lavalink 3.7+
 
 
 Documentation
 ---------------------------
-`Official Documentation <https://wavelink.readthedocs.io/en/latest/index.html>`_
+`Official Documentation <https://wavelink.dev/>`_
 
 Support
 ---------------------------
 For support using WaveLink, please join the official `support server
 <https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
 
 .. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
@@ -106,15 +106,20 @@
         """Simple play command."""
 
         if not ctx.voice_client:
             vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
         else:
             vc: wavelink.Player = ctx.voice_client
 
-        track = await wavelink.YouTubeTrack.search(search, return_first=True)
+        tracks = await wavelink.YouTubeTrack.search(search)
+        if not tracks:
+            await ctx.send(f'No tracks found with query: `{search}`')
+            return
+
+        track = tracks[0]
         await vc.play(track)
 
 
     @bot.command()
     async def disconnect(ctx: commands.Context) -> None:
         """Simple disconnect command.
 
@@ -123,20 +128,20 @@
         vc: wavelink.Player = ctx.voice_client
         await vc.disconnect()
 
 
 Lavalink Installation
 ---------------------
 
-Head to the official `Lavalink repo <https://github.com/freyacodes/Lavalink>`_ and give it a star!
+Head to the official `Lavalink repo <https://github.com/lavalink-devs/Lavalink>`_ and give it a star!
 
 - Create a folder for storing Lavalink.jar and related files/folders.
 - Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
 - Change your password in the ``application.yml`` and store it in a config for your bot.
 - Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
 - Save and exit.
 - Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
-- Download `Lavalink.jar <https://ci.fredboat.com/viewLog.html?buildId=lastSuccessful&buildTypeId=Lavalink_Build&tab=artifacts&guest=1>`_ and place it in the folder created earlier.
+- Download `Lavalink.jar <https://github.com/lavalink-devs/Lavalink/releases>`_ and place it in the folder created earlier.
 - Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
 - Run: ``java -jar Lavalink.jar``
 
-If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
+If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
```

### Comparing `Wavelink-2.5.1/Wavelink.egg-info/PKG-INFO` & `Wavelink-2.6.0/Wavelink.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.5.1
+Version: 2.6.0
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -55,15 +55,15 @@
 - Spotify Support
 - Node Balancing and Fail-over
 - Supports Lavalink 3.7+
 
 
 Documentation
 ---------------------------
-`Official Documentation <https://wavelink.readthedocs.io/en/latest/index.html>`_
+`Official Documentation <https://wavelink.dev/>`_
 
 Support
 ---------------------------
 For support using WaveLink, please join the official `support server
 <https://discord.gg/RAKc3HF>`_ on `Discord <https://discordapp.com/>`_.
 
 .. image:: https://discordapp.com/api/guilds/490948346773635102/widget.png?style=banner2
@@ -126,15 +126,20 @@
         """Simple play command."""
 
         if not ctx.voice_client:
             vc: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
         else:
             vc: wavelink.Player = ctx.voice_client
 
-        track = await wavelink.YouTubeTrack.search(search, return_first=True)
+        tracks = await wavelink.YouTubeTrack.search(search)
+        if not tracks:
+            await ctx.send(f'No tracks found with query: `{search}`')
+            return
+
+        track = tracks[0]
         await vc.play(track)
 
 
     @bot.command()
     async def disconnect(ctx: commands.Context) -> None:
         """Simple disconnect command.
 
@@ -143,20 +148,20 @@
         vc: wavelink.Player = ctx.voice_client
         await vc.disconnect()
 
 
 Lavalink Installation
 ---------------------
 
-Head to the official `Lavalink repo <https://github.com/freyacodes/Lavalink>`_ and give it a star!
+Head to the official `Lavalink repo <https://github.com/lavalink-devs/Lavalink>`_ and give it a star!
 
 - Create a folder for storing Lavalink.jar and related files/folders.
 - Copy and paste the example `application.yml <https://github.com/freyacodes/Lavalink#server-configuration>`_ to ``application.yml`` in the folder we created earlier. You can open the yml in Notepad or any simple text editor.
 - Change your password in the ``application.yml`` and store it in a config for your bot.
 - Set local to true in the ``application.yml`` if you wish to use ``wavelink.LocalTrack`` for local machine search options... Otherwise ignore.
 - Save and exit.
 - Install `Java 17(Windows) <https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.exe>`_ or **Java 13+** on the machine you are running.
-- Download `Lavalink.jar <https://ci.fredboat.com/viewLog.html?buildId=lastSuccessful&buildTypeId=Lavalink_Build&tab=artifacts&guest=1>`_ and place it in the folder created earlier.
+- Download `Lavalink.jar <https://github.com/lavalink-devs/Lavalink/releases>`_ and place it in the folder created earlier.
 - Open a cmd prompt or terminal and change directory ``cd`` into the folder we made earlier.
 - Run: ``java -jar Lavalink.jar``
 
 If you are having any problems installing Lavalink, please join the official Discord Server listed above for help.
```

### Comparing `Wavelink-2.5.1/Wavelink.egg-info/SOURCES.txt` & `Wavelink-2.6.0/Wavelink.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 requirements.txt
 Wavelink.egg-info/PKG-INFO
 Wavelink.egg-info/SOURCES.txt
 Wavelink.egg-info/dependency_links.txt
 Wavelink.egg-info/requires.txt
 Wavelink.egg-info/top_level.txt
 wavelink/__init__.py
+wavelink/__main__.py
 wavelink/backoff.py
 wavelink/enums.py
 wavelink/exceptions.py
 wavelink/filters.py
 wavelink/node.py
 wavelink/payloads.py
 wavelink/player.py
 wavelink/queue.py
 wavelink/tracks.py
 wavelink/websocket.py
 wavelink/ext/spotify/__init__.py
+wavelink/ext/spotify/utils.py
 wavelink/types/events.py
 wavelink/types/request.py
 wavelink/types/state.py
 wavelink/types/track.py
```

### Comparing `Wavelink-2.5.1/pyproject.toml` & `Wavelink-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Wavelink"
-version = "2.5.1"
+version = "2.6.0"
 authors = [
   { name="EvieePy", email="evieepy@gmail.com" },
 ]
 dynamic = ["dependencies"]
 description = "A robust and powerful Lavalink wrapper for discord.py"
 readme = "README.rst"
 requires-python = ">=3.10"
```

### Comparing `Wavelink-2.5.1/wavelink/__init__.py` & `Wavelink-2.6.0/wavelink/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 __title__ = "WaveLink"
 __author__ = "PythonistaGuild, EvieePy"
 __license__ = "MIT"
 __copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "2.5.1"
+__version__ = "2.6.0"
 
 from .enums import *
 from .exceptions import *
 from .node import *
 from .payloads import *
 from .player import Player as Player
 from .tracks import *
```

### Comparing `Wavelink-2.5.1/wavelink/backoff.py` & `Wavelink-2.6.0/wavelink/backoff.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.1/wavelink/enums.py` & `Wavelink-2.6.0/wavelink/enums.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.1/wavelink/exceptions.py` & `Wavelink-2.6.0/wavelink/exceptions.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.1/wavelink/ext/spotify/__init__.py` & `Wavelink-2.6.0/wavelink/ext/spotify/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,109 +21,47 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from __future__ import annotations
 
 import asyncio
 import base64
-import enum
-import re
+import logging
 import time
 from typing import Any, List, Optional, Type, TypeVar, Union, TYPE_CHECKING
 
 import aiohttp
 from discord.ext import commands
 
 import wavelink
 from wavelink import Node, NodePool
 
+from .utils import *
+
+
 if TYPE_CHECKING:
     from wavelink import Player, Playable
 
 
-__all__ = ('SpotifySearchType',
-           'SpotifyClient',
-           'SpotifyTrack',
-           'SpotifyRequestError',
-           'decode_url')
+__all__ = (
+    'SpotifySearchType',
+    'SpotifyClient',
+    'SpotifyTrack',
+    'SpotifyRequestError',
+    'decode_url',
+    'SpotifyDecodePayload'
+)
 
 
-GRANTURL = 'https://accounts.spotify.com/api/token?grant_type=client_credentials'
-URLREGEX = re.compile(r'(https?://open.)?(spotify)(.com/|:)'
-                      r'(?P<type>album|playlist|track|artist)([/:])'
-                      r'(?P<id>[a-zA-Z0-9]+)(\?si=[a-zA-Z0-9]+)?(&dl_branch=[0-9]+)?')
-BASEURL = 'https://api.spotify.com/v1/{entity}s/{identifier}'
-RECURL = 'https://api.spotify.com/v1/recommendations?seed_tracks={tracks}'
+logger: logging.Logger = logging.getLogger(__name__)
 
 
 ST = TypeVar("ST", bound="Playable")
 
 
-def decode_url(url: str) -> Optional[dict]:
-    """Check whether the given URL is a valid Spotify URL and return it's type and ID.
-
-    Parameters
-    ----------
-    url: str
-        The URL to check.
-
-    Returns
-    -------
-    Optional[dict]
-        An mapping of :class:`SpotifySearchType` and Spotify ID. Type will be either track, album or playlist.
-        If type is not track, album or playlist, a special unusable type is returned.
-
-        Could return None if the URL is invalid.
-
-    Examples
-    --------
-
-    .. code:: python3
-
-        from wavelink.ext import spotify
-
-        ...
-
-        decoded = spotify.decode_url("https://open.spotify.com/track/6BDLcvvtyJD2vnXRDi1IjQ?si=e2e5bd7aaf3d4a2a")
-
-        if decoded and decoded['type'] is spotify.SpotifySearchType.track:
-            track = await spotify.SpotifyTrack.search(query=decoded["id"], type=decoded["type"])
-    """
-    match = URLREGEX.match(url)
-    if match:
-        try:
-            type_ = SpotifySearchType[match['type']]
-        except KeyError:
-            type_ = SpotifySearchType.unusable
-
-        return {'type': type_, 'id': match['id']}
-
-    return None
-
-
-class SpotifySearchType(enum.Enum):
-    """An enum specifying which type to search for with a given Spotify ID.
-
-    Attributes
-    ----------
-    track
-        Default search type. Unless specified otherwise this will always be the search type.
-    album
-        Album search type.
-    playlist
-        Playlist search type.
-    unusable
-        Unusable type. This type is returned when Wavelink can not be used to play this track.
-    """
-    track = 0
-    album = 1
-    playlist = 2
-    unusable = 3
-
-
 class SpotifyAsyncIterator:
 
     def __init__(self, *, query: str, limit: int, type: SpotifySearchType, node: Node):
         self._query = query
         self._limit = limit
         self._type = type
         self._node = node
@@ -178,14 +116,30 @@
         self.status = status
         self.reason = reason
 
 
 class SpotifyTrack:
     """A track retrieved via Spotify.
 
+
+    .. container:: operations
+
+        .. describe:: str(track)
+
+            Returns a string representing this SpotifyTrack's name and artists.
+
+        .. describe:: repr(track)
+
+            Returns an official string representation of this SpotifyTrack.
+
+        .. describe:: track == other_track
+
+            Check whether a track is equal to another. Tracks are equal if they both have the same Spotify ID.
+
+
     Attributes
     ----------
     raw: dict[str, Any]
         The raw payload from Spotify for this track.
     album: str
         The album name this track belongs to.
     images: list[str]
@@ -199,32 +153,35 @@
     title: str
         An alias to name.
     uri: str
         The URI for this spotify track.
     id: str
         The spotify ID for this track.
     isrc: str | None
-        The International Standard Recording Code associated with this track if given.
+        The International Standard Recording Code associated with this track.
     length: int
         The track length in milliseconds.
     duration: int
         Alias to length.
+    explicit: bool
+        Whether this track is explicit or not.
     """
 
     __slots__ = (
         'raw',
         'album',
         'images',
         'artists',
         'name',
         'title',
         'uri',
         'id',
         'length',
         'duration',
+        'explicit',
         'isrc',
         '__dict__'
     )
 
     def __init__(self, data: dict[str, Any]) -> None:
         self.raw: dict[str, Any] = data
 
@@ -238,125 +195,134 @@
 
         self.name: str = data['name']
         self.title: str = self.name
         self.uri: str = data['uri']
         self.id: str = data['id']
         self.length: int = data['duration_ms']
         self.duration: int = self.length
-
-        self.isrc: str | None = data["external_ids"].get("isrc")
+        self.isrc: str | None = data.get("external_ids", {}).get('irsc')
+        self.explicit: bool = data.get('explicit', False) in {"true", True}
 
     def __str__(self) -> str:
         return f'{self.name} - {self.artists[0]}'
 
     def __repr__(self) -> str:
         return f'SpotifyTrack(id={self.id}, isrc={self.isrc}, name={self.name}, duration={self.duration})'
 
     def __eq__(self, other) -> bool:
         if isinstance(other, SpotifyTrack):
             return self.id == other.id
         raise NotImplemented
 
     @classmethod
     async def search(
-        cls: Type[ST],
+            cls,
             query: str,
             *,
-            type: SpotifySearchType = SpotifySearchType.track,
             node: Node | None = None,
-    ) -> Union[Optional[ST], List[ST]]:
+    ) -> list['SpotifyTrack']:
         """|coro|
 
         Search for tracks with the given query.
 
         Parameters
         ----------
         query: str
-            The song to search for.
-        type: Optional[:class:`~SpotifySearchType`]
-            An optional enum value to use when searching with Spotify. Defaults to track.
+            The Spotify URL to query for.
         node: Optional[:class:`wavelink.Node`]
             An optional Node to use to make the search with.
 
         Returns
         -------
         List[:class:`SpotifyTrack`]
 
         Examples
         --------
         Searching for a singular tack to play...
 
         .. code:: python3
 
-            track: spotify.SpotifyTrack = await spotify.SpotifyTrack.search(query=SPOTIFY_URL)
+            tracks: list[spotify.SpotifyTrack] = await spotify.SpotifyTrack.search(query=SPOTIFY_URL)
+            if not tracks:
+                # No tracks found, do something?
+                return
+
+            track: spotify.SpotifyTrack = tracks[0]
 
 
         Searching for all tracks in an album...
 
         .. code:: python3
 
-            tracks: list[spotify.SpotifyTrack] =
-            await spotify.SpotifyTrack.search(query=SPOTIFY_URL, type=spotify.SpotifySearchType.album)
+            tracks: list[spotify.SpotifyTrack] = await spotify.SpotifyTrack.search(query=SPOTIFY_URL)
+            if not tracks:
+                # No tracks found, do something?
+                return
 
 
-        .. note::
+        .. versionchanged:: 2.6.0
 
-            See :func:`~.decode_url` for gathering information about the supplied URL, including search type.
-            Before using this method.
+            This method no longer takes in the ``type`` parameter. The query provided will be automatically decoded,
+            if the ``type`` returned by :func:`decode_url` is unusable, this method will return an empty :class:`list`
         """
         if node is None:
             node: Node = NodePool.get_connected_node()
 
-        return await node._spotify._search(query=query, type=type)
+        decoded: SpotifyDecodePayload = decode_url(query)
+
+        if not decoded or decoded.type is SpotifySearchType.unusable:
+            logger.debug(f'Spotify search handled an unusable search type for query: "{query}".')
+            return []
+
+        return await node._spotify._search(query=query, type=decoded.type)
 
     @classmethod
     def iterator(cls,
                  *,
                  query: str,
                  limit: int | None = None,
-                 type: SpotifySearchType = SpotifySearchType.playlist,
                  node: Node | None = None,
                  ):
         """An async iterator version of search.
 
         This can be useful when searching for large playlists or albums with Spotify.
 
         Parameters
         ----------
         query: str
-            The Spotify URL or ID to search for. Must be of type Playlist or Album.
+            The Spotify URL to search for. Must be of type Playlist or Album.
         limit: Optional[int]
             Limit the amount of tracks returned.
-        type: :class:`~SpotifySearchType`
-            The type of search. Must be either playlist or album. Defaults to playlist.
         node: Optional[:class:`wavelink.Node`]
             An optional node to use when querying for tracks. Defaults to the best available.
 
         Examples
         --------
 
         .. code:: python3
 
-                async for track in spotify.SpotifyTrack.iterator(query=..., type=spotify.SpotifySearchType.playlist):
+                async for track in spotify.SpotifyTrack.iterator(query=...):
                     ...
 
 
-        .. note::
+        .. versionchanged:: 2.6.0
 
-            See :func:`~.decode_url` for gathering information about the supplied URL, including search type.
-            Before using this method.
+            This method no longer takes in the ``type`` parameter. The query provided will be automatically decoded,
+            if the ``type`` returned by :func:`decode_url` is not either ``album`` or ``playlist`` this method will
+            raise a :exc:`TypeError`.
         """
+        decoded: SpotifyDecodePayload = decode_url(query)
 
-        if type is not SpotifySearchType.album and type is not SpotifySearchType.playlist:
-            raise TypeError("Iterator search type must be either album or playlist.")
+        if not decoded or decoded.type is not SpotifySearchType.album and decoded.type is not SpotifySearchType.playlist:
+            raise TypeError('Spotify iterator query must be either a valid Spotify album or playlist URL.')
 
         if node is None:
             node = NodePool.get_connected_node()
 
-        return SpotifyAsyncIterator(query=query, limit=limit, node=node, type=type)
+        return SpotifyAsyncIterator(query=query, limit=limit, node=node, type=decoded.type)
 
     @classmethod
     async def convert(cls: Type[ST], ctx: commands.Context, argument: str) -> ST:
         """Converter which searches for and returns the first track.
 
         Used as a type hint in a
         `discord.py command <https://discordpy.readthedocs.io/en/stable/ext/commands/commands.html>`_.
@@ -380,17 +346,21 @@
         Parameters
         ----------
         player: :class:`wavelink.player.Player`
             If :attr:`wavelink.Player.autoplay` is enabled, this search will fill the AutoPlay Queue with more tracks.
         cls
             The class to convert this Spotify Track to.
         """
-        tracks: list[cls] = await cls.search(f'"{self.isrc}"')
-        if not tracks:
+
+        if not self.isrc:
             tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
+        else:
+            tracks: list[cls] = await cls.search(f'"{self.isrc}"')
+            if not tracks:
+                tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
 
         if not player.autoplay or not populate:
             return tracks[0]
 
         node: Node = player.current_node
         sc: SpotifyClient | None = node._spotify
 
@@ -411,15 +381,15 @@
                 raise SpotifyRequestError(resp.status, resp.reason)
 
             data = await resp.json()
 
         recos = [SpotifyTrack(t) for t in data['tracks']]
         for reco in recos:
             if reco in player.auto_queue or reco in player.auto_queue.history:
-                pass
+                continue
 
             await player.auto_queue.put_wait(reco)
 
         return tracks[0]
 
 
 class SpotifyClient:
@@ -478,25 +448,29 @@
         url = (
             BASEURL.format(
                 entity=regex_result['type'], identifier=regex_result['id']
             )
             if regex_result
             else BASEURL.format(entity=type.name, identifier=query)
         )
+
         async with self.session.get(url, headers=self.bearer_headers) as resp:
-            if resp.status != 200:
+            if resp.status == 400:
+                return []
+
+            elif resp.status != 200:
                 raise SpotifyRequestError(resp.status, resp.reason)
 
             data = await resp.json()
 
         if data['type'] == 'track':
             return [SpotifyTrack(data)]
 
         elif data['type'] == 'album':
-            album_data: dict[str, Any]= {
+            album_data: dict[str, Any] = {
                                         'album_type': data['album_type'],
                                         'artists': data['artists'],
                                         'available_markets': data['available_markets'],
                                         'external_urls': data['external_urls'],
                                         'href': data['href'],
                                         'id': data['id'],
                                         'images': data['images'],
@@ -514,26 +488,24 @@
                     tracks.append(track)
                 else:
                     tracks.append(SpotifyTrack(track))
 
             return tracks
 
         elif data['type'] == 'playlist':
-            if iterator:
-                if not data['tracks']['next']:
-                    return [t['track'] for t in data['tracks']['items']]
-
-                url = data['tracks']['next']
-
-                items = [t['track'] for t in data['tracks']['items']]
-                while True:
-                    async with self.session.get(url, headers=self.bearer_headers) as resp:
-                        data = await resp.json()
-
-                        items.extend([t['track'] for t in data['items']])
-                        if not data['next']:
-                            return items
-
-                        url = data['next']
-            else:
-                tracks = data['tracks']['items']
-                return [SpotifyTrack(t) for t in tracks]
+            if not iterator:
+                return [SpotifyTrack(t['track']) for t in data['tracks']['items']]
+            if not data['tracks']['next']:
+                return [t['track'] for t in data['tracks']['items']]
+
+            url = data['tracks']['next']
+
+            items = [t['track'] for t in data['tracks']['items']]
+            while True:
+                async with self.session.get(url, headers=self.bearer_headers) as resp:
+                    data = await resp.json()
+
+                    items.extend([t['track'] for t in data['items']])
+                    if not data['next']:
+                        return items
+
+                    url = data['next']
```

### Comparing `Wavelink-2.5.1/wavelink/filters.py` & `Wavelink-2.6.0/wavelink/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,21 @@
     "ChannelMix",
     "LowPass",
     "Filter",
 )
 
 
 class BaseFilter(abc.ABC):
+    """
+    .. container:: operations
+
+        .. describe:: repr(filter)
+
+            Returns an official string representation of this filter.
+    """
 
     def __init__(self, name: str | None = None) -> None:
         self.name: str = name or "Unknown"
 
     def __repr__(self) -> str:
         return f"<wavelink.BaseFilter name={self.name}>"
 
@@ -528,14 +535,22 @@
 
 class Filter:
     """A filter that can be applied to a track.
 
     This filter accepts an instance of itself as a parameter which allows
     you to keep previous filters while also applying new ones or overwriting old ones.
 
+
+    .. container:: operations
+
+        .. describe:: repr(filter)
+
+            Returns an official string representation of this filter.
+
+
     Parameters
     ----------
     filter: wavelink.Filter
         An instance of this filter class.
     equalizer: wavelink.Equalizer
         An equalizer to apply to the track.
     karaoke: wavelink.Karaoke
@@ -550,15 +565,14 @@
         A rotation filter to apply to the track.
     distortion: wavelink.Distortion
         A distortion filter to apply to the track.
     channel_mix: wavelink.ChannelMix
         A channel mix filter to apply to the track.
     low_pass: wavelink.LowPass
         A low pass filter to apply to the track.
-
     """
 
     def __init__(
         self,
         _filter: Filter | None = None,
         /, *,
         equalizer: Equalizer | None = None,
```

### Comparing `Wavelink-2.5.1/wavelink/node.py` & `Wavelink-2.6.0/wavelink/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 import aiohttp
 import discord
 from discord.enums import try_enum
 from discord.utils import MISSING, classproperty
 import urllib.parse
 
+from . import __version__
 from .enums import LoadType, NodeStatus
 from .exceptions import *
 from .websocket import Websocket
 
 if TYPE_CHECKING:
     from .player import Player
     from .tracks import *
@@ -66,14 +67,22 @@
         The Node class should only be created once per Lavalink connection.
         To retrieve a Node use the appropriate :class:`NodePool` methods instead.
 
     .. warning::
 
         The Node will not be connected until passed to :meth:`NodePool.connect`.
 
+
+    .. container:: operations
+
+        .. describe:: repr(node)
+
+            Returns an official string representation of this Node.
+
+
     Parameters
     ----------
     id: Optional[str]
         The unique identifier for this Node. If not passed, one will be generated randomly.
     uri: str
         The uri to connect to your Lavalink server. E.g ``http://localhost:2333``.
     password: str
@@ -126,22 +135,23 @@
         self._retries: int | None = retries
 
         self.client: discord.Client | None = None
         self._websocket: Websocket = MISSING
         self._session_id: str | None = None
 
         self._players: dict[int, Player] = {}
+        self._invalidated: dict[int, Player] = {}
 
         self._status: NodeStatus = NodeStatus.DISCONNECTED
         self._major_version: int | None = None
 
         self._spotify: spotify_.SpotifyClient | None = None
 
     def __repr__(self) -> str:
-        return f'Node: id="{self._id}", uri="{self.uri}", status={self.status}'
+        return f'Node(id="{self._id}", uri="{self.uri}", status={self.status})'
 
     def __eq__(self, other: object) -> bool:
         return self.id == other.id if isinstance(other, Node) else NotImplemented
 
     @property
     def id(self) -> str:
         """The Nodes unique identifier."""
@@ -204,22 +214,32 @@
         async with self._session.get(f'{self._host}/version') as resp:
             version: str = await resp.text()
 
             if version.endswith('-SNAPSHOT'):
                 self._major_version = 3
                 return
 
-            version_tuple = tuple(int(v) for v in version.split('.'))
+            try:
+                version_tuple = tuple(int(v) for v in version.split('.'))
+            except ValueError:
+                logging.warning(f'Lavalink "{version}" is unknown and may not be compatible with: '
+                                f'Wavelink "{__version__}". Wavelink is assuming the Lavalink version.')
+
+                self._major_version = 3
+                return
+
             if version_tuple[0] < 3:
-                raise InvalidLavalinkVersion(f'Wavelink 2 is not compatible with Lavalink "{version}".')
+                raise InvalidLavalinkVersion(f'Wavelink "{__version__}" is not compatible with Lavalink "{version}".')
 
             if version_tuple[0] == 3 and version_tuple[1] < 7:
-                raise InvalidLavalinkVersion('Wavelink 2 is not compatible with Lavalink versions under "3.7".')
+                raise InvalidLavalinkVersion(f'Wavelink "{__version__}" is not compatible with '
+                                             f'Lavalink versions under "3.7".')
 
             self._major_version = version_tuple[0]
+            logger.info(f'Lavalink version "{version}" connected for Node: {self.id}')
 
     async def _send(self,
                     *,
                     method: str,
                     path: str,
                     guild_id: int | str | None = None,
                     query: str | None = None,
@@ -228,23 +248,33 @@
 
         uri: str = f'{self._host}/' \
                    f'v{self._major_version}/' \
                    f'{path}' \
                    f'{f"/{guild_id}" if guild_id else ""}' \
                    f'{f"?{query}" if query else ""}'
 
+        logger.debug(f'Node {self} is sending payload to [{method}] "{uri}" with payload: {data}')
+
         async with self._session.request(method=method, url=uri, json=data or {}) as resp:
+            rdata: dict[str | int, Any] | None = None
+
+            if resp.content_type == 'application/json':
+                rdata = await resp.json()
+
+            logger.debug(f'Node {self} received payload from Lavalink after sending to "{uri}" with response: '
+                         f'<status={resp.status}, data={rdata}>')
+
             if resp.status >= 300:
                 raise InvalidLavalinkResponse(f'An error occurred when attempting to reach: "{uri}".',
                                               status=resp.status)
 
             if resp.status == 204:
                 return
 
-            return await resp.json()
+            return rdata
 
     async def get_tracks(self, cls: type[PlayableT], query: str) -> list[PlayableT]:
         """|coro|
 
         Search for and retrieve Tracks based on the query and cls provided.
 
         .. note::
@@ -260,14 +290,16 @@
             The query to search for and return tracks.
 
         Returns
         -------
         list[PlayableT]
             A list of found tracks converted to the provided cls.
         """
+        logger.debug(f'Node {self} is requesting tracks with query "{query}".')
+
         data = await self._send(method='GET', path='loadtracks', query=f'identifier={query}')
         load_type = try_enum(LoadType, data.get("loadType"))
 
         if load_type is LoadType.load_failed:
             # TODO - Proper Exception...
 
             raise ValueError('Track Failed to load.')
@@ -306,14 +338,16 @@
         Raises
         ------
         ValueError
             Loading the playlist failed.
         WavelinkException
             An unspecified error occurred when loading the playlist.
         """
+        logger.debug(f'Node {self} is requesting a playlist with query "{query}".')
+
         encoded_query = urllib.parse.quote(query)
         data = await self._send(method='GET', path='loadtracks', query=f'identifier={encoded_query}')
 
         load_type = try_enum(LoadType, data.get("loadType"))
 
         if load_type is LoadType.load_failed:
             # TODO Proper exception...
@@ -338,14 +372,15 @@
             The type of Playable track that should be returned.
         encoded: str
             The Tracks unique encoded string.
         """
         encoded_query = urllib.parse.quote(encoded)
         data = await self._send(method='GET', path='decodetrack', query=f'encodedTrack={encoded_query}')
 
+        logger.debug(f'Node {self} built encoded track with encoding "{encoded}". Response data: {data}')
         return cls(data=data)
 
 
 # noinspection PyShadowingBuiltins
 class NodePool:
     """The Wavelink NodePool is responsible for keeping track of all :class:`Node`.
 
@@ -510,15 +545,16 @@
         """|coro|
 
         Helper method to retrieve a playlist from the NodePool without fetching a :class:`Node`.
 
 
         .. warning::
 
-            The only playlist currently supported is :class:`tracks.YouTubePlaylist`.
+            The only playlists currently supported are :class:`tracks.YouTubePlaylist` and
+            :class:`tracks.YouTubePlaylist`.
 
 
         Parameters
         ----------
         query: str
             The query to search for and return a playlist.
         cls: type[PlayableT]
```

### Comparing `Wavelink-2.5.1/wavelink/payloads.py` & `Wavelink-2.6.0/wavelink/payloads.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.1/wavelink/player.py` & `Wavelink-2.6.0/wavelink/player.py`

 * *Files 27% similar despite different names*

```diff
@@ -60,18 +60,41 @@
 
 
 class Player(discord.VoiceProtocol):
     """Wavelink Player class.
 
     This class is used as a :class:`~discord.VoiceProtocol` and inherits all its members.
 
+    You must pass this class to :meth:`discord.VoiceChannel.connect` with ``cls=...``. This ensures the player is
+    set up correctly and put into the discord.py voice client cache.
+
+    You **can** make an instance of this class *before* passing it to
+    :meth:`discord.VoiceChannel.connect` with ``cls=...``, but you **must** still pass it.
+
+    Once you have connected this class you do not need to store it anywhere as it will be stored on the
+    :class:`~wavelink.Node` and in the discord.py voice client cache. Meaning you can access this player where you
+    have access to a :class:`~wavelink.NodePool`, the specific :class:`~wavelink.Node` or a :class:`~discord.Guild`
+    including in :class:`~discord.ext.commands.Context` and :class:`~discord.Interaction`.
+
+    Examples
+    --------
+
+    .. code:: python3
+
+        # Connect the player...
+        player: wavelink.Player = await ctx.author.voice.channel.connect(cls=wavelink.Player)
+
+        # Retrieve the player later...
+        player: wavelink.Player = ctx.guild.voice_client
+
 
     .. note::
 
-        The Player class come with an in-built queue. See :class:`queue.Queue`.
+        The Player class comes with an in-built queue. See :class:`queue.Queue` for more information on how this queue
+        works.
 
     Parameters
     ----------
     nodes: Optional[list[:class:`node.Node`]]
         An optional list of :class:`node.Node` to use with this Player. If no Nodes are provided
         the best connected Node will be used.
     swap_node_on_disconnect: bool
@@ -89,17 +112,16 @@
     current_node: :class:`node.Node`
         The Node this player is currently using.
     queue: :class:`queue.Queue`
         The wavelink built in Queue. See :class:`queue.Queue`. This queue always takes precedence over the auto_queue.
         Meaning any songs in this queue will be played before auto_queue songs.
     auto_queue: :class:`queue.Queue`
         The built-in AutoPlay Queue. This queue keeps track of recommended songs only.
-        When a song is retrieved from this queue in the AutoPlay event, it is added to the main Queue.history.
-    filter: dict[:class:`str`, :class:`Any`]
-        The current filters applied.
+        When a song is retrieved from this queue in the AutoPlay event,
+        it is added to the main :attr:`wavelink.Queue.history` queue.
     """
 
     def __call__(self, client: discord.Client, channel: VoiceChannel) -> Self:
         self.client = client
         self.channel = channel
 
         return self
@@ -152,52 +174,103 @@
 
         self._volume: int = 50
         self._paused: bool = False
 
         self._track_seeds: list[str] = []
         self._autoplay: bool = False
         self.auto_queue: Queue = Queue()
-        self._auto_threshold: int = 20
+        self._auto_threshold: int = 100
         self._filter: Filter | None = None
 
+        self._destroyed: bool = False
+
     async def _auto_play_event(self, payload: TrackEventPayload) -> None:
+        logger.debug(f'Player {self.guild.id} entered autoplay event.')
+
         if not self.autoplay:
+            logger.debug(f'Player {self.guild.id} autoplay is set to False. Exiting autoplay event.')
             return
 
         if payload.reason == 'REPLACED':
+            logger.debug(f'Player {self.guild.id} autoplay reason is REPLACED. Exiting autoplay event.')
             return
 
         if self.queue.loop:
+            logger.debug(f'Player {self.guild.id} autoplay default queue.loop is set to True.')
+
             try:
                 track = self.queue.get()
             except QueueEmpty:
+                logger.debug(f'Player {self.guild.id} autoplay default queue.loop is set to True '
+                             f'but no track was available. Exiting autoplay event.')
                 return
 
+            logger.debug(f'Player {self.guild.id} autoplay default queue.loop is set to True. Looping track "{track}"')
             await self.play(track)
             return
 
         if self.queue:
+            track = self.queue.get()
+
             populate = len(self.auto_queue) < self._auto_threshold
-            await self.play(self.queue.get(), populate=populate)
+            await self.play(track, populate=populate)
+
+            logger.debug(f'Player {self.guild.id} autoplay found track in default queue, populate={populate}.')
+            return
 
+        if self.queue.loop_all:
+            await self.play(self.queue.get())
             return
 
         if not self.auto_queue:
+            logger.debug(f'Player {self.guild.id} has no auto queue. Exiting autoplay event.')
             return
 
         await self.queue.put_wait(await self.auto_queue.get_wait())
         populate = self.auto_queue.is_empty
 
-        await self.play(await self.queue.get_wait(), populate=populate)
+        track = await self.queue.get_wait()
+        await self.play(track, populate=populate)
+
+        logger.debug(f'Player {self.guild.id} playing track "{track}" from autoplay with populate={populate}.')
 
     @property
     def autoplay(self) -> bool:
-        """Bool whether the Player is in AutoPlay mode or not.
+        """Returns a ``bool`` indicating whether the :class:`~Player` is in AutoPlay mode or not.
+
+        This property can be set to ``True`` or ``False``.
+
+        When ``autoplay`` is ``True``, the player will automatically handle fetching and playing the next track from
+        the queue. It also searches tracks in the ``auto_queue``, a special queue populated with recommended tracks,
+        from the Spotify API or YouTube Recommendations.
+
+
+        .. note::
+
+            You can still use the :func:`~wavelink.on_wavelink_track_end` event when ``autoplay`` is ``True``,
+            but it is recommended to **not** do any queue logic or invoking play from this event.
+
+            Most users are able to use ``autoplay`` and :func:`~wavelink.on_wavelink_track_start` together to handle
+            their logic. E.g. sending a message when a track starts playing.
+
+
+        .. note::
+
+            The ``auto_queue`` will be populated when you play a :class:`~wavelink.ext.spotify.SpotifyTrack` or
+            :class:`~wavelink.YouTubeTrack`, and have initially set ``populate`` to ``True`` in
+            :meth:`~wavelink.Player.play`. See :meth:`~wavelink.Player.play` for more info.
+
+
+        .. versionadded:: 2.0
+
 
-        Can be set to True or False.
+        .. versionchanged:: 2.6.0
+
+            The autoplay event now populates the ``auto_queue`` when playing :class:`~wavelink.YouTubeTrack` **or**
+            :class:`~wavelink.ext.spotify.SpotifyTrack`.
         """
         return self._autoplay
 
     @autoplay.setter
     def autoplay(self, value: bool) -> None:
         """Set AutoPlay to True or False."""
         self._autoplay = value
@@ -237,27 +310,31 @@
         delta = (datetime.datetime.now(datetime.timezone.utc) - self.last_update).total_seconds() * 1000
         position = self.last_position + delta
 
         return min(position, self.current.duration)
 
     @property
     def ping(self) -> int:
-        """The ping to the discord endpoint in milliseconds."""
+        """The ping to the discord endpoint in milliseconds.
+
+        .. versionadded:: 2.0
+        """
         return self._ping
 
     @property
     def current(self) -> Playable | None:
         """The currently playing Track if there is one.
 
-        Could be None if no Track is playing.
+        Could be ``None`` if no Track is playing.
         """
         return self._current
 
     @property
     def filter(self) -> dict[str, Any]:
+        """The currently applied filter."""
         return self._filter._payload
 
     async def _update_event(self, data: PlayerUpdateOp | None) -> None:
         assert self._guild is not None
 
         if data is None: 
             if self.swap_on_disconnect:
@@ -284,20 +361,37 @@
         state: PlayerState = data['state']
         self.last_update = datetime.datetime.fromtimestamp(state.get("time", 0) / 1000, datetime.timezone.utc)
         self.last_position = state.get('position', 0)
 
         self._ping = state['ping']
 
     async def on_voice_server_update(self, data: VoiceServerUpdate) -> None:
+        """|coro|
+
+        An abstract method that is called when initially connecting to voice. This corresponds to VOICE_SERVER_UPDATE.
+
+        .. warning::
+
+            Do not override this method.
+        """
         self._voice_state['token'] = data['token']
         self._voice_state['endpoint'] = data['endpoint']
 
         await self._dispatch_voice_update()
 
     async def on_voice_state_update(self, data: GuildVoiceState) -> None:
+        """|coro|
+
+        An abstract method that is called when the client’s voice state has changed.
+        This corresponds to VOICE_STATE_UPDATE.
+
+        .. warning::
+
+            Do not override this method.
+        """
         assert self._guild is not None
 
         channel_id = data["channel_id"]
 
         if not channel_id:
             await self._destroy()
             return
@@ -326,105 +420,172 @@
         self._player_state.update(**voice)
 
         resp: dict[str, Any] = await self.current_node._send(method='PATCH',
                                                              path=f'sessions/{self.current_node._session_id}/players',
                                                              guild_id=self._guild.id,
                                                              data=voice)
 
-        logger.debug(f'Dispatching VOICE_UPDATE: {resp}')
+        logger.debug(f'Player {self.guild.id} is dispatching VOICE_UPDATE: {resp}')
 
-    async def connect(self, *, timeout: float, reconnect: bool, **kwargs: Any) -> None:
-        if self.channel is None:
-            self._invalidate()
-
-            msg: str = 'Please use the method "discord.VoiceChannel.connect" and pass this player to cls='
-            raise InvalidChannelStateError(msg)
+    def _connection_check(self, channel: VoiceChannel) -> None:
+        if channel.permissions_for(channel.guild.me).administrator:
+            return
 
-        if not self.channel.permissions_for(self.channel.guild.me).connect:
-            self._invalidate()
+        if not channel.permissions_for(channel.guild.me).connect:
+            logger.debug(f'Player tried connecting to channel "{channel.id}", but does not have correct permissions.')
 
             raise InvalidChannelPermissions('You do not have connect permissions to join this channel.')
 
-        limit: int = self.channel.user_limit
-        total: int = len(self.channel.members)
+        limit: int = channel.user_limit
+        total: int = len(channel.members)
 
         if limit == 0:
             pass
 
         elif total >= limit:
-            self._invalidate()
-
             msg: str = f'There are currently too many users in this channel. <{total}/{limit}>'
+            logger.debug(f'Player tried connecting to channel "{channel.id}", but the it is full. <{total}/{limit}>')
+
             raise InvalidChannelPermissions(msg)
 
+    async def connect(self, *, timeout: float, reconnect: bool, **kwargs: Any) -> None:
+        if self.channel is None:
+            self._invalidate(before_connect=True)
+
+            msg: str = 'Please use the method "discord.VoiceChannel.connect" and pass this player to cls='
+            logger.debug(f'Player tried connecting without a channel. {msg}')
+
+            raise InvalidChannelStateError(msg)
+
         if not self._guild:
             self._guild = self.channel.guild
             self.current_node._players[self._guild.id] = self
 
+        try:
+            self._connection_check(self.channel)
+        except InvalidChannelPermissions as e:
+            self._invalidate(before_connect=True)
+            raise e
+
         await self.channel.guild.change_voice_state(channel=self.channel, **kwargs)
+        logger.info(f'Player {self.guild.id} connected to channel: {self.channel}')
 
     async def move_to(self, channel: discord.VoiceChannel) -> None:
         """|coro|
 
         Moves the player to a different voice channel.
 
         Parameters
         -----------
         channel: :class:`discord.VoiceChannel`
             The channel to move to. Must be a voice channel.
         """
+        self._connection_check(channel)
+
         await self.guild.change_voice_state(channel=channel)
-        logger.info(f"Moving to voice channel:: {channel.id}")
+        logger.info(f'Player {self.guild.id} moved to channel: {channel}')
 
     async def play(self,
-                   track: Playable,
+                   track: Playable | spotify.SpotifyTrack,
                    replace: bool = True,
                    start: int | None = None,
                    end: int | None = None,
                    volume: int | None = None,
                    *,
                    populate: bool = False
                    ) -> Playable:
         """|coro|
 
         Play a WaveLink Track.
 
         Parameters
         ----------
         track: :class:`tracks.Playable`
-            The :class:`tracks.Playable` track to start playing.
+            The :class:`tracks.Playable` or :class:`~wavelink.ext.spotify.SpotifyTrack` track to start playing.
         replace: bool
             Whether this track should replace the current track. Defaults to ``True``.
         start: Optional[int]
             The position to start the track at in milliseconds.
             Defaults to ``None`` which will start the track at the beginning.
         end: Optional[int]
             The position to end the track at in milliseconds.
             Defaults to ``None`` which means it will play until the end.
         volume: Optional[int]
             Sets the volume of the player. Must be between ``0`` and ``1000``.
             Defaults to ``None`` which will not change the volume.
         populate: bool
-            Whether to populate the AutoPlay queue. This is done automatically when AutoPlay is on.
-            Defaults to False.
+            Whether to populate the AutoPlay queue. Defaults to ``False``.
+
+            .. versionadded:: 2.0
 
         Returns
         -------
-        :class:`tracks.Playable`
+        :class:`~tracks.Playable`
             The track that is now playing.
+
+
+        .. note::
+
+            If you pass a :class:`~wavelink.YouTubeTrack` **or** :class:`~wavelink.ext.spotify.SpotifyTrack` and set
+            ``populate=True``, **while** :attr:`~wavelink.Player.autoplay` is set to ``True``, this method will populate
+            the ``auto_queue`` with recommended songs. When the ``auto_queue`` is low on tracks this method will
+            automatically populate the ``auto_queue`` with more tracks, and continue this cycle until either the
+            player has been disconnected or :attr:`~wavelink.Player.autoplay` is set to ``False``.
+
+
+        Example
+        -------
+
+        .. code:: python3
+
+            tracks: list[wavelink.YouTubeTrack] = await wavelink.YouTubeTrack.search(...)
+            if not tracks:
+                # Do something as no tracks were found...
+                return
+
+            await player.queue.put_wait(tracks[0])
+
+            if not player.is_playing():
+                await player.play(player.queue.get(), populate=True)
+
+
+        .. versionchanged:: 2.6.0
+
+            This method now accepts :class:`~wavelink.YouTubeTrack` or :class:`~wavelink.ext.spotify.SpotifyTrack`
+            when populating the ``auto_queue``.
         """
         assert self._guild is not None
 
-        if isinstance(track, spotify.SpotifyTrack):
+        if isinstance(track, YouTubeTrack) and self.autoplay and populate:
+            query: str = f'https://www.youtube.com/watch?v={track.identifier}&list=RD{track.identifier}'
+
+            recos: YouTubePlaylist = await self.current_node.get_playlist(query=query, cls=YouTubePlaylist)
+            recos: list[YouTubeTrack] = getattr(recos, 'tracks', [])
+
+            queues = set(self.queue) | set(self.auto_queue) | set(self.auto_queue.history) | {track}
+
+            for track_ in recos:
+                if track_ in queues:
+                    continue
+
+                await self.auto_queue.put_wait(track_)
+
+            self.auto_queue.shuffle()
+
+        elif isinstance(track, spotify.SpotifyTrack):
             original = track
             track = await track.fulfill(player=self, cls=YouTubeTrack, populate=populate)
 
+            if populate:
+                self.auto_queue.shuffle()
+
             for attr, value in original.__dict__.items():
                 if hasattr(track, attr):
-                    logger.warning(f'Unable to set attribute "{attr}" as it conflicts with new track type.')
+                    logger.warning(f'Player {self.guild.id} was unable to set attribute "{attr}" '
+                                   f'when converting a SpotifyTrack as it conflicts with the new track type.')
                     continue
 
                 setattr(track, attr, value)
 
         data = {
             'encodedTrack': track.encoded,
             'position': start or 0,
@@ -446,19 +607,25 @@
                 data=data,
                 query=f'noReplace={not replace}'
             )
 
         except InvalidLavalinkResponse as e:
             self._current = None
             self._original = None
+            logger.debug(f'Player {self._guild.id} attempted to load track: {track}, but failed: {e}')
             raise e
 
         self._player_state['track'] = resp['track']['encoded']
+
+        if not (self.queue.loop and self.queue._loaded):
+            self.queue.history.put(track)
+
         self.queue._loaded = track
 
+        logger.debug(f'Player {self._guild.id} loaded and started playing track: {track}.')
         return track
 
     async def set_volume(self, value: int) -> None:
         """|coro|
 
         Set the Player volume.
 
@@ -524,28 +691,40 @@
                                                              path=f'sessions/{self.current_node._session_id}/players',
                                                              guild_id=self._guild.id,
                                                              data={'paused': False})
 
         self._paused = False
         logger.debug(f'Player {self.guild.id} was resumed.')
 
-    async def stop(self) -> None:
+    async def stop(self, *, force: bool = True) -> None:
         """|coro|
 
         Stops the currently playing Track.
+
+        Parameters
+        ----------
+        force: Optional[bool]
+            Whether to stop the currently playing track and proceed to the next regardless if :attr:`~Queue.loop`
+            is ``True``. Defaults to ``True``.
+
+
+        .. versionchanged:: 2.6
+
+            Added the ``force`` keyword argument.
         """
         assert self._guild is not None
 
+        if force:
+            self.queue._loaded = None
+
         resp: dict[str, Any] = await self.current_node._send(method='PATCH',
                                                              path=f'sessions/{self.current_node._session_id}/players',
                                                              guild_id=self._guild.id,
                                                              data={'encodedTrack': None})
 
-        self.queue._loaded = None
-
         self._player_state['track'] = None
         logger.debug(f'Player {self.guild.id} was stopped.')
 
     async def set_filter(
         self,
         _filter: Filter,
         /, *,
@@ -572,52 +751,75 @@
         resp: dict[str, Any] = await self.current_node._send(method='PATCH',
                                                              path=f'sessions/{self.current_node._session_id}/players',
                                                              guild_id=self._guild.id,
                                                              data=data)        
 
         if self.is_playing() and seek:
             await self.seek(int(self.position))
-        logger.debug(f"Set filter:: {self._filter} ({self.channel.id})")
 
-    def _invalidate(self) -> None:
+        logger.debug(f'Player {self.guild.id} set filter to: {_filter}')
+
+    def _invalidate(self, *, silence: bool = False, before_connect: bool = False) -> None:
+        self.current_node._players.pop(self._guild.id, None)
+
+        if not before_connect:
+            self.current_node._invalidated[self._guild.id] = self
+
         try:
             self.cleanup()
+        except AttributeError:
+            pass
         except Exception as e:
             logger.debug(f'Failed to cleanup player, most likely due to never having been connected: {e}')
 
         self._voice_state = {}
         self._player_state = {}
         self.channel = None
 
-    async def _destroy(self) -> None:
-        self._invalidate()
+        if not silence:
+            logger.debug(f'Player {self._guild.id} was invalidated.')
+
+    async def _destroy(self, *, guild_id: int | None = None) -> None:
+        if self._destroyed:
+            return
+
+        self._invalidate(silence=True)
+
+        guild_id = guild_id or self._guild.id
 
         await self.current_node._send(method='DELETE',
                                       path=f'sessions/{self.current_node._session_id}/players',
-                                      guild_id=self._guild.id)
+                                      guild_id=guild_id)
 
-        del self.current_node._players[self._guild.id]
-        logger.debug(f'Player {self._guild.id} was destroyed.')
+        self._destroyed = True
+        self.current_node._invalidated.pop(guild_id, None)
+        logger.debug(f'Player {guild_id} was destroyed.')
 
     async def disconnect(self, **kwargs) -> None:
         """|coro|
 
         Disconnect the Player from voice and cleanup the Player state.
+
+        .. versionchanged:: 2.5
+
+            The discord.py Voice Client cache and Player are invalidated as soon as this is called.
         """
         self._invalidate()
         await self.guild.change_voice_state(channel=None)
 
+        logger.debug(f'Player {self._guild.id} was disconnected.')
+
     async def _swap_state(self) -> None:
         assert self._guild is not None
 
         try:
             self._player_state['track']
         except KeyError:
             return
 
         data: EncodedTrackRequest = {'encodedTrack': self._player_state['track'], 'position': self.position}
         resp: dict[str, Any] = await self.current_node._send(method='PATCH',
                                                              path=f'sessions/{self.current_node._session_id}/players',
                                                              guild_id=self._guild.id,
                                                              data=data)
 
-        logger.debug(f'Swapping State: {resp}')
+        logger.debug(f'Player {self.guild.id} is swapping State: {resp}')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Wavelink-2.5.1/wavelink/tracks.py` & `Wavelink-2.6.0/wavelink/tracks.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 __all__ = (
     'Playable',
     'Playlist',
     'YouTubeTrack',
     'GenericTrack',
     'YouTubeMusicTrack',
     'SoundCloudTrack',
-    'YouTubePlaylist'
+    'YouTubePlaylist',
+    'SoundCloudPlaylist'
 )
 
 
 _source_mapping: dict[str, TrackSource] = {
     'youtube': TrackSource.YouTube
 }
 
@@ -67,14 +68,30 @@
     def __init__(self, data: dict[str, Any]):
         self.data: dict[str, Any] = data
 
 
 class Playable(metaclass=abc.ABCMeta):
     """Base ABC Track used in all the Wavelink Track types.
 
+
+    .. container:: operations
+
+        .. describe:: str(track)
+
+            Returns a string representing the tracks name.
+
+        .. describe:: repr(track)
+
+            Returns an official string representation of this track.
+
+        .. describe:: track == other_track
+
+            Check whether a track is equal to another. A track is equal when they have the same Base64 Encoding.
+
+
     Attributes
     ----------
     data: dict[str, Any]
         The raw data received via Lavalink.
     encoded: str
         The encoded Track string.
     is_seekable: bool
@@ -117,14 +134,17 @@
         source: str | None = info.get('sourceName')
         self.source: TrackSource = _source_mapping.get(source, TrackSource.Unknown)
 
         self.uri: str | None = info.get('uri')
         self.author: str | None = info.get('author')
         self.identifier: str | None = info.get('identifier')
 
+    def __hash__(self) -> int:
+        return hash(self.encoded)
+
     def __str__(self) -> str:
         return self.title
 
     def __repr__(self) -> str:
         return f'Playable: source={self.source}, title={self.title}'
 
     def __eq__(self, other: object) -> bool:
@@ -145,44 +165,34 @@
     @overload
     @classmethod
     async def search(cls,
                      query: str,
                      /,
                      *,
                      node: Node | None = ...
-                     ) -> Self:
-        ...
-
-    @overload
-    @classmethod
-    async def search(cls,
-                     query: str,
-                     /,
-                     *,
-                     node: Node | None = ...
-                     ) -> Self | list[Self]:
+                     ) -> YouTubePlaylist:
         ...
 
     @overload
     @classmethod
     async def search(cls,
                      query: str,
                      /,
                      *,
                      node: Node | None = ...
-                     ) -> YouTubePlaylist:
+                     ) -> SoundCloudPlaylist:
         ...
 
     @classmethod
     async def search(cls,
                      query: str,
                      /,
                      *,
                      node: Node | None = None
-                     ) -> Self | list[Self]:
+                     ) -> list[Self]:
         """Search and retrieve tracks for the given query.
 
         Parameters
         ----------
         query: str
             The query to search for.
         node: Optional[:class:`wavelink.Node`]
@@ -193,14 +203,18 @@
         check = yarl.URL(query)
 
         if str(check.host) == 'youtube.com' or str(check.host) == 'www.youtube.com' and check.query.get("list") or \
                 cls.PREFIX == 'ytpl:':
 
             playlist = await NodePool.get_playlist(query, cls=YouTubePlaylist, node=node)
             return playlist
+        elif str(check.host) == 'soundcloud.com' or str(check.host) == 'www.soundcloud.com' and 'sets' in check.parts:
+
+            playlist = await NodePool.get_playlist(query, cls=SoundCloudPlaylist, node=node)
+            return playlist
         elif check.host:
             tracks = await NodePool.get_tracks(query, cls=cls, node=node)
         else:
             tracks = await NodePool.get_tracks(f'{cls.PREFIX}{query}', cls=cls, node=node)
 
         return tracks
 
@@ -296,14 +310,22 @@
 
     PREFIX: str = "scsearch:"
 
 
 class YouTubePlaylist(Playable, Playlist):
     """Represents a Lavalink YouTube playlist object.
 
+
+    .. container:: operations
+
+        .. describe:: str(playlist)
+
+            Returns a string representing the playlists name.
+
+
     Attributes
     ----------
     name: str
         The name of the playlist.
     tracks: :class:`YouTubeTrack`
         The list of :class:`YouTubeTrack` in the playlist.
     selected_track: Optional[int]
@@ -320,9 +342,50 @@
         if self.selected_track is not None:
             self.selected_track = int(self.selected_track)
 
         for track_data in data["tracks"]:
             track = YouTubeTrack(track_data)
             self.tracks.append(track)
 
+        self.source = TrackSource.YouTube
+
+    def __str__(self) -> str:
+        return self.name
+
+
+class SoundCloudPlaylist(Playable, Playlist):
+    """Represents a Lavalink SoundCloud playlist object.
+
+
+    .. container:: operations
+
+        .. describe:: str(playlist)
+
+            Returns a string representing the playlists name.
+
+
+    Attributes
+    ----------
+    name: str
+        The name of the playlist.
+    tracks: :class:`SoundCloudTrack`
+        The list of :class:`SoundCloudTrack` in the playlist.
+    selected_track: Optional[int]
+        The selected video in the playlist. This could be ``None``.
+    """
+
+    def __init__(self, data: dict):
+        self.tracks: list[SoundCloudTrack] = []
+        self.name: str = data["playlistInfo"]["name"]
+
+        self.selected_track: Optional[int] = data["playlistInfo"].get("selectedTrack")
+        if self.selected_track is not None:
+            self.selected_track = int(self.selected_track)
+
+        for track_data in data["tracks"]:
+            track = SoundCloudTrack(track_data)
+            self.tracks.append(track)
+
+        self.source = TrackSource.SoundCloud
+
     def __str__(self) -> str:
         return self.name
```

### Comparing `Wavelink-2.5.1/wavelink/types/events.py` & `Wavelink-2.6.0/wavelink/types/events.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.1/wavelink/types/request.py` & `Wavelink-2.6.0/wavelink/types/request.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.1/wavelink/websocket.py` & `Wavelink-2.6.0/wavelink/websocket.py`

 * *Files 14% similar despite different names*

```diff
@@ -83,23 +83,26 @@
         }
 
     def is_connected(self) -> bool:
         return self.socket is not None and not self.socket.closed
 
     async def connect(self) -> None:
         if self.node.status is NodeStatus.CONNECTED:
-            logger.error(f'The Node <{self.node!r}> is already in a connected state. Disregarding.')
+            logger.error(f'Node {self.node} websocket tried connecting in an already connected state. '
+                         f'Disregarding.')
             return
 
         self.node._status = NodeStatus.CONNECTING
 
-        try:
-            self._listener_task.cancel()
-        except Exception as e:
-            logger.debug(f'An error was raised while cancelling the websocket listener. {e}')
+        if self._listener_task:
+            try:
+                self._listener_task.cancel()
+            except Exception as e:
+                logger.debug(f'Node {self.node} encountered an error while cancelling the websocket listener: {e}. '
+                             f'This is likely not an issue and will not affect connection.')
 
         uri: str = self.node._host.removeprefix('https://').removeprefix('http://')
 
         if self.node._use_http:
             uri: str = f'{"https://" if self.node._secure else "http://"}{uri}'
         else:
             uri: str = f'{"wss://" if self.node._secure else "ws://"}{uri}'
@@ -125,22 +128,24 @@
         self._listener_task = asyncio.create_task(self._listen())
 
     async def _reconnect(self) -> None:
         self.node._status = NodeStatus.CONNECTING
         self.retry = self.backoff.calculate()
 
         if self.retries == 0:
-            logger.error('Wavelink 2.0 was unable to connect, and has exhausted the reconnection attempt limit. '
+            logger.error(f'Node {self.node} websocket was unable to connect, '
+                         f'and has exhausted the reconnection attempt limit. '
                          'Please check your Lavalink Node is started and your connection details are correct.')
 
             await self.cleanup()
             return
 
         retries = f'{self.retries} attempt(s) remaining.' if self.retries else ''
-        logger.error(f'Wavelink 2.0 was unable to connect, retrying connection in: "{self.retry}" seconds. {retries}')
+        logger.error(f'Node {self.node} websocket was unable to connect, retrying connection in: '
+                     f'"{self.retry}" seconds. {retries}')
 
         if self.retries:
             self.retries -= 1
 
         await asyncio.sleep(self.retry)
         await self.connect()
 
@@ -153,60 +158,73 @@
                 for player in self.node.players.copy().values():
                     await player._update_event(data=None)
 
                 self._reconnect_task = asyncio.create_task(self._reconnect())
                 return
 
             if message.data == 1011:
-                logger.error('Lavalink encountered an internal error which can not be resolved. '
+                logger.error(f'Node {self.node} websocket encountered an internal error which can not be resolved. '
                              'Make sure your Lavalink sever is up to date, and try restarting.')
 
                 await self.cleanup()
                 return
 
             if message.data is None:
-                logger.info('Received a message from Lavalink with empty data. Disregarding.')
+                logger.info(f'Node {self.node} websocket received a message from Lavalink with empty data. '
+                            f'Disregarding.')
                 continue
 
             data = message.json()
-            logger.debug(f'Received a message from Lavalink: {data}')
+            logger.debug(f'Node {self.node} websocket received a message from Lavalink: {data}')
 
             op = data.get('op', None)
             if not op:
-                logger.info('Message "op" from Lavalink was None. Disregarding.')
+                logger.info(f'Node {self.node} websocket payload "op" from Lavalink was None. Disregarding.')
                 continue
 
             if op == 'ready':
                 self.node._status = NodeStatus.CONNECTED
                 self.node._session_id = data['sessionId']
 
                 self.dispatch('node_ready', self.node)
 
             elif op == 'stats':
                 payload = ...
-                logger.debug(f'Stats Update: {data}')
+                logger.debug(f'Node {self.node} websocket received a Stats Update payload: {data}')
                 self.dispatch('stats_update', data)
 
             elif op == 'event':
-                logger.debug(f'Websocket Event: {data}')
+                logger.debug(f'Node {self.node} websocket received an event payload: {data}')
                 player = self.get_player(data)
 
-                if player is None:
-                    logger.debug('Received payload from Lavalink without an attached player. Disregarding.')
-                    continue
-
                 if data['type'] == 'WebSocketClosedEvent':
-                    logger.debug(f'WebSocketClosed Event: '
-                                 f'<code: {data["code"]}, reason: {data["reason"]}, by_discord: {data["byRemote"]}>')
+                    player = player or self.node._invalidated.get(int(data['guildId']), None)
+
+                    if not player:
+                        logger.debug(f'Node {self.node} received a WebsocketClosedEvent in an "unknown" state. '
+                                     f'Disregarding.')
+                        continue
+
+                    if self.node._invalidated.get(player.guild.id):
+                        await player._destroy()
+
+                    logger.debug(f'Node {self.node} websocket acknowledged "WebsocketClosedEvent": '
+                                 f'<code: {data["code"]}, reason: {data["reason"]}, by_discord: {data["byRemote"]}>. '
+                                 f'Cleanup on player {player.guild.id} has been completed.')
 
                     payload: WebsocketClosedPayload = WebsocketClosedPayload(data=data, player=player)
 
                     self.dispatch('websocket_closed', payload)
                     continue
 
+                if player is None:
+                    logger.debug(f'Node {self.node} received a payload from Lavalink without an attached player. '
+                                 f'Disregarding.')
+                    continue
+
                 track = await self.node.build_track(cls=wavelink.GenericTrack, encoded=data['encodedTrack'])
                 payload: TrackEventPayload = TrackEventPayload(
                     data=data,
                     track=track,
                     player=player,
                     original=player._original
                 )
@@ -222,38 +240,42 @@
 
                 elif payload.event is TrackEventType.START:
                     self.dispatch('track_start', payload)
 
             elif op == 'playerUpdate':
                 player = self.get_player(data)
                 if player is None:
-                    logger.debug('Received payload from Lavalink without an attached player. Disregarding.')
+                    logger.debug(f'Node {self.node} received a payload from Lavalink without an attached player. '
+                                 f'Disregarding.')
                     continue
 
                 await player._update_event(data)
                 self.dispatch("player_update", data)
-                logger.debug(f'Websocket Player Update: {data}')
+                logger.debug(f'Node {self.node} websocket received Player Update payload: {data}')
 
             else:
-                logger.info(f'Received unknown payload from Lavalink: <{data}>. '
-                            f'If this continues consider making a ticket on the Wavelink GitHub. '
-                            f'https://github.com/PythonistaGuild/Wavelink')
+                logger.warning(f'Received unknown payload from Lavalink: <{data}>. '
+                               f'If this continues consider making a ticket on the Wavelink GitHub. '
+                               f'https://github.com/PythonistaGuild/Wavelink')
 
     def get_player(self, payload: dict[str, Any]) -> Optional['Player']:
         return self.node.players.get(int(payload['guildId']), None)
 
     def dispatch(self, event, *args: Any, **kwargs: Any) -> None:
         self.node.client.dispatch(f"wavelink_{event}", *args, **kwargs)
+        logger.debug(f'Node {self.node} is dispatching an event: "on_wavelink_{event}".')
 
     # noinspection PyBroadException
     async def cleanup(self) -> None:
         try:
             await self.socket.close()
         except AttributeError:
             pass
 
         try:
             self._listener_task.cancel()
         except Exception:
             pass
 
         self.node._status = NodeStatus.DISCONNECTED
+
+        logger.debug(f'Successfully cleaned up websocket for node: {self.node}')
```

