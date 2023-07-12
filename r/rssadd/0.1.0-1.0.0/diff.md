# Comparing `tmp/rssadd-0.1.0-py3-none-any.whl.zip` & `tmp/rssadd-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3878 bytes, number of entries: 8
--rw-r--r--  2.0 unx     1940 b- defN 23-Jul-10 04:36 rssadd/__init__.py
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-10 04:36 rssadd/parser.py
--rw-r--r--  2.0 unx     1378 b- defN 23-Jul-10 04:36 rssadd/source_type.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-10 04:36 rssadd-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      912 b- defN 23-Jul-10 04:36 rssadd-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 04:36 rssadd-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-10 04:36 rssadd-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      603 b- defN 23-Jul-10 04:36 rssadd-0.1.0.dist-info/RECORD
-8 files, 6083 bytes uncompressed, 2830 bytes compressed:  53.5%
+Zip file size: 3971 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     2247 b- defN 23-Jul-11 23:58 rssadd/__init__.py
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-11 23:58 rssadd/parser.py
+-rw-r--r--  2.0 unx     1378 b- defN 23-Jul-11 23:58 rssadd/source_type.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-11 23:58 rssadd-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      912 b- defN 23-Jul-11 23:58 rssadd-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 23:58 rssadd-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-11 23:58 rssadd-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      603 b- defN 23-Jul-11 23:58 rssadd-1.0.0.dist-info/RECORD
+8 files, 6390 bytes uncompressed, 2923 bytes compressed:  54.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: rssadd/parser.py
 Comment: 
 
 Filename: rssadd/source_type.py
 Comment: 
 
-Filename: rssadd-0.1.0.dist-info/LICENSE
+Filename: rssadd-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: rssadd-0.1.0.dist-info/METADATA
+Filename: rssadd-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: rssadd-0.1.0.dist-info/WHEEL
+Filename: rssadd-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: rssadd-0.1.0.dist-info/top_level.txt
+Filename: rssadd-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rssadd-0.1.0.dist-info/RECORD
+Filename: rssadd-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rssadd/__init__.py

```diff
@@ -1,60 +1,69 @@
 from datetime import datetime
 from lxml.etree import parse, Element, fromstring, tostring
 
 from .parser import FeedParser
 from .source_type import SourceType
 
 
-__version__ = "0.1.0"
+__version__ = "1.0.0"
 
 _PUBDATE_FORMAT = "%a, %d %b %Y %H:%M:%S %z"
 _FEED_EMPTY = b"""<?xml version="1.0" encoding="utf-8"?>
 <rss xmlns:atom="http://www.w3.org/2005/Atom" version="2.0">
   <channel>
       <title> </title>
       <link> </link>
       <description> </description>
   </channel>
 </rss>"""
 
 
-def add_item(from_source=None, to_source=None, tags=None):
+def add_item(from_source=None, to_source=None, tags=None, max_items=None):
     if from_source is None:
         from_source = _FEED_EMPTY
     from_type = SourceType.from_source(from_source)
     to_type = SourceType.to_source(to_source)
 
     if tags is None:
         tags = []
     else:
         tags = tags.copy()
 
-    item = Element("item")
+    new_item = Element("item")
     for tag in tags:
         if isinstance(tag, str):
             tag = fromstring(tag, parser=FeedParser)
         elif not isinstance(tag, type(Element("a"))):
             raise TypeError(f"Unexpected type {tag}")
-        item.append(tag)
-    if item.find("pubDate") is None:
+        new_item.append(tag)
+    if new_item.find("pubDate") is None:
         tag = Element("pubDate")
         tag.text = datetime.now().strftime(_PUBDATE_FORMAT)
-        item.append(tag)
+        new_item.append(tag)
 
     if from_type == SourceType.ELEMENT:
         root = from_source
     elif from_type == SourceType.STRING:
         root = fromstring(from_source, parser=FeedParser)
     elif from_type == SourceType.FILE:
         tree = parse(from_source, FeedParser)
         root = tree.getroot()
 
     channel = root.find("channel")
-    channel.append(item)
+    first_item = channel.find("item")
+    if first_item is None:
+        channel.append(new_item)
+    else:
+        first_item.addprevious(new_item)
+
+    if max_items is not None:
+        items = channel.findall("item")
+        while len(items) > max_items:
+            channel.remove(items.pop(-1))
 
     kwargs = {
         "pretty_print": True,
         "xml_declaration": True,
         "encoding": "utf-8",
     }
     if to_type == SourceType.ELEMENT:
```

## Comparing `rssadd-0.1.0.dist-info/LICENSE` & `rssadd-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rssadd-0.1.0.dist-info/METADATA` & `rssadd-1.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssadd
-Version: 0.1.0
+Version: 1.0.0
 Summary: Add an item to an RSS feed
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/rssadd
 Keywords: rssadd,utility,rss,add
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

