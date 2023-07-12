# Comparing `tmp/modernmt-1.3.0.tar.gz` & `tmp/modernmt-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernmt-1.3.0.tar", last modified: Thu Jun 15 09:18:59 2023, max compression
+gzip compressed data, was "modernmt-1.4.0.tar", last modified: Wed Jul 12 14:06:40 2023, max compression
```

## Comparing `modernmt-1.3.0.tar` & `modernmt-1.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-15 09:18:59.652890 modernmt-1.3.0/
--rw-rw-r--   0 davide    (1000) davide    (1000)     1065 2021-05-05 13:02:28.000000 modernmt-1.3.0/LICENSE
--rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-06-15 09:18:59.652890 modernmt-1.3.0/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      197 2021-05-05 13:02:28.000000 modernmt-1.3.0/README.md
--rw-rw-r--   0 davide    (1000) davide    (1000)      105 2021-05-05 13:02:28.000000 modernmt-1.3.0/pyproject.toml
--rw-rw-r--   0 davide    (1000) davide    (1000)      655 2023-06-15 09:18:59.652890 modernmt-1.3.0/setup.cfg
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-15 09:18:59.648890 modernmt-1.3.0/src/
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-15 09:18:59.648890 modernmt-1.3.0/src/modernmt/
--rw-rw-r--   0 davide    (1000) davide    (1000)      166 2021-05-05 13:02:28.000000 modernmt-1.3.0/src/modernmt/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)    12266 2023-06-15 09:18:35.000000 modernmt-1.3.0/src/modernmt/modernmt.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-15 09:18:59.652890 modernmt-1.3.0/src/modernmt.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-06-15 09:18:59.000000 modernmt-1.3.0/src/modernmt.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      271 2023-06-15 09:18:59.000000 modernmt-1.3.0/src/modernmt.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-06-15 09:18:59.000000 modernmt-1.3.0/src/modernmt.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       15 2023-06-15 09:18:59.000000 modernmt-1.3.0/src/modernmt.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        9 2023-06-15 09:18:59.000000 modernmt-1.3.0/src/modernmt.egg-info/top_level.txt
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-12 14:06:40.168267 modernmt-1.4.0/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1065 2021-05-05 13:02:28.000000 modernmt-1.4.0/LICENSE
+-rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-07-12 14:06:40.168267 modernmt-1.4.0/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      197 2021-05-05 13:02:28.000000 modernmt-1.4.0/README.md
+-rw-rw-r--   0 davide    (1000) davide    (1000)      105 2021-05-05 13:02:28.000000 modernmt-1.4.0/pyproject.toml
+-rw-rw-r--   0 davide    (1000) davide    (1000)      655 2023-07-12 14:06:40.168267 modernmt-1.4.0/setup.cfg
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-12 14:06:40.168267 modernmt-1.4.0/src/
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-12 14:06:40.168267 modernmt-1.4.0/src/modernmt/
+-rw-rw-r--   0 davide    (1000) davide    (1000)      166 2021-05-05 13:02:28.000000 modernmt-1.4.0/src/modernmt/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)    12746 2023-07-12 14:06:16.000000 modernmt-1.4.0/src/modernmt/modernmt.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-07-12 14:06:40.168267 modernmt-1.4.0/src/modernmt.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)      690 2023-07-12 14:06:40.000000 modernmt-1.4.0/src/modernmt.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      271 2023-07-12 14:06:40.000000 modernmt-1.4.0/src/modernmt.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-07-12 14:06:40.000000 modernmt-1.4.0/src/modernmt.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       15 2023-07-12 14:06:40.000000 modernmt-1.4.0/src/modernmt.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        9 2023-07-12 14:06:40.000000 modernmt-1.4.0/src/modernmt.egg-info/top_level.txt
```

### Comparing `modernmt-1.3.0/LICENSE` & `modernmt-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modernmt-1.3.0/PKG-INFO` & `modernmt-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modernmt
-Version: 1.3.0
+Version: 1.4.0
 Summary: ModernMT API wrapper
 Home-page: https://github.com/modernmt/modernmt-python
 Author: ModernMT
 Author-email: info@modernmt.com
 Project-URL: Bug Tracker, https://github.com/modernmt/modernmt-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `modernmt-1.3.0/setup.cfg` & `modernmt-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modernmt
