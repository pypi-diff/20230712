# Comparing `tmp/fuo_kuwo-0.1.6.tar.gz` & `tmp/fuo-kuwo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuo_kuwo-0.1.6.tar", last modified: Wed Jun  8 09:00:01 2022, max compression
+gzip compressed data, was "fuo-kuwo-0.2.0.tar", last modified: Wed Jul 12 17:02:22 2023, max compression
```

## Comparing `fuo_kuwo-0.1.6.tar` & `fuo-kuwo-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 09:00:01.000000 fuo_kuwo-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 09:00:01.000000 fuo_kuwo-0.1.6/fuo_kuwo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-08 09:00:00.000000 fuo_kuwo-0.1.6/fuo_kuwo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 09:00:00.000000 fuo_kuwo-0.1.6/fuo_kuwo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-08 09:00:00.000000 fuo_kuwo-0.1.6/fuo_kuwo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-06-08 09:00:01.000000 fuo_kuwo-0.1.6/fuo_kuwo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-06-08 09:00:00.000000 fuo_kuwo-0.1.6/fuo_kuwo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-08 09:00:00.000000 fuo_kuwo-0.1.6/fuo_kuwo.egg-info/requires.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 09:00:01.000000 fuo_kuwo-0.1.6/fuo_kuwo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 09:00:01.000000 fuo_kuwo-0.1.6/fuo_kuwo/enc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/enc/decrypt.py
--rw-r--r--   0 runner    (1001) docker     (121)     6870 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/enc/DES.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     5507 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16935 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    10678 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 09:00:01.000000 fuo_kuwo-0.1.6/fuo_kuwo/assets/
--rw-r--r--   0 runner    (1001) docker     (121)    14913 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/fuo_kuwo/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-08 09:00:01.000000 fuo_kuwo-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-06-08 08:59:57.000000 fuo_kuwo-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-06-08 09:00:01.000000 fuo_kuwo-0.1.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.227140 fuo-kuwo-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-12 17:02:22.227140 fuo-kuwo-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.223140 fuo-kuwo-0.2.0/fuo_kuwo/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.223140 fuo-kuwo-0.2.0/fuo_kuwo/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/assets/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.223140 fuo-kuwo-0.2.0/fuo_kuwo/enc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/enc/DES.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/enc/decrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.227140 fuo-kuwo-0.2.0/fuo_kuwo/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/pages/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.223140 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:02:22.227140 fuo-kuwo-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fuo_kuwo-0.1.6/fuo_kuwo/enc/decrypt.py` & `fuo-kuwo-0.2.0/fuo_kuwo/enc/decrypt.py`

 * *Files identical despite different names*

### Comparing `fuo_kuwo-0.1.6/fuo_kuwo/enc/DES.py` & `fuo-kuwo-0.2.0/fuo_kuwo/enc/DES.py`

 * *Files identical despite different names*

### Comparing `fuo_kuwo-0.1.6/fuo_kuwo/ui.py` & `fuo-kuwo-0.2.0/fuo_kuwo/ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import os
 from pathlib import Path
 
 from feeluown.consts import DATA_DIR
+from feeluown.library import BriefUserModel
 from feeluown.gui.widgets import CookiesLoginDialog
 from feeluown.gui.widgets.login import InvalidCookies
 from feeluown.uimodels.provider import ProviderUiManager
 from feeluown.utils import aio
 
-from . import __alias__
+from . import __identifier__, __alias__
 from .provider import provider
 
 USER_INFO_FILE = DATA_DIR + '/kuwo_music_user_session.json'
 
 
 class KuwoUiManager:
     def __init__(self, app):
@@ -22,30 +23,41 @@
             name='kuwo',
             text=__alias__,
             symbol='♫ ',
             desc='点击登录',
             colorful_svg=str(Path(__file__).resolve().parent / 'assets' / 'icon.svg'))
         self._pvd_item.clicked.connect(self.login_or_show)
         self._pvd_uimgr.add_item(self._pvd_item)
+        self.initialize()
 
     def login_or_show(self):
         if provider.user is None:
             dialog = LoginDialog()
-            dialog.login_succeed.connect(self.load_user)
+            dialog.login_succeed.connect(lambda: aio.run_afn(self.load_user))
             dialog.show()
             dialog.autologin()
         else:
-            self.load_user()
+            aio.run_afn(self.load_user)
 
