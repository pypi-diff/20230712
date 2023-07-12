# Comparing `tmp/last_fm_api_client-0.2.2.tar.gz` & `tmp/last_fm_api_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "last_fm_api_client-0.2.2.tar", max compression
+gzip compressed data, was "last_fm_api_client-0.2.3.tar", max compression
```

## Comparing `last_fm_api_client-0.2.2.tar` & `last_fm_api_client-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-28 17:55:46.624956 last_fm_api_client-0.2.2/last_fm_api_client/__init__.py
--rw-r--r--   0        0        0    11414 2023-06-03 18:30:38.302558 last_fm_api_client-0.2.2/last_fm_api_client/client.py
--rw-r--r--   0        0        0    10120 2023-06-20 18:40:55.197491 last_fm_api_client-0.2.2/last_fm_api_client/models.py
--rw-r--r--   0        0        0      383 2023-06-20 18:42:56.258685 last_fm_api_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1037 2023-06-20 18:42:43.830654 last_fm_api_client-0.2.2/README.md
--rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 last_fm_api_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-28 17:55:46.624956 last_fm_api_client-0.2.3/last_fm_api_client/__init__.py
+-rw-r--r--   0        0        0    11414 2023-06-03 18:30:38.302558 last_fm_api_client-0.2.3/last_fm_api_client/client.py
+-rw-r--r--   0        0        0    10190 2023-07-12 19:01:01.648159 last_fm_api_client-0.2.3/last_fm_api_client/models.py
+-rw-r--r--   0        0        0      383 2023-07-12 19:01:19.291143 last_fm_api_client-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1204 2023-07-12 19:01:01.642144 last_fm_api_client-0.2.3/README.md
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 last_fm_api_client-0.2.3/PKG-INFO
```

### Comparing `last_fm_api_client-0.2.2/last_fm_api_client/client.py` & `last_fm_api_client-0.2.3/last_fm_api_client/client.py`

 * *Files identical despite different names*

### Comparing `last_fm_api_client-0.2.2/last_fm_api_client/models.py` & `last_fm_api_client-0.2.3/last_fm_api_client/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,17 @@
     """Represents data for a detailed tag in the Last.FM database (as retrieved from the tag.getInfo) method"""
     name: str
     total: int
     reach: int
     wiki: TagDetailsWiki
 
 class Tags(BaseModel):
-    """Represents a list of tags."""
-    tag: List[Tag]
+    """Represents a list of tags or a single tag under the "tags" key (new since v0.2.3)."""
+    tag: Union[List[Tag], Tag]
+
 
 # Artist-related  things
 class ArtistStats(BaseModel):
     """Represents Last.FM stats for an artist."""
     listeners: int
     playcount: int
```

### Comparing `last_fm_api_client-0.2.2/README.md` & `last_fm_api_client-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 The following [Last.FM API methods](https://www.last.fm/api/intro) are implemented:
 * `album.getInfo` - get information about an album
 * `artist.getInfo` - get information about an artist
 * `tag.getInfo` - get information about a tag
 * `user.getRecentTracks` - retrieve scrobbles
 
 ### Changelog:
+* `v0.2.3`: Fixed a bug that crashed the deserialization if an album only had one tag, which made
+Last.FM return a dictionary rather than a list containing the tag.
 * `v0.2.2`: Fixed a bug related to the loading of album images.
   
   **Breaking changes**
     * The field `Image.size` is now optional and may return `None`.  
 * `v0.2.1`: Fixed empty album text being converted to None.
 * `v0.2.0`: Better handling of unset/empty Last.FM values.
```

### Comparing `last_fm_api_client-0.2.2/PKG-INFO` & `last_fm_api_client-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: last-fm-api-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: William04A
 Author-email: 35110380+William04A@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,14 +23,16 @@
 The following [Last.FM API methods](https://www.last.fm/api/intro) are implemented:
 * `album.getInfo` - get information about an album
 * `artist.getInfo` - get information about an artist
 * `tag.getInfo` - get information about a tag
 * `user.getRecentTracks` - retrieve scrobbles
 
 ### Changelog:
+* `v0.2.3`: Fixed a bug that crashed the deserialization if an album only had one tag, which made
+Last.FM return a dictionary rather than a list containing the tag.
 * `v0.2.2`: Fixed a bug related to the loading of album images.
   
   **Breaking changes**
     * The field `Image.size` is now optional and may return `None`.  
 * `v0.2.1`: Fixed empty album text being converted to None.
 * `v0.2.0`: Better handling of unset/empty Last.FM values.
```