-version = 1.3.0
+version = 1.4.0
 author = ModernMT
 author_email = info@modernmt.com
 description = ModernMT API wrapper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/modernmt/modernmt-python
 project_urls =
```

### Comparing `modernmt-1.3.0/src/modernmt/modernmt.py` & `modernmt-1.4.0/src/modernmt/modernmt.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.message = message
 
         if metadata is not None:
             self.metadata = metadata
 
 
 class ModernMT(object):
-    def __init__(self, api_key, platform="modernmt-python", platform_version="1.3.0", api_client=None) -> None:
+    def __init__(self, api_key, platform="modernmt-python", platform_version="1.4.0", api_client=None) -> None:
         self.__batch_public_key = None
         self.__batch_public_key_timestamp_sec = 0
 
         self.__base_url = "https://api.modernmt.com"
         self.__headers = {
             "MMT-ApiKey": api_key,
             "MMT-Platform": platform,
@@ -74,14 +74,16 @@
                 data["multiline"] = options["multiline"]
             if "timeout" in options:
                 data["timeout"] = options["timeout"]
             if "format" in options:
                 data["format"] = options["format"]
             if "alt_translations" in options:
                 data["alt_translations"] = options["alt_translations"]
+            if "session" in options:
+                data["session"] = options["session"]
 
         res = self.__send("get", "/translate", data=data)
 
         if not isinstance(res, list):
             return Translation(res)
 
         translations = []
@@ -114,14 +116,16 @@
                 data["multiline"] = options["multiline"]
             if "format" in options:
                 data["format"] = options["format"]
             if "alt_translations" in options:
                 data["alt_translations"] = options["alt_translations"]
             if "metadata" in options:
                 data["metadata"] = options["metadata"]
+            if "session" in options:
+                data["session"] = options["session"]
 
         headers = None
         if options is not None and "idempotency_key" in options:
             headers = {"x-idempotency-key": options["idempotency_key"]}
 
         res = self.__send("post", "/translate/batch", data=data, headers=headers)
 
@@ -291,23 +295,42 @@
             data["description"] = description
 
         return self.__send("put", "/memories/%s" % id, data=data, cls=Memory)
 
     def delete(self, id):
         return self.__send("delete", "/memories/%s" % id, cls=Memory)
 
-    def add(self, id, source, target, sentence, translation, tuid=None):
-        data = {"source": source, "target": target, "sentence": sentence, "translation": translation}
+    def add(self, id, source, target, sentence, translation, tuid=None, session=None):
+        data = {
+            "source": source,
+            "target": target,
+            "sentence": sentence,
+            "translation": translation
+        }
+
         if tuid is not None:
             data["tuid"] = tuid
 
+        if session is not None:
+            data["session"] = session
+
         return self.__send("post", "/memories/%s/content" % id, data=data, cls=ImportJob)
 
-    def replace(self, id, tuid, source, target, sentence, translation):
-        data = {"tuid": tuid, "source": source, "target": target, "sentence": sentence, "translation": translation}
+    def replace(self, id, tuid, source, target, sentence, translation, session=None):
+        data = {
+            "tuid": tuid,
+            "source": source,
+            "target": target,
+            "sentence": sentence,
+            "translation": translation
+        }
+
+        if session is not None:
+            data["session"] = session
+
         return self.__send("put", "/memories/%s/content" % id, data=data, cls=ImportJob)
 
     def import_tmx(self, id, tmx, compression=None):
         if isinstance(tmx, str):
             tmx = open(tmx, "rb")
 
         data = {}
```

### Comparing `modernmt-1.3.0/src/modernmt.egg-info/PKG-INFO` & `modernmt-1.4.0/src/modernmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modernmt
-Version: 1.3.0
+Version: 1.4.0
 Summary: ModernMT API wrapper
 Home-page: https://github.com/modernmt/modernmt-python
 Author: ModernMT
 Author-email: info@modernmt.com
 Project-URL: Bug Tracker, https://github.com/modernmt/modernmt-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