-    def load_user(self):
-        user = provider.user
-        self._app.ui.left_panel.my_music_con.hide()
+    def initialize(self):
+        from .pages.explorer import render as explore_render # noqa
+        self._app.browser.route('/providers/kuwo/explore')(explore_render)
+
+    async def load_user(self):
+        self._app.ui.left_panel.my_music_con.show()
         self._app.ui.left_panel.playlists_con.show()
         self._app.pl_uimgr.clear()
-        self._app.pl_uimgr.add(user.playlists)
+        user_playlists = await aio.run_fn(provider.current_user_playlists)
+        self._app.pl_uimgr.add(user_playlists)
+        kw_explore_item = self._app.mymusic_uimgr.create_item('🎵 发现音乐')
+        kw_explore_item.clicked.connect(
+            lambda: self._app.browser.goto(page='/providers/kuwo/explore'),
+            weak=False)
+        self._app.mymusic_uimgr.clear()
+        self._app.mymusic_uimgr.add_item(kw_explore_item)
         self._pvd_item.text = f'{__alias__} - 已登录'
 
 
 class LoginDialog(CookiesLoginDialog):
 
     def setup_user(self, user):
         provider.user = user
@@ -57,15 +69,15 @@
         userid, sid = provider.api.get_user_from_cookies(cookies)
         if not userid:
             raise InvalidCookies("can't extract user info from cookies")
 
         provider.api.set_cookies(cookies)
         # try to extract current user
         try:
-            user = await aio.run_in_executor(None, provider.User.get, userid)
+            user = BriefUserModel(source=__identifier__, identifier=userid)
         except Exception:
             provider.api.set_cookies(None)
             raise InvalidCookies('get user info with cookies failed, expired cookies?')
         else:
             return user
 
     def load_user_cookies(self):
```

### Comparing `fuo_kuwo-0.1.6/fuo_kuwo/schemas.py` & `fuo-kuwo-0.2.0/fuo_kuwo/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import unicodedata
 import html
 
 from marshmallow import Schema, fields, post_load, EXCLUDE
+from feeluown.library import (
+    SongModel, BriefAlbumModel, BriefArtistModel,
+    AlbumModel, ArtistModel, PlaylistModel, BriefPlaylistModel,
+)
+
+SOURCE = 'kuwo'
 
 
 def normalize_str(s):
     # String returned from kuwo server may contain charactor
     # which is supposed to normalized.
     #
     # For example, there may be '&nbsp' in album name, which is
@@ -31,128 +37,137 @@
     identifier = fields.Int(data_key='rid', required=True)
     duration = fields.Int(data_key='duration', required=True)
     title = fields.Str(data_key='name', required=True)
     artist = fields.Str(data_key='artist', required=True)
     artistid = fields.Int(data_key='artistid', required=True)
     album = fields.Str(data_key='album', required=False)
     albumid = fields.Int(data_key='albumid', required=False)
