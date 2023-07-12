# Comparing `tmp/rssadd-1.0.0-py3-none-any.whl.zip` & `tmp/rssadd-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3971 bytes, number of entries: 8
--rw-r--r--  2.0 unx     2247 b- defN 23-Jul-11 23:58 rssadd/__init__.py
--rw-r--r--  2.0 unx       82 b- defN 23-Jul-11 23:58 rssadd/parser.py
--rw-r--r--  2.0 unx     1378 b- defN 23-Jul-11 23:58 rssadd/source_type.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jul-11 23:58 rssadd-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      912 b- defN 23-Jul-11 23:58 rssadd-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 23:58 rssadd-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-11 23:58 rssadd-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      603 b- defN 23-Jul-11 23:58 rssadd-1.0.0.dist-info/RECORD
-8 files, 6390 bytes uncompressed, 2923 bytes compressed:  54.3%
+Zip file size: 4010 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     2458 b- defN 23-Jul-12 03:10 rssadd/__init__.py
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-12 03:10 rssadd/parser.py
+-rw-r--r--  2.0 unx     1378 b- defN 23-Jul-12 03:10 rssadd/source_type.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-12 03:10 rssadd-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      912 b- defN 23-Jul-12 03:10 rssadd-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 03:10 rssadd-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-12 03:10 rssadd-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      603 b- defN 23-Jul-12 03:10 rssadd-1.1.0.dist-info/RECORD
+8 files, 6601 bytes uncompressed, 2962 bytes compressed:  55.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: rssadd/parser.py
 Comment: 
 
 Filename: rssadd/source_type.py
 Comment: 
 
-Filename: rssadd-1.0.0.dist-info/LICENSE
+Filename: rssadd-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: rssadd-1.0.0.dist-info/METADATA
+Filename: rssadd-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: rssadd-1.0.0.dist-info/WHEEL
+Filename: rssadd-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: rssadd-1.0.0.dist-info/top_level.txt
+Filename: rssadd-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rssadd-1.0.0.dist-info/RECORD
+Filename: rssadd-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rssadd/__init__.py

```diff
@@ -1,64 +1,48 @@
 from datetime import datetime
 from lxml.etree import parse, Element, fromstring, tostring
 
 from .parser import FeedParser
 from .source_type import SourceType
 
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 _PUBDATE_FORMAT = "%a, %d %b %Y %H:%M:%S %z"
 _FEED_EMPTY = b"""<?xml version="1.0" encoding="utf-8"?>
 <rss xmlns:atom="http://www.w3.org/2005/Atom" version="2.0">
   <channel>
       <title> </title>
       <link> </link>
       <description> </description>
   </channel>
 </rss>"""
 
 
-def add_item(from_source=None, to_source=None, tags=None, max_items=None):
+def add_element(from_source=None, to_source=None, element=None, max_items=None):
     if from_source is None:
         from_source = _FEED_EMPTY
     from_type = SourceType.from_source(from_source)
     to_type = SourceType.to_source(to_source)
 
-    if tags is None:
-        tags = []
-    else:
-        tags = tags.copy()
-
-    new_item = Element("item")
-    for tag in tags:
-        if isinstance(tag, str):
-            tag = fromstring(tag, parser=FeedParser)
-        elif not isinstance(tag, type(Element("a"))):
-            raise TypeError(f"Unexpected type {tag}")
-        new_item.append(tag)
-    if new_item.find("pubDate") is None:
-        tag = Element("pubDate")
-        tag.text = datetime.now().strftime(_PUBDATE_FORMAT)
-        new_item.append(tag)
-
     if from_type == SourceType.ELEMENT:
         root = from_source
     elif from_type == SourceType.STRING:
         root = fromstring(from_source, parser=FeedParser)
     elif from_type == SourceType.FILE:
         tree = parse(from_source, FeedParser)
         root = tree.getroot()
-
     channel = root.find("channel")
-    first_item = channel.find("item")
-    if first_item is None:
-        channel.append(new_item)
-    else:
-        first_item.addprevious(new_item)
+
+    if element is not None:
+        first_item = channel.find("item")
+        if first_item is None:
+            channel.append(element)
+        else:
+            first_item.addprevious(element)
 
     if max_items is not None:
         items = channel.findall("item")
         while len(items) > max_items:
             channel.remove(items.pop(-1))
 
     kwargs = {
@@ -71,8 +55,29 @@
     if to_type == SourceType.STRING:
         return tostring(root, **kwargs)
     if to_type == SourceType.FILE:
         return tree.write(to_source, **kwargs)
     raise Exception("Unexpected value for to_source type")
 
 
-__all__ = ("add_item",)
+def add_item(from_source=None, to_source=None, tags=None, max_items=None):
+    if tags is None:
+        tags = []
+    else:
+        tags = tags.copy()
+
+    new_item = Element("item")
+    for tag in tags:
+        if isinstance(tag, str):
+            tag = fromstring(tag, parser=FeedParser)
+        elif not isinstance(tag, type(Element("a"))):
+            raise TypeError(f"Unexpected type {tag}")
+        new_item.append(tag)
+    if new_item.find("pubDate") is None:
+        tag = Element("pubDate")
+        tag.text = datetime.now().strftime(_PUBDATE_FORMAT)
+        new_item.append(tag)
+
+    return add_element(from_source, to_source, new_item, max_items)
+
+
+__all__ = ("add_element", "add_item")
```

## Comparing `rssadd-1.0.0.dist-info/LICENSE` & `rssadd-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rssadd-1.0.0.dist-info/METADATA` & `rssadd-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssadd
-Version: 1.0.0
+Version: 1.1.0
 Summary: Add an item to an RSS feed
 Author-email: Matt Wisniewski <healthycrowd@mattw.life>
 License: MIT
 Project-URL: homepage, https://github.com/healthycrowd/rssadd
 Keywords: rssadd,utility,rss,add
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

