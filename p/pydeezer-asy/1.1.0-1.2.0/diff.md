# Comparing `tmp/pydeezer_asy-1.1.0.tar.gz` & `tmp/pydeezer_asy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeezer_asy-1.1.0.tar", last modified: Sat Jul  8 13:36:59 2023, max compression
+gzip compressed data, was "pydeezer_asy-1.2.0.tar", last modified: Wed Jul 12 11:20:39 2023, max compression
```

## Comparing `pydeezer_asy-1.1.0.tar` & `pydeezer_asy-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 13:36:59.646851 pydeezer_asy-1.1.0/
--rw-rw-rw-   0        0        0      230 2023-07-08 13:36:59.645854 pydeezer_asy-1.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-08 13:36:59.578036 pydeezer_asy-1.1.0/deezer_asy/
--rw-rw-rw-   0        0        0    29534 2023-07-08 13:36:35.000000 pydeezer_asy-1.1.0/deezer_asy/DeezerAsy.py
--rw-rw-rw-   0        0        0      134 2023-07-07 16:55:48.000000 pydeezer_asy-1.1.0/deezer_asy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:36:59.601973 pydeezer_asy-1.1.0/deezer_asy/constants/
--rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/__init__.py
--rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/api_methods.py
--rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/api_urls.py
--rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/image_hosts.py
--rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/networking_settings.py
--rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/search_types.py
--rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/constants/track_formats.py
--rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-1.1.0/deezer_asy/exceptions.py
--rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-1.1.0/deezer_asy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-08 13:36:59.644858 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/
--rw-rw-rw-   0        0        0      230 2023-07-08 13:36:59.000000 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-07-08 13:36:59.000000 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 13:36:59.000000 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-08 13:36:59.000000 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-08 13:36:59.000000 pydeezer_asy-1.1.0/pydeezer_asy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 13:36:59.647850 pydeezer_asy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      445 2023-07-08 13:36:49.000000 pydeezer_asy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:20:39.785443 pydeezer_asy-1.2.0/
+-rw-rw-rw-   0        0        0      230 2023-07-12 11:20:39.785443 pydeezer_asy-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 11:20:39.725358 pydeezer_asy-1.2.0/deezer_asy/
+-rw-rw-rw-   0        0        0    30354 2023-07-12 11:17:17.000000 pydeezer_asy-1.2.0/deezer_asy/DeezerAsy.py
+-rw-rw-rw-   0        0        0      134 2023-07-07 16:55:48.000000 pydeezer_asy-1.2.0/deezer_asy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:20:39.744308 pydeezer_asy-1.2.0/deezer_asy/constants/
+-rw-rw-rw-   0        0        0      193 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/__init__.py
+-rw-rw-rw-   0        0        0      789 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/api_methods.py
+-rw-rw-rw-   0        0        0      191 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/api_urls.py
+-rw-rw-rw-   0        0        0      124 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/image_hosts.py
+-rw-rw-rw-   0        0        0      392 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/networking_settings.py
+-rw-rw-rw-   0        0        0       72 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/search_types.py
+-rw-rw-rw-   0        0        0      694 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/constants/track_formats.py
+-rw-rw-rw-   0        0        0      140 2023-05-22 20:25:26.000000 pydeezer_asy-1.2.0/deezer_asy/exceptions.py
+-rw-rw-rw-   0        0        0     2004 2023-07-07 16:54:00.000000 pydeezer_asy-1.2.0/deezer_asy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:20:39.782452 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/
+-rw-rw-rw-   0        0        0      230 2023-07-12 11:20:39.000000 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-07-12 11:20:39.000000 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:20:39.000000 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-12 11:20:39.000000 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-12 11:20:39.000000 pydeezer_asy-1.2.0/pydeezer_asy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 11:20:39.786440 pydeezer_asy-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      500 2023-07-12 11:20:28.000000 pydeezer_asy-1.2.0/setup.py
```

### Comparing `pydeezer_asy-1.1.0/deezer_asy/DeezerAsy.py` & `pydeezer_asy-1.2.0/deezer_asy/DeezerAsy.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,36 @@
 import mutagen
 import aiofiles
 from mutagen.id3 import ID3, APIC
 from mutagen.easyid3 import EasyID3
 from os import path, remove
 import hashlib
 import httpx
-
-
+from  threading import Thread
 
 from .constants import *
 
 from .exceptions import LoginError
 from .exceptions import APIRequestError
 from .exceptions import DownloadLinkDecryptionError
 
 from . import util
 
 
+class ResultThread(Thread):
+    def __init__(self, *args, **kwargs):
+        super(ResultThread, self).__init__(*args, **kwargs)
+        self._result = None
+
+    def run(self):
+        self._result = self._target(*self._args, **self._kwargs)
+
+    def result(self):
+        return self._result
+
 class DeezerAsy:
     def __init__(self, arl) -> None:
         """Instantiates a Deezer object
 
         Keyword Arguments:
             arl {str} -- Login using the given arl (default: {None})
         """
@@ -722,14 +732,15 @@
             if not lyric_check[0]:
                 asyncio.get_event_loop().run_in_executor(None, remove, lyric_check[1])
                 return (download_path)
 
             return (download_path, lyric_check[1])
 
         return (download_path)
+    
     async def get_tracks(self, track_ids):
         """Gets the list of the tracks that corresponds with the given {track_ids}
 
         Arguments:
             track_ids {list} -- List of track id
 
         Returns:
@@ -806,38 +817,51 @@
         return (True, save_path)
     
     """
         TAG EDIT
 
         p.s: It might be blocking the thread, not sure
     """
-    async def _write_mp3_tags(self, path, track, tags=None):
-        track = track["DATA"] if "DATA" in track else track
-
-        if not tags:
-            tags = await self.get_track_tags(track)
+    async def __write_mp3_tags(self, path, track, tags=None):
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+        _result = loop.run_until_complete(self._write_mp3_tags(path, track, tags))
+        result = await _result
 
+        return result
+    
+    def __update_mp3(self, path, tags):
         audio = mutagen.File(path, easy=True)
         if audio is None:
             raise ValueError("Invalid file format")
 
         audio.delete()
         EasyID3.RegisterTextKey("label", "TPUB")
 
         cover = tags["_albumart"]
         del tags["_albumart"]
 
         for key, val in tags.items():
             if val:
                 audio[key] = str(val)
-        audio.save()
+        
 
         if cover:
             cover_handle = ID3(path)
             cover_handle["APIC"] = APIC(
                 type=3,
                 mime=cover["mime_type"],
                 data=cover["image"]
             )
             cover_handle.save(path)
+        audio.save()
+
+    async def _write_mp3_tags(self, path, track, tags=None):
+        track = track["DATA"] if "DATA" in track else track
+
+        if not tags:
+            tags = await self.get_track_tags(track)
 
+        _update_tags = ResultThread(target=self.__update_mp3, args=(path, tags,))
+        _update_tags.start()
+        _update_tags.join()
         return True
```

### Comparing `pydeezer_asy-1.1.0/deezer_asy/constants/api_methods.py` & `pydeezer_asy-1.2.0/deezer_asy/constants/api_methods.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.1.0/deezer_asy/constants/track_formats.py` & `pydeezer_asy-1.2.0/deezer_asy/constants/track_formats.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.1.0/deezer_asy/util.py` & `pydeezer_asy-1.2.0/deezer_asy/util.py`

 * *Files identical despite different names*

### Comparing `pydeezer_asy-1.1.0/pydeezer_asy.egg-info/SOURCES.txt` & `pydeezer_asy-1.2.0/pydeezer_asy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