-    albumpic = fields.Str(data_key='albumpic', required=False)
+    albumpic = fields.Str(data_key='albumpic', required=False, missing='')
     lossless = fields.Bool(data_key='hasLossless', required=False)
     hasmv = fields.Int(data_key='hasmv', required=False)
 
     @post_load
     def create_model(self, data, **kwargs):
         if data.get('artistid'):
             artists = [
-                KuwoArtistModel(
+                BriefArtistModel(
+                    source=SOURCE,
                     identifier=data.get('artistid'),
                     name=normalize_field(data.get('artist'))
                 )
             ]
         else:
             artists = []
         if data.get('albumid'):
-            album = KuwoAlbumModel(identifier=data.get('albumid'),
-                                   name=normalize_field(data.get('album')),
-                                   cover=data.get('albumpic', ''))
+            album = BriefAlbumModel(
+                source=SOURCE,
+                identifier=data.get('albumid'),
+                name=normalize_field(data.get('album')),
+            )
         else:
             album = None
-        return KuwoSongModel(identifier=data.get('identifier'),
-                             duration=data.get('duration') * 1000,
-                             title=normalize_field(data.get('title')),
-                             artists=artists,
-                             album=album,
-                             lossless=data.get('lossless', False),
-                             hasmv=data.get('hasmv', 0))
+        song = SongModel(
+            source=SOURCE,
+            identifier=str(data.get('identifier')),
+            duration=data.get('duration') * 1000,
+            title=normalize_field(data.get('title')),
+            artists=artists,
+            album=album,
+            pic_url=data['albumpic'],
+        )
+        song.cache_set('lossless', data.get('lossless', False))  # bool
+        song.cache_set('hasmv', bool(data.get('hasmv', 0)))  # int
+        return song
 
 
 class KuwoAlbumSchema(Schema):
     identifier = fields.Int(data_key='albumid', required=True)
     name = fields.Str(data_key='album', required=True)
-    cover = fields.Str(data_key='pic', required=False)
+    cover = fields.Str(data_key='pic', required=False, missing='')
     artist = fields.Str(data_key='artist', required=True)
     artistid = fields.Int(data_key='artistid', required=True)
     albuminfo = fields.Str(data_key='albuminfo', required=False)
     songs = fields.List(fields.Nested('KuwoSongSchema'),
                         data_key='musicList',
                         allow_none=True, required=False)
+    song_count = fields.Int(data_key='total', required=False, missing=-1)
+    released = fields.Str(data_key='releaseDate', required=True)
 
     @post_load
     def create_model(self, data, **kwargs):
-        return KuwoAlbumModel(
+        return AlbumModel(
+            source=SOURCE,
             identifier=data.get('identifier'),
             name=normalize_field(data.get('name')),
-            artists=[KuwoArtistModel(
+            artists=[BriefArtistModel(
+                source=SOURCE,
                 identifier=data.get('artistid'),
                 name=normalize_field(data.get('artist')))],
-            desc=normalize_field(data.get('albuminfo', '')).replace('\n', '<br>'),
+            description=normalize_field(data.get('albuminfo', '')).replace('\n', '<br>'),
             cover=data.get('cover'),
-            songs=[],
-            _songs=data.get('songs')
+            songs=data.get('songs') or [],
+            song_count=data['song_count'],
+            released=data['released'],
         )
 
 
-class KuwoArtistSchema(Schema):
+class KuwoBriefArtistSchema(Schema):
     identifier = fields.Int(data_key='id', required=True)
     name = fields.Str(data_key='name', required=True)
-    pic = fields.Str(data_key='pic', required=False)
-    pic300 = fields.Str(data_key='pic300', required=False)
-    desc = fields.Str(data_key='info', required=False)
 
     @post_load
     def create_model(self, data, **kwargs):
-        return KuwoArtistModel(
+        return BriefArtistModel(
+            source=SOURCE,
+            identifier=data.get['identifier'],
+            name=normalize_field(data.get['name']),
+        )
+
+
+class KuwoArtistSchema(KuwoBriefArtistSchema):
+    pic = fields.Str(data_key='pic', required=False, missing='')
+    pic300 = fields.Str(data_key='pic300', required=False, missing='')
+    desc = fields.Str(data_key='info', required=False, missing='')
+
+    @post_load
+    def create_model(self, data, **kwargs):
+        return ArtistModel(
+            source=SOURCE,
             identifier=data.get('identifier'),
             name=normalize_field(data.get('name')),
-            cover=data.get('pic300'),
-            desc=data.get('desc'), info=data.get('desc')
+            pic_url=data.get('pic300'),
+            aliases=[],
+            hot_songs=[],
+            description=normalize_field(data.get('desc')),
         )
 
 
 class KuwoPlaylistSchema(Schema):
     identifier = fields.Int(data_key='id', required=True)
-    cover = fields.Str(data_key='img', required=False)
+    cover = fields.Str(data_key='img', required=False, missing='')
     name = fields.Str(data_key='name', required=True)
-    desc = fields.Str(data_key='info', required=False)
-    songs = fields.List(fields.Nested('KuwoSongSchema'),
-                        data_key='musicList',
-                        allow_none=True,
-                        required=False)
+    desc = fields.Str(data_key='info', required=False, missing='')
 
     @post_load
     def create_model(self, data, **kwargs):
-        return KuwoPlaylistModel(
+        return PlaylistModel(
+            source=SOURCE,
             identifier=data.get('identifier'),
+            creator=None,
             name=normalize_field(data.get('name')),
             cover=data.get('cover'),
-            desc=data.get('desc'),
-            songs=data.get('songs')
+            description=data.get('desc'),
         )
 
 
 class KuwoUserPlaylistSchema(Schema):
     identifier = fields.Int(data_key='id', required=True)
     cover = fields.Str(data_key='pic', required=False)
     name = fields.Str(data_key='title', required=True)
 
     @post_load
     def create_model(self, data, **kwargs):
-        return KuwoPlaylistModel(
+        return BriefPlaylistModel(
+            source=SOURCE,
             identifier=data.get('identifier'),
             name=normalize_field(data.get('name')),
-            cover=data.get('cover'),
-            desc='',
-            songs=None
-        )
-
-
-class KuwoUserSchema(Schema):
-    identifier = fields.Str(data_key='id', required=True)
-
-    @post_load
-    def create_model(self, data, **kwargs):
-        return KuwoUserModel(
-            identifier=data.get('identifier', '')
         )
-
-
-from .models import KuwoSongModel, KuwoArtistModel, KuwoAlbumModel, KuwoPlaylistModel, KuwoUserModel
```

### Comparing `fuo_kuwo-0.1.6/fuo_kuwo/__init__.py` & `fuo-kuwo-0.2.0/fuo_kuwo/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_kuwo-0.1.6/fuo_kuwo/api.py` & `fuo-kuwo-0.2.0/fuo_kuwo/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
-
 import time
 from pathlib import Path
+from hashlib import md5
 
 import requests
 from requests.cookies import RequestsCookieJar
 from fuo_kuwo.enc.DES import base64_encrypt
 from fuo_kuwo.utils import digest_encrypt
 
 logger = logging.getLogger(__name__)
@@ -63,29 +63,22 @@
             'Accept-Language': 'zh-CN,zh;q=0.8,gl;q=0.6,zh-TW;q=0.4',
             'Referer': 'http://kuwo.cn',
             'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) '
                           'Chrome/81.0.4044.138 Safari/537.36',
             'Host': 'kuwo.cn',
         }
         self.mobi_headers = {'User-Agent': 'okhttp/3.10.0'}
-        self.get_cookie_token()
-        self.headers['csrf'] = self.token
+        random_str = '123456789'
+        self.headers['csrf'] = random_str
+        self.cookie = {'kw_token': random_str, 'Hm_token': random_str}
+        self.headers['Cross'] = md5(random_str.encode('utf-8')).hexdigest()
         self._userid = ''
         self._sid = ''
         self._cookies = {}
 
-    def get_cookie_token(self):
-        """get kuwo token & set cookie jar"""
-        token_uri = KuwoApi.HTTP_HOST + '/search/list?key=hello'
-        with requests.Session() as session:
-            response = session.get(token_uri, headers=self.headers)
-            token = response.cookies.get('kw_token')
-            self.token = token
-            self.cookie = response.cookies
-
     def set_cookies(self, cookies):
         if cookies:
             self._cookies = cookies
             self._userid, self._sid = self.get_user_from_cookies(cookies)
         else:
             self._cookies, self._userid, self._sid = {}, '', ''
```

### Comparing `fuo_kuwo-0.1.6/fuo_kuwo/utils.py` & `fuo-kuwo-0.2.0/fuo_kuwo/utils.py`

 * *Files identical despite different names*

### Comparing `fuo_kuwo-0.1.6/fuo_kuwo/assets/icon.svg` & `fuo-kuwo-0.2.0/fuo_kuwo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo_kuwo-0.1.6/README.md` & `fuo-kuwo-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,45 @@
+Metadata-Version: 2.1
+Name: fuo-kuwo
+Version: 0.2.0
+Summary: Kuwo music provider for FeelUOwn music player
+Home-page: https://github.com/feeluown/feeluown-kuwo
+Author: feeluown team
+Requires-Python: >=3.8,<4.0
+License-File: LICENSE
+
 # Kuwo music provider for FeelUOwn player
 
 ## Installation
 
 ### Arch Linux
 `pacman -S feeluown-kuwo`
 
 ### Install from pypi
 `pip install --user feeluown-kuwo`
 
 ### Install with pip
 `pip install --user .`
 
-## Development with pipenv
-`pipenv install` to create venv and start development.
+## Development with poetry
+`poetry install` to create venv and start development.
+`poetry run pre-commit install` to setup git pre-commit hooks.
+`poetry run poetry2setup > setup.py` before commit.
 
 ## Run tests
 `pytest -v`
 
 test_kuwo_api.py -- Kuwo API tests
 
 ## Changelog
 
+### v0.2.0 (2023-07-13)
+* 修复 API 不可用的问题
+* 适配 feeluown v2 model，废弃 v1 models
+
 ### v0.1.6 (2022-06-08)
 * 修复获取歌曲/mv播放链接有一定概率会失败的问题
 
 ### v0.1.5 (2021-11-06)
 * 处理 html 字符实体
 
 ### v0.1.4 (2021-05-27)
```

